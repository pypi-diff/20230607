# Comparing `tmp/mri-nufft-0.0.0.tar.gz` & `tmp/mri-nufft-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mri-nufft-0.0.0.tar", last modified: Thu May 25 08:51:51 2023, max compression
+gzip compressed data, was "mri-nufft-0.1.0.tar", last modified: Wed Jun  7 15:54:31 2023, max compression
```

## Comparing `mri-nufft-0.0.0.tar` & `mri-nufft-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.410958 mri-nufft-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.410958 mri-nufft-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.410958 mri-nufft-0.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.410958 mri-nufft-0.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/docs/nufft.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.410958 mri-nufft-0.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.410958 mri-nufft-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/src/mri_nufft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 08:51:51.000000 mri-nufft-0.0.0/src/mri_nufft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-25 08:51:51.000000 mri-nufft-0.0.0/src/mri_nufft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:51:51.000000 mri-nufft-0.0.0/src/mri_nufft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 08:51:51.000000 mri-nufft-0.0.0/src/mri_nufft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 08:51:51.000000 mri-nufft-0.0.0/src/mri_nufft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/src/mrinufft/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 08:51:51.000000 mri-nufft-0.0.0/src/mrinufft/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/src/mrinufft/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/pynufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/src/mrinufft/operators/off_resonnance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:51:51.414959 mri-nufft-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 08:51:17.000000 mri-nufft-0.0.0/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.713644 mri-nufft-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.713644 mri-nufft-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/docs/nufft.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/examples/example_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/examples/example_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.713644 mri-nufft-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mri_nufft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mri_nufft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 15:54:31.000000 mri-nufft-0.1.0/src/mrinufft/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/pynufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/operators/off_resonnance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.717644 mri-nufft-0.1.0/src/mrinufft/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/expansions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/trajectory2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/trajectory3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/src/mrinufft/trajectories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:31.721644 mri-nufft-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 15:54:02.000000 mri-nufft-0.1.0/tests/test_interface.py
```

### Comparing `mri-nufft-0.0.0/.github/workflows/master-cd.yml` & `mri-nufft-0.1.0/.github/workflows/master-cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         with:
           python-version: "3.10"
       - name: Install dependencies
         shell: bash -l {0}
         run: |
           python -m pip install --upgrade pip
           python -m pip install .[doc]
+          python -m pip install finufft
 
       - name: Build API documentation
         run: |
           python -m sphinx docs docs_build
 
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v1
```

### Comparing `mri-nufft-0.0.0/.github/workflows/tags-release.yml` & `mri-nufft-0.1.0/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/.github/workflows/test-ci.yml` & `mri-nufft-0.1.0/.github/workflows/test-ci.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/LICENSE.txt` & `mri-nufft-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/README.rst` & `mri-nufft-0.1.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,88 @@
 =========
 MRI-NUFFT
 =========
 
+Doing non-Cartesian MR Imaging has never been so easy.
+
 .. list-table::
    :widths: 25 25 25
    :header-rows: 0
 
    * - .. image:: https://img.shields.io/badge/coverage-TBA-green
         :target: https://app.codecov.io/gh/mind-inria/mri-nufft
      - .. image:: https://github.com/mind-inria/mri-nufft/workflows/CI/badge.svg
      - .. image:: https://github.com/mind-inria/mri-nufft/workflows/CD/badge.svg
    * - .. image:: https://img.shields.io/badge/style-black-black
      - .. image:: https://img.shields.io/badge/docs-Sphinx-blue
         :target: https://mind-inria.github.io/mri-nufft
-     - .. image:: https://img.shields.io/badge/release-TBA-blue
+     - .. image:: https://img.shields.io/pypi/v/mri-nufft
         :target: https://pypi.org/project/mri-nufft/
 
 
