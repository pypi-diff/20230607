# Comparing `tmp/gemseo-fmu-1.0.0.tar.gz` & `tmp/gemseo-fmu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-fmu-1.0.0.tar", last modified: Mon Jan 16 14:07:43 2023, max compression
+gzip compressed data, was "gemseo-fmu-1.0.1.tar", last modified: Wed Jun  7 08:46:21 2023, max compression
```

## Comparing `gemseo-fmu-1.0.0.tar` & `gemseo-fmu-1.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.877152 gemseo-fmu-1.0.0/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      463 2022-07-26 12:42:26.000000 gemseo-fmu-1.0.0/.gitattributes
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      189 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.0/.gitignore
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      170 2023-01-06 14:11:35.000000 gemseo-fmu-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2524 2022-08-29 06:48:12.000000 gemseo-fmu-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     9105 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.0/.pylintrc
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      961 2023-01-16 10:29:54.000000 gemseo-fmu-1.0.0/CHANGELOG.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1865 2023-01-16 10:28:24.000000 gemseo-fmu-1.0.0/CREDITS.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7652 2021-10-11 07:26:02.000000 gemseo-fmu-1.0.0/LICENSE.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.865152 gemseo-fmu-1.0.0/LICENSES/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7652 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.0/LICENSES/LGPLv3.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.865152 gemseo-fmu-1.0.0/LICENSES/headers/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      729 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.0/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      334 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      710 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.0/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3388 2023-01-16 14:07:43.877152 gemseo-fmu-1.0.0/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2430 2023-01-16 14:06:56.000000 gemseo-fmu-1.0.0/README.rst
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.866152 gemseo-fmu-1.0.0/examples/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3166 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/examples/example_fmu_mass_damper.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2086 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/examples/example_fmu_sellar_jacobians.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2807 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/examples/example_fmu_sellar_mdo_analysis.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     4377 2022-08-26 15:15:12.000000 gemseo-fmu-1.0.0/examples/example_ishigami_sensitivity.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.862152 gemseo-fmu-1.0.0/fmu_files/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.869152 gemseo-fmu-1.0.0/fmu_files/linux/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   585847 2022-08-26 11:13:40.000000 gemseo-fmu-1.0.0/fmu_files/linux/IshigamiFunction.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   607544 2022-08-26 11:13:40.000000 gemseo-fmu-1.0.0/fmu_files/linux/Mass_Damper.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   586540 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/fmu_files/linux/Sellar1.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   585063 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/fmu_files/linux/Sellar2.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   587500 2022-08-26 11:13:40.000000 gemseo-fmu-1.0.0/fmu_files/linux/SellarSystem.fmu
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.873152 gemseo-fmu-1.0.0/fmu_files/win32/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   726790 2022-08-26 11:13:40.000000 gemseo-fmu-1.0.0/fmu_files/win32/IshigamiFunction.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   745560 2022-08-26 11:13:40.000000 gemseo-fmu-1.0.0/fmu_files/win32/Mass_Damper.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   733740 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/fmu_files/win32/Sellar1.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   725536 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/fmu_files/win32/Sellar2.fmu
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)   728458 2022-08-26 11:13:40.000000 gemseo-fmu-1.0.0/fmu_files/win32/SellarSystem.fmu
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.874152 gemseo-fmu-1.0.0/problems/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      735 2022-08-29 06:47:40.000000 gemseo-fmu-1.0.0/problems/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     8267 2022-08-26 12:04:35.000000 gemseo-fmu-1.0.0/problems/sellar.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      611 2022-07-22 12:40:49.000000 gemseo-fmu-1.0.0/pyproject.toml
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.875152 gemseo-fmu-1.0.0/requirements/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       79 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.0/requirements/check.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      596 2022-08-26 12:30:55.000000 gemseo-fmu-1.0.0/requirements/check.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      104 2022-08-26 15:33:59.000000 gemseo-fmu-1.0.0/requirements/conda.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       12 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.0/requirements/dist.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1373 2022-07-26 08:01:56.000000 gemseo-fmu-1.0.0/requirements/dist.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2124 2023-01-16 13:22:44.000000 gemseo-fmu-1.0.0/requirements/test-python3.10.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2287 2023-01-16 13:22:44.000000 gemseo-fmu-1.0.0/requirements/test-python3.7.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2122 2023-01-16 13:22:44.000000 gemseo-fmu-1.0.0/requirements/test-python3.8.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2122 2023-01-16 13:22:44.000000 gemseo-fmu-1.0.0/requirements/test-python3.9.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1559 2023-01-16 14:07:43.878152 gemseo-fmu-1.0.0/setup.cfg
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      839 2022-08-04 07:30:27.000000 gemseo-fmu-1.0.0/setup.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.863152 gemseo-fmu-1.0.0/src/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.876152 gemseo-fmu-1.0.0/src/gemseo_fmu/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      803 2022-08-26 12:12:09.000000 gemseo-fmu-1.0.0/src/gemseo_fmu/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    11943 2023-01-06 11:33:33.000000 gemseo-fmu-1.0.0/src/gemseo_fmu/fmu_discipline.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.877152 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3388 2023-01-16 14:07:43.000000 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1472 2023-01-16 14:07:43.000000 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/SOURCES.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        1 2023-01-16 14:07:43.000000 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/dependency_links.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       41 2023-01-16 14:07:43.000000 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/entry_points.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       70 2023-01-16 14:07:43.000000 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/requires.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       11 2023-01-16 14:07:43.000000 gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/top_level.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.877152 gemseo-fmu-1.0.0/tests/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      763 2022-08-26 12:11:16.000000 gemseo-fmu-1.0.0/tests/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     6152 2023-01-06 11:32:22.000000 gemseo-fmu-1.0.0/tests/test_fmu_discipline.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     4292 2023-01-06 10:51:15.000000 gemseo-fmu-1.0.0/tests/test_sellar_problem_with_fmu_disc.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3725 2023-01-06 10:27:47.000000 gemseo-fmu-1.0.0/tox.ini
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2023-01-16 14:07:43.877152 gemseo-fmu-1.0.0/utils/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2106 2022-08-26 12:04:36.000000 gemseo-fmu-1.0.0/utils/discipline_plots.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     4781 2022-08-04 07:30:23.000000 gemseo-fmu-1.0.0/utils/input_functions.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.325979 gemseo-fmu-1.0.1/
+-rw-r--r--   0 ad        (1000) ad        (1000)      463 2022-07-26 12:42:26.000000 gemseo-fmu-1.0.1/.gitattributes
+-rw-r--r--   0 ad        (1000) ad        (1000)      189 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.1/.gitignore
+-rw-r--r--   0 ad        (1000) ad        (1000)      170 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 ad        (1000) ad        (1000)     3051 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 ad        (1000) ad        (1000)     9105 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.1/.pylintrc
+-rw-r--r--   0 ad        (1000) ad        (1000)     1034 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     1865 2023-01-16 10:28:24.000000 gemseo-fmu-1.0.1/CREDITS.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     7652 2021-10-11 07:26:02.000000 gemseo-fmu-1.0.1/LICENSE.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.315979 gemseo-fmu-1.0.1/LICENSES/
+-rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.1/LICENSES/LGPLv3.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.316979 gemseo-fmu-1.0.1/LICENSES/headers/
+-rw-r--r--   0 ad        (1000) ad        (1000)      729 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.1/LICENSES/headers/BSD-0-Clause.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      334 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.1/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      710 2022-03-24 13:18:51.000000 gemseo-fmu-1.0.1/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     3338 2023-06-07 08:46:21.325979 gemseo-fmu-1.0.1/PKG-INFO
+-rw-r--r--   0 ad        (1000) ad        (1000)     2430 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.316979 gemseo-fmu-1.0.1/examples/
+-rw-r--r--   0 ad        (1000) ad        (1000)     3202 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/examples/example_fmu_mass_damper.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2122 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/examples/example_fmu_sellar_jacobians.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2837 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/examples/example_fmu_sellar_mdo_analysis.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4413 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/examples/example_ishigami_sensitivity.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.313979 gemseo-fmu-1.0.1/fmu_files/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.318979 gemseo-fmu-1.0.1/fmu_files/linux/
+-rw-r--r--   0 ad        (1000) ad        (1000)   585847 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/linux/IshigamiFunction.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   607544 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/linux/Mass_Damper.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   586540 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/linux/Sellar1.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   585063 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/linux/Sellar2.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   587500 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/linux/SellarSystem.fmu
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.321979 gemseo-fmu-1.0.1/fmu_files/win32/
+-rw-r--r--   0 ad        (1000) ad        (1000)   726790 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/win32/IshigamiFunction.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   745560 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/win32/Mass_Damper.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   733740 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/win32/Sellar1.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   725536 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/win32/Sellar2.fmu
+-rw-r--r--   0 ad        (1000) ad        (1000)   728458 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/fmu_files/win32/SellarSystem.fmu
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.322979 gemseo-fmu-1.0.1/problems/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/problems/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8171 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/problems/sellar.py
+-rw-r--r--   0 ad        (1000) ad        (1000)      611 2023-06-02 10:15:00.000000 gemseo-fmu-1.0.1/pyproject.toml
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.323979 gemseo-fmu-1.0.1/requirements/
+-rw-r--r--   0 ad        (1000) ad        (1000)       79 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.1/requirements/check.in
+-rw-r--r--   0 ad        (1000) ad        (1000)      573 2023-06-02 10:10:39.000000 gemseo-fmu-1.0.1/requirements/check.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      104 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/requirements/conda.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       12 2022-07-22 10:45:42.000000 gemseo-fmu-1.0.1/requirements/dist.in
+-rw-r--r--   0 ad        (1000) ad        (1000)     1493 2023-06-02 10:11:15.000000 gemseo-fmu-1.0.1/requirements/dist.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2187 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/requirements/test-python3.10.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2287 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/requirements/test-python3.7.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2277 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/requirements/test-python3.8.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2277 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/requirements/test-python3.9.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     1552 2023-06-07 08:46:21.325979 gemseo-fmu-1.0.1/setup.cfg
+-rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-08-04 07:30:27.000000 gemseo-fmu-1.0.1/setup.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.313979 gemseo-fmu-1.0.1/src/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.323979 gemseo-fmu-1.0.1/src/gemseo_fmu/
+-rw-r--r--   0 ad        (1000) ad        (1000)      803 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/src/gemseo_fmu/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)    12051 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/src/gemseo_fmu/fmu_discipline.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.324979 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/
+-rw-r--r--   0 ad        (1000) ad        (1000)     3338 2023-06-07 08:46:21.000000 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/PKG-INFO
+-rw-r--r--   0 ad        (1000) ad        (1000)     1472 2023-06-07 08:46:21.000000 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/SOURCES.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-06-07 08:46:21.000000 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/dependency_links.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       41 2023-06-07 08:46:21.000000 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/entry_points.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       67 2023-06-07 08:46:21.000000 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/requires.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       11 2023-06-07 08:46:21.000000 gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/top_level.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.324979 gemseo-fmu-1.0.1/tests/
+-rw-r--r--   0 ad        (1000) ad        (1000)      798 2023-06-02 10:16:16.000000 gemseo-fmu-1.0.1/tests/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     6188 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/tests/test_fmu_discipline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4326 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/tests/test_sellar_problem_with_fmu_disc.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3566 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/tox.ini
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 08:46:21.324979 gemseo-fmu-1.0.1/utils/
+-rw-r--r--   0 ad        (1000) ad        (1000)     2142 2023-06-07 08:45:36.000000 gemseo-fmu-1.0.1/utils/discipline_plots.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4817 2023-06-02 10:23:31.000000 gemseo-fmu-1.0.1/utils/input_functions.py
```

### Comparing `gemseo-fmu-1.0.0/.pylintrc` & `gemseo-fmu-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/CREDITS.rst` & `gemseo-fmu-1.0.1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/LICENSE.txt` & `gemseo-fmu-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/LICENSES/LGPLv3.txt` & `gemseo-fmu-1.0.1/LICENSES/LGPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-fmu-1.0.1/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/LICENSES/headers/LGPL-3.0.txt` & `gemseo-fmu-1.0.1/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/PKG-INFO` & `gemseo-fmu-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: gemseo-fmu
-Version: 1.0.0
+Version: 1.0.1
 Summary: GEMSEO plugin for FMU dynamic models.
 Home-page: https://www.irt-saintexupery.com
 Author: GEMSEO team
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-fmu-1.0.0/README.rst` & `gemseo-fmu-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/examples/example_fmu_mass_damper.py` & `gemseo-fmu-1.0.1/examples/example_fmu_mass_damper.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """
 Create a discipline from a FMU file
 ===================================
 """
 # %%
