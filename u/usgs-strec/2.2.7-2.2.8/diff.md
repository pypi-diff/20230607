# Comparing `tmp/usgs-strec-2.2.7.tar.gz` & `tmp/usgs-strec-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-strec-2.2.7.tar", last modified: Wed Apr 12 22:11:20 2023, max compression
+gzip compressed data, was "usgs-strec-2.2.8.tar", last modified: Wed Jun  7 18:04:01 2023, max compression
```

## Comparing `usgs-strec-2.2.7.tar` & `usgs-strec-2.2.8.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/.gitlab-ci.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/.travis.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/CONTRIBUTING.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/DISCLAIMER.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/LICENSE.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10781 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/README.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/code.json
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/install.sh
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/license.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-04-12 21:02:21.000000 usgs-strec-2.2.7/pyproject.toml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/select_regions.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/setup.cfg
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/src/strec/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/__init__.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/src/strec/bin/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8371 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/bin/regcalc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8152 2023-04-12 20:23:25.000000 usgs-strec-2.2.7/src/strec/bin/strec_cfg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9523 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/calc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/cmt.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4869 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/config.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/src/strec/data/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/REGION_GRIDS_README.txt
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/active.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/domains.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/land.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/maximum_interface_depths.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/moment_tensors.db
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/ocean.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6153 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/data/select.conf
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1753 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/data/selectspec.conf
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/stable.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/strec.ini
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/subduction.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/volcanic.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5461 2023-04-12 20:50:34.000000 usgs-strec-2.2.7/src/strec/database.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/distance.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/gcmt.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/gmreg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/kagan.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/slab.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13185 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/sm_probs.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/subduction.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    23230 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/subtype.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8163 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/utils.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/src/usgs_strec.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2222 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/SOURCES.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/test/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/test/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/test/src/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/AMlvPS_trench.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/large_events.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/strec.db
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/test.ndk
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/test_regimes.xlsx
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/test/src/strec/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10144 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/calc_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/cmt_test.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/test/src/strec/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/big_focals.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/comcatid_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/focal_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/hypocols_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/id_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/moment_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/nga_matched.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10154 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/data/simple_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/subsampled_nga_results.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_dep_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_dip_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_str_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_thk_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_unc_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/database_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/distance_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/gcmt_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/gmreg_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/kagan_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8109 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/probs_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/slab_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/subduction_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8116 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/subtype_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/utils_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.742189 usgs-strec-2.2.8/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/.gitignore
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/.gitlab-ci.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/.travis.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/CONTRIBUTING.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/DISCLAIMER.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/LICENSE.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12106 2023-06-07 18:04:01.742189 usgs-strec-2.2.8/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10861 2023-06-07 17:17:35.000000 usgs-strec-2.2.8/README.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/code.json
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/install.sh
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/license.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-06-07 18:03:42.000000 usgs-strec-2.2.8/pyproject.toml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/select_regions.png
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-06-07 18:04:01.742189 usgs-strec-2.2.8/setup.cfg
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.712189 usgs-strec-2.2.8/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.722189 usgs-strec-2.2.8/src/strec/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/__init__.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.722189 usgs-strec-2.2.8/src/strec/bin/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8371 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/bin/regcalc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8152 2023-06-05 16:02:35.000000 usgs-strec-2.2.8/src/strec/bin/strec_cfg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9523 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/calc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/cmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4869 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/config.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.732189 usgs-strec-2.2.8/src/strec/data/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/REGION_GRIDS_README.txt
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/active.geojson
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    23487 2023-06-07 17:17:35.000000 usgs-strec-2.2.8/src/strec/data/backarc.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/domains.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/land.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/maximum_interface_depths.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/moment_tensors.db
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/ocean.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6153 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/data/select.conf
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1753 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/data/selectspec.conf
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/stable.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/strec.ini
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/subduction.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/data/volcanic.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5461 2023-06-05 16:02:35.000000 usgs-strec-2.2.8/src/strec/database.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3632 2023-06-07 17:17:35.000000 usgs-strec-2.2.8/src/strec/distance.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/gcmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3384 2023-06-07 17:17:35.000000 usgs-strec-2.2.8/src/strec/gmreg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/kagan.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/slab.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13185 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/sm_probs.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/src/strec/subduction.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    23230 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/subtype.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8163 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/src/strec/utils.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.732189 usgs-strec-2.2.8/src/usgs_strec.egg-info/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12106 2023-06-07 18:04:01.000000 usgs-strec-2.2.8/src/usgs_strec.egg-info/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2253 2023-06-07 18:04:01.000000 usgs-strec-2.2.8/src/usgs_strec.egg-info/SOURCES.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-06-07 18:04:01.000000 usgs-strec-2.2.8/src/usgs_strec.egg-info/dependency_links.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-06-07 18:04:01.000000 usgs-strec-2.2.8/src/usgs_strec.egg-info/entry_points.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-06-07 18:04:01.000000 usgs-strec-2.2.8/src/usgs_strec.egg-info/requires.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-06-07 18:04:01.000000 usgs-strec-2.2.8/src/usgs_strec.egg-info/top_level.txt
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.722189 usgs-strec-2.2.8/test/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.722189 usgs-strec-2.2.8/test/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.742189 usgs-strec-2.2.8/test/src/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/data/AMlvPS_trench.json
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/data/large_events.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/data/strec.db
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/data/test.ndk
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/data/test_regimes.xlsx
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.742189 usgs-strec-2.2.8/test/src/strec/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10144 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/test/src/strec/calc_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/cmt_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-06-07 18:04:01.742189 usgs-strec-2.2.8/test/src/strec/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/big_focals.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/comcatid_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/focal_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/hypocols_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/id_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/moment_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/nga_matched.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10154 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/test/src/strec/data/simple_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/data/subsampled_nga_results.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/test/src/strec/data/van_slab2_dep_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/test/src/strec/data/van_slab2_dip_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/test/src/strec/data/van_slab2_str_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/test/src/strec/data/van_slab2_thk_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/test/src/strec/data/van_slab2_unc_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/database_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    11813 2023-06-07 17:17:35.000000 usgs-strec-2.2.8/test/src/strec/distance_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/gcmt_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/gmreg_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/kagan_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8109 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/test/src/strec/probs_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.8/test/src/strec/slab_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.8/test/src/strec/subduction_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8116 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/test/src/strec/subtype_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-04-11 15:31:23.000000 usgs-strec-2.2.8/test/src/strec/utils_test.py
```

### Comparing `usgs-strec-2.2.7/.gitlab-ci.yml` & `usgs-strec-2.2.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/.travis.yml` & `usgs-strec-2.2.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/CONTRIBUTING.md` & `usgs-strec-2.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/DISCLAIMER.md` & `usgs-strec-2.2.8/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/LICENSE.md` & `usgs-strec-2.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/PKG-INFO` & `usgs-strec-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.7
+Version: 2.2.8
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -273,14 +273,16 @@
 
  - *Oceanic*: Another region, not exclusive with the four Tectonic
    Regions, that indicates whether the point supplied is in the ocean
    (i.e., not continental).
 
  - *Continental*: The opposite of Oceanic.
 
