# Comparing `tmp/sunraster-0.4.3.tar.gz` & `tmp/sunraster-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunraster-0.4.3.tar", last modified: Thu Oct  6 21:55:01 2022, max compression
+gzip compressed data, was "sunraster-0.5.0rc1.tar", last modified: Wed Jun  7 15:43:20 2023, max compression
```

## Comparing `sunraster-0.4.3.tar` & `sunraster-0.5.0rc1.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.649806 sunraster-0.4.3/.circleci/
--rw-r--r--   0 vsts      (1001) docker     (121)     1584 2022-10-06 21:54:44.000000 sunraster-0.4.3/.circleci/config.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-10-06 21:54:44.000000 sunraster-0.4.3/.circleci/early_exit.sh
--rw-r--r--   0 vsts      (1001) docker     (121)      140 2022-10-06 21:54:44.000000 sunraster-0.4.3/.codecov.yaml
--rw-r--r--   0 vsts      (1001) docker     (121)     3293 2022-10-06 21:54:44.000000 sunraster-0.4.3/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)     1201 2022-10-06 21:54:44.000000 sunraster-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 vsts      (1001) docker     (121)      286 2022-10-06 21:54:44.000000 sunraster-0.4.3/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     4473 2022-10-06 21:54:44.000000 sunraster-0.4.3/CHANGELOG.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-10-06 21:54:44.000000 sunraster-0.4.3/LICENSE.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      452 2022-10-06 21:54:44.000000 sunraster-0.4.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     4637 2022-10-06 21:55:01.653806 sunraster-0.4.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     3476 2022-10-06 21:54:44.000000 sunraster-0.4.3/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3050 2022-10-06 21:54:44.000000 sunraster-0.4.3/azure-pipelines.yml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.649806 sunraster-0.4.3/changelog/
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-10-06 21:54:44.000000 sunraster-0.4.3/changelog/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.649806 sunraster-0.4.3/docs/
--rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)      104 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/api.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      147 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/changelog.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3544 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/conf.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/docs/data_types/
--rw-r--r--   0 vsts      (1001) docker     (121)      119 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/data_types/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)    15957 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/data_types/raster.rst
--rw-r--r--   0 vsts      (1001) docker     (121)    26532 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/data_types/spectrogram.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2392 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3882 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/installation.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      760 2022-10-06 21:54:44.000000 sunraster-0.4.3/docs/make.bat
--rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-10-06 21:54:44.000000 sunraster-0.4.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     3382 2022-10-06 21:55:01.653806 sunraster-0.4.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)      863 2022-10-06 21:54:44.000000 sunraster-0.4.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/
--rw-r--r--   0 vsts      (1001) docker     (121)      255 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      176 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/extern/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/extern/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10051 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/extern/meta.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/extern/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/extern/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5493 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/extern/tests/test_meta.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/instr/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/instr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16000 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/instr/spice.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/instr/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/instr/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13621 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/instr/tests/test_spice.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1938 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/meta.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23271 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/spectrogram.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14936 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/spectrogram_sequence.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)      147 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (121)   132480 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/tests/data/solo_L2_spice-n-ras-db_20200602T081733_V01_12583760-000.fits
--rw-r--r--   0 vsts      (1001) docker     (121)    69120 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/tests/data/solo_L2_spice-n-sit_20200620T235901_V01_16777431-000.fits
--rw-r--r--   0 vsts      (1001) docker     (121)     7349 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/tests/test_spectrogram.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9969 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/tests/test_spectrogramsequence.py
--rw-r--r--   0 vsts      (1001) docker     (121)      998 2022-10-06 21:54:44.000000 sunraster-0.4.3/sunraster/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-06 21:55:01.653806 sunraster-0.4.3/sunraster.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4637 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1292 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      299 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       10 2022-10-06 21:55:01.000000 sunraster-0.4.3/sunraster.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-10-06 21:54:44.000000 sunraster-0.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.982523 sunraster-0.5.0rc1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.circleci/early_exit.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.978523 sunraster-0.5.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.982523 sunraster-0.5.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.982523 sunraster-0.5.0rc1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/changelog/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.982523 sunraster-0.5.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.982523 sunraster-0.5.0rc1/docs/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/data_types/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/data_types/raster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/data_types/spectrogram.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.982523 sunraster-0.5.0rc1/joss_paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/joss_paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/joss_paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/extern/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/extern/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/extern/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/extern/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/instr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/instr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/instr/spice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/instr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/instr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/instr/tests/test_spice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/spectrogram_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   132480 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/tests/data/solo_L2_spice-n-ras-db_20200602T081733_V01_12583760-000.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    69120 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/tests/data/solo_L2_spice-n-sit_20200620T235901_V01_16777431-000.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/tests/test_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/tests/test_spectrogramsequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/sunraster/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:20.986523 sunraster-0.5.0rc1/sunraster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 15:43:20.000000 sunraster-0.5.0rc1/sunraster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-07 15:43:01.000000 sunraster-0.5.0rc1/tox.ini
```

### Comparing `sunraster-0.4.3/.circleci/config.yml` & `sunraster-0.5.0rc1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/.gitignore` & `sunraster-0.5.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/.pre-commit-config.yaml` & `sunraster-0.5.0rc1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 repos:
-  - repo: https://github.com/PyCQA/docformatter
-    rev: v1.5.0
-    hooks:
-      - id: docformatter
-        args: [--in-place, --pre-summary-newline, --make-summary-multi]
   - repo: https://github.com/PyCQA/autoflake