+from __future__ import annotations
+
 import sys
 from pathlib import Path
 
 import numpy as np
 from gemseo_fmu.fmu_discipline import FMUDiscipline
 
 from utils.discipline_plots import plot_discipline_fmu
```

### Comparing `gemseo-fmu-1.0.0/examples/example_fmu_sellar_jacobians.py` & `gemseo-fmu-1.0.1/examples/example_fmu_sellar_jacobians.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """
 Create a discipline for the Sellar problem from a FMU file and computes its jacobians
 ==========================================
 """
+from __future__ import annotations
+
 import sys
 from pathlib import Path
 
 from problems.sellar import Sellar1
 from problems.sellar import Sellar2
 from problems.sellar import SellarSystem
```

### Comparing `gemseo-fmu-1.0.0/examples/example_fmu_sellar_mdo_analysis.py` & `gemseo-fmu-1.0.1/examples/example_fmu_sellar_mdo_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """
 FMU-based Sellar MDO use case
 =============================
 """
+from __future__ import annotations
+
 import sys
 from pathlib import Path
 
-from gemseo.api import configure_logger
-from gemseo.api import create_design_space
-from gemseo.api import create_scenario
+from gemseo import configure_logger
+from gemseo import create_design_space
+from gemseo import create_scenario
 
 from problems.sellar import Sellar1
 from problems.sellar import Sellar2
 from problems.sellar import SellarSystem
 
 configure_logger()
 