+ - *Backarc*: The area of a subduction region that is behind the volcanic arc.
+
  - *Focal Mechanism*: A set of parameters that define the deformation in
    the source region that generates the seismic waves of an earthquake.
 
  - *Tensor Type*: The short name for the algorithm used to generate
    the moment tensor used to determine focal mechanism, Kagan angle,
    etc.  This is usually a short code like *Mww* (W-phase), *Mwr*
    (regional), *Mwb* (body wave), or *composite*, which indicates that
```

### Comparing `usgs-strec-2.2.7/README.md` & `usgs-strec-2.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,16 @@
 
  - *Oceanic*: Another region, not exclusive with the four Tectonic
    Regions, that indicates whether the point supplied is in the ocean
    (i.e., not continental).
 
  - *Continental*: The opposite of Oceanic.
 
+ - *Backarc*: The area of a subduction region that is behind the volcanic arc.
+
  - *Focal Mechanism*: A set of parameters that define the deformation in
    the source region that generates the seismic waves of an earthquake.
 
  - *Tensor Type*: The short name for the algorithm used to generate
    the moment tensor used to determine focal mechanism, Kagan angle,
    etc.  This is usually a short code like *Mww* (W-phase), *Mwr*
    (regional), *Mwb* (body wave), or *composite*, which indicates that
