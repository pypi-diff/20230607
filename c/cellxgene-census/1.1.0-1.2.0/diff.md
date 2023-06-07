# Comparing `tmp/cellxgene_census-1.1.0.tar.gz` & `tmp/cellxgene_census-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.1.0.tar", last modified: Wed May 31 14:56:32 2023, max compression
+gzip compressed data, was "cellxgene_census-1.2.0.tar", last modified: Wed Jun  7 03:41:02 2023, max compression
```

## Comparing `cellxgene_census-1.1.0.tar` & `cellxgene_census-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.612868 cellxgene_census-1.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.612868 cellxgene_census-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.612868 cellxgene_census-1.1.0/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:56:32.000000 cellxgene_census-1.1.0/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:32.616868 cellxgene_census-1.1.0/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/experimental/ml/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 14:56:20.000000 cellxgene_census-1.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.882763 cellxgene_census-1.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.882763 cellxgene_census-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/pp/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_util.py
```

### Comparing `cellxgene_census-1.1.0/LICENSE` & `cellxgene_census-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/PKG-INFO` & `cellxgene_census-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.1.0
+Version: 1.2.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.1.0/README.md` & `cellxgene_census-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/pyproject.toml` & `cellxgene_census-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 ]
 
 [project.optional-dependencies]
 experimental = [
     "torch==2.0.1",
     "torchdata==0.6.1",
     "scikit-learn==1.2.2",
+    "scikit-misc==0.2.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/chanzuckerberg/cellxgene-census"
 repository = "https://github.com/chanzuckerberg/cellxgene-census"
 
 [tool.setuptools.packages.find]
```

### Comparing `cellxgene_census-1.1.0/release_process.md` & `cellxgene_census-1.2.0/release_process.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 5. Built packages are published to PyPi _from_ the GitHub assets, i.e. are never hand-created, to reduce errors.
 
 ## Prerequisites
 
 While not strictly required, this process assumes you have met the following prerequisites:
 
 - You have write access to the `chanzuckerberg/cellxgene-census` repo
-- You have an account on pypi.org and test.pypi.org, both with access to the cellxgene_census project
+- You have an account on pypi.org and test.pypi.org, both with access to the cellxgene_census project. You will need to have created an API token on each account so that you can authenticate to test.pypi.org and pypi.org accounts when using `twine`. Usually this means adding these tokens to your `~/.pypirc` file. See https://pypi.org/help/#apitoken for more information.
 - You have the Github CLI tool (`gh`) installed. See [documentation](https://cli.github.com/).
-- You have the `pipx` CLI tool installed. See [documentation](https://pypa.github.io/pipx/).
+- You have the `pipx` CLI tool installed. See [documentation](https://pypa.github.io/pipx/). 
 
 ## Step 1: Building the package assets
 
 A build will occur automatically upon each commit to main, upon each commit to a PR, or when the build workflow is manually invoked. The build workflow is defined by the GH `py-build.yml` workflow. Build artifacts are the Python setuptools-created `sdist` and `wheel`, and are retained for a limited period of time (currently the GH default of 90 days).
 
 Unless you are revising and testing the build process itself, there is no need to manually perform a build.
 
@@ -77,29 +77,41 @@
    ```
 3. Trigger a build for this tag by manually triggering the `py-build.yml` workflow. For example:
    ```shell
    $ gh workflow run py-build.yml --ref <SEMVER>
    ```
 4. When the workflow completes, make note of the run ID (e.g., using `gh run list`).
 5. Optional, _but recommended_: download the asset from the build workflow and validate it.
-6. Create and publish a GitHub Release, using the `<SEMVER>` tag above (e.g., `v1.9.4`). It is recommended that you include a release summary and change log in the GH release.
+6. Create and publish a GitHub Release [here](https://github.com/chanzuckerberg/cellxgene-census/releases/new). Set the release title to the `<SEMVER>`. Select `Set as the latest release`. Use the `Generate Release Notes` button to auto-populate the summary with a changelog. It is reasonable to remove any R-specific or builder-specific entries. Add a prelude to the summary, noting any major new features or API changes. 
 
 ## Step 4: Publish assets to PyPi
 
 To publish built release assets to PyPi (_note_: this will require your pypi/testpypi login):
 
-1. Download the assets built for your release commit, using the same method as step 2 above, e.g.,
+1. Delete any existing release builds you may have accumulated in the past: `rm ./artifact/*`.
+2. Download the assets built for your release commit, using the same method as step 2 above, e.g.,
    ```shell
    $ gh run download <ID>
    ```
-2. Optional: upload to TestPyPi (this assumes the downloaded assets are in ./artifact/).
+3. Optional: upload to TestPyPi (this assumes the downloaded assets are in ./artifact/).
 
    ```shell
    pipx run twine upload --repository testpypi ./artifact/*
    ```
 
-   Following the upload, confirm correct presentation on the project page and ability to download install from TestPyPi. To test with TestPyPi, use `pipx run twine upload --repository testpypi ./artifact/*`. You can find more information [here](https://packaging.python.org/en/latest/guides/using-testpypi/).
-
-3. Use twine to upload to PyPi (this assumes the downloaded assets are in ./artifact/), e.g.,
+   Following the upload, confirm correct presentation on the project page and ability to download install from TestPyPi. 
+4. To test installation from TestPyPi:
+   ```shell
+   pip install --no-cache-dir -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple cellxgene-census
+   python -c "import cellxgene_census; print(cellxgene_census.__version__)"
+   ```
+   Note that the `--extra-index-url` option ensures that any transitive package dependencies that are _not_ available on
+   `test.pypi.org` can be satisfied by installing them from the production `pypi.org`.  You can find more information
+   [here](https://packaging.python.org/en/latest/guides/using-testpypi/).
+5. Use twine to upload to PyPi (this assumes the downloaded assets are in ./artifact/), e.g.,
    ```shell
    pipx run twine upload ./artifact/*
+6. Test the installation from PyPi, as a final sanity check. Note that it may take a minute for the new release to be visible on pypi.org:
+   ```shell
+   pip install --no-cache-dir cellxgene-census
+   python -c "import cellxgene_census; print(cellxgene_census.__version__)"
    ```
```

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/__init__.py` & `cellxgene_census-1.2.0/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.2.0/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.2.0/src/cellxgene_census/_get_anndata.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,34 +6,29 @@
 
 Methods to retrieve slices of the census as AnnData objects.
 """
 from typing import Optional
 
 import anndata
 import tiledbsoma as soma
-
-# TODO: waiting on https://github.com/single-cell-data/TileDB-SOMA/issues/872.
 from somacore.options import SparseDFCoord
 
-# TODO: rm this import and use `soma.AxisColumnNames` after https://github.com/single-cell-data/TileDB-SOMA/issues/791
-from somacore.query.query import AxisColumnNames
-
 from ._experiment import _get_experiment
 
 
 def get_anndata(
     census: soma.Collection,
     organism: str,
     measurement_name: str = "RNA",
     X_name: str = "raw",
     obs_value_filter: Optional[str] = None,
     obs_coords: Optional[SparseDFCoord] = None,
     var_value_filter: Optional[str] = None,
     var_coords: Optional[SparseDFCoord] = None,
-    column_names: Optional[AxisColumnNames] = None,
+    column_names: Optional[soma.AxisColumnNames] = None,
 ) -> anndata.AnnData:
     """
     Convience wrapper around ``soma.Experiment`` query, to build and execute a query,
     and return it as an :class:`anndata.AnnData` object.
 
     Args:
         census:
```

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/_open.py` & `cellxgene_census-1.2.0/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.2.0/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.2.0/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import os
 import sys
 from datetime import timedelta
 from time import time
-from typing import Any, Dict, Iterator, Optional, Sequence, Tuple
+from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple
 
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import pyarrow as pa
 import scipy
 import somacore
 import tiledbsoma as soma
 import torch
 import torchdata.datapipes.iter as pipes
@@ -20,15 +21,15 @@
 from torch import Tensor
 from torch.utils.data import DataLoader
 from torch.utils.data.dataset import Dataset
 
 import cellxgene_census
 from cellxgene_census._open import _build_soma_tiledb_context
 
-ObsDatum = Tuple[Tensor, torch.sparse_coo_tensor]
+ObsDatum = Tuple[Tensor, Tensor]
 
 Encoders = Dict[str, LabelEncoder]
 
 pytorch_logger = logging.getLogger("cellxgene_census.experimental.pytorch")
 pytorch_logger.setLevel(logging.INFO)
 
 
@@ -92,28 +93,27 @@
     """All X data for the ``soma_joinid``s of the current obs - batch"""
 
     i: int = -1
     """Index into current obs ``SOMA`` batch"""
 
     def __init__(
         self,
-        obs_joinids: pa.Array,
+        obs_joinids: List[int],
         var_joinids: pa.Array,
         exp_uri: str,
         aws_region: Optional[str],
         measurement_name: str,
         X_layer_name: str,
         batch_size: int,
         encoders: Dict[str, LabelEncoder],
         stats: Stats,
         obs_column_names: Sequence[str],
         sparse_X: bool,
         soma_buffer_bytes: Optional[int] = None,
     ) -> None:
-        self.obs_joinids = obs_joinids
         self.var_joinids = var_joinids
         self.batch_size = batch_size
         self.sparse_X = sparse_X
 
         # holding reference to SOMA object prevents it from being closed
         self.exp = _open_experiment(exp_uri, aws_region, soma_buffer_bytes=soma_buffer_bytes)
         self.X: soma.SparseNDArray = self.exp.ms[measurement_name].X[X_layer_name]
@@ -235,17 +235,15 @@
         experimental
     """
 
     _query: Optional[soma.ExperimentAxisQuery]
     """In multi-processing mode (i.e. num_workers > 0), this ``ExperimentAxisQuery`` object will *not* be pickled; 
     each worker will instantiate a new query"""
 
-    _obs_joinids_partitioned: Optional[pa.Array]
-
-    _obs_and_x_iter: Optional[_ObsAndXIterator]
+    _obs_joinids_partitioned: Optional[npt.NDArray[np.int64]] = None
 
     _encoders: Optional[Encoders]
 
     _stats: Stats
 
     # TODO: Consider adding another convenience method wrapper to construct this object whose signature is more closely
     #  aligned with get_anndata() params (i.e. "exploded" AxisQuery params).
@@ -255,15 +253,14 @@
         measurement_name: str,
         X_name: str,
         obs_query: Optional[soma.AxisQuery] = None,
         var_query: Optional[soma.AxisQuery] = None,
         obs_column_names: Sequence[str] = (),
         batch_size: int = 1,
         sparse_X: bool = False,
-        num_workers: int = 0,
         soma_buffer_bytes: Optional[int] = None,
     ) -> None:
         """
         Construct a new ``ExperimentDataPipe``.
 
         Returns:
             ``ExperimentDataPipe``.
@@ -325,28 +322,43 @@
 
         if num_partitions is not None:
             # partitioned data loading
             # NOTE: Can alternately use a `worker_init_fn` to split among workers split workload
             partition_size = len(obs_joinids) // num_partitions
             partition_start = partition_size * partition
             partition_end_excl = min(len(obs_joinids), partition_start + partition_size)
-            self._obs_joinids_partitioned = obs_joinids[partition_start:partition_end_excl]
+            # The to_numpy() call is a workaround for a possible bug in TileDB-SOMA:
+            # https://github.com/single-cell-data/TileDB-SOMA/issues/1456
+            self._obs_joinids_partitioned = obs_joinids[partition_start:partition_end_excl].to_numpy()
+
+            if pytorch_logger.isEnabledFor(logging.DEBUG):
+                if self._obs_joinids_partitioned is not None and len(self._obs_joinids_partitioned) > 0:
+                    joinids_start = self._obs_joinids_partitioned[0]
+                    joinids_end = self._obs_joinids_partitioned[-1]
+                else:
+                    joinids_start = joinids_end = 0
 
-            pytorch_logger.debug(
-                f"Process {os.getpid()} handling partition {partition + 1} of {num_partitions}, "
-                f"range={partition_start}:{partition_end_excl}, "
-                f"{partition_size:}"
-            )
+                pytorch_logger.debug(
+                    f"Process {os.getpid()} handling partition {partition + 1} of {num_partitions}, "
+                    f"index range={partition_start}:{partition_end_excl}, "
+                    f"soma_joinid range={joinids_start}:{joinids_end}, "
+                    f"{partition_size:}"
+                )
 
     def __iter__(self) -> Iterator[ObsDatum]:
+        # TODO: avoid re-initializing query if in multi-processing mode, when _obs_joinids_partitioned is set. will need to cache var_joinids for serialization
         self._init()
         assert self._query is not None
 
+        obs_joinids = (
+            self._obs_joinids_partitioned if self._obs_joinids_partitioned is not None else self._query.obs_joinids()
+        )
+
         return _ObsAndXIterator(
-            obs_joinids=self._obs_joinids_partitioned or self._query.obs_joinids(),
+            obs_joinids=obs_joinids,
             var_joinids=self._query.var_joinids(),
             exp_uri=self.exp_uri,
             aws_region=self.aws_region,
             measurement_name=self.measurement_name,
             X_layer_name=self.layer_name,
             batch_size=self.batch_size,
             encoders=self.obs_encoders(),
```

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.2.0/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.1.0
+Version: 1.2.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.1.0/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.2.0/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,25 @@
 src/cellxgene_census.egg-info/SOURCES.txt
 src/cellxgene_census.egg-info/dependency_links.txt
 src/cellxgene_census.egg-info/requires.txt
 src/cellxgene_census.egg-info/top_level.txt
 src/cellxgene_census/experimental/__init__.py
 src/cellxgene_census/experimental/ml/__init__.py
 src/cellxgene_census/experimental/ml/pytorch.py
+src/cellxgene_census/experimental/pp/__init__.py
+src/cellxgene_census/experimental/pp/_eager_iter.py
+src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+src/cellxgene_census/experimental/pp/_online.py
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/test_acceptance.py
 tests/test_directory.py
 tests/test_get_anndata.py
 tests/test_get_helpers.py
 tests/test_open.py
 tests/test_util.py
 tests/experimental/__init__.py
 tests/experimental/ml/__init__.py
-tests/experimental/ml/test_pytorch.py
+tests/experimental/ml/test_pytorch.py
+tests/experimental/pp/test_hvg.py
+tests/experimental/pp/test_online.py
```

### Comparing `cellxgene_census-1.1.0/tests/README.md` & `cellxgene_census-1.2.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/conftest.py` & `cellxgene_census-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.2.0/tests/experimental/ml/test_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -258,14 +258,32 @@
 
     labels_encoded = batch[1][:, 1]
     labels_decoded = exp_data_pipe.obs_encoders()["label"].inverse_transform(labels_encoded)
     assert labels_decoded.tolist() == ["0", "1", "2"]
 
 
 @pytest.mark.experimental
+# noinspection PyTestParametrized
+@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+def test__multiprocessing__returns_full_result(soma_experiment: Experiment) -> None:
+    dp = ExperimentDataPipe(
+        soma_experiment,
+        measurement_name="RNA",
+        X_name="raw",
+        obs_column_names=["label"],
+    )
+    dl = experiment_dataloader(dp, num_workers=2)
+
+    full_result = list(iter(dl))
+
+    soma_joinids = [t[1][0].item() for t in full_result]
+    assert sorted(soma_joinids) == list(range(6))
+
+
+@pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
 @pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(3, 3, ("raw",), pytorch_x_value_gen)])
 def test_experiment_dataloader__non_batched(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"])
     dl = experiment_dataloader(dp)
     torch_data = [row for row in dl]
 
@@ -340,18 +358,16 @@
     """
 
     dp = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
-        num_workers=1,
-        sparse_X=True,
     )
-    dl = experiment_dataloader(dp)
+    dl = experiment_dataloader(dp, num_workers=2)
     dp.obs_encoders()  # trigger query building
     row = next(iter(dl))  # trigger multiprocessing
 
     assert row is not None
 
 
 @pytest.mark.experimental
```

### Comparing `cellxgene_census-1.1.0/tests/test_acceptance.py` & `cellxgene_census-1.2.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/test_directory.py` & `cellxgene_census-1.2.0/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/test_get_anndata.py` & `cellxgene_census-1.2.0/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/test_get_helpers.py` & `cellxgene_census-1.2.0/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/test_open.py` & `cellxgene_census-1.2.0/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.1.0/tests/test_util.py` & `cellxgene_census-1.2.0/tests/test_util.py`

 * *Files identical despite different names*