@@ -65,12 +67,12 @@
 scenario.add_constraint("c_2", "ineq")
 scenario.set_differentiation_method("finite_differences", 1e-6)
 scenario.execute({"algo": "SLSQP", "max_iter": 15})
 
 # %%
 # Analyze the results
 # -------------------
-optimum = scenario.get_optimum()
+optimum = scenario.optimization_result
 print(optimum)
 x_opt = scenario.design_space.get_current_value(as_dict=True)
 print(x_opt)
 scenario.post_process("OptHistoryView", show=True, save=False)
```

### Comparing `gemseo-fmu-1.0.0/examples/example_ishigami_sensitivity.py` & `gemseo-fmu-1.0.1/examples/example_ishigami_sensitivity.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 # NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Comparing sensitivity indices."""
+from __future__ import annotations
+
 import sys
 from pathlib import Path
 
 from gemseo.algos.parameter_space import ParameterSpace
 from gemseo.uncertainty.sensitivity.correlation.analysis import CorrelationAnalysis
 from gemseo.uncertainty.sensitivity.morris.analysis import MorrisAnalysis
 from gemseo_fmu.fmu_discipline import FMUDiscipline
```

### Comparing `gemseo-fmu-1.0.0/fmu_files/linux/IshigamiFunction.fmu` & `gemseo-fmu-1.0.1/fmu_files/linux/IshigamiFunction.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/linux/Mass_Damper.fmu` & `gemseo-fmu-1.0.1/fmu_files/linux/Mass_Damper.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/linux/Sellar1.fmu` & `gemseo-fmu-1.0.1/fmu_files/linux/Sellar1.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/linux/Sellar2.fmu` & `gemseo-fmu-1.0.1/fmu_files/linux/Sellar2.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/linux/SellarSystem.fmu` & `gemseo-fmu-1.0.1/fmu_files/linux/SellarSystem.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/win32/IshigamiFunction.fmu` & `gemseo-fmu-1.0.1/fmu_files/win32/IshigamiFunction.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/win32/Mass_Damper.fmu` & `gemseo-fmu-1.0.1/fmu_files/win32/Mass_Damper.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/win32/Sellar1.fmu` & `gemseo-fmu-1.0.1/fmu_files/win32/Sellar1.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/win32/Sellar2.fmu` & `gemseo-fmu-1.0.1/fmu_files/win32/Sellar2.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/fmu_files/win32/SellarSystem.fmu` & `gemseo-fmu-1.0.1/fmu_files/win32/SellarSystem.fmu`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/problems/__init__.py` & `gemseo-fmu-1.0.1/problems/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+from __future__ import annotations
```