```

#### html2text {}

```diff
@@ -103,15 +103,16 @@
 in the crust. * *Stable*: Tectonic regions which unlike Active regions, do not
 experience crustal deformation (e.g., the interior of the Australian
 continent.) ![Map showing tectonic regions](select_regions.png "Map Showing
 Tectonic Regions") *Fig 1 - Map showing tectonic regions. ACR=Active Crustal
 Region, SUB=Subduction Zone, VOL=HotSpot Region, SCR=Stable Continental Region*
 - *Oceanic*: Another region, not exclusive with the four Tectonic Regions, that
 indicates whether the point supplied is in the ocean (i.e., not continental). -
-*Continental*: The opposite of Oceanic. - *Focal Mechanism*: A set of
+*Continental*: The opposite of Oceanic. - *Backarc*: The area of a subduction
+region that is behind the volcanic arc. - *Focal Mechanism*: A set of
 parameters that define the deformation in the source region that generates the
 seismic waves of an earthquake. - *Tensor Type*: The short name for the
 algorithm used to generate the moment tensor used to determine focal mechanism,
 Kagan angle, etc. This is usually a short code like *Mww* (W-phase), *Mwr*
 (regional), *Mwb* (body wave), or *composite*, which indicates that there is no
 computed moment tensor, so a composite of historical moment tensors around the
 input coordinates is used instead. - *Tensor Source*: When available, this is
```

### Comparing `usgs-strec-2.2.7/code.json` & `usgs-strec-2.2.8/code.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/install.sh` & `usgs-strec-2.2.8/install.sh`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/pyproject.toml` & `usgs-strec-2.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "usgs-strec"
-version = "2.2.7"
+version = "2.2.8"
 description = "USGS SeismoTectonic Regime Earthquake Calculator (STREC)"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Eric Thompson", email="ethompson@usgs.gov"},
 ]
 
 license = {file = "LICENSE.md"}
```

### Comparing `usgs-strec-2.2.7/select_regions.png` & `usgs-strec-2.2.8/select_regions.png`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/bin/regcalc.py` & `usgs-strec-2.2.8/src/strec/bin/regcalc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/bin/strec_cfg.py` & `usgs-strec-2.2.8/src/strec/bin/strec_cfg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/calc.py` & `usgs-strec-2.2.8/src/strec/calc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/cmt.py` & `usgs-strec-2.2.8/src/strec/cmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/config.py` & `usgs-strec-2.2.8/src/strec/config.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/REGION_GRIDS_README.txt` & `usgs-strec-2.2.8/src/strec/data/REGION_GRIDS_README.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/active.geojson` & `usgs-strec-2.2.8/src/strec/data/active.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/domains.xlsx` & `usgs-strec-2.2.8/src/strec/data/domains.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/land.geojson` & `usgs-strec-2.2.8/src/strec/data/land.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/moment_tensors.db` & `usgs-strec-2.2.8/src/strec/data/moment_tensors.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/ocean.geojson` & `usgs-strec-2.2.8/src/strec/data/ocean.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/select.conf` & `usgs-strec-2.2.8/src/strec/data/select.conf`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/selectspec.conf` & `usgs-strec-2.2.8/src/strec/data/selectspec.conf`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/stable.geojson` & `usgs-strec-2.2.8/src/strec/data/stable.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/strec.ini` & `usgs-strec-2.2.8/src/strec/data/strec.ini`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/subduction.geojson` & `usgs-strec-2.2.8/src/strec/data/subduction.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/data/volcanic.geojson` & `usgs-strec-2.2.8/src/strec/data/volcanic.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/database.py` & `usgs-strec-2.2.8/src/strec/database.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/distance.py` & `usgs-strec-2.2.8/src/strec/distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 TECTONIC_REGIONS = {
     "stable": "DistanceToStable",
     "active": "DistanceToActive",
     "volcanic": "DistanceToHotSpot",
     "subduction": "DistanceToSubduction",
     "ocean": "DistanceToOceanic",
     "land": "DistanceToContinental",
+    "backarc": "DistanceToBackarc",
 }
 
 
 def get_distance_to_shape(polygon_shape, clat, clon, dest_crs, regime):
     """Calculate distance to input geometry from lat/lon in given projection.
 
     Args:
@@ -49,15 +50,16 @@
 
 def get_distance_to_regime(lat, lon, regime):
     """Calculate distance from point to nearest polygon in a given regime.
 
     Args:
         lat (float): Earthquake latitude.
         lon (float): Earthquake longitude.