-    rev: v1.6.1
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|__init__.py|docs/conf.py)$"
   -   repo: https://github.com/psf/black
-      rev: 22.8.0
+      rev: 23.3.0
       hooks:
       - id: black
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
   -   repo: https://github.com/PyCQA/isort
-      rev: 5.10.1
+      rev: 5.12.0
       hooks:
       - id: isort
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
   -   repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.3.0
+      rev: v4.4.0
       hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: trailing-whitespace
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: mixed-line-ending
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
```

### Comparing `sunraster-0.4.3/CHANGELOG.rst` & `sunraster-0.5.0rc1/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+0.5.0 (2023-06-06)
+==================
+
+Breaking Changes
+----------------
+
+- Increased the minimum version of ``sunpy`` to 5.0.0
+- Increased the minimum version of ``ndcube`` to 2.1.2
+- Increased the minimum version of Python to 3.9
+
 0.4.3 (2022-10-06)
 ==================
 
 Bug Fixes
 ---------
 
 - Fixed SPICE reader failing on FITS files containing ``WCSDVARR`` HDUs (with additional distortion information), by ignoring these HDUs. (`#215 <https://github.com/sunpy/sunraster/pull/215>`__)
```

### Comparing `sunraster-0.4.3/LICENSE.rst` & `sunraster-0.5.0rc1/LICENSE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2013-2021 The SunPy developers
+Copyright (c) 2013-2022 The SunPy Developers
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 * Redistributions of source code must retain the above copyright
```

### Comparing `sunraster-0.4.3/PKG-INFO` & `sunraster-0.5.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: sunraster
-Version: 0.4.3
+Version: 0.5.0rc1
 Summary: sunraster is an open-source Python library that provides the tools to read in and analyze spectrogram data.
 Home-page: https://docs.sunpy.org/projects/sunraster/en/stable/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Keywords: solar physics,solar,science,sun,wcs,coordinates,spectra,raster
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: sunraster
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: instr
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.rst
@@ -102,15 +102,15 @@
 
 For more information on contributing to sunraster, please read SunPy's `Newcomers' guide`_.
 
 .. _SunPy mailing list: https://groups.google.com/forum/#!forum/sunpy
 .. _Developers Guide: https://docs.sunpy.org/en/latest/dev_guide/index.html
 .. _`#sunpy:openastronomy.org`: https://chat.openastronomy.org/#/room/#sunpy:openastronomy.org
 .. _issues page: https://github.com/sunpy/sunraster/issues
-.. _Newcomers' guide: https://docs.sunpy.org/en/latest/dev_guide/newcomers.html
+.. _Newcomers' guide: https://docs.sunpy.org/en/latest/dev_guide/contents/newcomers.html
 
 Code of Conduct
 ===============
 
 When you are interacting with the SunPy community you are asked to follow our `Code of Conduct`_.
 