-This python package extends various NUFFT (Non Uniform Fast Fourier Transform) python bindings for MRI Reconstruction usage.
+This python package extends various NUFFT (Non-Uniform Fast Fourier Transform) python bindings used for MRI reconstruction.
+
+In particular, it provides a unified interface for all the methods, with extra features such as coil sensitivity, density compensated adjoint and off-resonance corrections (for B0 inhomogeneities).
+
+
+Usage
+=====
+
+.. TODO use a include file directive.
+.. code:: python
+
+      import matplotlib.pyplot as plt
+      from scipy.datasets import face
+
+      import mrinufft
+      from mrinufft.trajectories import display
+
+      # Create a 2D Radial trajectory for demo
+      samples_loc = mrinufft.initialize_2D_radial(Nc=100, Ns=500)
+      # Get a 2D image for the demo
+      image = face(gray=True)[256:768, 256:768]
+
+      ## The real deal starts here ##
+      # Choose your NUFFT backend (installed independly from the package)
+      # And create the associated operator.
+      NufftOperator = mrinufft.get_operator("finufft")
+      nufft = NufftOperator(
+          samples_loc.reshape(-1, 2), shape=(512, 512), density=True, n_coils=1
+      )
+
+      kspace_data = nufft.op(image)  # Image -> Kspace
+      image2 = nufft.adj_op(kspace_data)  # Kspace -> Image
+
+      # Show the results
+      fig, ax = plt.subplots(1, 3)
+
+      ax[0].imshow(image)
+      ax[0].set_title("original image")
+      display.display_2D_trajectory(samples_loc, subfigure=ax[1])
+      ax[1].set_aspect("equal")
+      ax[1].set_title("Sampled points in k-space")
+      ax[2].imshow(abs(image2))
+      ax[2].set_title("Auto adjoint image")
+      plt.show()
+
+
+.. TODO Add image
+
+For best image quality, embed these steps in a more complex reconstruction pipeline (for instance using `PySAP <https://github.com/CEA-COSMIC/pysap-mri>`_).
+
+Want to see more ?
+
+- Check the `Documentation <https://mind-inria.github.io/mri-nufft/>`_
+
+- Or go visit the `Examples <https://mind-inria.github.io/mri-nufft/auto_examples/index.html>`_
 
-In particular it provides an unified interface for all the methods, with extra forward Model step, such as coil sensitivity, density compensated adjoint and Off Resonance corrections (B0 inhomogeneities)
+Supported Libraries
+-------------------
 
-Supported Library are:
+These libraries needs to be installed seperately from this package.
 
 - GPU Implementations:
 
   - `cufinufft <https://github.com/flatironinstitute/cufinufft/>`_
       Developed and maintained by the `Flat Iron Institute <https://github.com/flatironinstitut>`_.
       Requires a separate installation of cufinufft C++/CUDA library.
       Current bindings only support float32/complex64 data.
@@ -41,15 +98,15 @@
   - `finufft <https://github.com/flatironinstitute/finufft>`_
       Developed and maintained by the `Flat Iron Institute <https://github.com/flatironinstitut>`_.
       C/C++ implementation with Multithread and batch computation support.
 
   - `pyNUFFT <https://github.com/jyhmiinlin/pynufft>`_
       CPU version of pyNUFFT, using standard python libraries.
 
-The NUFFT operation is often not enough to provide good image quality by itself. It is best used in an Compress Sensing setup. For such use cases,
+The NUFFT operation is often not enough to provide good image quality by itself: It is best used in a Compress Sensing setup. For such use cases,
 
 you can check the `pysap <https://github.com/CEA-COSMIC/pysap/>`_ package suite and  `pysap-mri <https://github.com/CEA-COSMIC/pysap-mri>`_ for MRI dedicated solutions.
 
 Installation
 ------------
 
 Be sure that you have your GPU librairies properly installed (CUDA, Pytorch, Tensorflow, etc).
@@ -58,30 +115,31 @@
 Then clone and install the package::
 
     $ git clone https://github.com:mind-inria/mri-nufft
     $ pip install ./mri-nufft
 
 Tests
 -----
+TBA
 
 
 Documentation
 -------------
 
 Documentation is available online at https://mind-inria.github.io/mri-nufft
 
 It can also be built locally ::
 
   $ cd mri-nufft
   $ pip install -e .[doc]
-  $ python -m sphinx-build docs docs_build
+  $ python -m sphinx docs docs_build
 
 To view the html doc locally you can use ::
 
   $ python -m http.server --directory docs_build 8000
 
 And visit `localhost:8000` on your web browser.
 
 
 Related Packages
 ----------------
-For Reconstruction methods of MRI image from non cartesian sampling, see `pysap-mri <https://github.com/CEA-COSMIC/pysap-mri>`_ and `ModOpt <https://github.com/CEA-COSMIC/ModOpt>`_ 
+For reconstruction methods of MR images from non-Cartesian sampling, see `pysap-mri <https://github.com/CEA-COSMIC/pysap-mri>`_ and `ModOpt <https://github.com/CEA-COSMIC/ModOpt>`_
```

### Comparing `mri-nufft-0.0.0/docs/Makefile` & `mri-nufft-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/docs/_templates/custom-class-template.rst` & `mri-nufft-0.1.0/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/docs/_templates/custom-module-template.rst` & `mri-nufft-0.1.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/docs/conf.py` & `mri-nufft-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/pyproject.toml` & `mri-nufft-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [project]
 name = "mri-nufft"