-        regime (str): One of ["land", "ocean", "active", "stable", "hotspot", "subduction"]
+        regime (str): One of ["land", "ocean", "active", "stable", "hotspot",
+                              "subduction", "backarc"]
     Returns:
         float: Distance (km) to nearest regime polygon.
     """
     config = get_config()
     longest_axis = float(config["DATA"]["longest_axis"])
     ortho_crs = pyproj.CRS(f"+proj=aeqd +lon_0={lon:.6f} +lat_0={lat:.6f} +ellps=WGS84")
     root = pathlib.Path(__file__).parent / "data"
@@ -90,15 +92,15 @@
               - DistanceToStable
               - DistanceToSubduction
               - DistanceToHotSpot
               - DistanceToOceanic
               - DistanceToContinental
     """
     distances = {}
-    regimes = ["active", "stable", "subduction", "volcanic", "ocean", "land"]
+    regimes = ["active", "stable", "subduction", "volcanic", "ocean", "land", "backarc"]
     for regime in regimes:
         mindist = get_distance_to_regime(lat, lon, regime)
         distances[regime] = mindist
 
     for oldkey, newkey in TECTONIC_REGIONS.items():
         if oldkey not in distances:
             continue
```

### Comparing `usgs-strec-2.2.7/src/strec/gcmt.py` & `usgs-strec-2.2.8/src/strec/gcmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/gmreg.py` & `usgs-strec-2.2.8/src/strec/gmreg.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,16 @@
                                         region.
                 - DistanceToHotSpot: Distance in km to nearest hotspot
                                       region.
                 - Oceanic: Boolean indicating if epicenter is in the ocean.
                 - DistanceToOceanic: Distance in km to nearest oceanic region.
                 - DistanceToContinental: Distance in km to nearest continental
                                          region.
