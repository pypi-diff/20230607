# Comparing `tmp/ruptures-1.1.8.tar.gz` & `tmp/ruptures-1.1.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruptures-1.1.8.tar", last modified: Wed Jun  7 13:10:58 2023, max compression
+gzip compressed data, was "ruptures-1.1.8rc1.tar", last modified: Wed Jun  7 12:33:10 2023, max compression
```

## Comparing `ruptures-1.1.8.tar` & `ruptures-1.1.8rc1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.849240 ruptures-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-07 13:10:30.000000 ruptures-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 13:10:30.000000 ruptures-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-07 13:10:58.849240 ruptures-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-07 13:10:30.000000 ruptures-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-07 13:10:30.000000 ruptures-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-07 13:10:58.853240 ruptures-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-07 13:10:30.000000 ruptures-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.841240 ruptures-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.841240 ruptures-1.1.8/src/ruptures/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.845240 ruptures-1.1.8/src/ruptures/costs/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costautoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costclinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costcosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costl1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costl2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costlinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costnormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costrank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/costrbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/costs/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.845240 ruptures-1.1.8/src/ruptures/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/datasets/pw_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/datasets/pw_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/datasets/pw_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/datasets/pw_wavy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.845240 ruptures-1.1.8/src/ruptures/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.845240 ruptures-1.1.8/src/ruptures/detection/_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   851723 2023-06-07 13:10:57.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd.c
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd_computation.c
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd_computation.h
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd_pelt_computation.c
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd_pelt_computation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/kernels.c
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/_detection/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/binseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/bottomup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/dynp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/kernelcpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/pelt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/detection/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.849240 ruptures-1.1.8/src/ruptures/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/hamming.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/hausdorff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/precisionrecall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/randindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/sanity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/metrics/timeerror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.849240 ruptures-1.1.8/src/ruptures/show/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/show/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.849240 ruptures-1.1.8/src/ruptures/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.849240 ruptures-1.1.8/src/ruptures/utils/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   790719 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix.c
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix_c.h
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/bnode.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/drawbkps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-07 13:10:30.000000 ruptures-1.1.8/src/ruptures/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.841240 ruptures-1.1.8/src/ruptures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:10:58.000000 ruptures-1.1.8/src/ruptures.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:58.849240 ruptures-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/test_bnode.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/test_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-07 13:10:30.000000 ruptures-1.1.8/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.280312 ruptures-1.1.8rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-07 12:33:10.280312 ruptures-1.1.8rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-07 12:33:10.284312 ruptures-1.1.8rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.264312 ruptures-1.1.8rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.268312 ruptures-1.1.8rc1/src/ruptures/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.268312 ruptures-1.1.8rc1/src/ruptures/costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costautoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costclinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costcosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costl1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costl2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costlinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costnormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costrank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/costrbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/costs/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.268312 ruptures-1.1.8rc1/src/ruptures/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/datasets/pw_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/datasets/pw_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/datasets/pw_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/datasets/pw_wavy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.272312 ruptures-1.1.8rc1/src/ruptures/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.276312 ruptures-1.1.8rc1/src/ruptures/detection/_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   851723 2023-06-07 12:33:08.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd.c
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd_computation.c
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd_computation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd_pelt_computation.c
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd_pelt_computation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/kernels.c
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/_detection/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/binseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/bottomup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/dynp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/kernelcpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/pelt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/detection/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.276312 ruptures-1.1.8rc1/src/ruptures/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/hausdorff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/precisionrecall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/randindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/sanity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/metrics/timeerror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.276312 ruptures-1.1.8rc1/src/ruptures/show/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/show/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.276312 ruptures-1.1.8rc1/src/ruptures/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.280312 ruptures-1.1.8rc1/src/ruptures/utils/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   790719 2023-06-07 12:33:09.000000 ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix.c
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/bnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/drawbkps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/src/ruptures/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 12:33:10.000000 ruptures-1.1.8rc1/src/ruptures/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.268312 ruptures-1.1.8rc1/src/ruptures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-07 12:33:10.000000 ruptures-1.1.8rc1/src/ruptures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-07 12:33:10.000000 ruptures-1.1.8rc1/src/ruptures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:33:10.000000 ruptures-1.1.8rc1/src/ruptures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 12:33:10.000000 ruptures-1.1.8rc1/src/ruptures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 12:33:10.000000 ruptures-1.1.8rc1/src/ruptures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:33:09.000000 ruptures-1.1.8rc1/src/ruptures.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:10.280312 ruptures-1.1.8rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/test_bnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/test_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-07 12:32:42.000000 ruptures-1.1.8rc1/tests/test_metrics.py
```

### Comparing `ruptures-1.1.8/LICENSE` & `ruptures-1.1.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/PKG-INFO` & `ruptures-1.1.8rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruptures
-Version: 1.1.8
+Version: 1.1.8rc1
 Summary: Change point detection for signals in Python.
 Home-page: https://github.com/deepcharles/ruptures/
 Author: Charles Truong, Laurent Oudre, Nicolas Vayatis
 Author-email: charles@doffy.net
 Maintainer: Charles Truong, Olivier Boulant
 License: BSD-2-Clause
 Project-URL: Documentation, https://centre-borelli.github.io/ruptures-docs/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ruptures Version: 1.1.8 Summary: Change point
