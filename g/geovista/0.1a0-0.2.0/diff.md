# Comparing `tmp/geovista-0.1a0.tar.gz` & `tmp/geovista-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovista-0.1a0.tar", last modified: Tue Sep 14 22:03:57 2021, max compression
+gzip compressed data, was "geovista-0.2.0.tar", last modified: Wed Jun  7 16:10:44 2023, max compression
```

## Comparing `geovista-0.1a0.tar` & `geovista-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,80 @@
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2021-09-14 22:03:57.432030 geovista-0.1a0/
--rw-r--r--   0 itwl      (6006) avd       (1091)     1875 2021-09-14 21:41:22.000000 geovista-0.1a0/.gitignore
--rw-r--r--   0 itwl      (6006) avd       (1091)     1313 2021-09-14 21:43:50.000000 geovista-0.1a0/.pre-commit-config.yaml
--rw-r--r--   0 itwl      (6006) avd       (1091)     1519 2021-09-14 21:40:28.000000 geovista-0.1a0/LICENSE
--rw-r--r--   0 itwl      (6006) avd       (1091)     2234 2021-09-14 22:03:57.433033 geovista-0.1a0/PKG-INFO
--rw-r--r--   0 itwl      (6006) avd       (1091)     1059 2021-09-14 21:40:28.000000 geovista-0.1a0/README.md
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2021-09-14 22:03:57.406036 geovista-0.1a0/geovista/
--rw-r--r--   0 itwl      (6006) avd       (1091)       59 2021-09-14 21:41:43.000000 geovista-0.1a0/geovista/__init__.py
--rw-r--r--   0 itwl      (6006) avd       (1091)      139 2021-09-14 22:03:57.000000 geovista-0.1a0/geovista/_version.py
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2021-09-14 22:03:57.425036 geovista-0.1a0/geovista.egg-info/
--rw-r--r--   0 itwl      (6006) avd       (1091)     2234 2021-09-14 22:03:57.000000 geovista-0.1a0/geovista.egg-info/PKG-INFO
--rw-r--r--   0 itwl      (6006) avd       (1091)      344 2021-09-14 22:03:57.000000 geovista-0.1a0/geovista.egg-info/SOURCES.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)        1 2021-09-14 22:03:57.000000 geovista-0.1a0/geovista.egg-info/dependency_links.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)        1 2021-09-14 21:43:16.000000 geovista-0.1a0/geovista.egg-info/not-zip-safe
--rw-r--r--   0 itwl      (6006) avd       (1091)       98 2021-09-14 22:03:57.000000 geovista-0.1a0/geovista.egg-info/requires.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)        9 2021-09-14 22:03:57.000000 geovista-0.1a0/geovista.egg-info/top_level.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)      490 2021-09-14 21:41:50.000000 geovista-0.1a0/pyproject.toml
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2021-09-14 22:03:57.429038 geovista-0.1a0/requirements/
--rw-r--r--   0 itwl      (6006) avd       (1091)      327 2021-09-14 21:41:59.000000 geovista-0.1a0/requirements/geovista.yml
--rw-r--r--   0 itwl      (6006) avd       (1091)     1687 2021-09-14 22:03:57.438030 geovista-0.1a0/setup.cfg
--rw-r--r--   0 itwl      (6006) avd       (1091)      100 2021-09-14 21:42:05.000000 geovista-0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.069115 geovista-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 16:10:32.000000 geovista-0.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-07 16:10:32.000000 geovista-0.2.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-07 16:10:32.000000 geovista-0.2.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-07 16:10:32.000000 geovista-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 16:10:32.000000 geovista-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 16:10:32.000000 geovista-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28873 2023-06-07 16:10:44.069115 geovista-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25966 2023-06-07 16:10:32.000000 geovista-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-07 16:10:32.000000 geovista-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.057114 geovista-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 16:10:32.000000 geovista-0.2.0/requirements/pypi-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 16:10:32.000000 geovista-0.2.0/requirements/pypi-optional-cmap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 16:10:32.000000 geovista-0.2.0/requirements/pypi-optional-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 16:10:32.000000 geovista-0.2.0/requirements/pypi-optional-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:10:44.069115 geovista-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 16:10:32.000000 geovista-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.053114 geovista-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.061114 geovista-0.2.0/src/geovista/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 16:10:43.000000 geovista-0.2.0/src/geovista/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36689 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.069115 geovista-0.2.0/src/geovista/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_1d__oisst.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1738 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_1d__oisst_eqc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_1d__synthetic_face_m1_n1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_1d__synthetic_face_m1_n1_robin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_1d__synthetic_node_m1_n1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1484 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_1d__synthetic_node_m1_n1_moll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1475 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_2d__orca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_2d__orca_moll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1405 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_2d__synthetic_face_m1n1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_2d__synthetic_face_m1n1_robin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_2d__synthetic_node_m1n1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1546 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_2d__synthetic_node_m1n1_moll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_points__orca_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1543 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__fesom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1837 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__fesom_fouc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__fvcom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__hexahedron.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__hexahedron_poly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__icon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1634 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__icon_eqc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__lam_pacific.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1602 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__lam_pacific_moll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1485 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__lfric_orog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__lfric_orog_warp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1655 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__lfric_sst.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__lfric_sst_bonne.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1499 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__smc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1630 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__smc_sinu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__tri.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1888 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/examples/from_unstructured__tri_hammer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33256 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/geoplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/pantry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-07 16:10:32.000000 geovista-0.2.0/src/geovista/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.061114 geovista-0.2.0/src/geovista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28873 2023-06-07 16:10:44.000000 geovista-0.2.0/src/geovista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-07 16:10:44.000000 geovista-0.2.0/src/geovista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:10:44.000000 geovista-0.2.0/src/geovista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 16:10:44.000000 geovista-0.2.0/src/geovista.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:10:43.000000 geovista-0.2.0/src/geovista.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-07 16:10:44.000000 geovista-0.2.0/src/geovista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 16:10:44.000000 geovista-0.2.0/src/geovista.egg-info/top_level.txt
```

### Comparing `geovista-0.1a0/LICENSE` & `geovista-0.2.0/LICENSE`

 * *Files identical despite different names*