-.. _Code of Conduct: https://docs.sunpy.org/en/latest/code_of_conduct.html
+.. _Code of Conduct: https://sunpy.org/coc
```

### Comparing `sunraster-0.4.3/README.rst` & `sunraster-0.5.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 For more information on contributing to sunraster, please read SunPy's `Newcomers' guide`_.
 
 .. _SunPy mailing list: https://groups.google.com/forum/#!forum/sunpy
 .. _Developers Guide: https://docs.sunpy.org/en/latest/dev_guide/index.html
 .. _`#sunpy:openastronomy.org`: https://chat.openastronomy.org/#/room/#sunpy:openastronomy.org
 .. _issues page: https://github.com/sunpy/sunraster/issues
-.. _Newcomers' guide: https://docs.sunpy.org/en/latest/dev_guide/newcomers.html
+.. _Newcomers' guide: https://docs.sunpy.org/en/latest/dev_guide/contents/newcomers.html
 
 Code of Conduct
 ===============
 
 When you are interacting with the SunPy community you are asked to follow our `Code of Conduct`_.
 
-.. _Code of Conduct: https://docs.sunpy.org/en/latest/code_of_conduct.html
+.. _Code of Conduct: https://sunpy.org/coc
```

### Comparing `sunraster-0.4.3/changelog/README.rst` & `sunraster-0.5.0rc1/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/Makefile` & `sunraster-0.5.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/conf.py` & `sunraster-0.5.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/data_types/raster.rst` & `sunraster-0.5.0rc1/docs/data_types/raster.rst`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/data_types/spectrogram.rst` & `sunraster-0.5.0rc1/docs/data_types/spectrogram.rst`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/index.rst` & `sunraster-0.5.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/installation.rst` & `sunraster-0.5.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/docs/make.bat` & `sunraster-0.5.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/pyproject.toml` & `sunraster-0.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/setup.cfg` & `sunraster-0.5.0rc1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 license_file = LICENSE.rst
 url = https://docs.sunpy.org/projects/sunraster/en/stable/
 edit_on_github = True
 github_project = sunpy/sunraster
 platform = any
 keywords = solar physics, solar, science, sun, wcs, coordinates, spectra, raster
 classifiers = 
-	Development Status :: 5 - Production/Stable
+	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
-python_requires = >=3.8
+python_requires = >=3.9
 packages = find:
 include_package_data = True
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	numpy
 	astropy
-	ndcube[plotting]>=2.0.1
+	ndcube[plotting]>=2.1.2
 
 [options.extras_require]
 instr = 
-	sunpy>=4.0.0
+	sunpy>=5.0.0rc1
 tests = 
 	pytest-astropy
 docs = 
 	sphinx
 	sphinx_automodapi
 	sphinx-changelog
 	sphinx-gallery
@@ -69,14 +69,15 @@
 	ignore:numpy.ufunc size changed:RuntimeWarning
 	ignore:numpy.ndarray size changed:RuntimeWarning
 	ignore:invalid value encountered in sqrt:RuntimeWarning
 	ignore::astropy.wcs.wcs.FITSFixedWarning
 	ignore::astropy.io.fits.verify.VerifyWarning
 	ignore:target cannot be converted to ICRS, so will not be set on SpectralCoord
 	ignore: invalid value encountered in true_divide
+	ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning
 
 [pycodestyle]
 max_line_length = 120
 
 [flake8]
 max-line-length = 120
 exclude =
```

### Comparing `sunraster-0.4.3/setup.py` & `sunraster-0.5.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python
-# Licensed under a 3-clause BSD style license - see LICENSE.rst
-
+from setuptools import setup  # isort:skip
 import os
 from itertools import chain
 
-from setuptools import setup
-from setuptools.config import read_configuration
+try:
+    # Recommended for setuptools 61.0.0+
+    # (though may disappear in the future)
+    from setuptools.config.setupcfg import read_configuration
+except ImportError:
+    from setuptools.config import read_configuration
 
-##############################################
-# Programmatically generate some extras combos
-##############################################
+################################################################################
+# Programmatically generate some extras combos.
+################################################################################
 extras = read_configuration("setup.cfg")["options"]["extras_require"]
 
 # Dev is everything
 extras["dev"] = list(chain(*extras.values()))
 
 # All is everything but tests and docs
 exclude_keys = ("tests", "docs", "dev")