### Comparing `gemseo-fmu-1.0.0/problems/sellar.py` & `gemseo-fmu-1.0.1/problems/sellar.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
-r"""The disciplines for the MDO problem proposed by Sellar et al. in
+r"""The disciplines for the MDO problem proposed by Sellar et al. in.
 
 Sellar, R., Batill, S., & Renaud, J. (1996).
 Response surface based, concurrent subspace optimization
 for multidisciplinary system design.
 In 34th aerospace sciences meeting and exhibit (p. 714).
 
 The MDO problem is written as follows:
@@ -70,24 +70,23 @@
 - :class:`.Sellar2`:
   this :class:`.MDODiscipline` computes :math:`y_2`
   from :math:`y_1`, :math:`x_{shared,1}` and :math:`x_{shared,2}`.
 - :class:`.SellarSystem`:
   this :class:`.MDODiscipline` computes both objective and constraints
   from :math:`y_1`, :math:`y_2`, :math:`x_{local}` and :math:`x_{shared,2}`.
 """
+from __future__ import annotations
+
 from cmath import exp
 from cmath import sqrt
-from typing import Iterable
-from typing import Optional
 
 import numpy as np
 from gemseo_fmu.fmu_discipline import FMUDiscipline
 from numpy import array
 from numpy import atleast_2d
-from numpy import ndarray
 from numpy import ones
 from numpy import zeros
 
 Y_1 = "y_1"
 Y_2 = "y_2"
 X_SHARED_1 = "x_shared_1"
 X_SHARED_2 = "x_shared_2"
@@ -151,15 +150,15 @@
         return y_2[0] - 24.0
 
     def _compute_jacobian(
         self,
         inputs=None,  # type: Optional[Iterable[str]]
         outputs=None,  # type: Optional[Iterable[str]]
     ):  # type: (...) -> None
-        self._init_jacobian(inputs, outputs, with_zeros=True)
+        self._init_jacobian(inputs, outputs)
 
         x_local, _, y_1, y_2 = self.get_inputs_by_name([X_LOCAL, X_SHARED_2, Y_1, Y_2])
         self.jac[C_1][Y_1] = atleast_2d(array([-2.0 * y_1]))
         self.jac[C_2][Y_2] = ones((1, 1))
         self.jac[OBJ][X_LOCAL] = atleast_2d(array([2.0 * x_local[0]]))
         self.jac[OBJ][X_SHARED_1] = atleast_2d(array([0.0]))
         self.jac[OBJ][X_SHARED_2] = atleast_2d(array([1.0]))
@@ -189,15 +188,15 @@
         return sqrt(x_shared[0] ** 2 + x_shared[1] + x_local[0] - 0.2 * y_2[0])
 
     def _compute_jacobian(
         self,
         inputs=None,  # type: Optional[Iterable[str]]
         outputs=None,  # type: Optional[Iterable[str]]
     ):  # type: (...) -> None
-        self._init_jacobian(inputs, outputs, with_zeros=True)
+        self._init_jacobian(inputs, outputs)
         x_local, x_shared_1, x_shared_2, y_2 = self.get_inputs_by_name(
             [X_LOCAL, X_SHARED_1, X_SHARED_2, Y_2]
         )
         x_shared = np.concatenate([x_shared_1, x_shared_2], axis=None)
 
         inv_denom = 1.0 / (self.compute_y_1(x_local, x_shared, y_2))
         self.jac[Y_1] = {}
@@ -211,15 +210,15 @@
     """The discipline to compute the coupling variable :math:`y_2`."""
 
     def _compute_jacobian(
         self,
         inputs=None,  # type: Optional[Iterable[str]]
         outputs=None,  # type: Optional[Iterable[str]]
     ):  # type: (...) -> None
-        self._init_jacobian(inputs, outputs, with_zeros=True)
+        self._init_jacobian(inputs, outputs)
         y_1 = self.get_inputs_by_name(Y_1)
         self.jac[Y_2] = {}
         self.jac[Y_2][X_LOCAL] = zeros((1, 1))
         self.jac[Y_2][X_SHARED_1] = ones((1, 1))
         self.jac[Y_2][X_SHARED_2] = ones((1, 1))
         if y_1[0] < 0.0:
             self.jac[Y_2][Y_1] = -ones((1, 1))
```

### Comparing `gemseo-fmu-1.0.0/pyproject.toml` & `gemseo-fmu-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # logging settings identical to the defaults of gemseo.api.configure_logger()
 log_file_level = "INFO"
 log_file_date_format = "%H:%M:%S"
 log_file_format = "%(levelname)8s - %(asctime)s: %(message)s"
 # filterwarnings = ignore::pytest.PytestExperimentalApiWarning
 
 [tool.black]
-target-version = ['py37']
+target-version = ['py38']
```

### Comparing `gemseo-fmu-1.0.0/requirements/dist.txt` & `gemseo-fmu-1.0.1/requirements/dist.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile requirements/dist.in
 #
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.8.0
+build==0.10.0
     # via -r requirements/dist.in
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-commonmark==0.9.1
-    # via rich
-cryptography==37.0.4
+cryptography==41.0.1
     # via secretstorage
-docutils==0.19
+docutils==0.20.1
     # via readme-renderer
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.12.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
+jaraco-classes==3.2.3
+    # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==23.7.0
+keyring==23.13.1
     # via twine
-packaging==21.3
-    # via build
-pep517==0.12.0
+markdown-it-py==2.2.0
+    # via rich
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
+    # via jaraco-classes
+packaging==23.1
     # via build
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.12.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pyparsing==3.0.9
-    # via packaging
-readme-renderer==35.0
+pyproject-hooks==1.0.0
+    # via build
+readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==13.4.1
     # via twine
-secretstorage==3.3.2
+secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   build
-    #   pep517
-twine==4.0.1
+    #   pyproject-hooks
+twine==4.0.2
     # via -r requirements/dist.in
-urllib3==1.26.11
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-zipp==3.8.1
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `gemseo-fmu-1.0.0/requirements/test-python3.10.txt` & `gemseo-fmu-1.0.1/requirements/test-python3.8.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,114 +1,122 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.6
+contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-fmu (setup.py)
-coverage[toml]==7.0.3
+coverage[toml]==7.2.7
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
-docstring-inheritance==1.0.0
+docstring-inheritance==1.1.1
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
 gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-fmu (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via gemseo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-fmu (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
+pydantic==1.10.8
+    # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.0
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-fmu (setup.py)
     #   pytest-cov
     #   pytest-xdist
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via gemseo-fmu (setup.py)
-pytest-xdist==3.1.0
+pytest-xdist==3.3.1
     # via gemseo-fmu (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
+requests==2.31.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via gemseo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
-    # via gemseo
-typing-extensions==4.4.0
+tqdm==4.65.0
     # via gemseo
-urllib3==1.26.13
+typing-extensions==4.6.3
+    # via
+    #   gemseo
+    #   pydantic
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-fmu-1.0.0/requirements/test-python3.7.txt` & `gemseo-fmu-1.0.1/requirements/test-python3.7.txt`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/requirements/test-python3.8.txt` & `gemseo-fmu-1.0.1/requirements/test-python3.9.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,114 +1,122 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.6
+contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-fmu (setup.py)
-coverage[toml]==7.0.3
+coverage[toml]==7.2.7
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
-docstring-inheritance==1.0.0
+docstring-inheritance==1.1.1
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
 gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-fmu (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via gemseo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-fmu (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
+pydantic==1.10.8
+    # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.0
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-fmu (setup.py)
     #   pytest-cov
     #   pytest-xdist
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via gemseo-fmu (setup.py)
-pytest-xdist==3.1.0
+pytest-xdist==3.3.1
     # via gemseo-fmu (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
+requests==2.31.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via gemseo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
-    # via gemseo
-typing-extensions==4.4.0
+tqdm==4.65.0
     # via gemseo
-urllib3==1.26.13
+typing-extensions==4.6.3
+    # via
+    #   gemseo
+    #   pydantic
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-fmu-1.0.0/requirements/test-python3.9.txt` & `gemseo-fmu-1.0.1/requirements/test-python3.10.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,114 +1,118 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.6
+contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-fmu (setup.py)
-coverage[toml]==7.0.3
+coverage[toml]==7.2.7
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
-docstring-inheritance==1.0.0
+docstring-inheritance==1.1.1
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
 gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-fmu (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via gemseo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-fmu (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
+pydantic==1.10.8
+    # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.0
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-fmu (setup.py)
     #   pytest-cov
     #   pytest-xdist
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via gemseo-fmu (setup.py)
-pytest-xdist==3.1.0
+pytest-xdist==3.3.1
     # via gemseo-fmu (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
+requests==2.31.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via gemseo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
-    # via gemseo
-typing-extensions==4.4.0
+tqdm==4.65.0
     # via gemseo
-urllib3==1.26.13
+typing-extensions==4.6.3
+    # via
+    #   gemseo
+    #   pydantic
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
```

### Comparing `gemseo-fmu-1.0.0/setup.py` & `gemseo-fmu-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/src/gemseo_fmu/__init__.py` & `gemseo-fmu-1.0.1/src/gemseo_fmu/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/src/gemseo_fmu/fmu_discipline.py` & `gemseo-fmu-1.0.1/src/gemseo_fmu/fmu_discipline.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,18 @@
     - INFO = 4
     - VERBOSE = 5
     - DEBUG = 6
     - ALL = 7
     """
 
     SILENT_PYFMI_CS: ClassVar[bool] = True