-description = "MRI Non Cartesian Fourier Operators based on (cu)finufft."
+description = "MRI Non-Cartesian Fourier Operators with multiple computation backends."
 authors = [{name="Pierre-antoine Comby", email="pierre-antoine.comby@crans.org"}]
 
 readme = "README.md"
 dependencies = ["numpy", "scipy", "matplotlib", "tqdm"]
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 
 gpu = ["cupy-wheel"]
 test = ["pytest", "pytest-cov", "pytest-xdist", "pytest-sugar"]
 dev = ["black", "isort", "ruff"]
-doc = ["sphinx<5", "pydata-sphinx-theme", "sphinx-gallery", "matplotlib"]
+
+doc = ["sphinx==4.5.0", "pydata-sphinx-theme", "sphinx-gallery", "matplotlib", "pooch"]
+# pooch is for scipy.datasets
 
 [build-system]
 requires = ["setuptools", "setuptools-scm[toml]", "wheel"]
 
 [tool.setuptools_scm]
 write_to = "src/mrinufft/_version.py"
 version_scheme = "python-simplified-semver"
@@ -39,14 +41,15 @@
 src = ["src", "tests"]
 select = ["E", "F", "B", "Q", "UP", "D"]
 
 ignore = [
 "B905", #zip() without an explicit strict= parameter
 "B028", #No explicit stacklevel keyword argument found
 ]
+extend-exclude = [ "example_*.py" ]
 [tool.ruff.pydocstyle]
 convention="numpy"
 
 [tool.isort]
 profile="black"
 
 [tool.pytest.ini_options]
```

### Comparing `mri-nufft-0.0.0/src/mri_nufft.egg-info/SOURCES.txt` & `mri-nufft-0.1.0/src/mri_nufft.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/nufft.rst
 docs/_templates/custom-class-template.rst
 docs/_templates/custom-module-template.rst
 examples/README.rst
+examples/example_readme.py
+examples/example_trajectories.py
 src/mri_nufft.egg-info/PKG-INFO
 src/mri_nufft.egg-info/SOURCES.txt
 src/mri_nufft.egg-info/dependency_links.txt
 src/mri_nufft.egg-info/requires.txt
 src/mri_nufft.egg-info/top_level.txt
 src/mrinufft/__init__.py
 src/mrinufft/_version.py
@@ -33,9 +35,15 @@
 src/mrinufft/operators/interfaces/gpu/_cufinufft.py
 src/mrinufft/operators/interfaces/gpu/css_colors.py
 src/mrinufft/operators/interfaces/gpu/cufinufft.py
 src/mrinufft/operators/interfaces/gpu/cupy_kernels.py
 src/mrinufft/operators/interfaces/gpu/pynufft.py
 src/mrinufft/operators/interfaces/gpu/tfnufft.py
 src/mrinufft/operators/interfaces/gpu/utils.py
+src/mrinufft/trajectories/__init__.py
+src/mrinufft/trajectories/display.py
+src/mrinufft/trajectories/expansions.py
+src/mrinufft/trajectories/trajectory2D.py
+src/mrinufft/trajectories/trajectory3D.py
+src/mrinufft/trajectories/utils.py
 tests/test_cpu.py
 tests/test_interface.py
```

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/__init__.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/base.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/base.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         self,
         samples,
         shape,
         density=False,
         n_coils=1,
         smaps=None,
     ):
-
         self.shape = shape
         self.n_samples = len(samples)
         if samples.max() > np.pi:
             warnings.warn("samples will be normalized in [-pi, pi]")
             samples *= np.pi / samples.max()
         # we will access the samples by their coordinate first.
         self.samples = np.asfortranarray(samples)
```

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/cpu_kernels.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/finufft_interface.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/cpu/pynufft_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     PYNUFFT_CPU_AVAILABLE = False
 
 
 class RawPyNUFFT:
     """Wrapper around PyNUFFT object."""
 
     def __init__(self, samples, shape, osf=2, interpolator_shape=6):
-
         self._nufft_obj = pynufft.NUFFT()
         self._nufft_obj.plan(
             samples,
             shape,
             tuple(osf * s for s in shape),
             tuple([interpolator_shape] * len(shape)),
         )
```

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/_cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/css_colors.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/css_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,8 +143,9 @@
     16737095,
     4251856,
     15631086,
     16113331,
     16777215,
     16119285,
     16776960,
-    10145074]
+    10145074,
+]
```

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/cupy_kernels.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/tfnufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/interfaces/gpu/utils.py` & `mri-nufft-0.1.0/src/mrinufft/operators/interfaces/gpu/utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.0.0/src/mrinufft/operators/off_resonnance.py` & `mri-nufft-0.1.0/src/mrinufft/operators/off_resonnance.py`

 * *Files identical despite different names*