```

### Comparing `sunraster-0.4.3/sunraster/extern/meta.py` & `sunraster-0.5.0rc1/sunraster/extern/meta.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/extern/tests/test_meta.py` & `sunraster-0.5.0rc1/sunraster/extern/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/instr/spice.py` & `sunraster-0.5.0rc1/sunraster/instr/spice.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/instr/tests/test_spice.py` & `sunraster-0.5.0rc1/sunraster/instr/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/meta.py` & `sunraster-0.5.0rc1/sunraster/meta.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/spectrogram.py` & `sunraster-0.5.0rc1/sunraster/spectrogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 SUPPORTED_EXPOSURE_NAMES += [name.upper() for name in SUPPORTED_EXPOSURE_NAMES] + [
     name.capitalize() for name in SUPPORTED_EXPOSURE_NAMES
 ]
 SUPPORTED_EXPOSURE_NAMES = np.array(SUPPORTED_EXPOSURE_NAMES)
 
 
 class SpectrogramABC(abc.ABC):
-
     # Abstract Base Class to define the basic API of Spectrogram classes.
 
     @abc.abstractproperty
     def spectral_axis(self):
         """
         Return the spectral coordinates for each pixel.
         """
@@ -544,15 +543,14 @@
     new_data: `numpy.ndarray`
         Data array with exposure time corrected for.
     new_uncertainty: `astropy.nddata.nduncertainty.NDUncertainty`
         The uncertainty of each element in new_data.
     new_unit: `astropy.unit.Unit`
         Unit of new_data array after exposure time correction.
     """
-
     # If force is not set to True and unit already includes inverse time,
     # raise error as exposure time correction has probably already been
     # applied and should not be applied again.
     if force is not True and u.s in unit.decompose().bases:
         raise ValueError(APPLY_EXPOSURE_TIME_ERROR)
     else:
         # Else, either unit does not include inverse time and so
@@ -589,15 +587,14 @@
     new_data: `numpy.ndarray`
         Data array with exposure time corrected for.
     new_uncertainty: `astropy.nddata.nduncertainty.NDUncertainty`
         The uncertainty of each element in new_data.
     new_unit: `astropy.unit.Unit`
         Unit of new_data array after exposure time correction.
     """
-
     # If force is not set to True and unit does not include inverse time,
     # raise error as exposure time correction has probably already been
     # undone and should not be undone again.
     if force is not True and u.s in (unit * u.s).decompose().bases:
         raise ValueError(UNDO_EXPOSURE_TIME_ERROR)
     else:
         # Else, either unit does include inverse time and so
```

### Comparing `sunraster-0.4.3/sunraster/spectrogram_sequence.py` & `sunraster-0.5.0rc1/sunraster/spectrogram_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,27 +122,36 @@
             for i, cube in enumerate(self):
                 self.data[i]._time_name, self.data[i]._time_loc = _find_axis_name(
                     SUPPORTED_TIME_NAMES,
                     cube.wcs.world_axis_physical_types,
                     cube.extra_coords,
                     cube.meta,
                 )