+Metadata-Version: 2.1 Name: ruptures Version: 1.1.8rc1 Summary: Change point
 detection for signals in Python. Home-page: https://github.com/deepcharles/
 ruptures/ Author: Charles Truong, Laurent Oudre, Nicolas Vayatis Author-email:
 charles@doffy.net Maintainer: Charles Truong, Olivier Boulant License: BSD-2-
 Clause Project-URL: Documentation, https://centre-borelli.github.io/ruptures-
 docs/ Project-URL: Source, https://github.com/deepcharles/ruptures/ Project-
 URL: Bug Tracker, https://github.com/deepcharles/ruptures/issues/ Keywords:
 change point detection,signal segmentation,computer science,machine
```

### Comparing `ruptures-1.1.8/README.md` & `ruptures-1.1.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/pyproject.toml` & `ruptures-1.1.8rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/setup.cfg` & `ruptures-1.1.8rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/setup.py` & `ruptures-1.1.8rc1/setup.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/base.py` & `ruptures-1.1.8rc1/src/ruptures/base.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costautoregressive.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costautoregressive.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costclinear.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costclinear.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costcosine.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costcosine.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costl1.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costl1.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costl2.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costl2.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costlinear.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costlinear.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costml.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costml.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costnormal.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costnormal.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costrank.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costrank.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/costs/costrbf.py` & `ruptures-1.1.8rc1/src/ruptures/costs/costrbf.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/datasets/pw_constant.py` & `ruptures-1.1.8rc1/src/ruptures/datasets/pw_constant.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/datasets/pw_linear.py` & `ruptures-1.1.8rc1/src/ruptures/datasets/pw_linear.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/datasets/pw_normal.py` & `ruptures-1.1.8rc1/src/ruptures/datasets/pw_normal.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/datasets/pw_wavy.py` & `ruptures-1.1.8rc1/src/ruptures/datasets/pw_wavy.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd.c` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd.c`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd.pxd` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd.pxd`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd.pyx` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd.pyx`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd_computation.c` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd_computation.c`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/ekcpd_pelt_computation.c` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/ekcpd_pelt_computation.c`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/kernels.c` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/kernels.c`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/_detection/kernels.h` & `ruptures-1.1.8rc1/src/ruptures/detection/_detection/kernels.h`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/binseg.py` & `ruptures-1.1.8rc1/src/ruptures/detection/binseg.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/bottomup.py` & `ruptures-1.1.8rc1/src/ruptures/detection/bottomup.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/dynp.py` & `ruptures-1.1.8rc1/src/ruptures/detection/dynp.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/kernelcpd.py` & `ruptures-1.1.8rc1/src/ruptures/detection/kernelcpd.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/pelt.py` & `ruptures-1.1.8rc1/src/ruptures/detection/pelt.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/detection/window.py` & `ruptures-1.1.8rc1/src/ruptures/detection/window.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/__init__.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/hamming.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/hamming.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/hausdorff.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/hausdorff.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/precisionrecall.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/precisionrecall.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/randindex.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/randindex.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/sanity_check.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/sanity_check.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/metrics/timeerror.py` & `ruptures-1.1.8rc1/src/ruptures/metrics/timeerror.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/show/display.py` & `ruptures-1.1.8rc1/src/ruptures/show/display.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix.c` & `ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix.c`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix.pyx` & `ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix.pyx`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/utils/_utils/convert_path_matrix_c.c` & `ruptures-1.1.8rc1/src/ruptures/utils/_utils/convert_path_matrix_c.c`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/utils/bnode.py` & `ruptures-1.1.8rc1/src/ruptures/utils/bnode.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures/utils/utils.py` & `ruptures-1.1.8rc1/src/ruptures/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/src/ruptures.egg-info/PKG-INFO` & `ruptures-1.1.8rc1/src/ruptures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruptures
-Version: 1.1.8
+Version: 1.1.8rc1
 Summary: Change point detection for signals in Python.
 Home-page: https://github.com/deepcharles/ruptures/
 Author: Charles Truong, Laurent Oudre, Nicolas Vayatis
 Author-email: charles@doffy.net
 Maintainer: Charles Truong, Olivier Boulant
 License: BSD-2-Clause
 Project-URL: Documentation, https://centre-borelli.github.io/ruptures-docs/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ruptures Version: 1.1.8 Summary: Change point
+Metadata-Version: 2.1 Name: ruptures Version: 1.1.8rc1 Summary: Change point
 detection for signals in Python. Home-page: https://github.com/deepcharles/
 ruptures/ Author: Charles Truong, Laurent Oudre, Nicolas Vayatis Author-email:
 charles@doffy.net Maintainer: Charles Truong, Olivier Boulant License: BSD-2-
 Clause Project-URL: Documentation, https://centre-borelli.github.io/ruptures-
 docs/ Project-URL: Source, https://github.com/deepcharles/ruptures/ Project-
 URL: Bug Tracker, https://github.com/deepcharles/ruptures/issues/ Keywords:
 change point detection,signal segmentation,computer science,machine
```

### Comparing `ruptures-1.1.8/src/ruptures.egg-info/SOURCES.txt` & `ruptures-1.1.8rc1/src/ruptures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/tests/test_bnode.py` & `ruptures-1.1.8rc1/tests/test_bnode.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/tests/test_costs.py` & `ruptures-1.1.8rc1/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/tests/test_datasets.py` & `ruptures-1.1.8rc1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/tests/test_detection.py` & `ruptures-1.1.8rc1/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/tests/test_display.py` & `ruptures-1.1.8rc1/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `ruptures-1.1.8/tests/test_metrics.py` & `ruptures-1.1.8rc1/tests/test_metrics.py`

 * *Files identical despite different names*