-    """Whether to disable the PyFMI log on console. The default is ``True``."""
+    """Whether to disable the PyFMI log on console.
+
+    The default is ``True``.
+    """
 
     model: FMUModel
     """The PyFMI model."""
 
     def __init__(
         self,
         fmu_file_path: str | Path,
@@ -169,28 +172,30 @@
         self._unfiltered_data = self.__input_variables.copy()
         self._unfiltered_data.update(self.__parameters)
         self.input_data = {
             k: v
             for k, v in self._unfiltered_data.items()
             if isinstance(self._unfiltered_data[k][0], float)
         }
-        self.default_inputs = self.input_data
 
         history_outputs = history_outputs or []
         self.__history_outputs = history_outputs
         self.__history_outputs_with_suffix = []
         for history_output in self.__history_outputs:
             self.__history_outputs_with_suffix.append(f"{history_output}_history")
 
         # Define input/output grammar and default inputs
         self.__fmu_input_names = list(self.input_data.keys())
         self.__fmu_output_names = list(self.__output_variables.keys())
 
-        self.input_grammar.update(self.__fmu_input_names)
-        self.output_grammar.update(
+        self.input_grammar.update_from_names(self.__fmu_input_names)
+        self.default_inputs = {
+            k: v for k, v in self.input_data.items() if k in self.input_grammar
+        }
+        self.output_grammar.update_from_names(
             self.__fmu_output_names + self.__history_outputs_with_suffix
         )
 
         self.__model_simulation_results = {}
 
     def __check_simulate_options(self) -> None:
         """Check if the simulation options provided are PyFMI options.
```

### Comparing `gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/PKG-INFO` & `gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: gemseo-fmu
-Version: 1.0.0
+Version: 1.0.1
 Summary: GEMSEO plugin for FMU dynamic models.
 Home-page: https://www.irt-saintexupery.com
 Author: GEMSEO team
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-fmu-1.0.0/src/gemseo_fmu.egg-info/SOURCES.txt` & `gemseo-fmu-1.0.1/src/gemseo_fmu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemseo-fmu-1.0.0/tests/__init__.py` & `gemseo-fmu-1.0.1/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Tests for gemseo-fmu."""
+from __future__ import annotations
```

### Comparing `gemseo-fmu-1.0.0/tests/test_fmu_discipline.py` & `gemseo-fmu-1.0.1/tests/test_fmu_discipline.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Tests for FMUDiscipline."""
+from __future__ import annotations
+
 import re
 import sys
 from pathlib import Path
 from typing import Any
 
 import pytest
 from gemseo_fmu.fmu_discipline import FMUDiscipline
```

### Comparing `gemseo-fmu-1.0.0/tests/test_sellar_problem_with_fmu_disc.py` & `gemseo-fmu-1.0.1/tests/test_sellar_problem_with_fmu_disc.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Tests for the Sellar problem based on FMU models."""
+from __future__ import annotations
+
 import numpy as np
 import pytest
-from gemseo.api import create_design_space
-from gemseo.api import create_scenario
+from gemseo import create_design_space
+from gemseo import create_scenario
 from numpy import array
 from numpy import ones
 from numpy import zeros
 
 from .test_fmu_discipline import FMU_DIR_PATH
 from problems.sellar import Sellar1
 from problems.sellar import Sellar2
@@ -102,9 +104,9 @@
     objective_ref = array([2.0 + 0.0j, 1.0 + 0.0j])
     assert np.allclose(objective, objective_ref)
 
 
 def test_fmu_optim_results(fmu_scenario):
     """Test obtained optimal values when solving sellar problem with fmu discipline."""
     fmu_scenario.execute(input_data={"max_iter": 20, "algo": "SLSQP"})
-    optim_res = fmu_scenario.get_optimum()
+    optim_res = fmu_scenario.optimization_result
     assert pytest.approx(optim_res.f_opt) == 3.188547
```

### Comparing `gemseo-fmu-1.0.0/tox.ini` & `gemseo-fmu-1.0.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -24,31 +24,29 @@
 setenv =
     # Workaround matplotlib on windows server 2012 and gitlab-runner,
     # matplotlib cannot access a registry key and falls back to the WINDIR var
     # https://matplotlib.org/stable/api/font_manager_api.html#matplotlib.font_manager.win32FontDirectory.
     WINDIR = {env:WINDIR:C:\Windows}
     # Use a non GUI rendering backend for matplotlib.
     MPLBACKEND = AGG
-    py37: PATH = {envdir}{:}{envdir}\Library\mingw-w64\bin{:}{envdir}\Library\usr\bin{:}{envdir}\Library\bin{:}{envdir}\Scripts{:}{envdir}\bin{:}{env:PATH}
     # Define pytest options for using coverage.
     coverage: __COVERAGE_POSARGS=--cov --cov-config=setup.cfg --cov-report=xml --cov-report=html
 passenv =
     # See dev docs.
     GEMSEO_KEEP_IMAGE_COMPARISONS
 commands =
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
 conda_spec =
 skip_install = true
-whitelist_externals =
-    git
+whitelist_externals = pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files
 
 [testenv:doc]
 description = build documentation
 basepython = python3.9
@@ -73,40 +71,41 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-fmu[test]
 skip_install = true
 
 [testenv:update-deps-{doc,dist,check}]
 description = update the non test envs dependencies
 basepython = python3.9
 extras =
     doc: {[testenv:doc]extras}
 setenv =
 passenv =
 deps = pip-tools
 conda_spec =
 skip_install = true
-whitelist_externals = pip-compile
+whitelist_externals =
+    pip-compile
+    check: pre-commit
 commands =
     doc: pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra doc -o requirements/doc.txt
     dist: pip-compile --upgrade requirements/dist.in
     check: pip-compile --upgrade requirements/check.in
     check: pre-commit autoupdate
 
-[testenv:update-deps-test-py{37,38,39,310}]
+[testenv:update-deps-test-py{38,39,310}]
 description = update the test envs dependencies
 extras = {[testenv]extras}
 setenv =
 passenv =
 conda_spec =
 deps = pip-tools
-whitelist_externals = sed
 skip_install = true
 commands =
     pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra test -o requirements/test-{basepython}.txt
```

### Comparing `gemseo-fmu-1.0.0/utils/discipline_plots.py` & `gemseo-fmu-1.0.1/utils/discipline_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Plots for FMUDiscipline."""
+from __future__ import annotations
+
 import matplotlib.pyplot as plt
 
 
 def plot_discipline_fmu(
     discipline,
     x_name,
     variable_names=None,
```

### Comparing `gemseo-fmu-1.0.0/utils/input_functions.py` & `gemseo-fmu-1.0.1/utils/input_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #    INITIAL AUTHORS - initial API and implementation and/or initial documentation
 #        :author: Jorge CAMACHO CASERO
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Utility to create basic signals in the form of numpy arrays.
 
 It is useful to seamlessly generate input data usable by the FMUDiscipline.
 """
+from __future__ import annotations
+
 import pylab as plt
 import scipy.signal as signal
 from numpy import cos
 from numpy import exp
 from numpy import linspace
 from numpy import pi
 from numpy import random
@@ -68,15 +70,15 @@
 
 def chirp_wave(
     x, amplitude=1, f0=6, f1=1, t1=10, method="linear", phi=0, vertex_zero=True
 ):
     return amplitude * signal.chirp(x, f0, t1, f1, method, phi, vertex_zero)
 
 
-def pattern_wave(x, amplitude=1, pattern=[0.0, 1.0, 0.0, 1.0, 0.0, 1.0]):
+def pattern_wave(x, amplitude=1, pattern=(0.0, 1.0, 0.0, 1.0, 0.0, 1.0)):
     # pattern =  [0., 1., 1., 0., 1., 0., 0., 1.]
     return amplitude * repeat(pattern, len(x) / len(pattern))
 
 
 def noisy_wave(func, scale=1, size=0.9):
     sig_noise = random.normal(scale, size, func.shape)
     return func + sig_noise
```