-                (self.data[i]._longitude_name, self.data[i]._longitude_loc,) = _find_axis_name(
+                (
+                    self.data[i]._longitude_name,
+                    self.data[i]._longitude_loc,
+                ) = _find_axis_name(
                     SUPPORTED_LONGITUDE_NAMES,
                     cube.wcs.world_axis_physical_types,
                     cube.extra_coords,
                     cube.meta,
                 )
-                (self.data[i]._latitude_name, self.data[i]._latitude_loc,) = _find_axis_name(
+                (
+                    self.data[i]._latitude_name,
+                    self.data[i]._latitude_loc,
+                ) = _find_axis_name(
                     SUPPORTED_LATITUDE_NAMES,
                     cube.wcs.world_axis_physical_types,
                     cube.extra_coords,
                     cube.meta,
                 )
-                (self.data[i]._spectral_name, self.data[i]._spectral_loc,) = _find_axis_name(
+                (
+                    self.data[i]._spectral_name,
+                    self.data[i]._spectral_loc,
+                ) = _find_axis_name(
                     SUPPORTED_SPECTRAL_NAMES,
                     cube.wcs.world_axis_physical_types,
                     cube.extra_coords,
                     cube.meta,
                 )
         data0 = self.data[0]
         if data0._time_name:
@@ -238,15 +247,18 @@
             # Slit step axis name.
             if self._common_axis is not None:
                 self._single_scan_instrument_axes_types[self._common_axis] = self._slit_step_axis_name
             # Spectral axis name.
             # If spectral name not present in raster cube, try finding it.
             if not self.data[0]._spectral_name:
                 for i, cube in enumerate(self):
-                    (self.data[i]._spectral_name, self.data[i]._spectral_name,) = _find_axis_name(
+                    (
+                        self.data[i]._spectral_name,
+                        self.data[i]._spectral_name,
+                    ) = _find_axis_name(
                         SUPPORTED_SPECTRAL_NAMES,
                         cube.wcs.world_axis_physical_types,
                         cube.extra_coords,
                         cube.meta,
                     )
             spectral_name = self.data[0]._spectral_name
             array_axis_physical_types = self.data[0].array_axis_physical_types
```

### Comparing `sunraster-0.4.3/sunraster/tests/data/solo_L2_spice-n-ras-db_20200602T081733_V01_12583760-000.fits` & `sunraster-0.5.0rc1/sunraster/tests/data/solo_L2_spice-n-ras-db_20200602T081733_V01_12583760-000.fits`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/tests/data/solo_L2_spice-n-sit_20200620T235901_V01_16777431-000.fits` & `sunraster-0.5.0rc1/sunraster/tests/data/solo_L2_spice-n-sit_20200620T235901_V01_16777431-000.fits`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/tests/test_spectrogram.py` & `sunraster-0.5.0rc1/sunraster/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/tests/test_spectrogramsequence.py` & `sunraster-0.5.0rc1/sunraster/tests/test_spectrogramsequence.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster/version.py` & `sunraster-0.5.0rc1/sunraster/version.py`

 * *Files identical despite different names*

### Comparing `sunraster-0.4.3/sunraster.egg-info/PKG-INFO` & `sunraster-0.5.0rc1/sunraster.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: sunraster
-Version: 0.4.3
+Version: 0.5.0rc1
 Summary: sunraster is an open-source Python library that provides the tools to read in and analyze spectrogram data.
 Home-page: https://docs.sunpy.org/projects/sunraster/en/stable/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Keywords: solar physics,solar,science,sun,wcs,coordinates,spectra,raster
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: sunraster
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: instr
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.rst
@@ -102,15 +102,15 @@
 
 For more information on contributing to sunraster, please read SunPy's `Newcomers' guide`_.
 
 .. _SunPy mailing list: https://groups.google.com/forum/#!forum/sunpy
 .. _Developers Guide: https://docs.sunpy.org/en/latest/dev_guide/index.html
 .. _`#sunpy:openastronomy.org`: https://chat.openastronomy.org/#/room/#sunpy:openastronomy.org
 .. _issues page: https://github.com/sunpy/sunraster/issues
-.. _Newcomers' guide: https://docs.sunpy.org/en/latest/dev_guide/newcomers.html
+.. _Newcomers' guide: https://docs.sunpy.org/en/latest/dev_guide/contents/newcomers.html
 
 Code of Conduct
 ===============
 
 When you are interacting with the SunPy community you are asked to follow our `Code of Conduct`_.
 
-.. _Code of Conduct: https://docs.sunpy.org/en/latest/code_of_conduct.html
+.. _Code of Conduct: https://sunpy.org/coc
```

### Comparing `sunraster-0.4.3/sunraster.egg-info/SOURCES.txt` & `sunraster-0.5.0rc1/sunraster.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
-azure-pipelines.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .circleci/config.yml
 .circleci/early_exit.sh
+.github/workflows/ci.yml
+.github/workflows/draft-pdf.yml
 changelog/README.rst
 docs/Makefile
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/data_types/index.rst
 docs/data_types/raster.rst
 docs/data_types/spectrogram.rst
+joss_paper/paper.bib
+joss_paper/paper.md
 sunraster/__init__.py
 sunraster/_version.py
 sunraster/meta.py
 sunraster/spectrogram.py
 sunraster/spectrogram_sequence.py
 sunraster/version.py
 sunraster.egg-info/PKG-INFO
```