+                - DistanceToBackarc: Distance in km to nearest backarc
+                                         region.
         """
         regions = OrderedDict()
 
         region_dict = calc_distances(lat, lon)
 
         if region_dict["DistanceToActive"] == 0:
             region_dict["TectonicRegion"] = "Active"
@@ -82,11 +84,12 @@
                 "DistanceToStable",
                 "DistanceToActive",
                 "DistanceToSubduction",
                 "DistanceToHotSpot",
                 "Oceanic",
                 "DistanceToOceanic",
                 "DistanceToContinental",
+                "DistanceToBackarc",
             ],
         )
 
         return regions
```

### Comparing `usgs-strec-2.2.7/src/strec/kagan.py` & `usgs-strec-2.2.8/src/strec/kagan.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/slab.py` & `usgs-strec-2.2.8/src/strec/slab.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/sm_probs.py` & `usgs-strec-2.2.8/src/strec/sm_probs.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/subduction.py` & `usgs-strec-2.2.8/src/strec/subduction.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/subtype.py` & `usgs-strec-2.2.8/src/strec/subtype.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/strec/utils.py` & `usgs-strec-2.2.8/src/strec/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/src/usgs_strec.egg-info/PKG-INFO` & `usgs-strec-2.2.8/src/usgs_strec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.7
+Version: 2.2.8
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -273,14 +273,16 @@
 
  - *Oceanic*: Another region, not exclusive with the four Tectonic
    Regions, that indicates whether the point supplied is in the ocean
    (i.e., not continental).
 
  - *Continental*: The opposite of Oceanic.
 
+ - *Backarc*: The area of a subduction region that is behind the volcanic arc.
+
  - *Focal Mechanism*: A set of parameters that define the deformation in
    the source region that generates the seismic waves of an earthquake.
 
  - *Tensor Type*: The short name for the algorithm used to generate
    the moment tensor used to determine focal mechanism, Kagan angle,
    etc.  This is usually a short code like *Mww* (W-phase), *Mwr*
    (regional), *Mwb* (body wave), or *composite*, which indicates that
```

### Comparing `usgs-strec-2.2.7/src/usgs_strec.egg-info/SOURCES.txt` & `usgs-strec-2.2.8/src/usgs_strec.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/strec/subduction.py
 src/strec/subtype.py
 src/strec/utils.py
 src/strec/bin/regcalc.py
 src/strec/bin/strec_cfg.py
 src/strec/data/REGION_GRIDS_README.txt
 src/strec/data/active.geojson
+src/strec/data/backarc.geojson
 src/strec/data/domains.xlsx
 src/strec/data/land.geojson
 src/strec/data/maximum_interface_depths.csv
 src/strec/data/moment_tensors.db
 src/strec/data/ocean.geojson
 src/strec/data/select.conf
 src/strec/data/selectspec.conf
```

### Comparing `usgs-strec-2.2.7/test/src/data/AMlvPS_trench.json` & `usgs-strec-2.2.8/test/src/data/AMlvPS_trench.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/data/large_events.xlsx` & `usgs-strec-2.2.8/test/src/data/large_events.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/data/strec.db` & `usgs-strec-2.2.8/test/src/data/strec.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/data/test_regimes.xlsx` & `usgs-strec-2.2.8/test/src/data/test_regimes.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/calc_test.py` & `usgs-strec-2.2.8/test/src/strec/calc_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/cmt_test.py` & `usgs-strec-2.2.8/test/src/strec/cmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/big_focals.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/big_focals.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/comcatid_catalog.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/comcatid_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/focal_catalog.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/focal_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/hypocols_catalog.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/hypocols_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/id_catalog.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/id_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/moment_catalog.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/moment_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/nga_matched.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/nga_matched.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/simple_catalog.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/simple_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/subsampled_nga_results.xlsx` & `usgs-strec-2.2.8/test/src/strec/data/subsampled_nga_results.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/van_slab2_dep_02.23.18.grd` & `usgs-strec-2.2.8/test/src/strec/data/van_slab2_dep_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/van_slab2_dip_02.23.18.grd` & `usgs-strec-2.2.8/test/src/strec/data/van_slab2_dip_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/van_slab2_str_02.23.18.grd` & `usgs-strec-2.2.8/test/src/strec/data/van_slab2_str_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/van_slab2_thk_02.23.18.grd` & `usgs-strec-2.2.8/test/src/strec/data/van_slab2_thk_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/data/van_slab2_unc_02.23.18.grd` & `usgs-strec-2.2.8/test/src/strec/data/van_slab2_unc_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/database_test.py` & `usgs-strec-2.2.8/test/src/strec/database_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/distance_test.py` & `usgs-strec-2.2.8/test/src/strec/distance_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,59 +14,62 @@
 
 def print_dict(dict):
     for key, value in dict.items():
         print(f"{key} = {value:.1f} km")
 
 
 def test_calc_tectonic_distances():
-
     points = [
         {
             "name": "Big Island",
             "region": "HotSpot",
             "lat": 19.630525,
             "lon": -155.435738,
             "order": [
                 "DistanceToHotSpot",
                 "DistanceToStable",
                 "DistanceToActive",
                 "DistanceToSubduction",
+                "DistanceToBackarc",
             ],
         },
         {
             "name": "Valparaiso, Chile",
             "region": "Subduction",
             "lat": -33.045879,
             "lon": -71.624954,
             "order": [
                 "DistanceToSubduction",
                 "DistanceToActive",
+                "DistanceToBackarc",
                 "DistanceToHotSpot",
                 "DistanceToStable",
             ],
         },
         {
             "name": "Coast of Greenland",
             "region": "Stable",
             "lat": 68.626508,
             "lon": -29.261091,
             "order": [
                 "DistanceToStable",
                 "DistanceToActive",
                 "DistanceToHotSpot",
                 "DistanceToSubduction",
+                "DistanceToBackarc",
             ],
         },
         {
             "name": "Tierra del Fuego",
             "region": "Active",
             "lat": -54.816815,
             "lon": -65.554447,
             "order": [
                 "DistanceToActive",
+                "DistanceToBackarc",
                 "DistanceToStable",
                 "DistanceToHotSpot",
                 "DistanceToSubduction",
             ],
         },
     ]
 
@@ -195,14 +198,15 @@
             )
         )
         distances = calc_distances(pdict["lat"], pdict["lon"])
         distances.pop("DistanceToActive", None)
         distances.pop("DistanceToStable", None)
         distances.pop("DistanceToSubduction", None)
         distances.pop("DistanceToHotSpot", None)
+        distances.pop("DistanceToBackarc", None)
         sorted_distances = {
             k: v for k, v in sorted(distances.items(), key=lambda item: item[1])
         }
         cmp_order = list(sorted_distances.keys())
         print_dict(sorted_distances)
         print()
         assert pdict["order"] == cmp_order
@@ -327,13 +331,73 @@
             rdist = distances[rtype]
             cdist = distances[ctype]
             print(
                 f"Point ({lat},{lon}) should be {rtype} ({rdist:.2f}), came back as {ctype} ({cdist:.2f})."
             )
 
 
+def test_backarc_distances():
+    inside_points = {
+        "South America": [
+            (-79.181, -6.154),
+            (-62.305, -19.523),
+            (-67.625, -55.351),
+            (-104.5034, 23.9527),
+        ],
+        "Cascadia": [
+            (-118.8087, 38.2870),
+            (-117.863, 47.757),
+            (-124.4573, 52.1561),
+        ],
+        "Aleutians": [
+            (-149.16980, 67.05374),
+            (-164.000, 54.754),
+            (-179.5206, 51.8203),
+        ],
+        "Indonesia": [
+            (130.05, -5.39),
+            (121.534, -6.004),
+            (101.4415, -2.1269),
+            (95.7179, 7.8991),
+            (95.959, 26.817),
+        ],
+        "Papua New Guinea": [
+            (142.60, -3.88),
+            (153.541, -4.219),
+            (162.93403, -11.04424),
+        ],
+        "Solomon Islands": [
+            (165.501, -10.056),
+            (168.5403, -17.4573),
+            (174.1541, -22.6454),
+        ],
+        "New Zealand": [
+            (169.420, -42.454),
+            (175.9794, -33.7461),
+            (179.1128, -21.1232),
+        ],
+        "Japan": [(121.295, 25.922), (132.0792, 35.9040), (160.5104, 58.2823)],
+    }
+    for region, points in inside_points.items():
+        errors = []
+        for point in points:
+            distance = get_distance_to_regime(point[1], point[0], "backarc")
+            try:
+                assert distance == 0
+            except AssertionError as ae:
+                msg = f"Distance test for {region} point {point} failed."
+                errors.append(msg)
+    if len(errors):
+        for error in errors:
+            print(error)
+        raise AssertionError(
+            "Distance calculations for backarc failed. See above for details."
+        )
+
+
 if __name__ == "__main__":
+    test_backarc_distances()
     test_calc_tectonic_distances()
     test_distances_along_lat()
     test_get_regime_distance()
     test_calc_tectonic_distances()
     test_calc_oceanic_distances()
```

### Comparing `usgs-strec-2.2.7/test/src/strec/gcmt_test.py` & `usgs-strec-2.2.8/test/src/strec/gcmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/gmreg_test.py` & `usgs-strec-2.2.8/test/src/strec/gmreg_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/kagan_test.py` & `usgs-strec-2.2.8/test/src/strec/kagan_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/probs_test.py` & `usgs-strec-2.2.8/test/src/strec/probs_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/slab_test.py` & `usgs-strec-2.2.8/test/src/strec/slab_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/subduction_test.py` & `usgs-strec-2.2.8/test/src/strec/subduction_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/subtype_test.py` & `usgs-strec-2.2.8/test/src/strec/subtype_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.7/test/src/strec/utils_test.py` & `usgs-strec-2.2.8/test/src/strec/utils_test.py`

 * *Files identical despite different names*

