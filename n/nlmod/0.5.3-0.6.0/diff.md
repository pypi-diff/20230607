# Comparing `tmp/nlmod-0.5.3.tar.gz` & `tmp/nlmod-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlmod-0.5.3.tar", last modified: Wed Apr 12 17:24:24 2023, max compression
+gzip compressed data, was "nlmod-0.6.0.tar", last modified: Wed Jun  7 19:39:43 2023, max compression
```

## Comparing `nlmod-0.5.3.tar` & `nlmod-0.6.0.tar`

### file list

```diff
@@ -1,91 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.495427 nlmod-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-12 17:24:14.000000 nlmod-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 17:24:24.495427 nlmod-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 17:24:14.000000 nlmod-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.483427 nlmod-0.5.3/nlmod/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.487427 nlmod-0.5.3/nlmod/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.487427 nlmod-0.5.3/nlmod/data/geotop/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/geotop/geo_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/geotop/litho_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.cpg
--rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.prj
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.qpj
--rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.shp
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.shx
--rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/regis_2_2.gleg
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.487427 nlmod-0.5.3/nlmod/dims/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    55292 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    35438 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/gwf/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/gwf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/horizontal_flow_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/lake.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/recharge.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/wells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/gwt/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/gwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/modpath/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/modpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/modpath/modpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/read/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/ahn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/bgt.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/brp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/jarkus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/meteobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/regis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/rws.py
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/waterboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/webservices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/sim/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/sim/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.483427 nlmod-0.5.3/nlmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:24:24.495427 nlmod-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 17:24:14.000000 nlmod-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.495427 nlmod-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_001_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_002_regis_geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_003_mfpackages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_004_northsea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_005_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_006_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_007_run_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_008_waterschappen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_009_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_010_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_011_dcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_012_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_013_surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_014_gis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_015_gwf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_016_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_017_metbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.218493 nlmod-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 19:39:28.000000 nlmod-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 19:39:43.218493 nlmod-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-07 19:39:28.000000 nlmod-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/examples/cache_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/examples/generate_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/examples/run_all_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/nlmod/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/nlmod/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1860872 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/bin/mp7_2_002_provisional
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.202493 nlmod-0.6.0/nlmod/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.202493 nlmod-0.6.0/nlmod/data/geotop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/geotop/geo_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/geotop/litho_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/regis_2_2.gleg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.206493 nlmod-0.6.0/nlmod/data/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.qpj
+-rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.shx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/dims/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56949 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35657 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/gwf/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/gwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/horizontal_flow_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/recharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36621 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/wells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/gwt/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/gwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/mfoutput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/modpath/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/modpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/modpath/modpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/dcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/flopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/plotutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.214493 nlmod-0.6.0/nlmod/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/ahn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/bgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/brp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/jarkus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/knmi_data_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/meteobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/regis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/rws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/waterboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/webservices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.214493 nlmod-0.6.0/nlmod/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/sim/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/nlmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-07 19:39:28.000000 nlmod-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:39:43.218493 nlmod-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.218493 nlmod-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_001_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_002_regis_geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_003_mfpackages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_004_northsea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_005_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_006_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_007_run_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_008_waterschappen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_009_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_010_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_011_dcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_012_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_013_surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_014_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_015_gwf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_016_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_017_metbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_018_knmi_data_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/util.py
```

### Comparing `nlmod-0.5.3/LICENSE` & `nlmod-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/PKG-INFO` & `nlmod-0.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,42 @@
-Metadata-Version: 2.1
-Name: nlmod
-Version: 0.5.3
-Summary: nlmod module by Artesia
-Home-page: https://github.com/ArtesiaWater/nlmod
-Author: Artesia
-License: MIT
-Platform: Windows
-Platform: Mac OS-X
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
-
 # nlmod
+
 <img src="docs/_static/logo_10000_2.png" width="256"/>
 
 [![nlmod](https://github.com/ArtesiaWater/nlmod/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/ArtesiaWater/nlmod/actions/workflows/ci.yml)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/6fadea550ea04ea28b6ccde88fc56f35)](https://www.codacy.com/gh/ArtesiaWater/nlmod/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ArtesiaWater/nlmod&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/6fadea550ea04ea28b6ccde88fc56f35)](https://www.codacy.com/gh/ArtesiaWater/nlmod/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/nlmod&utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/6fadea550ea04ea28b6ccde88fc56f35)](https://www.codacy.com/gh/ArtesiaWater/nlmod/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/nlmod&utm_campaign=Badge_Coverage)
 [![PyPI version](https://badge.fury.io/py/nlmod.svg)](https://badge.fury.io/py/nlmod)
 [![Documentation Status](https://readthedocs.org/projects/nlmod/badge/?version=stable)](https://nlmod.readthedocs.io/en/stable/?badge=stable)
 
-Python package with functions to process, build and visualise MODFLOW models in the Netherlands. 
+Python package with functions to process, build and visualise MODFLOW models in the Netherlands.
 
 The functions in nlmod have four main objectives:
+
 1. Create and adapt the temporal and spatial discretization of a MODFLOW model using an xarray Dataset (`nlmod.dims`).
 2. Download and read data from external sources, project this data on the modelgrid and add this data to an xarray Dataset (`nlmod.read`).
 3. Use data in an xarray Dataset to build modflow packages using FloPy (`nlmod.gwf` for Modflow 6 and `nlmod.modpath` for Modpath).
 4. Visualise modeldata in Python (`nlmod.plot`) or GIS software (`nlmod.gis`).
 
 More information can be found on the documentation-website: https://nlmod.readthedocs.io/.
 
 ## Installation
 
 Install the module with pip:
 
 `pip install nlmod`
 
-`nlmod` has many dependencies `xarray`, `flopy`, `rasterio`, `rioxarray`, `owslib`, `hydropandas`, `netcdf4`, `pyshp`, `rtree`, `openpyxl` and `matplotlib`.
+`nlmod` has many required dependencies: `flopy`, `xarray`, `netcdf4`, `rasterio`, `rioxarray`, `affine`, `geopandas`, `owslib`, `hydropandas`, `shapely`, `pyshp`, `rtree`, `matplotlib`, `dask` and `colorama`. On top of that there are some optional dependecies, only needed (and imported) in a single method. Examples of this are `bottleneck` (used in calculate_gxg), `geocube` (used in add_min_ahn_to_gdf), `h5netcdf` (used for hdf5 files backend in xarray). To install the nlmod with the optional dependencies use:
 
-When using pip the dependencies are automatically installed. Some dependencies are notoriously hard to install on certain platforms. 
-Please see the [dependencies](https://github.com/ArtesiaWater/hydropandas#dependencies) section of the `hydropandas` package for more information on how to install these packages manually. 
+`pip install nlmod[full]`
 
+When using pip the dependencies are automatically installed. Some dependencies are notoriously hard to install on certain platforms.
+Please see the [dependencies](https://github.com/ArtesiaWater/hydropandas#dependencies) section of the `hydropandas` package for more information on how to install these packages manually.
 
 ## Getting started
+
 If you are using nlmod for the first time you need to download the MODFLOW executables. You can easily download these executables by running this Python code:
 
-	import nlmod
-	nlmod.util.download_mfbinaries()
+    import nlmod
+	nlmod.download_mfbinaries()
 
-After you've downloaded the executables you can run the Jupyter Notebooks in the examples folder. These notebooks illustrate how you to use the nlmod package. 
+After you've downloaded the executables you can run the Jupyter Notebooks in the examples folder. These notebooks illustrate how you to use the nlmod package.
```

### Comparing `nlmod-0.5.3/nlmod/cache.py` & `nlmod-0.6.0/nlmod/cache.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/data/geotop/geo_eenheden.csv` & `nlmod-0.6.0/nlmod/data/geotop/geo_eenheden.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv` & `nlmod-0.6.0/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/data/opp_water.dbf` & `nlmod-0.6.0/nlmod/data/shapes/opp_water.dbf`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/data/opp_water.qpj` & `nlmod-0.6.0/nlmod/data/shapes/opp_water.qpj`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/data/opp_water.shp` & `nlmod-0.6.0/nlmod/data/shapes/opp_water.shp`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/data/regis_2_2.gleg` & `nlmod-0.6.0/nlmod/data/regis_2_2.gleg`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/dcs.py` & `nlmod-0.6.0/nlmod/plot/dcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 from matplotlib.collections import LineCollection, PatchCollection
 from matplotlib.patches import Rectangle
 from shapely.geometry import LineString, MultiLineString, Point, Polygon
 
-from .dims.grid import modelgrid_from_ds
+from ..dims.grid import modelgrid_from_ds
 
 
 class DatasetCrossSection:
     # assumes:
     # x and y are 1d-vectors
     # x is increasing, y is decreasing
     # the layers are ordered from the top down
@@ -147,30 +147,33 @@
             points.append(Point(cs_line.coords[-1]))
         # generate ax x, y, d -array
         xys = []
         for point in points:
             xys.append([point.x, point.y, cs_line.project(point)])
         xys = np.array(xys)
         if xys.size == 0:
-            raise (Exception("The line does not instersect with the dataset"))
+            raise ValueError("The line does not instersect with the dataset")
         # sort the points along the line
         xys = xys[xys[:, -1].argsort()]
         return xys
 
     def plot_layers(self, colors=None, min_label_area=np.inf, **kwargs):
         if colors is None:
             cmap = plt.get_cmap("tab20")
             colors = [cmap(i) for i in range(len(self.layer))]
         if isinstance(colors, pd.DataFrame):
             colors = colors["color"]
         if isinstance(colors, (dict, pd.Series)):
             colors = [colors[layer] for layer in self.layer]
 
+        if colors == "none":
+            colors = ["none"] * len(self.layer)
+
         polygons = []
-        for i in range(len(self.layer)):
+        for i, _ in enumerate(self.layer):
             if np.all(np.isnan(self.bot[i]) | (self.bot[i] == self.zmax)):
                 continue
             if np.all(np.isnan(self.top[i]) | (self.top[i] == self.zmin)):
                 continue
             z_not_nan = np.where(~np.isnan(self.top[i]) & ~np.isnan(self.bot[i]))[0]
             vans = [z_not_nan[0]]
             tots = []
@@ -226,15 +229,15 @@
     def plot_grid(
         self,
         edgecolor="k",
         facecolor="none",
         horizontal=True,
         vertical=True,
         ilayers=None,
-        **kwargs
+        **kwargs,
     ):
         lines = []
         if ilayers is None:
             ilayers = range(self.top.shape[0])
         if horizontal and not vertical:
             for i in ilayers:
                 for j in range(self.bot.shape[1]):
@@ -276,15 +279,15 @@
                                     (self.s[j + 1, 0], self.bot[i, j + 1]),
                                 ]
                             )
             line_collection = LineCollection(lines, edgecolor=edgecolor, **kwargs)
             self.ax.add_collection(line_collection)
             return line_collection
         if vertical and not horizontal:
-            raise (Exception("Not implemented yet. Why would you want this!?"))
+            raise NotImplementedError("Why would you want this!?")
         patches = []
         for i in range(self.top.shape[0]):
             for j in range(self.bot.shape[1]):
                 if not (np.isnan(self.top[i, j]) or np.isnan(self.bot[i, j])):
                     if self.bot[i, j] == self.zmax or self.top[i, j] == self.zmin:
                         continue
                     width = self.s[j, 1] - self.s[j, 0]
```

### Comparing `nlmod-0.5.3/nlmod/dims/base.py` & `nlmod-0.6.0/nlmod/read/webservices.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,424 +1,449 @@
-import datetime as dt
 import logging
-import numbers
+import xml.etree.ElementTree as ET
+from io import BytesIO
 
+import geopandas as gpd
 import numpy as np
-import xarray as xr
-from scipy.spatial import cKDTree
+import pandas as pd
+import requests
+import rioxarray
+from owslib.wcs import WebCoverageService
+from rasterio import merge
+from rasterio.io import MemoryFile
+from shapely.geometry import MultiPolygon, Point, Polygon
+from tqdm import tqdm
 
-from .. import util
-from . import resample
-from .layers import fill_nan_top_botm_kh_kv, set_idomain
+# from owslib.wfs import WebFeatureService
 
 logger = logging.getLogger(__name__)
 
 
-def set_ds_attrs(ds, model_name, model_ws, mfversion="mf6", exe_name=None):
-    """set the attribute of a model dataset.
+def arcrest(
+    url,
+    layer,
+    extent=None,
+    sr=28992,
+    f="geojson",
+    max_record_count=None,
+    timeout=120,
+    **kwargs,
+):
+    """Download data from an arcgis rest FeatureServer."""
+    params = {
+        "f": f,
+        "outFields": "*",
+        "outSR": sr,
+        "where": "1=1",
+    }
+    if extent is not None:
+        xmin, xmax, ymin, ymax = extent
+        params["spatialRel"] = "esriSpatialRelIntersects"
+        params["geometry"] = f"{xmin},{ymin},{xmax},{ymax}"
+        params["geometryType"] = "esriGeometryEnvelope"
+        params["inSR"] = sr
+    props = _get_data(url, {"f": "json"}, timeout=timeout, **kwargs)
+    if max_record_count is None:
+        max_record_count = props["maxRecordCount"]
+    else:
+        max_record_count = min(max_record_count, props["maxRecordCount"])
 
-    Parameters
-    ----------
-    ds : xarray dataset
-        An existing model dataset
-    model_name : str
-        name of the model.
-    model_ws : str or None
-        workspace of the model. This is where modeldata is saved to.
-    mfversion : str, optional
-        modflow version. The default is "mf6".
-    exe_name: str, optional
-        path to modflow executable, default is None, which assumes binaries
-        are available in nlmod/bin directory. Binaries can be downloaded
-        using `nlmod.util.download_mfbinaries()`.
+    params["returnIdsOnly"] = True
+    url_query = f"{url}/{layer}/query"
+    props = _get_data(url_query, params, timeout=timeout, **kwargs)
+    params.pop("returnIdsOnly")
+    if "objectIds" in props:
+        object_ids = props["objectIds"]
+        object_id_field_name = props["objectIdFieldName"]
+    else:
+        object_ids = props["properties"]["objectIds"]
+        object_id_field_name = props["properties"]["objectIdFieldName"]
+    if object_ids is not None and len(object_ids) > max_record_count:
+        # download in batches
+        object_ids.sort()
+        n_d = int(np.ceil((len(object_ids) / max_record_count)))
+        features = []
+        for i_d in tqdm(range(n_d)):
+            i_min = i_d * max_record_count
+            i_max = min(i_min + max_record_count - 1, len(object_ids) - 1)
+            where = "{}>={} and {}<={}".format(
+                object_id_field_name,
+                object_ids[i_min],
+                object_id_field_name,
+                object_ids[i_max],
+            )
+            params["where"] = where
+            data = _get_data(url_query, params, timeout=timeout, **kwargs)
+            features.extend(data["features"])
+    else:
+        # download all data in one go
+        data = _get_data(url_query, params, timeout=timeout, **kwargs)
+        features = data["features"]
+    if f == "json" or f == "pjson":
+        # Interpret the geometry field
+        data = []
+        for feature in features:
+            if "rings" in feature["geometry"]:
+                if len(feature["geometry"]) > 1:
+                    raise (Exception("Not supported yet"))
+                if len(feature["geometry"]["rings"]) == 1:
+                    geometry = Polygon(feature["geometry"]["rings"][0])
+                else:
+                    pols = [Polygon(xy) for xy in feature["geometry"]["rings"]]
+                    keep = [0]
+                    for i in range(1, len(pols)):
+                        if pols[i].within(pols[keep[-1]]):
+                            pols[keep[-1]] = pols[keep[-1]].difference(pols[i])
+                        else:
+                            keep.append(i)
+                    if len(keep) == 1:
+                        geometry = pols[keep[0]]
+                    else:
+                        geometry = MultiPolygon([pols[i] for i in keep])
+            elif (
+                len(feature["geometry"]) == 2
+                and "x" in feature["geometry"]
+                and "y" in feature["geometry"]
+            ):
+                geometry = Point(feature["geometry"]["x"], feature["geometry"]["y"])
+            else:
+                raise (Exception("Not supported yet"))
+            feature["attributes"]["geometry"] = geometry
+            data.append(feature["attributes"])
+        gdf = gpd.GeoDataFrame(data, crs=sr)
+    else:
+        # for geojson-data we can transform to GeoDataFrame right away
+        if len(features) == 0:
+            # Assigning CRS to a GeoDataFrame without a geometry column is not supported
+            gdf = gpd.GeoDataFrame()
+        else:
+            gdf = gpd.GeoDataFrame.from_features(features, crs=sr)
+    return gdf
 
-    Returns
-    -------
-    ds : xarray dataset
-        model dataset.
-    """
 
-    if model_name is not None and len(model_name) > 16 and mfversion == "mf6":
-        raise ValueError("model_name can not have more than 16 characters")
-    ds.attrs["model_name"] = model_name
-    ds.attrs["mfversion"] = mfversion
-    fmt = "%Y%m%d_%H:%M:%S"
-    ds.attrs["model_dataset_created_on"] = dt.datetime.now().strftime(fmt)
-
-    if exe_name is None:
-        exe_name = util.get_exe_path(mfversion)
-
-    ds.attrs["exe_name"] = exe_name
-
-    # add some directories
-    if model_ws is not None:
-        figdir, cachedir = util.get_model_dirs(model_ws)
-        ds.attrs["model_ws"] = model_ws
-        ds.attrs["figdir"] = figdir
-        ds.attrs["cachedir"] = cachedir
-
-    return ds
-
-
-def to_model_ds(
-    ds,
-    model_name=None,
-    model_ws=None,
+def _get_data(url, params, timeout=120, **kwargs):
+    r = requests.get(url, params=params, timeout=timeout, **kwargs)
+    if not r.ok:
+        raise (Exception(f"Request not successful: {r.url}"))
+    data = r.json()
+    if "error" in data:
+        code = data["error"]["code"]
+        message = data["error"]["message"]
+        raise (Exception(f"Error code {code}: {message}"))
+    return data
+
+
+def wfs(
+    url,
+    layer,
     extent=None,
-    delr=100.0,
-    delc=None,
-    fill_nan=True,
-    extrapolate=True,
-    anisotropy=10,
-    fill_value_kh=1.0,
-    fill_value_kv=0.1,
-    xorigin=0.0,
-    yorigin=0.0,
-    angrot=0.0,
-    drop_attributes=True,
-    transport=False,
+    version="2.0.0",
+    paged=True,
+    max_record_count=None,
+    driver="GML",
+    timeout=120,
 ):
-    """Transform a regis datset to a model dataset with another resolution.
+    """Download data from a wfs server."""
+    params = dict(version=version, request="GetFeature")
+    if version == "2.0.0":
+        params["typeNames"] = layer
+    else:
+        params["typeName"] = layer
+    if extent is not None:
+        params["bbox"] = f"{extent[0]},{extent[2]},{extent[1]},{extent[3]}"
+    if paged:
+        # wfs = WebFeatureService(url)
+        # get the maximum number of features
+        r = requests.get(f"{url}&request=getcapabilities", timeout=120)
+        if not r.ok:
+            raise (Exception(f"Request not successful: {r.url}"))
+        root = ET.fromstring(r.text)
+        ns = {"ows": "http://www.opengis.net/ows/1.1"}
+
+        constraints = {}
+
+        def add_constrains(elem, constraints):
+            for child in elem.findall("ows:Constraint", ns):
+                key = child.attrib["name"]
+                dv = child.find("ows:DefaultValue", ns)
+                if not hasattr(dv, "text"):
+                    continue
+                value = dv.text
+                if value[0].isdigit():
+                    if "." in value:
+                        value = float(value)
+                    else:
+                        value = int(value)
+                elif value.lower() in ["true", "false"]:
+                    value = bool(value)
+                constraints[key] = value
+
+        om = root.find("ows:OperationsMetadata", ns)
+        add_constrains(om, constraints)
+        ops = om.findall("ows:Operation", ns)
+        for op in ops:
+            if op.attrib["name"] == "GetFeature":
+                add_constrains(op, constraints)
+
+        if "CountDefault" not in constraints:
+            logger.info("Cannot find CountDefault. Setting CountDefault to inf")
+            constraints["CountDefault"] = np.inf
+        if max_record_count is None:
+            max_record_count = constraints["CountDefault"]
+        else:
+            max_record_count = min(max_record_count, constraints["CountDefault"])
+
+        # get the number of features
+        params["resultType"] = "hits"
+        r = requests.get(url, params=params, timeout=timeout)
+        if not r.ok:
+            raise (Exception(f"Request not successful: {r.url}"))
+        params.pop("resultType")
+        root = ET.fromstring(r.text)
+        if "ExceptionReport" in root.tag:
+            raise Exception(root[0].attrib)
+        if version == "1.1.0":
+            n = int(root.attrib["numberOfFeatures"])
+        else:
+            n = int(root.attrib["numberMatched"])
+        if n <= max_record_count:
+            paged = False
+
+    if paged:
+        # download the features per page
+        gdfs = []
+        params["count"] = max_record_count
+        for ip in range(int(np.ceil(n / max_record_count))):
+            params["startindex"] = ip * max_record_count
+            r = requests.get(url, params=params, timeout=timeout)
+            if not r.ok:
+                raise (Exception(f"Request not successful: {r.url}"))
+            gdfs.append(gpd.read_file(BytesIO(r.content), driver=driver))
+        gdf = pd.concat(gdfs).reset_index(drop=True)
+    else:
+        # download all features in one go
+        r = requests.get(url, params=params, timeout=timeout)
+        if not r.ok:
+            raise (Exception(f"Request not successful: {r.url}"))
+        gdf = gpd.read_file(BytesIO(r.content), driver=driver)
+
+    return gdf
+
+
+def wcs(
+    url,
+    extent,
+    res,
+    identifier=None,
+    version="1.0.0",
+    fmt="GEOTIFF_FLOAT32",
+    crs="EPSG:28992",
+    maxsize=2000,
+):
+    """Download data from a web coverage service (WCS), return a MemoryFile.
 
     Parameters
     ----------
-    ds : xarray.dataset
-        A layer model dataset.
-    model_name : str, optional
-        name of the model. THe default is None
-    model_ws : str, optional
-        workspace of the model. This is where modeldata is saved to. The
-        default is None
-    extent : list or tuple of length 4, optional
-        The extent of the new grid. Get from ds when None. The default is None.
-    delr : int, float, list, tuple or array, optional
-        The gridsize along columns (dx). The default is 100. meter.
-    delc : None, int, float, list, tuple or array, optional
-        The gridsize along rows (dy). Set to delr when None. If None delc=delr
-        The default is None.
-    fill_nan : bool, optional
-        if True nan values in the top, botm, kh and kv are filled using the
-        fill_nan_top_botm_kh_kv function. Layers with only nan values in the
-        botm are removed.
-    extrapolate : bool, optional
-        When true, extrapolate data-variables, into the sea or other areas with
-        only nans. THe default is True
-    anisotropy : int or float
-        factor to calculate kv from kh or the other way around
-    fill_value_kh : int or float, optional
-        use this value for kh if there is no data. The default is 1.0.
-    fill_value_kv : int or float, optional
-        use this value for kv if there is no data. The default is 0.1.
-    xorigin : int or float, optional
-        lower left x coordinate of the model grid only used if angrot != 0.
-        Default is 0.0.
-    yorigin : int or float, optional
-        lower left y coordinate of the model grid only used if angrot != 0.
-        Default is 0.0.
-    angrot : int or float, optinal
-        the rotation of the grid in counter clockwise degrees, default is 0.0
-    drop_attributes : bool, optional
-        if True drop the attributes from the layer model dataset. Otherwise
-        keep the attributes. Default is True.
-    transport : bool, optional
-        flag indicating whether dataset includes data for a groundwater
-        transport model (GWT). Default is False, no transport.
+    extent : list, tuple or np.array
+        extent
+    res : float, optional
+        resolution of wcs raster
+    url : str
+        webservice url.
+    identifier : str
+        identifier.
+    version : str
+        version of wcs service, options are '1.0.0' and '2.0.1'.
+    fmt : str, optional
+        geotif format
+    crs : str, optional
+        coördinate reference system
+
+    Raises
+    ------
+    Exception
+        wrong version
 
     Returns
     -------
-    ds : xarray.dataset
-        the model Dataset.
+    memfile : rasterio.io.MemoryFile
+        MemoryFile.
     """
-    if extent is None:
-        extent = ds.attrs["extent"]
-
-    # drop attributes
-    if drop_attributes:
-        ds = ds.copy()
-        for attr in list(ds.attrs):
-            del ds.attrs[attr]
-
-    # convert dataset to grid
-    logger.info("resample layer model data to structured modelgrid")
-    ds = resample.ds_to_structured_grid(
-        ds, extent, delr, delc, xorigin=xorigin, yorigin=yorigin, angrot=angrot
-    )
-
-    # add cell area variable
-    if delc is None:
-        delc = delr
-    if isinstance(delr, (numbers.Number)) and isinstance(delc, (numbers.Number)):
-        ds["area"] = ("y", "x"), ds.delr * ds.delc * np.ones(
-            (ds.dims["y"], ds.dims["x"])
-        )
-    elif isinstance(delr, np.ndarray) and isinstance(delc, np.ndarray):
-        ds["area"] = ("y", "x"), np.outer(delc, delr)
-        ds["delr"] = ("x"), delr
-        ds["delc"] = ("y"), delc
+    # check if wcs is within limits
+    dx = extent[1] - extent[0]
+    dy = extent[3] - extent[2]
+
+    # check if size exceeds maxsize
+    if (dx / res) > maxsize:
+        x_segments = int(np.ceil((dx / res) / maxsize))
     else:
-        raise TypeError("unexpected type for delr and/or delc")
+        x_segments = 1
 
-    if extrapolate:
-        ds = extrapolate_ds(ds)
+    if (dy / res) > maxsize:
+        y_segments = int(np.ceil((dy / res) / maxsize))
+    else:
+        y_segments = 1
 
-    # add attributes
-    ds = set_ds_attrs(ds, model_name, model_ws)
-    ds.attrs["transport"] = int(transport)
-
-    # fill nan's and add idomain
-    if fill_nan:
-        ds = fill_nan_top_botm_kh_kv(
-            ds,
-            anisotropy=anisotropy,
-            fill_value_kh=fill_value_kh,
-            fill_value_kv=fill_value_kv,
+    if (x_segments * y_segments) > 1:
+        st = f"""requested wcs raster width or height bigger than {maxsize*res}
+            -> splitting extent into {x_segments} * {y_segments} tiles"""
+        logger.info(st)
+        memfile = _split_wcs_extent(
+            extent,
+            x_segments,
+            y_segments,
+            maxsize,
+            res,
+            url,
+            identifier,
+            version,
+            fmt,
+            crs,
         )
+        da = rioxarray.open_rasterio(memfile.open(), mask_and_scale=True)[0]
     else:
-        ds = set_idomain(ds, remove_nan_layers=False)
-
-    return ds
+        memfile = _download_wcs(extent, res, url, identifier, version, fmt, crs)
+        da = rioxarray.open_rasterio(memfile.open(), mask_and_scale=True)[0]
+        # load the data from memfile otherwise lazy loading of xarray causes problems
+        da.load()
 
+    return da
 
-def extrapolate_ds(ds, mask=None):
-    """Fill missing data in layermodel based on nearest interpolation.
 
-    Used for ensuring layer model contains data everywhere. Useful for
-    filling in data beneath the sea for coastal groundwater models, or models
-    near the border of the Netherlands.
+def _split_wcs_extent(
+    extent,
+    x_segments,
+    y_segments,
+    maxsize,
+    res,
+    url,
+    identifier,
+    version,
+    fmt,
+    crs,
+):
+    """There is a max height and width limit for the wcs server. This function
+    splits your extent in chunks smaller than the limit. It returns a list of
+    Memory files.
 
     Parameters
     ----------
-    ds : xarray.DataSet
-        Model layer DataSet
-    mask: np.ndarray, optional
-        Boolean mask for each cell, with a value of True if its value needs to
-        be determined. When mask is None, it is determined from the botm-
-        variable. The default is None.
+    extent : list, tuple or np.array
+        extent
+    res : float
+        The resolution of the requested output-data
+    x_segments : int
+        number of tiles on the x axis
+    y_segments : int
+        number of tiles on the y axis
+    maxsize : int or float
+        maximum widht or height of wcs tile
 
     Returns
     -------
-    ds : xarray.DataSet
-        filled layermodel
+    MemoryFile
+        Rasterio MemoryFile of the merged data
+    Notes
+    -----
+    1. The resolution is used to obtain the data from the wcs server. Not sure
+    what kind of interpolation is used to resample the original grid.
     """
-    if mask is None:
-        mask = np.isnan(ds["botm"]).all("layer").data
-    if not mask.any():
-        # all of the model cells are is inside the known area
-        return ds
-    if mask.all():
-        raise (Exception("The model only contains NaNs"))
-    if "gridtype" in ds.attrs and ds.gridtype == "vertex":
-        x = ds.x.data
-        y = ds.y.data
-        dims = ("icell2d",)
-    else:
-        x, y = np.meshgrid(ds.x, ds.y)
-        dims = ("y", "x")
-    points = np.stack((x[~mask], y[~mask]), axis=1)
-    xi = np.stack((x[mask], y[mask]), axis=1)
-    # geneterate the tree only once, to increase speed
-    tree = cKDTree(points)
-    _, i = tree.query(xi)
-    for key in ds:
-        if not np.any([dim in ds[key].dims for dim in dims]):
-            continue
-        data = ds[key].data
-        if ds[key].dims == dims:
-            data[mask] = data[~mask][i]
-        elif ds[key].dims == ("layer",) + dims:
-            for lay in range(len(ds["layer"])):
-                data[lay][mask] = data[lay][~mask][i]
+
+    # write tiles
+    datasets = []
+    start_x = extent[0]
+    pbar = tqdm(total=x_segments * y_segments)
+    for tx in range(x_segments):
+        if (tx + 1) == x_segments:
+            end_x = extent[1]
         else:
-            raise (Exception(f"Dimensions {ds[key].dims} not supported"))
-        # make sure to set the data (which for some reason is sometimes needed)
-        ds[key].data = data
-    return ds
+            end_x = start_x + maxsize * res
+        start_y = extent[2]
+        for ty in range(y_segments):
+            if (ty + 1) == y_segments:
+                end_y = extent[3]
+            else:
+                end_y = start_y + maxsize * res
+            subextent = [start_x, end_x, start_y, end_y]
+            logger.debug(
+                f"segment x {tx+1} of {x_segments}, segment y {ty+1} of {y_segments}"
+            )
 
+            memfile = _download_wcs(subextent, res, url, identifier, version, fmt, crs)
 
-def get_ds(
-    extent,
-    delr=100.0,
-    delc=None,
-    model_name=None,
-    model_ws=None,
-    layer=None,
-    top=0.0,
-    botm=None,
-    kh=10.0,
-    kv=1.0,
-    crs=28992,
-    xorigin=0.0,
-    yorigin=0.0,
-    angrot=0.0,
-    attrs=None,
-    extrapolate=True,
-    fill_nan=True,
-    transport=False,
-    **kwargs,
-):
-    """Create a model dataset from scratch, so without a layer model.
+            datasets.append(memfile)
+            start_y = end_y
+            pbar.update(1)
+
+        start_x = end_x
+
+    pbar.close()
+    memfile = MemoryFile()
+    merge.merge([b.open() for b in datasets], dst_path=memfile)
+
+    return memfile
+
+
+def _download_wcs(extent, res, url, identifier, version, fmt, crs):
+    """Download the wcs-data, return a MemoryFile.
 
     Parameters
     ----------
     extent : list, tuple or np.array
-        desired model extent (xmin, xmax, ymin, ymax)
-    delr : int, float, list, tuple or array, optional
-        The gridsize along columns (dx). The default is 100. meter.
-    delc : None, int, float, list, tuple or array, optional
-        The gridsize along rows (dy). Set to delr when None. If None delc=delr. The
-        default is None.
-    model_name : str, optional
-        name of the model. THe default is None
-    model_ws : str, optional
-        workspace of the model. This is where modeldata is saved to. The default is
-        None.
-    layer : int, list, tuple or ndarray, optional
-        The names or index of the layers of the model. When layer is an integer it is
-        the number of layers. When layer is None, the number of layers is caluclated
-        from botm. When botm is None as well, the number of layers is set to 10. The
-        default is None.
-    top : float, list or ndarray, optional
-        The top of the model. It has to be of shape (len(y), len(x)) or it is
-        transformed into that shape if top is a float. The default is 0.0.
-    botm : list or ndarray, optional
-        The botm of the model layers. It has to be of shape
-        (len(layer), len(y), len(x)) or it is transformed to that shape if botm
-        is or a list/array of len(layer). When botm is None, a botm is
-        generated with a constant layer thickness of 10 meter. The default is
-        None.
-    kh : float, list or ndarray, optional
-        The horizontal conductivity of the model layers. It has to be of shape
-        (len(layer), len(y), len(x)) or it is transformed to that shape if kh
-        is a float or a list/array of len(layer). The default is 10.0.
-    kv : float, list or ndarray, optional
-        The vertical conductivity of the model layers. It has to be of shape
-        (len(layer), len(y), len(x)) or it is transformed to that shape if kv
-        is a float or a list/array of len(layer). The default is 1.0.
-    crs : int, optional
-        THe coordinate reference system of the model. The default is 28992.
-    xorigin : float, optional
-        x-position of the lower-left corner of the model grid. Only used when angrot is
-        not 0. The defauls is 0.0.
-    yorigin : float, optional
-        y-position of the lower-left corner of the model grid. Only used when angrot is
-        not 0. The defauls is 0.0.
-    angrot : float, optional
-        counter-clockwise rotation angle (in degrees) of the lower-left corner of the
-        model grid. The default is 0.0
-    attrs : dict, optional
-        Attributes of the model dataset. The default is None.
-    extrapolate : bool, optional
-        When true, extrapolate data-variables, into the sea or other areas with
-        only nans. The default is True
-    fill_nan : bool, optional
-        if True nan values in the top, botm, kh and kv are filled using the
-        fill_nan_top_botm_kh_kv function. Layers with only nan values in the
-        botm are removed.
-    transport : bool, optional
-        flag indicating whether dataset includes data for a groundwater
-        transport model (GWT). Default is False, no transport.
-
-
-    **kwargs : dict
-        Kwargs are passed into mbase.to_ds. These can be the model_name
-        or ds.
+        extent
+    res : float, optional
+        resolution of wcs raster
+    url : str
+        webservice url.
+    identifier : str
+        identifier.
+    version : str
+        version of wcs service, options are '1.0.0' and '2.0.1'.
+    fmt : str, optional
+        geotif format
+    crs : str, optional
+        coördinate reference system
+
+    Raises
+    ------
+    Exception
+        wrong version
 
     Returns
     -------
-    xr.Dataset
-        The model dataset.
+    memfile : rasterio.io.MemoryFile
+        MemoryFile.
     """
-    if delc is None:
-        delc = delr
-
-    if isinstance(delr, (tuple, list)):
-        delr = np.asarray(delr)
-
-    if isinstance(delc, (tuple, list)):
-        delc = np.asarray(delc)
-
-    if attrs is None:
-        attrs = {}
-
-    if layer is None:
-        if botm is None:
-            layer = 10
-        else:
-            layer = len(botm)
-    if isinstance(layer, int):
-        layer = np.arange(1, layer + 1)
-    if botm is None:
-        botm = top - 10 * np.arange(1.0, len(layer) + 1)
-
-    # check for nan
-    for par in [top, botm, kh, kv]:
-        if isinstance(par, numbers.Number):
-            if np.isnan(par) and (extrapolate or fill_nan):
-                raise ValueError(
-                    "extrapolate and remove_nan_layer should be "
-                    "False when setting model parameters to nan"
-                )
-
-    resample._set_angrot_attributes(extent, xorigin, yorigin, angrot, attrs)
-    x, y = resample.get_xy_mid_structured(attrs["extent"], delr, delc)
-    coords = dict(x=x, y=y, layer=layer)
-    if angrot != 0.0:
-        affine = resample.get_affine_mod_to_world(attrs)
-        xc, yc = affine * np.meshgrid(x, y)
-        coords["xc"] = (("y", "x"), xc)
-        coords["yc"] = (("y", "x"), yc)
-
-    def check_variable(var, shape):
-        if isinstance(var, int):
-            # the variable is a single integer
-            var = float(var)
-        if isinstance(var, float):
-            # the variable is a single float
-            var = np.full(shape, var)
-        else:
-            # assume the variable is an array of some kind
-            if not isinstance(var, np.ndarray):
-                var = np.array(var)
-            if var.dtype != float:
-                var = var.astype(float)
-            if len(var.shape) == 1 and len(shape) == 3:
-                # the variable is defined per layer
-                assert len(var) == shape[0]
-                var = var[:, np.newaxis, np.newaxis]
-                var = np.repeat(np.repeat(var, shape[1], 1), shape[2], 2)
-            else:
-                assert var.shape == shape
-        return var
-
-    shape = (len(y), len(x))
-    top = check_variable(top, shape)
-    shape = (len(layer),) + shape
-    botm = check_variable(botm, shape)
-    kh = check_variable(kh, shape)
-    kv = check_variable(kv, shape)
-
-    dims = ["layer", "y", "x"]
-    ds = xr.Dataset(
-        data_vars=dict(
-            top=(dims[1:], top),
-            botm=(dims, botm),
-            kh=(dims, kh),
-            kv=(dims, kv),
-        ),
-        coords=coords,
-        attrs=attrs,
-    )
-    ds = to_model_ds(
-        ds,
-        model_name=model_name,
-        model_ws=model_ws,
-        extent=extent,
-        delr=delr,
-        delc=delc,
-        drop_attributes=False,
-        extrapolate=extrapolate,
-        fill_nan=fill_nan,
-        transport=transport,
-        **kwargs,
+    # download file
+    logger.debug(
+        f"- download wcs between: x ({str(extent[0])}, {str(extent[1])}); "
+        f"y ({str(extent[2])}, {str(extent[3])})"
     )
-    ds.rio.set_crs(crs)
-    return ds
+    wcs = WebCoverageService(url, version=version)
+    if identifier is None:
+        identifiers = list(wcs.contents)
+        if len(identifiers) > 1:
+            raise (Exception("wcs contains more than 1 identifier. Please specify."))
+        identifier = identifiers[0]
+    if version == "1.0.0":
+        bbox = (extent[0], extent[2], extent[1], extent[3])
+        output = wcs.getCoverage(
+            identifier=identifier,
+            bbox=bbox,
+            format=fmt,
+            crs=crs,
+            resx=res,
+            resy=res,
+        )
+    elif version == "2.0.1":
+        # bbox, resx and resy do nothing in version 2.0.1
+        subsets = [("x", extent[0], extent[1]), ("y", extent[2], extent[3])]
+        output = wcs.getCoverage(
+            identifier=[identifier], subsets=subsets, format=fmt, crs=crs
+        )
+    else:
+        raise Exception(f"Version {version} not yet supported")
+    if "xml" in output.info()["Content-Type"]:
+        root = ET.fromstring(output.read())
+        raise (Exception("Download failed: {}".format(root[0].text)))
+    memfile = MemoryFile(output.read())
+    return memfile
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nlmod-0.5.3/nlmod/dims/grid.py` & `nlmod-0.6.0/nlmod/dims/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 -   project data on different grid types
 -   obtain various types of reclists from a grid that
     can be used as input for a MODFLOW package
 -   fill, interpolate and resample grid data
 """
 import logging
+import os
 import warnings
 
 import flopy
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import shapely
@@ -22,15 +23,15 @@
 from packaging import version
 from scipy.interpolate import griddata
 from shapely.affinity import affine_transform
 from shapely.geometry import Point, Polygon
 from tqdm import tqdm
 
 from .. import cache, util
-from .base import extrapolate_ds
+from .base import _get_structured_grid_ds, _get_vertex_grid_ds, extrapolate_ds
 from .layers import fill_nan_top_botm_kh_kv, get_first_active_layer, set_idomain
 from .rdp import rdp
 from .resample import (
     affine_transform_gdf,
     get_affine_mod_to_world,
     get_affine_world_to_mod,
     structured_da_to_ds,
@@ -168,16 +169,67 @@
     for i in range(mg.ncpl):
         icvert[i, : cell2d[i][3]] = cell2d[i][4:]
     ds["icvert"] = ("icell2d", "icv"), icvert
     ds["icvert"].attrs["_FillValue"] = nodata
     return ds
 
 
+def modelgrid_to_ds(mg):
+    """Create Dataset from flopy modelgrid object.
+
+    Parameters
+    ----------
+    mg : flopy.discretization.Grid
+        flopy modelgrid object
+
+    Returns
+    -------
+    ds : xarray.Dataset
+        Dataset containing grid information
+    """
+    if mg.grid_type == "structured":
+        x, y = mg.xyedges
+
+        ds = _get_structured_grid_ds(
+            xedges=x,
+            yedges=y,
+            nlay=mg.nlay,
+            botm=mg.botm,
+            top=mg.top,
+            xorigin=mg.xoffset,
+            yorigin=mg.yoffset,
+            angrot=mg.angrot,
+            attrs=None,
+            crs=None,
+        )
+    elif mg.grid_type == "vertex":
+        ds = _get_vertex_grid_ds(
+            x=mg.xcellcenters,
+            y=mg.ycellcenters,
+            xv=mg.verts[:, 0],
+            yv=mg.verts[:, 1],
+            cell2d=mg.cell2d,
+            extent=mg.extent,
+            nlay=mg.nlay,
+            angrot=mg.angrot,
+            xorigin=np.concatenate(mg.xvertices).min(),
+            yorigin=np.concatenate(mg.yvertices).min(),
+            botm=mg.botm,
+            top=mg.top,
+            attrs=None,
+            crs=None,
+        )
+    else:
+        raise NotImplementedError(f"Grid type '{mg.grid_type}' not supported!")
+
+    return ds
+
+
 def gridprops_to_vertex_ds(gridprops, ds, nodata=-1):
-    """Gridprops is a dictionairy containing keyword arguments needed to
+    """Gridprops is a dictionary containing keyword arguments needed to
     generate a flopy modelgrid instance."""
     _, xv, yv = zip(*gridprops["vertices"])
     ds["xv"] = ("iv", np.array(xv))
     ds["yv"] = ("iv", np.array(yv))
 
     cell2d = gridprops["cell2d"]
     ncvert_max = np.max([x[3] for x in cell2d])
@@ -232,15 +284,15 @@
     """Refine the grid (discretization by vertices, disv), using Gridgen.
 
     Parameters
     ----------
     ds : xarray.Datset
         A structured model Dataset.
     model_ws : str, optional
-        The working directory fpr GridGen. Get from ds when model_ws is None.
+        The working directory for GridGen. Get from ds when model_ws is None.
         The default is None.
     refinement_features : list of tuples of length 2 or 3, optional
         List of tuples containing refinement features. Each tuple must be of
         the form (GeoDataFrame, level) or (geometry, shape_type, level). When
         refinement_features is None, no refinement is added, but the structured model
         Dataset is transformed to a Vertex Dataset. The default is None.
     exe_name : str, optional
@@ -263,15 +315,16 @@
     assert ds.gridtype == "structured", "Can only refine a structured grid"
     logger.info("create vertex grid using gridgen")
 
     if exe_name is None:
         exe_name = util.get_exe_path("gridgen")
 
     if model_ws is None:
-        model_ws = ds.model_ws
+        model_ws = os.path.join(ds.model_ws, "gridgen")
+        os.makedirs(model_ws, exist_ok=True)
 
     if version.parse(flopy.__version__) < version.parse("3.3.6"):
         sim = flopy.mf6.MFSimulation()
         gwf = flopy.mf6.MFModel(sim)
         dis = flopy.mf6.ModflowGwfdis(
             gwf,
             nrow=len(ds.y),
@@ -358,43 +411,45 @@
     """
 
     logger.info("resample model Dataset to vertex modelgrid")
 
     assert isinstance(ds_in, xr.core.dataset.Dataset)
 
     xyi, _ = get_xyi_icell2d(gridprops)
-    x = xr.DataArray(xyi[:, 0], dims=("icell2d"))
-    y = xr.DataArray(xyi[:, 1], dims=("icell2d"))
+    x = xr.DataArray(xyi[:, 0], dims=("icell2d",))
+    y = xr.DataArray(xyi[:, 1], dims=("icell2d",))
     if method in ["nearest", "linear"]:
         # resample the entire dataset in one line
         ds_out = ds_in.interp(x=x, y=y, method=method, kwargs={"fill_value": None})
     else:
         ds_out = xr.Dataset(coords={"layer": ds_in.layer.data, "x": x, "y": y})
 
         # add other variables
         for data_var in ds_in.data_vars:
             data_arr = structured_da_to_ds(ds_in[data_var], ds_out, method=method)
             ds_out[data_var] = data_arr
 
     if "area" in gridprops:
+        if "area" in ds_out:
+            ds_out = ds_out.drop_vars("area")
         # only keep the first layer of area
         area = gridprops["area"][: len(ds_out["icell2d"])]
         ds_out["area"] = ("icell2d", area)
 
     # add information about the vertices
     ds_out = gridprops_to_vertex_ds(gridprops, ds_out, nodata=nodata)
 
     # then finally change the gridtype in the attributes
     ds_out.attrs["gridtype"] = "vertex"
 
     return ds_out
 
 
 def get_xyi_icell2d(gridprops=None, ds=None):
-    """Get x and y coördinates of the cell mids from the cellids in the grid
+    """Get x and y coordinates of the cell mids from the cellids in the grid
     properties.
 
     Parameters
     ----------
     gridprops : dictionary, optional
         dictionary with grid properties output from gridgen. If gridprops is
         None xyi and icell2d will be obtained from ds.
@@ -449,15 +504,16 @@
         layer_ds = layer_ds.copy()
         # update layers in ds
         drop_vars = []
         for var in ds.data_vars:
             if "layer" in ds[var].dims:
                 if var not in layer_ds.data_vars:
                     logger.info(
-                        f"Variable {var} is dropped, as it has dimension layer, but is not defined in layer_ds"
+                        f"Variable {var} is dropped, as it has dimension layer, "
+                        "but is not defined in layer_ds"
                     )
                 drop_vars.append(var)
         if len(drop_vars) > 0:
             ds = ds.drop_vars(drop_vars)
         ds = ds.assign_coords({"layer": layer_ds.layer})
     has_rotation = "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0
     if method in ["nearest", "linear"]:
@@ -1089,22 +1145,24 @@
     return val
 
 
 def _get_aggregates_values(group, fields_methods, gwf=None):
     agg_dic = {}
     for field, method in fields_methods.items():
         # aggregation is only necesary if group shape is greater than 1
-        if group.shape[0] == 1:
+        if (group.shape[0] == 1) or (method == "first"):
             agg_dic[field] = group[field].values[0]
-        if method == "max":
+        elif method == "max":
             agg_dic[field] = group[field].max()
         elif method == "min":
             agg_dic[field] = group[field].min()
         elif method == "mean":
             agg_dic[field] = group[field].mean()
+        elif method == "sum":
+            agg_dic[field] = group[field].sum()
         elif method == "nearest":
             agg_dic[field] = _agg_nearest(group, field, gwf)
         elif method == "length_weighted":  # only for lines
             agg_dic[field] = _agg_length_weighted(group, field)
         elif method == "max_length":  # only for lines
             agg_dic[field] = _agg_max_length(group, field)
         elif method == "area_weighted":  # only for polygons
@@ -1125,15 +1183,15 @@
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         GeoDataFrame containing points, lines or polygons per grid cell.
     fields_methods: dict
         fields (keys) in the Geodataframe with their aggregation method (items)
         aggregation methods can be:
-        max, min, mean, length_weighted (lines), max_length (lines),
+        max, min, mean, sum, length_weighted (lines), max_length (lines),
         area_weighted (polygon), max_area (polygon).
     gwf : flopy Groundwater flow model
         only necesary if one of the field methods is 'nearest'
 
     Returns
     -------
     celldata : pd.DataFrame
@@ -1264,16 +1322,17 @@
     gdf,
     ml=None,
     method="vertex",
     ix=None,
     desc="Intersecting with grid",
     **kwargs,
 ):
-    """Cut a geodataframe gdf by the grid of a flopy modflow model ml. This method is a
-    wrapper around the GridIntersect method from flopy.
+    """Intersect a geodataframe with the grid of a MODFLOW model.
+
+    Note: This method is a wrapper around the GridIntersect method in flopy.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame that needs to be cut by the grid. The GeoDataFrame can consist of
         multiple types (Point, LineString, Polygon and the Multi-variants).
     ml : flopy.modflow.Modflow or flopy.mf6.ModflowGwf or xarray.Dataset, optional
@@ -1316,17 +1375,17 @@
     geometry = gdf.geometry.name
     for _, shp in tqdm(gdf.iterrows(), total=gdf.shape[0], desc=desc):
         r = ix.intersect(shp[geometry], **kwargs)
         for i in range(r.shape[0]):
             shpn = shp.copy()
             shpn["cellid"] = r["cellids"][i]
             shpn[geometry] = r["ixshapes"][i]
-            if shp[geometry].geom_type == "LineString":
+            if shp[geometry].geom_type == ["LineString", "MultiLineString"]:
                 shpn["length"] = r["lengths"][i]
-            elif shp[geometry].geom_type == "Polygon":
+            elif shp[geometry].geom_type in ["Polygon", "MultiPolygon"]:
                 shpn["area"] = r["areas"][i]
             shps.append(shpn)
     gdfg = gpd.GeoDataFrame(shps, geometry=geometry, crs=gdf.crs)
     gdfg.index.name = gdf.index.name
     return gdfg
```

### Comparing `nlmod-0.5.3/nlmod/dims/layers.py` & `nlmod-0.6.0/nlmod/dims/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,18 @@
                 if lay == 0:
                     thickness[lay] = ds[top] - ds[bot][lay]
                 else:
                     thickness[lay] = ds[bot][lay - 1] - ds[bot][lay]
         else:
             raise ValueError("2d top should have same last dimension as bot")
     if isinstance(ds[bot], xr.DataArray):
+        if hasattr(ds[bot], "long_name"):
+            thickness.attrs["long_name"] = "thickness"
+        if hasattr(ds[bot], "standard_name"):
+            thickness.attrs["standard_name"] = "thickness_of_layer"
         if hasattr(ds[bot], "units"):
             if ds[bot].units == "mNAP":
                 thickness.attrs["units"] = "m"
             else:
                 thickness.attrs["units"] = ds[bot].units
 
     return thickness
@@ -140,15 +144,15 @@
         for lay0 in split_dict:
             reindexer.pop(lay0)
         return ds, reindexer
     return ds
 
 
 def _split_var(ds, var, layer, thickness, fctrs, top, bot):
-    """Internal method to split a variable of one layer in multiple layers"""
+    """Internal method to split a variable of one layer in multiple layers."""
     for i in range(len(fctrs)):
         name = layer + "_" + str(i + 1)
         if var == top:
             # take orignal top and subtract thickness of higher splitted layers
             ds[var].loc[name] = ds[var].loc[layer] - np.sum(fctrs[:i]) * thickness
         elif var == bot:
             # take original bottom and add thickness of lower splitted layers
@@ -568,15 +572,15 @@
     ds["top"] = top
     # recalculate idomain
     ds = set_idomain(ds)
     return ds
 
 
 def set_layer_top(ds, layer, top):
-    """Set the top of a layer"""
+    """Set the top of a layer."""
     assert layer in ds.layer
     lay = np.where(ds.layer == layer)[0][0]
     if lay == 0:
         # change the top of the model
         ds["top"] = top
         # make sure the botm of all layers is never higher than the new top
         ds["botm"] = ds["botm"].where(ds["botm"] < top, top)
@@ -592,15 +596,15 @@
         # make sure the botms of lower layers are lower than top
         ds["botm"][lay:] = ds["botm"][lay:].where(ds["botm"][lay:] < top, top)
     ds = set_idomain(ds)
     return ds
 
 
 def set_layer_botm(ds, layer, botm):
-    """Set the bottom of a layer"""
+    """Set the bottom of a layer."""
     assert layer in ds.layer
     lay = np.where(ds.layer == layer)[0][0]
     # if lay > 0 and np.any(botm > ds["botm"][lay - 1]):
     #    raise (Exception("set_layer_botm cannot change botm of higher layers yet"))
     ds["botm"][:lay] = ds["botm"][:lay].where(ds["botm"][:lay] > botm, botm)
     ds["botm"][lay] = botm
     # make sure the botm of the layers below is never higher than the new botm
@@ -609,29 +613,30 @@
     # make sure the botm of the layers above is lever lower than the new botm
 
     ds = set_idomain(ds)
     return ds
 
 
 def set_layer_thickness(ds, layer, thickness, change="botm"):
-    """Set the layer thickness by changing the bottom of the layer"""
+    """Set the layer thickness by changing the bottom of the layer."""
     assert layer in ds.layer
     assert change == "botm", "Only change=botm allowed for now"
     lay = np.where(ds.layer == layer)[0][0]
     if lay == 0:
         top = ds["top"]
     else:
         top = ds["botm"][lay - 1]
     new_botm = top - thickness
     ds = set_layer_botm(ds, layer, new_botm)
     return ds
 
 
 def set_minimum_layer_thickness(ds, layer, min_thickness, change="botm"):
-    """Make sure layer has a minimum thickness by lowering the botm of the layer where neccesary"""
+    """Make sure layer has a minimum thickness by lowering the botm of the
+    layer where neccesary."""
     assert layer in ds.layer
     assert change == "botm", "Only change=botm allowed for now"
     lay = np.where(ds.layer == layer)[0][0]
     if lay == 0:
         top = ds["top"]
     else:
         top = ds["botm"][lay - 1]
@@ -997,15 +1002,14 @@
     ------
     ValueError
         if source_ds does not have a layer dimension
 
     See also
     --------
     nlmod.read.geotop.aggregate_to_ds
-
     """
     msg = "x and/or y coordinates do not match between 'ds' and 'source_ds'"
     assert (ds.x == source_ds.x).all() and (ds.y == source_ds.y).all(), msg
 
     if "layer" in ds["top"].dims:
         # make sure there is no layer dimension in top
         ds["top"] = ds["top"].max(dim="layer")
```

### Comparing `nlmod-0.5.3/nlmod/dims/rdp.py` & `nlmod-0.6.0/nlmod/dims/rdp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/dims/resample.py` & `nlmod-0.6.0/nlmod/dims/resample.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     descending_y : bool, optional
         if True the resulting ymid array is in descending order. This is the
         default for MODFLOW models. default is True.
 
     Returns
     -------
     x : np.array
-        x-coordinates of the cell centers shape(ncol)
+        x-coordinates of the cell centers shape (ncol)
     y : np.array
-        y-coordinates of the cell centers shape(nrow)
+        y-coordinates of the cell centers shape (nrow)
     """
     if isinstance(delr, (numbers.Number)):
         if not isinstance(delc, (numbers.Number)):
             raise TypeError("if delr is a number delc should be a number as well")
 
         # check if extent is valid
         if (extent[1] - extent[0]) % delr != 0.0:
@@ -371,19 +371,20 @@
 
 def vertex_da_to_ds(da, ds, method="nearest"):
     """Resample a vertex DataArray to a model dataset.
 
     Parameters
     ----------
     da : xaray.DataArray
-        A vertex DataArray. When the DataArray does not have 'icell2d' as a
-        dimension, the original DataArray is retured. The DataArray da can
-        contain other dimensions as well (for example 'layer' or time'' ).
+        A vertex DataArray. When the DataArray does not have 'icell2d' as a dimension,
+        the original DataArray is retured. The DataArray da can contain other dimensions
+        as well (for example 'layer' or time'' ).
     ds : xarray.Dataset
-        The model dataset with coordinates x and y.
+        The model dataset to which the DataArray needs to be resampled, with coordinates
+        x and y.
     method : str, optional
         The interpolation method, see griddata. The default is "nearest".
 
     Returns
     -------
     xarray.DataArray
         A DataArray, with the same gridtype as ds.
@@ -625,14 +626,15 @@
 def get_affine(ds, sx=None, sy=None):
     """Get the affine-transformation, from pixel to real-world coordinates."""
     attrs = _get_attrs(ds)
     if sx is None:
         sx = attrs["delr"]
     if sy is None:
         sy = -attrs["delc"]
+
     if "angrot" in attrs:
         xorigin = attrs["xorigin"]
         yorigin = attrs["yorigin"]
         angrot = -attrs["angrot"]
         # xorigin and yorigin represent the lower left corner, while for the transform we
         # need the upper left
         dy = attrs["extent"][3] - attrs["extent"][2]
```

### Comparing `nlmod-0.5.3/nlmod/dims/time.py` & `nlmod-0.6.0/nlmod/dims/time.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 import datetime as dt
 import logging
 
 import numpy as np
 import pandas as pd
+from xarray import IndexVariable
 
 logger = logging.getLogger(__name__)
 
 
 def set_ds_time(
     ds,
     time=None,
@@ -141,15 +142,15 @@
     last time step of the previous stress period. The ratio between the
     two time-step durations can be at most tsmult.
 
     Parameters
     ----------
     forcing : array-like
         Array with a forcing value for each stress period. Forcing can be
-        for example a pumping rate of a rainfall intensity.
+        for example a pumping rate or a rainfall intensity.
     perlen : float or array of floats (nper)
         An array of the stress period lengths.
     tsmult : float or array of floats (nper)
         Time step multiplier.
     nstp : int or array of ints (nper)
         Number of time steps in each stress period.
     nstp_min : int
@@ -212,7 +213,77 @@
         ]
         dt_arr = np.concatenate(dt_lists)
 
         return nstp_ceiled, dt_arr
 
     else:
         return nstp_ceiled
+
+
+def ds_time_from_model(gwf):
+    """Get time index variable from model (gwf or gwt).
+
+    Parameters
+    ----------
+    gwf : flopy MFModel object
+        groundwater flow or groundwater transport model
+
+    Returns
+    -------
+    IndexVariable
+        time coordinate for xarray data-array or dataset
+    """
+
+    return ds_time_from_modeltime(gwf.modeltime)
+
+
+def ds_time_from_modeltime(modeltime):
+    """Get time index variable from modeltime object.
+
+    Parameters
+    ----------
+    modeltime : flopy ModelTime object
+        modeltime object (e.g. gwf.modeltime)
+
+    Returns
+    -------
+    IndexVariable
+        time coordinate for xarray data-array or dataset
+    """
+
+    return ds_time_idx(
+        np.cumsum(modeltime.perlen),
+        start_datetime=modeltime.start_datetime,
+        time_units=modeltime.time_units,
+    )
+
+
+def ds_time_idx(t, start_datetime=None, time_units="D"):
+    """Get time index variable from elapsed time array.
+
+    Parameters
+    ----------
+    t : np.array
+        array containing elapsed time, usually in days
+    start_datetime : str, pd.Timestamp, optional
+        starting datetime
+    time_units : str, optional
+        time units, default is days
+
+    Returns
+    -------
+    IndexVariable
+        time coordinate for xarray data-array or dataset
+    """
+    if start_datetime is not None:
+        dt = pd.to_timedelta(t, time_units)
+        times = pd.Timestamp(start_datetime) + dt
+
+    else:
+        times = t
+
+    time = IndexVariable(["time"], times)
+    time.attrs["time_units"] = time_units
+    if start_datetime is not None:
+        time.attrs["start"] = str(start_datetime)
+
+    return time
```

### Comparing `nlmod-0.5.3/nlmod/gis.py` & `nlmod-0.6.0/nlmod/gis.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/gwf/gwf.py` & `nlmod-0.6.0/nlmod/gwf/gwf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 """Created on Thu Jan  7 17:20:34 2021.
 
 @author: oebbe
 """
 import logging
 import numbers
+import warnings
 
 import flopy
 import numpy as np
 import xarray as xr
 
 from ..dims import grid
 from ..sim import ims, sim, tdis
+from ..util import _get_value_from_ds_attr, _get_value_from_ds_datavar
 from . import recharge
 
 logger = logging.getLogger(__name__)
 
 
 def gwf(ds, sim, under_relaxation=False, **kwargs):
     """create groundwater flow model from the model dataset.
@@ -264,26 +266,34 @@
 
     if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
         model.modelgrid.set_coord_info(xoff=xorigin, yoff=yorigin, angrot=angrot)
 
     return disv
 
 
-def npf(ds, gwf, icelltype=0, save_flows=False, pname="npf", **kwargs):
+def npf(
+    ds, gwf, k="kh", k33="kv", icelltype=0, save_flows=False, pname="npf", **kwargs
+):
     """get node property flow package from model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
         groundwaterflow object.
     icelltype : int or str, optional
         celltype, if int the icelltype for all layer, if str the icelltype from
         the model ds is used. The default is 0.
+    k : str or array-like
+        horizontal hydraulic conductivity, when passed as string, the array
+        is obtained from ds. By default assumes data is stored as "kh".
+    k33 : str or array-like
+        vertical hydraulic conductivity, when passed as string, the array
+        is obtained from ds. By default assumes data is stored as "kv".
     save_flows : bool, optional
         value is passed to flopy.mf6.ModflowGwfnpf() to determine if cell by
         cell flows should be saved to the cbb file. Default is False
     pname : str, optional
         package name
 
     Raises
@@ -297,36 +307,56 @@
         npf package.
     """
     logger.info("creating modflow NPF")
 
     if isinstance(icelltype, str):
         icelltype = ds[icelltype]
 
+    k = _get_value_from_ds_datavar(ds, "k", k)
+    k33 = _get_value_from_ds_datavar(ds, "k33", k33)
+
     npf = flopy.mf6.ModflowGwfnpf(
         gwf,
         pname=pname,
         icelltype=icelltype,
-        k=ds["kh"].data,
-        k33=ds["kv"].data,
+        k=k.data,
+        k33=k33.data,
         save_flows=save_flows,
         **kwargs,
     )
 
     return npf
 
 
-def ghb(ds, gwf, da_name, pname="ghb", auxiliary=None, **kwargs):
+def ghb(
+    ds,
+    gwf,
+    bhead=None,
+    cond=None,
+    da_name=None,
+    pname="ghb",
+    auxiliary=None,
+    **kwargs,
+):
     """get general head boundary from model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
         groundwaterflow object.
+    bhead : str or xarray.DataArray, optional
+        ghb boundary head, either as string pointing to data
+        array in ds or as data array. By default None, which assumes
+        data array is stored under "ghb_bhead".
+    cond : str or xarray.DataArray, optional
+        ghb conductance, either as string pointing to data
+        array in ds or as data array. By default None, which assumes
+        data array is stored under "ghb_cond".
     da_name : str
         name of the ghb files in the model dataset.
     pname : str, optional
         package name
     auxiliary : str or list of str
         name(s) of data arrays to include as auxiliary data to reclist
 
@@ -338,19 +368,31 @@
     Returns
     -------
     ghb : flopy ModflowGwfghb
         ghb package
     """
     logger.info("creating modflow GHB")
 
+    if da_name is not None:
+        warnings.warn(
+            "the kwarg 'da_name' is no longer supported, "
+            "specify 'bhead' and 'cond' explicitly!",
+            DeprecationWarning,
+        )
+        bhead = f"{da_name}_peil"
+        cond = f"{da_name}_cond"
+
+    mask_arr = _get_value_from_ds_datavar(ds, "cond", cond)
+    mask = mask_arr != 0
+
     ghb_rec = grid.da_to_reclist(
         ds,
-        ds[f"{da_name}_cond"] != 0,
-        col1=f"{da_name}_peil",
-        col2=f"{da_name}_cond",
+        mask,
+        col1=bhead,
+        col2=cond,
         first_active_layer=True,
         only_active_cells=False,
         layer=0,
         aux=auxiliary,
     )
 
     if len(ghb_rec) > 0:
@@ -361,53 +403,83 @@
             maxbound=len(ghb_rec),
             stress_period_data=ghb_rec,
             save_flows=True,
             pname=pname,
             **kwargs,
         )
         if (auxiliary is not None) and (ds.transport == 1):
+            logger.info("-> adding GHB to SSM sources list")
             ssm_sources = ds.attrs["ssm_sources"]
-            if ghb.name not in ssm_sources:
-                ssm_sources += ghb.name
+            if ghb.package_name not in ssm_sources:
+                ssm_sources += [ghb.package_name]
                 ds.attrs["ssm_sources"] = ssm_sources
         return ghb
 
     else:
-        logger.warning("no ghb cells added")
+        logger.warning("no ghb pkg added")
         return None
 
 
-def drn(ds, gwf, da_name, pname="drn", layer=None, **kwargs):
+def drn(
+    ds,
+    gwf,
+    elev="drn_elev",
+    cond="drn_cond",
+    da_name=None,
+    pname="drn",
+    layer=None,
+    **kwargs,
+):
     """get drain from model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
         groundwaterflow object.
-    da_name : str
-        name of the drn files in the model dataset
+    elev : str or xarray.DataArray, optional
+        drain elevation, either as string pointing to data
+        array in ds or as data array. By default assumes
+        data array is stored under "drn_elev".
+    cond : str or xarray.DataArray, optional
+        drain conductance, either as string pointing to data
+        array in ds or as data array. By default assumes
+        data array is stored under "drn_cond".
+    da_name : str, deprecated
+        this is deprecated, name of the drn files in the model dataset
     pname : str, optional
         package name
 
     Returns
     -------
     drn : flopy ModflowGwfdrn
         drn package
     """
     logger.info("creating modflow DRN")
 
+    if da_name is not None:
+        warnings.warn(
+            "the kwarg 'da_name' is no longer supported, "
+            "specify 'elev' and 'cond' explicitly!",
+            DeprecationWarning,
+        )
+        elev = f"{da_name}_peil"
+        cond = f"{da_name}_cond"
+
+    mask_arr = _get_value_from_ds_datavar(ds, "cond", cond)
+    mask = mask_arr != 0
+
     first_active_layer = layer is None
 
     drn_rec = grid.da_to_reclist(
         ds,
-        ds[f"{da_name}_cond"] != 0,
-        col1=f"{da_name}_peil",
-        col2=f"{da_name}_cond",
+        mask=mask,
+        col1=elev,
+        col2=cond,
         first_active_layer=first_active_layer,
         only_active_cells=False,
         layer=layer,
     )
 
     if len(drn_rec) > 0:
         drn = flopy.mf6.ModflowGwfdrn(
@@ -418,15 +490,15 @@
             save_flows=True,
             pname=pname,
             **kwargs,
         )
         return drn
 
     else:
-        logger.warning("no drn cells added")
+        logger.warning("no drn pkg added")
 
         return None
 
 
 def ic(ds, gwf, starting_head="starting_head", pname="ic", **kwargs):
     """get initial condictions package from model dataset.
 
@@ -446,22 +518,22 @@
     Returns
     -------
     ic : flopy ModflowGwfic
         ic package
     """
     logger.info("creating modflow IC")
 
-    if isinstance(starting_head, str):
-        pass
-    elif isinstance(starting_head, numbers.Number):
+    if isinstance(starting_head, numbers.Number):
+        logger.info("adding 'starting_head' data array to ds")
         ds["starting_head"] = starting_head * xr.ones_like(ds["idomain"])
         ds["starting_head"].attrs["units"] = "mNAP"
         starting_head = "starting_head"
 
-    ic = flopy.mf6.ModflowGwfic(gwf, pname=pname, strt=ds[starting_head].data, **kwargs)
+    strt = _get_value_from_ds_datavar(ds, "starting_head", starting_head)
+    ic = flopy.mf6.ModflowGwfic(gwf, pname=pname, strt=strt, **kwargs)
 
     return ic
 
 
 def sto(
     ds,
     gwf,
@@ -505,19 +577,16 @@
         if ds.time.steady_start:
             sts_spd = {0: True}
             trn_spd = {1: True}
         else:
             sts_spd = None
             trn_spd = {0: True}
 
-        if "sy" in ds:
-            sy = ds["sy"].data
-
-        if "ss" in ds:
-            ss = ds["ss"].data
+        sy = _get_value_from_ds_datavar(ds, "sy", sy)
+        ss = _get_value_from_ds_datavar(ds, "ss", ss)
 
         sto = flopy.mf6.ModflowGwfsto(
             gwf,
             pname=pname,
             save_flows=save_flows,
             iconvert=iconvert,
             ss=ss,
@@ -526,91 +595,115 @@
             transient=trn_spd,
             **kwargs,
         )
         return sto
 
 
 def chd(
-    ds, gwf, chd="chd", head="starting_head", pname="chd", auxiliary=None, **kwargs
+    ds, gwf, mask="chd_mask", head="chd_head", pname="chd", auxiliary=None, **kwargs
 ):
     """get constant head boundary at the model's edges from the model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
         groundwaterflow object.
-    chd : str, optional
+    mask : str, optional
         name of data variable in ds that is 1 for cells with a constant
-        head and zero for all other cells. The default is 'chd'.
+        head and zero for all other cells. The default is 'chd_mask'.
     head : str, optional
         name of data variable in ds that is used as the head in the chd
-        cells. The default is 'starting_head'.
+        cells. By default, assumes head data is stored as 'chd_head'.
     pname : str, optional
         package name
     auxiliary : str or list of str
         name(s) of data arrays to include as auxiliary data to reclist
+    chd : str, optional
+        deprecated, the new argument is 'mask'
 
     Returns
     -------
     chd : flopy ModflowGwfchd
         chd package
     """
     logger.info("creating modflow CHD")
 
+    if "chd" in kwargs:
+        warnings.warn(
+            "the 'chd' kwarg has been renamed to 'mask'!",
+            DeprecationWarning,
+        )
+        mask = kwargs.pop("chd")
+
+    maskarr = _get_value_from_ds_datavar(ds, "mask", mask)
+    mask = maskarr != 0
+
     # get the stress_period_data
-    chd_rec = grid.da_to_reclist(ds, ds[chd] != 0, col1=head, aux=auxiliary)
+    chd_rec = grid.da_to_reclist(ds, mask, col1=head, aux=auxiliary)
 
     chd = flopy.mf6.ModflowGwfchd(
         gwf,
         auxiliary="CONCENTRATION" if auxiliary is not None else None,
         pname=pname,
         maxbound=len(chd_rec),
         stress_period_data=chd_rec,
         save_flows=True,
         **kwargs,
     )
     if (auxiliary is not None) and (ds.transport == 1):
+        logger.info("-> adding CHD to SSM sources list")
         ssm_sources = ds.attrs["ssm_sources"]
-        if chd.name not in ssm_sources:
-            ssm_sources += chd.name
+        if chd.package_name not in ssm_sources:
+            ssm_sources += [chd.package_name]
             ds.attrs["ssm_sources"] = ssm_sources
 
-    return chd
+    if len(chd_rec) > 0:
+        return chd
+    else:
+        logger.warning("no chd pkg added")
+        return None
 
 
-def surface_drain_from_ds(ds, gwf, resistance, pname="drn", **kwargs):
+def surface_drain_from_ds(ds, gwf, resistance, elev="ahn", pname="drn", **kwargs):
     """get surface level drain (maaivelddrainage in Dutch) from the model
     dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
         groundwaterflow object.
     resistance : int or float
-        resistance of the surface drain, scaled with cell area to
-        calculate drain conductance.
+        resistance of the surface drain. This value is used to
+        calculate drain conductance by scaling with cell area.
+    elev : str or xarray.DataArray
+        name pointing to the data array containing surface drain elevation
+        data, or pass the data array directly. By default assumes
+        the elevation data is stored under "ahn".
     pname : str, optional
         package name
 
     Returns
     -------
     drn : flopy ModflowGwfdrn
         drn package
     """
 
     ds.attrs["surface_drn_resistance"] = resistance
-    mask = ds["ahn"].notnull()
+
+    maskarr = _get_value_from_ds_datavar(ds, "elev", elev)
+    mask = maskarr.notnull()
+
     drn_rec = grid.da_to_reclist(
         ds,
         mask,
-        col1="ahn",
+        col1=elev,
         col2=ds["area"] / ds.surface_drn_resistance,
         first_active_layer=True,
         only_active_cells=False,
     )
 
     drn = flopy.mf6.ModflowGwfdrn(
         gwf,
@@ -640,15 +733,15 @@
     Returns
     -------
     rch : flopy ModflowGwfrch
         rch package
     """
     logger.info("creating modflow RCH")
     # create recharge package
-    rch = recharge.model_datasets_to_rch(gwf, ds, pname=pname, **kwargs)
+    rch = recharge.ds_to_rch(gwf, ds, pname=pname, **kwargs)
 
     return rch
 
 
 def evt(ds, gwf, pname="evt", **kwargs):
     """get evapotranspiration package from model dataset.
 
@@ -665,15 +758,15 @@
     -------
     evt : flopy ModflowGwfevt
         rch package
     """
     logger.info("creating modflow EVT")
 
     # create recharge package
-    evt = recharge.model_datasets_to_evt(gwf, ds, pname=pname, **kwargs)
+    evt = recharge.ds_to_evt(gwf, ds, pname=pname, **kwargs)
 
     return evt
 
 
 def _set_record(out, budget, output="head"):
     record = []
     if isinstance(out, bool):
@@ -717,17 +810,23 @@
     if not ds.transport:
         logger.error("BUY package requires a groundwater transport model")
         raise ValueError(
             "BUY package requires a groundwater transport model. "
             "Set 'transport' to True in model dataset."
         )
 
-    drhodc = kwargs.pop("drhodc", ds.drhodc)
-    crhoref = kwargs.pop("crhoref", ds.crhoref)
-    denseref = kwargs.pop("denseref", ds.denseref)
+    drhodc = _get_value_from_ds_attr(
+        ds, "drhodc", attr="drhodc", value=kwargs.pop("drhodc", None)
+    )
+    crhoref = _get_value_from_ds_attr(
+        ds, "crhoref", attr="crhoref", value=kwargs.pop("crhoref", None)
+    )
+    denseref = _get_value_from_ds_attr(
+        ds, "denseref", attr="denseref", value=kwargs.pop("denseref", None)
+    )
 
     pdata = [(0, drhodc, crhoref, f"{ds.model_name}_gwt", "none")]
 
     buy = flopy.mf6.ModflowGwfbuy(
         gwf,
         denseref=denseref,
         nrhospecies=len(pdata),
@@ -783,15 +882,15 @@
         budget_filerecord=budget_filerecord,
         **kwargs,
     )
 
     return oc
 
 
-def ds_to_gwf(ds, complexity="MODERATE", icelltype=0, under_relaxation=False):
+def ds_to_gwf(ds, complexity="SIMPLE", icelltype=0, under_relaxation=False):
     """Generate Simulation and GWF model from model DataSet.
 
     Builds the following packages:
     - sim
     - tdis
     - ims
     - gwf
```

### Comparing `nlmod-0.5.3/nlmod/gwf/horizontal_flow_barrier.py` & `nlmod-0.6.0/nlmod/gwf/horizontal_flow_barrier.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/gwf/lake.py` & `nlmod-0.6.0/nlmod/gwf/lake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 import flopy
 import numpy as np
+import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 LAKE_KWDS = [
     "STATUS",
     "STAGE",
     "RAINFALL",
@@ -33,40 +34,40 @@
 
 def lake_from_gdf(
     gwf,
     gdf,
     ds,
     recharge=True,
     claktype="VERTICAL",
-    boundname_column='identificatie',
-    obs_type='STAGE',
+    boundname_column="identificatie",
+    obs_type="STAGE",
     surfdep=0.05,
     pname="lak",
     **kwargs,
 ):
-    """add a lake from a geodataframe
+    """Add a lake from a geodataframe.
 
     Parameters
     ----------
     gwf : flopy.mf6.modflow.mfgwf.ModflowGwf
         groundwater flow model.
     gdf : gpd.GeoDataframe
         geodataframe with the cellids as the index and the columns:
             lakeno : with the number of the lake
             strt : with the starting head of the lake
             clake : with the bed resistance of the lake
             optional columns are 'STATUS', 'STAGE', 'RAINFALL', 'EVAPORATION',
             'RUNOFF', 'INFLOW', 'WITHDRAWAL', 'AUXILIARY', 'RATE', 'INVERT',
             'WIDTH', 'SLOPE', 'ROUGH'. These columns should contain the name
             of a dataarray in ds with the dimension time.
-        if the lake have any outlets they should be specified in the columns
+        if the lake has any outlets they should be specified in the columns
             lakeout : the lake number of the outlet, if this is -1 the water
             is removed from the model.
             optinal columns are 'couttype', 'outlet_invert', 'outlet_width',
-            'outlet_rough' and 'outlet_slope. These column should contain a
+            'outlet_rough' and 'outlet_slope'. These columns should contain a
             unique value for each outlet.
     ds : xr.DataSet
         dataset containing relevant model grid and time information
     recharge : bool, optional
         if True recharge will be added to the lake and removed from the
         recharge package. The recharge
     claktype : str, optional
@@ -86,25 +87,26 @@
     Raises
     ------
     NotImplementedError
 
     Returns
     -------
     lak : flopy lake package
-
     """
     if claktype != "VERTICAL":
         raise NotImplementedError("function only tested for claktype=VERTICAL")
 
     if ds.gridtype != "vertex":
         raise NotImplementedError("only works with a vertex grid")
 
     assert ds.time.time_units.lower() == "days", "expected time unit days"
     time_conversion = 86400.0
     # length unit is always meters in nlmod
+    # TODO: Let's add a check for a length unit of meters if we ever add a length unit
+    # to ds
     length_conversion = 1.0
 
     packagedata = []
     connectiondata = []
     perioddata = {}
     for iper in range(ds.dims["time"]):
         perioddata[iper] = []
@@ -120,21 +122,21 @@
         use_outlets = False
         noutlets = None
         outlets = None
 
     for lakeno, lake_gdf in gdf.groupby("lakeno"):
         nlakeconn = lake_gdf.shape[0]
         strt = lake_gdf["strt"].iloc[0]
-        assert (lake_gdf["strt"] == strt).all(
-        ), "a single lake should have single strt"
+        assert (lake_gdf["strt"] == strt).all(), "a single lake should have single strt"
 
         if boundname_column is not None:
             boundname = lake_gdf[boundname_column].iloc[0]
-            assert (lake_gdf[boundname_column] == boundname).all(
-            ), f"a single lake should have a single {boundname_column}"
+            assert (
+                lake_gdf[boundname_column] == boundname
+            ).all(), f"a single lake should have a single {boundname_column}"
             packagedata.append([lakeno, strt, nlakeconn, boundname])
         else:
             packagedata.append([lakeno, strt, nlakeconn])
 
         iconn = 0
         for icell2d, row in lake_gdf.iterrows():
             cellid = (0, icell2d)  # assuming lake in the top layer
@@ -178,23 +180,24 @@
                 if outset not in lake_gdf.columns:
                     logger.debug(
                         f"no value specified for {outset} and lake no {lakeno}, using default value {default_value}"
                     )
                     setval = default_value
                 else:
                     setval = lake_gdf[outset].iloc[0]
-                    if np.isnan(setval):
+                    if pd.notna(setval):
+                        if not (lake_gdf[outset] == setval).all():
+                            raise ValueError(
+                                f"expected single data variable for {outset} and lake number {lakeno}, got {lake_gdf[outset]}"
+                            )
+                    else:  # setval is nan or None
                         setval = default_value
                         logger.debug(
                             f"no value specified for {outset} and lake no {lakeno}, using default value {default_value}"
                         )
-                    elif not (lake_gdf[outset] == setval).all():
-                        raise ValueError(
-                            f"expected single data variable for {outset} and lake number {lakeno}, got {lake_gdf[outset]}"
-                        )
                 if outset == "outlet_invert" and isinstance(setval, str):
                     if setval == "use_elevation":
                         setval = strt
                     else:
                         raise NotImplementedError(
                             "outlet_invert should not be a string"
                         )
@@ -214,19 +217,17 @@
                     perioddata[iper].append([lakeno, "EVAPORATION", -rech])
                 # set recharge to zero in dataset
                 ds["recharge"][iper, cellids] = 0
 
             # add other time variant settings to lake
             for lake_setting in lake_settings:
                 datavar = lake_gdf[lake_setting].iloc[0]
-                if not isinstance(datavar, str):
-                    if np.isnan(datavar):
-                        logger.debug(
-                            f"no {lake_setting} given for lake no {lakeno}")
-                        continue
+                if not pd.notna(datavar):  # None or nan
+                    logger.debug(f"no {lake_setting} given for lake no {lakeno}")
+                    continue
                 if not (lake_gdf[lake_setting] == datavar).all():
                     raise ValueError(
                         f"expected single data variable for {lake_setting} and lake number {lakeno}, got {lake_gdf[lake_setting]}"
                     )
                 perioddata[iper].append(
                     [lakeno, lake_setting, ds[datavar].values[iper]]
                 )
```

### Comparing `nlmod-0.5.3/nlmod/gwf/output.py` & `nlmod-0.6.0/nlmod/gwf/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,125 +1,92 @@
 import logging
 import os
+import warnings
 
 import flopy
 import numpy as np
 import pandas as pd
 import xarray as xr
 from shapely.geometry import Point
 
-import warnings
-
-from ..dims.resample import get_affine, get_xy_mid_structured
 from ..dims.grid import modelgrid_from_ds
+from ..mfoutput import _get_output_da
 
 logger = logging.getLogger(__name__)
 
 
-def get_heads_da(ds=None, gwf=None, fname_hds=None):
+def get_heads_da(ds=None, gwf=None, fname_heads=None, fname_hds=None):
     """Reads heads file given either a dataset or a groundwater flow object.
 
-    Note: Calling this function with ds is currently prevered over calling it
+    Note: Calling this function with ds is currently preferred over calling it
     with gwf, because the layer and time coordinates can not be fully
     reconstructed from gwf.
 
     Parameters
     ----------
     ds : xarray.Dataset
         Xarray dataset with model data.
     gwf : flopy ModflowGwf
         Flopy groundwaterflow object.
-    fname_hds : path, optional
+    fname_heads : path, optional
         Instead of loading the binary heads file corresponding to ds or gwf
         load the heads from
-
+    fname_hds : path, optional, Deprecated
+        please use fname_heads instead.
 
     Returns
     -------
-    head_ar : xarray.DataArray
-        heads array.
+    head_da : xarray.DataArray
+        heads data array.
     """
-    headobj = _get_hds(ds=ds, gwf=gwf, fname_hds=fname_hds)
-
-    if gwf is not None:
-        hdry = gwf.hdry
-        hnoflo = gwf.hnoflo
-    else:
-        hdry = -1e30
-        hnoflo = 1e30
-
-    heads = headobj.get_alldata()
-    heads[heads == hdry] = np.nan
-    heads[heads == hnoflo] = np.nan
-
-    if gwf is not None:
-        gridtype = gwf.modelgrid.grid_type
-    else:
-        gridtype = ds.gridtype
-
-    if gridtype == "vertex":
-        head_ar = xr.DataArray(
-            data=heads[:, :, 0],
-            dims=("time", "layer", "icell2d"),
-            coords={},
-            attrs={"units": "mNAP"},
+    if fname_hds is not None:
+        logger.warning(
+            "Kwarg 'fname_hds' was renamed to 'fname_heads'. Please update your code."
         )
+        fname_heads = fname_hds
+    head_da = _get_output_da(_get_heads, ds=ds, gwf_or_gwt=gwf, fname=fname_heads)
+    head_da.attrs["units"] = "m NAP"
+    return head_da
 
-    elif gridtype == "structured":
-        if gwf is not None:
-            delr = np.unique(gwf.modelgrid.delr).item()
-            delc = np.unique(gwf.modelgrid.delc).item()
-            extent = gwf.modelgrid.extent
-            x, y = get_xy_mid_structured(extent, delr, delc)
-
-        else:
-            x = ds.x
-            y = ds.y
-
-        head_ar = xr.DataArray(
-            data=heads,
-            dims=("time", "layer", "y", "x"),
-            coords={
-                "x": x,
-                "y": y,
-            },
-            attrs={"units": "mNAP"},
-        )
-    else:
-        assert 0, "Gridtype not supported"
 
-    if ds is not None:
-        head_ar.coords["layer"] = ds.layer
+def get_budget_da(text, ds=None, gwf=None, fname_cbc=None, kstpkper=None):
+    """Reads budget file given either a dataset or a groundwater flow object.
 
-        # TODO: temporarily only add time for when ds is passed because unable to
-        # exactly recreate ds.time from gwf.
-        head_ar.coords["time"] = ds.time
-
-    if ds is not None and "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
-        affine = get_affine(ds)
-        head_ar.rio.write_transform(affine, inplace=True)
-
-    elif gwf is not None and gwf.modelgrid.angrot != 0.0:
-        attrs = dict(
-            delr=np.unique(gwf.modelgrid.delr).item(),
-            delc=np.unique(gwf.modelgrid.delc).item(),
-            xorigin=gwf.modelgrid.xoffset,
-            yorigin=gwf.modelgrid.yoffset,
-            angrot=gwf.modelgrid.angrot,
-            extent=gwf.modelgrid.extent,
-        )
-        affine = get_affine(attrs)
-        head_ar.rio.write_transform(affine, inplace=True)
+    Parameters
+    ----------
+    text : str
+        record to get from budget file
+    ds : xarray.Dataset, optional
+        xarray dataset with model data. One of ds or gwf must be provided.
+    gwf : flopy ModflowGwf, optional
+        Flopy groundwaterflow object. One of ds or gwf must be provided.
+    fname_cbc : path, optional
+        specify the budget file to load, if not provided budget file will
+        be obtained from ds or gwf.
 
-    head_ar.rio.write_crs("EPSG:28992", inplace=True)
+    Returns
+    -------
+    q_da : xarray.DataArray
+        budget data array.
+    """
+    q_da = _get_output_da(
+        _get_cbc,
+        ds=ds,
+        gwf_or_gwt=gwf,
+        fname=fname_cbc,
+        text=text,
+        kstpkper=kstpkper,
+        full3D=True,
+    )
+    q_da.attrs["units"] = "m3/d"
 
-    return head_ar
+    return q_da
 
 
-def _get_hds(ds=None, gwf=None, fname_hds=None):
+def _get_heads(ds=None, gwf=None, fname_hds=None):
     msg = "Load the heads using either the ds, gwf or fname_hds"
     assert ((ds is not None) + (gwf is not None) + (fname_hds is not None)) >= 1, msg
 
     if fname_hds is None:
         if ds is None:
             return gwf.output.head()
         else:
@@ -132,25 +99,24 @@
 
 def _get_cbc(ds=None, gwf=None, fname_cbc=None):
     msg = "Load the budgets using either the ds or the gwf"
     assert ((ds is not None) + (gwf is not None)) == 1, msg
 
     if fname_cbc is None:
         if ds is None:
-            cbf = gwf.output.budget()
+            cbc = gwf.output.budget()
         else:
             fname_cbc = os.path.join(ds.model_ws, ds.model_name + ".cbc")
     if fname_cbc is not None:
-        cbf = flopy.utils.CellBudgetFile(fname_cbc)
-    return cbf
+        cbc = flopy.utils.CellBudgetFile(fname_cbc)
+    return cbc
 
 
 def get_gwl_from_wet_cells(head, layer="layer", botm=None):
-    """
-    Get the groundwater level from a multi-dimensional head array where dry
+    """Get the groundwater level from a multi-dimensional head array where dry
     cells are NaN. This methods finds the most upper non-nan-value of each cell
     or timestep.
 
     Parameters
     ----------
     head : xarray.DataArray or numpy array
         A multi-dimensional array of head values. NaN-values represent inactive
@@ -163,15 +129,14 @@
         A DataArray with the botm of each model-cell. It can be used to set heads below
         the botm of the cells to NaN. botm is only used when head is a DataArray.
 
     Returns
     -------
     gwl : numpy-array
         An array of the groundwater-level, without the layer-dimension.
-
     """
     if isinstance(head, xr.DataArray):
         head_da = head
         if botm is not None:
             head_da = head_da.where(head_da > botm)
         head = head_da.data
         if isinstance(layer, str):
@@ -190,16 +155,15 @@
         top_layer = np.take(top_layer, 0, axis=layer)
         coords["layer"] = (dims, head_da.layer.data[top_layer])
         gwl = xr.DataArray(gwl, dims=dims, coords=coords)
     return gwl
 
 
 def get_head_at_point(head, x, y, ds=None, gi=None, drop_nan_layers=True):
-    """
-    Get the head at a certain point from a head DataArray for all cells.
+    """Get the head at a certain point from a head DataArray for all cells.
 
     Parameters
     ----------
     head : xarray.DataArray
         A DataArray of heads, with dimensions (time, layer, y, x) or (time, layer,
         icell2d).
     x : float
@@ -216,15 +180,14 @@
     drop_nan_layers : bool, optional
         Drop layers that are NaN at all timesteps. The default is True.
 
     Returns
     -------
     head_point : xarray.DataArray
         A DataArray with dimensions (time, layer).
-
     """
     if "icell2d" in head.dims:
         if gi is None:
             if ds is None:
                 raise (Exception("Please supply either gi or ds for a vertex grid"))
             gi = flopy.utils.GridIntersect(modelgrid_from_ds(ds), method="vertex")
         icelld2 = gi.intersect(Point(x, y))["cellids"][0]
@@ -331,30 +294,29 @@
 
 
 def calculate_gxg(
     head: xr.DataArray,
     below_surfacelevel: bool = False,
     tolerance: pd.Timedelta = pd.Timedelta(days=7),
 ) -> xr.DataArray:
-    """
-    Calculate GxG groundwater characteristics from head time series.
+    """Calculate GxG groundwater characteristics from head time series.
 
     GLG and GHG (average lowest and average highest groundwater level respectively) are
     calculated as the average of the three lowest (GLG) or highest (GHG) head values per
     Dutch hydrological year (april - april), for head values measured at a semi-monthly
     frequency (14th and 28th of every month). GVG (average spring groundwater level) is
     calculated as the average of groundwater level on 14th and 28th of March, and 14th
     of April. Supplied head values are resampled (nearest) to the 14/28 frequency.
 
     Hydrological years without all 24 14/28 dates present are discarded for glg and ghg.
     Years without the 3 dates for gvg are discarded.
 
     This method is copied from imod-python, and edited so that head-DataArray does not
     need to contain dimensions 'x' and 'y', so this method also works for refined grids.
-    THe original method can be found in:
+    The original method can be found in:
     https://gitlab.com/deltares/imod/imod-python/-/blob/master/imod/evaluate/head.py
 
     Parameters
     ----------
     head : xr.DataArray of floats
         Head relative to sea level, in m, or m below surface level if
         `below_surfacelevel` is set to True. Must have dimenstion 'time'.
@@ -376,15 +338,14 @@
     Examples
     --------
     Load the heads, and calculate groundwater characteristics for the simulation period:
 
     >>> import nlmod
     >>> head = nlmod.gwf.get_heads_da(ds)
     >>> gxg = nlmod.evaluate.calculate_gxg(head)
-
     """
     # if not head.dims == ("time", "y", "x"):
     #    raise ValueError('Dimensions must be ("time", "y", "x")')
     if not np.issubdtype(head["time"].dtype, np.datetime64):
         raise ValueError("Time must have dtype numpy datetime64")
 
     # Reindex to GxG frequency date_range: every 14th and 28th of the month.
```

### Comparing `nlmod-0.5.3/nlmod/gwf/recharge.py` & `nlmod-0.6.0/nlmod/gwf/recharge.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from ..dims.grid import da_to_reclist
 from ..sim.sim import get_tdis_perioddata
 
 logger = logging.getLogger(__name__)
 
 
-def model_datasets_to_rch(gwf, ds, mask=None, pname="rch", **kwargs):
+def ds_to_rch(gwf, ds, mask=None, pname="rch", **kwargs):
     """Convert the recharge data in the model dataset to a rch package with
     time series.
 
     Parameters
     ----------
     gwf : flopy.mf6.modflow.mfgwf.ModflowGwf
         groundwater flow model.
@@ -69,17 +69,15 @@
 
     # create timeseries packages
     _add_time_series(rch, rch_unique_dic, ds)
 
     return rch
 
 
-def model_datasets_to_evt(
-    gwf, ds, pname="evt", nseg=1, surface=None, depth=None, **kwargs
-):
+def ds_to_evt(gwf, ds, pname="evt", nseg=1, surface=None, depth=None, **kwargs):
     """Convert the evaporation data in the model dataset to a evt package with
     time series.
 
     Parameters
     ----------
     gwf : flopy.mf6.modflow.mfgwf.ModflowGwf
         groundwater flow model.
```

### Comparing `nlmod-0.5.3/nlmod/gwf/surface_water.py` & `nlmod-0.6.0/nlmod/gwf/surface_water.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,14 +463,15 @@
                     raise (
                         Exception("rbot and stage are below the bottom of the model")
                     )
             lays = [np.where(mask)[0][0]]
             conds = [cond]
         else:
             raise (Exception(f"Method {layer_method} unknown"))
+
         auxlist = []
         if "aux" in row:
             auxlist.append(row["aux"])
         if "boundname" in row:
             auxlist.append(row["boundname"])
 
         if ds.gridtype == "vertex":
@@ -491,16 +492,17 @@
     gdf_from,
     gdf_to,
     columns=None,
     desc="",
     silent=False,
     min_total_overlap=0.5,
     geom_type="Polygon",
+    add_index_from_column=None,
 ):
-    """ "Add information from gdf_from to gdf_to."""
+    """Add information from 'gdf_from' to 'gdf_to', based on the spatial intersection."""
     gdf_to = gdf_to.copy()
     if columns is None:
         columns = gdf_from.columns[~gdf_from.columns.isin(gdf_to.columns)]
     s = STRtree(gdf_from.geometry)
     for index in tqdm(gdf_to.index, desc=desc, disable=silent):
         geom_to = gdf_to.geometry[index]
         inds = s.query(geom_to)
@@ -519,14 +521,16 @@
             msg = f"Unsupported geometry type: {geom_type}"
             raise (Exception(msg))
 
         if np.any(measure.sum() > min_total_overlap * measure_org):
             # take the largest
             ind = measure.idxmax()
             gdf_to.loc[index, columns] = gdf_from.loc[ind, columns]
+            if add_index_from_column:
+                gdf_to.loc[index, add_index_from_column] = ind
     return gdf_to
 
 
 def get_gdf_stage(gdf, season="winter"):
     """Get the stage from a GeoDataFrame for a specific season.
 
     Parameters
@@ -548,17 +552,18 @@
         # when the minimum surface level is above the stage
         # or when no stage is available
         # use the minimum surface level
         stage = pd.concat((stage, gdf["ahn_min"]), axis=1).max(axis=1)
     return stage
 
 
-def download_level_areas(gdf, extent=None, config=None, raise_exceptions=True):
-    """
-    Download level areas (peilgebieden) of bronhouders.
+def download_level_areas(
+    gdf, extent=None, config=None, raise_exceptions=True, **kwargs
+):
+    """Download level areas (peilgebieden) of bronhouders.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, containing the column "bronhouder".
     extent : list, tuple or np.array
         Model extent (xmin, xmax, ymin, ymax). When extent is None, all data of the
@@ -573,26 +578,25 @@
         True.
 
     Returns
     -------
     la : dict
         A dictionary with the name of the waterboards as keys and GeoDataFrames with
         level areas as values.
-
     """
     if config is None:
         config = waterboard.get_configuration()
     bronhouders = gdf["bronhouder"].unique()
     la = {}
     data_kind = "level_areas"
     for wb in config.keys():
         if config[wb]["bgt_code"] in bronhouders:
             logger.info(f"Downloading {data_kind} for {wb}")
             try:
-                lawb = waterboard.get_data(wb, data_kind, extent)
+                lawb = waterboard.get_data(wb, data_kind, extent, **kwargs)
                 if len(lawb) == 0:
                     logger.info(f"No {data_kind} for {wb} found within model area")
                     continue
                 la[wb] = lawb
                 mask = ~la[wb].is_valid
                 if mask.any():
                     logger.warning(
@@ -607,17 +611,18 @@
                 elif raise_exceptions:
                     raise
                 else:
                     logger.warning(e)
     return la
 
 
-def download_watercourses(gdf, extent=None, config=None, raise_exceptions=True):
-    """
-    Download watercourses of bronhouders.
+def download_watercourses(
+    gdf, extent=None, config=None, raise_exceptions=True, **kwargs
+):
+    """Download watercourses of bronhouders.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, containing the column "bronhouder".
     extent : list, tuple or np.array
         Model extent (xmin, xmax, ymin, ymax). When extent is None, all data of the
@@ -632,26 +637,25 @@
         True.
 
     Returns
     -------
     wc : dict
         A dictionary with the name of the waterboards as keys and GeoDataFrames with
         watercourses as values.
-
     """
     if config is None:
         config = waterboard.get_configuration()
     bronhouders = gdf["bronhouder"].unique()
     wc = {}
     data_kind = "watercourses"
     for wb in config.keys():
         if config[wb]["bgt_code"] in bronhouders:
             logger.info(f"Downloading {data_kind} for {wb}")
             try:
-                wcwb = waterboard.get_data(wb, data_kind, extent)
+                wcwb = waterboard.get_data(wb, data_kind, extent, **kwargs)
                 if len(wcwb) == 0:
                     logger.info(f"No {data_kind} for {wb} found within model area")
                     continue
                 wc[wb] = wcwb
             except Exception as e:
                 if str(e) == f"{data_kind} not available for {wb}":
                     logger.warning(e)
@@ -661,16 +665,15 @@
                     logger.warning(e)
     return wc
 
 
 def add_stages_from_waterboards(
     gdf, la=None, extent=None, columns=None, config=None, min_total_overlap=0.0
 ):
-    """
-    Add information from level areas (peilgebieden) to bgt-polygons.
+    """Add information from level areas (peilgebieden) to bgt-polygons.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, containing the column "bronhouder".
     la : dict, optional
         A dictionary with the name of the waterboards as keys and GeoDataFrames with
@@ -691,42 +694,40 @@
         in gdf with all the features from the waterboard is larger than the fraction
         min_total_overlap. The default is 0.0.
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, with the added columns
-
     """
     if config is None:
         config = waterboard.get_configuration()
     if la is None:
         la = download_level_areas(gdf, extent=extent, config=config)
     if columns is None:
         columns = ["summer_stage", "winter_stage"]
     gdf[columns] = np.NaN
     for wb in la.keys():
         if len(la[wb]) == 0:
             continue
         mask = gdf["bronhouder"] == config[wb]["bgt_code"]
-        gdf.loc[mask] = add_info_to_gdf(
+        gdf.loc[mask, columns] = add_info_to_gdf(
             la[wb],
             gdf[mask],
             columns=columns,
             min_total_overlap=min_total_overlap,
             desc=f"Adding {columns} from {wb}",
-        )
+        )[columns]
     return gdf
 
 
 def add_bottom_height_from_waterboards(
     gdf, wc=None, extent=None, columns=None, config=None, min_total_overlap=0.0
 ):
-    """
-    Add information from watercourses to bgt-polygons.
+    """Add information from watercourses to bgt-polygons.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, containing the column "bronhouder".
     wc : dict, optional
         A dictionary with the name of the waterboards as keys and GeoDataFrames with
@@ -747,41 +748,39 @@
         in gdf with all the features from the waterboard is larger than the fraction
         min_total_overlap. The default is 0.0.
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, with the added columns
-
     """
     if config is None:
         config = waterboard.get_configuration()
     if wc is None:
         wc = download_watercourses(gdf, extent=extent, config=config)
     if columns is None:
         columns = ["bottom_height"]
     gdf[columns] = np.NaN
     for wb in wc.keys():
         if len(wc[wb]) == 0:
             continue
         mask = gdf["bronhouder"] == config[wb]["bgt_code"]
-        gdf.loc[mask] = add_info_to_gdf(
+        gdf.loc[mask, columns] = add_info_to_gdf(
             wc[wb],
             gdf[mask],
             columns=columns,
             min_total_overlap=min_total_overlap,
             desc=f"Adding {columns} from {wb}",
-            geom_type=None,
-        )
+            geom_type="LineString",
+        )[columns]
     return gdf
 
 
 def get_gdf(ds=None, extent=None, fname_ahn=None, ahn=None, buffer=0.0):
-    """
-    Generate a GeoDataFrame based on BGT-data and data from waterboards.
+    """Generate a GeoDataFrame based on BGT-data and data from waterboards.
 
     Parameters
     ----------
     ds : TYPE, optional
         The Model Dataset, used to determine the extent (when None) and to grid the
         surface level features. The default is None.
     extent : list, tuple or np.array
@@ -800,15 +799,14 @@
         minimum surface level near these features. The default is 0.0.
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, with added columns from waterboards
         and gridded to the model grid (when ds is aupplied)
-
     """
     if extent is None:
         if ds is None:
             raise (Exception("Please supply either ds or extent to get_gdf"))
         extent = get_extent_polygon(ds)
     gdf = bgt.get_bgt(extent)
     if fname_ahn is not None:
@@ -827,16 +825,16 @@
     gdf = add_bottom_height_from_waterboards(gdf, extent=extent)
     if ds is not None:
         return gdf_to_grid(gdf, ds).set_index("cellid")
     return gdf
 
 
 def add_min_ahn_to_gdf(gdf, ahn, buffer=0.0, column="ahn_min"):
-    """
-    Add a column names with the minimum surface level height near surface water features
+    """Add a column names with the minimum surface level height near surface
+    water features.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features
     ahn : xarray.DataArray
         A DataArray containing the height of the surface level.
@@ -848,18 +846,18 @@
         The default is 'ahn_min'.
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         A GeoDataFrame with surface water features, with an added column containing the
         minimum surface level height near the features.
-
     """
-    from geocube.api.core import make_geocube
     from functools import partial
+
+    from geocube.api.core import make_geocube
     from geocube.rasterize import rasterize_image
 
     # use geocube
     gc = make_geocube(
         vector_data=gdf.buffer(buffer).reset_index().rename_geometry("geometry"),
         measurements=["index"],
         like=ahn,  # ensure the data are on the same grid
```

### Comparing `nlmod-0.5.3/nlmod/gwf/wells.py` & `nlmod-0.6.0/nlmod/gwf/wells.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,43 +14,49 @@
     aux=None,
     boundnames=None,
     **kwargs,
 ):
     # collect data
     well_lrcd = []
 
-    for _, irow in tqdm(df.iterrows(), total=df.index.size, desc="Adding WELs"):
+    for wnam, irow in tqdm(df.iterrows(), total=df.index.size, desc="Adding WELs"):
         try:
             cid1 = gwf.modelgrid.intersect(irow[x], irow[y], irow[top], forgive=False)
             cid2 = gwf.modelgrid.intersect(irow[x], irow[y], irow[botm], forgive=False)
         except Exception:
-            print(f"Warning! well {_} outside of model domain! ({irow[x]}, {irow[y]})")
+            print(
+                f"Warning! well {wnam} outside of model domain! ({irow[x]}, {irow[y]})"
+            )
             continue
+        kb = cid2[0]
         if len(cid1) == 2:
             kt, icell2d = cid1
+            idomain_mask = gwf.modelgrid.idomain[kt : kb + 1, icell2d] > 0
         elif len(cid1) == 3:
             kt, i, j = cid1
-        kb = cid2[0]
-        wlayers = np.arange(kt, kb + 1)
+            idomain_mask = gwf.modelgrid.idomain[kt : kb + 1, i, j] > 0
+        # mask only active cells
+        wlayers = np.arange(kt, kb + 1)[idomain_mask]
         for k in wlayers:
             if len(cid1) == 2:
                 wdata = [(k, icell2d), irow[Q] / len(wlayers)]
             elif len(cid1) == 3:
                 wdata = [(k, i, j), irow[Q] / len(wlayers)]
 
             if aux is not None:
-                wdata.append(irow[aux])
+                if not isinstance(aux, list):
+                    aux = [aux]
+                for iaux in aux:
+                    wdata.append(irow[iaux])
             if boundnames is not None:
                 wdata.append(irow[boundnames])
             well_lrcd.append(wdata)
 
     wel_spd = {0: well_lrcd}
 
-    if aux is not None:
-        aux = True
     wel = fp.mf6.ModflowGwfwel(
         gwf,
         stress_period_data=wel_spd,
         auxiliary=aux,
         boundnames=boundnames is not None,
         **kwargs,
     )
@@ -79,20 +85,23 @@
     for iw, irow in tqdm(df.iterrows(), total=df.index.size, desc="Adding MAWs"):
         try:
             cid1 = gwf.modelgrid.intersect(irow[x], irow[y], irow[top], forgive=False)
             cid2 = gwf.modelgrid.intersect(irow[x], irow[y], irow[botm], forgive=False)
         except Exception:
             print(f"Warning! well {iw} outside of model domain! ({irow[x]}, {irow[y]})")
             continue
+        kb = cid2[0]
         if len(cid1) == 2:
             kt, icell2d = cid1
+            idomain_mask = gwf.modelgrid.idomain[kt : kb + 1, icell2d] > 0
         elif len(cid1) == 3:
             kt, i, j = cid1
-        kb = cid2[0]
-        wlayers = np.arange(kt, kb + 1)
+            idomain_mask = gwf.modelgrid.idomain[kt : kb + 1, i, j] > 0
+
+        wlayers = np.arange(kt, kb + 1)[idomain_mask]
 
         # <wellno> <radius> <bottom> <strt> <condeqn> <ngwfnodes>
         pakdata = [iw, irow[rw], irow[top], strt, condeqn, len(wlayers)]
         if boundnames is not None:
             pakdata.append(irow[boundnames])
         maw_pakdata.append(pakdata)
         # <wellno> <mawsetting>
```

### Comparing `nlmod-0.5.3/nlmod/gwt/gwt.py` & `nlmod-0.6.0/nlmod/gwt/gwt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,19 @@
 import logging
 import numbers
 
 import flopy
 
 from ..dims import grid
 from ..gwf.gwf import _dis, _disv, _set_record
+from ..util import _get_value_from_ds_attr, _get_value_from_ds_datavar
 
 logger = logging.getLogger(__name__)
 
 
-def _get_value_from_ds_attr(ds, varname, attr=None, value=None, warn=True):
-    """Internal function to get value from dataset attributes.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        dataset containing model data
-    varname : str
-        name of the variable in flopy package
-    attr : str, optional
-        name of the attribute in dataset (is sometimes different to varname)
-    value : Any, optional
-        variable value, by default None
-    warn : bool, optional
-        log warning if value not found
-
-    Returns
-    -------
-    value : Any
-        returns variable value, if value was None, attempts to obtain
-        variable from dataset attributes.
-    """
-    if attr is None:
-        attr = varname
-
-    if value is not None and (attr in ds.attrs):
-        logger.info(
-            f"Using user-provided '{varname}' and not stored attribute 'ds.{attr}'"
-        )
-    elif value is None and (attr in ds.attrs):
-        value = ds.attrs[attr]
-    elif value is None:
-        if warn:
-            msg = (
-                f"No value found for '{varname}', passing None to flopy. "
-                f"To fix this error pass '{varname}' to function or set 'ds.{attr}'."
-            )
-            logger.warning(msg)
-        # raise ValueError(msg)
-    return value
-
-
-def _get_value_from_ds_datavar(ds, varname, datavar=None, value=None, warn=True):
-    """Internal function to get value from dataset data variables.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        dataset containing model data
-    varname : str
-        name of the variable in flopy package
-    datavar : str, optional
-        name of the data variable (is sometimes different to varname) in dataset
-    value : Any, optional
-        variable value, by default None
-    warn : bool, optional
-        log warning if value not found
-
-    Returns
-    -------
-    value : Any
-        returns variable value, if value was None, attempts to obtain
-        variable from dataset data variables.
-    """
-    if datavar is None:
-        datavar = varname
-
-    if (value is not None) and (datavar in ds):
-        logger.info(
-            f"Using user-provided '{varname}' and not"
-            f" stored data variable 'ds.{datavar}'"
-        )
-    elif value is None and (datavar in ds):
-        value = ds[datavar]
-    elif value is None:
-        if warn:
-            msg = (
-                f"No value found for '{varname}', passing None to flopy. "
-                f"To fix this error pass '{varname}' to function or set 'ds.{datavar}'."
-            )
-            logger.warning(msg)
-        # raise ValueError(msg)
-    return value
-
-
 def gwt(ds, sim, modelname=None, **kwargs):
     """create groundwater transport model from the model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data. Should have the dimension 'time' and the
@@ -271,22 +187,27 @@
 
     Returns
     -------
     mst : flopy ModflowGwtmst
         mst package
     """
     logger.info("creating modflow MST")
-    if isinstance(porosity, str):
-        porosity = None
+
     # NOTE: attempting to look for porosity in attributes first, then data variables.
     # If both are defined, the attribute value will be used. The log message in this
     # case is not entirely correct. This is something we may need to sort out, and
     # also think about the order we do this search.
-    porosity = _get_value_from_ds_attr(ds, "porosity", value=porosity, warn=False)
-    porosity = _get_value_from_ds_datavar(ds, "porosity", value=porosity)
+    if isinstance(porosity, str):
+        value = None
+    else:
+        value = porosity
+    porosity = _get_value_from_ds_attr(
+        ds, "porosity", porosity, value=value, warn=False
+    )
+    porosity = _get_value_from_ds_datavar(ds, "porosity", porosity)
     mst = flopy.mf6.ModflowGwtmst(gwt, porosity=porosity, **kwargs)
     return mst
 
 
 def cnc(ds, gwt, da_mask, da_conc, pname="cnc", **kwargs):
     """create constant concentration package for groundwater transport model.
```

### Comparing `nlmod-0.5.3/nlmod/gwt/prepare.py` & `nlmod-0.6.0/nlmod/gwt/prepare.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/modpath/modpath.py` & `nlmod-0.6.0/nlmod/modpath/modpath.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numbers
 import os
 from shutil import copyfile
 
 import flopy
 import geopandas as gpd
 import pandas as pd
+from packaging.version import parse as parse_version
 
 from .. import util
 from ..dims.grid import xy_to_icell2d
 
 logger = logging.getLogger(__name__)
 
 
@@ -157,15 +158,15 @@
                 if mpf.ib[lay, icell2d] > 0:
                     nodes.append(node)
             node += 1
 
     return nodes
 
 
-def mpf(gwf, exe_name=None, modelname=None):
+def mpf(gwf, exe_name=None, modelname=None, model_ws=None):
     """Create a modpath model from a groundwater flow model.
 
     Parameters
     ----------
     gwf : flopy.mf6.mfmodel.MFModel
         Groundwater flow model.
     exe_name: str, optional
@@ -186,14 +187,17 @@
     -------
     mpf : flopy.modpath.mp7.Modpath7
         modpath object.
     """
     if modelname is None:
         modelname = "mp7_" + gwf.name
 
+    if model_ws is None:
+        model_ws = os.path.join(gwf.model_ws, "modpath")
+
     # check if the save flows parameter is set in the npf package
     npf = gwf.get_package("npf")
     if not npf.save_flows.array:
         raise ValueError(
             "the save_flows option of the npf package should be True not None"
         )
 
@@ -201,25 +205,41 @@
     if gwf.simulation.tdis.start_date_time.array is not None:
         logger.warning(
             "older versions of modpath cannot handle this, see https://github.com/MODFLOW-USGS/modpath-v7/issues/31"
         )
 
     # get executable
     if exe_name is None:
-        exe_name = util.get_exe_path("mp7")
+        exe_name = util.get_exe_path("mp7_2_002_provisional")
 
     # create mpf model
     mpf = flopy.modpath.Modpath7(
         modelname=modelname,
         flowmodel=gwf,
         exe_name=exe_name,
-        model_ws=gwf.model_ws,
+        model_ws=model_ws,
         verbose=True,
     )
 
+    if model_ws != gwf.model_ws and parse_version(flopy.__version__) <= parse_version(
+        "3.3.6"
+    ):
+        mpf.grbdis_file = os.path.relpath(
+            os.path.join(gwf.model_ws, mpf.grbdis_file), model_ws
+        )
+        mpf.headfilename = os.path.relpath(
+            os.path.join(gwf.model_ws, mpf.headfilename), model_ws
+        )
+        mpf.budgetfilename = os.path.relpath(
+            os.path.join(gwf.model_ws, mpf.budgetfilename), model_ws
+        )
+        mpf.tdis_file = os.path.relpath(
+            os.path.join(gwf.model_ws, mpf.tdis_file), model_ws
+        )
+
     return mpf
 
 
 def bas(mpf, porosity=0.3, **kwargs):
     """Create the basic package for the modpath model.
 
     Parameters
```

### Comparing `nlmod-0.5.3/nlmod/plot.py` & `nlmod-0.6.0/nlmod/dims/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,718 +1,659 @@
-import os
-import warnings
+import datetime as dt
+import logging
+import numbers
 
-import flopy
-import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
-from matplotlib.collections import PatchCollection
-from matplotlib.colors import ListedColormap, Normalize
-from matplotlib.patches import Patch, Polygon
-from matplotlib.ticker import FuncFormatter, MultipleLocator
-
-from .dcs import DatasetCrossSection
-from .dims.grid import get_vertices, modelgrid_from_ds
-from .dims.resample import get_affine_mod_to_world, get_extent
-from .read import geotop, rws
-
-
-def surface_water(model_ds, ax=None, **kwargs):
-    surf_water = rws.get_gdf_surface_water(model_ds)
-
-    if ax is None:
-        _, ax = plt.subplots()
-    surf_water.plot(ax=ax, **kwargs)
-
-    return ax
-
-
-def modelgrid(ds, ax=None, add_surface_water=False, **kwargs):
-    if ax is None:
-        _, ax = plt.subplots(figsize=(10, 10))
-    modelgrid = modelgrid_from_ds(ds)
-    modelgrid.plot(ax=ax, **kwargs)
-    ax.axis("scaled")
-    if add_surface_water:
-        surface_water(ds, ax=ax)
-        ax.set_title("modelgrid with surface water")
-    else:
-        ax.set_title("modelgrid")
-    ax.set_ylabel("y [m RD]")
-    ax.set_xlabel("x [m RD]")
-
-    return ax
-
-
-def facet_plot(
-    gwf,
-    arr,
-    lbl="",
-    plot_dim="layer",
-    layer=None,
-    period=None,
-    cmap="viridis",
-    scale_cbar=True,
-    vmin=None,
-    vmax=None,
-    norm=None,
-    xlim=None,
-    ylim=None,
-    grid=False,
-    figdir=None,
-    figsize=(10, 8),
-    plot_bc=None,
-    plot_grid=False,
-):
-    if arr.ndim == 4 and plot_dim == "layer":
-        nplots = arr.shape[1]
-    elif arr.ndim == 4 and plot_dim == "time":
-        nplots = arr.shape[0]
-    elif arr.ndim == 3:
-        nplots = arr.shape[0]
-    else:
-        raise ValueError("Array must have at least 3 dimensions.")
-
-    plots_per_row = int(np.ceil(np.sqrt(nplots)))
-    plots_per_col = nplots // plots_per_row + 1
-
-    fig, axes = plt.subplots(
-        plots_per_col,
-        plots_per_row,
-        figsize=figsize,
-        sharex=True,
-        sharey=True,
-        constrained_layout=True,
-    )
-
-    if scale_cbar:
-        vmin = np.nanmin(arr)
-        vmax = np.nanmax(arr)
-
-    for i in range(nplots):
-        iax = axes.flat[i]
-        iax.set_aspect("equal")
-        if plot_dim == "layer":
-            ilay = i
-            iper = period
-            if arr.ndim == 4:
-                if iper is None:
-                    raise ValueError("Pass 'period' to select timestep to plot.")
-                a = arr[iper]
-        elif plot_dim == "time":
-            ilay = layer
-            iper = i
-            if arr.ndim == 4:
-                if ilay is None:
-                    raise ValueError("Pass 'layer' to select layer to plot.")
-                a = arr[iper]
-        else:
-            raise ValueError("'plot_dim' must be one of ['layer', 'time']")
-
-        mp = flopy.plot.PlotMapView(model=gwf, layer=ilay, ax=iax)
-        qm = mp.plot_array(a, cmap=cmap, vmin=vmin, vmax=vmax, norm=norm)
+from scipy.spatial import cKDTree
 
-        mp.plot_ibound(color_vpt="darkgray")
+from .. import util
+from . import resample
+from .layers import fill_nan_top_botm_kh_kv, set_idomain
 
-        if plot_grid:
-            mp.plot_grid(lw=0.25, color="k")
+logger = logging.getLogger(__name__)
 
-        if plot_bc is not None:
-            for bc, bc_kwargs in plot_bc.items():
-                mp.plot_bc(bc, **bc_kwargs)
 
-        iax.grid(grid)
-        iax.set_xticklabels([])
-        iax.set_yticklabels([])
-
-        if plot_dim == "layer":
-            iax.set_title(f"Layer {ilay}", fontsize=6)
-        elif plot_dim == "time":
-            iax.set_title(f"Timestep {iper}", fontsize=6)
-
-        if xlim is not None:
-            iax.set_xlim(xlim)
-        if ylim is not None:
-            iax.set_ylim(ylim)
-
-    for iax in axes.ravel()[nplots:]:
-        iax.set_visible(False)
-
-    cb = fig.colorbar(qm, ax=axes, shrink=1.0)
-    cb.set_label(lbl)
-
-    if figdir:
-        fig.savefig(
-            os.path.join(figdir, f"{lbl}_per_{plot_dim}.png"),
-            dpi=150,
-            bbox_inches="tight",
-        )
-
-    return fig, axes
-
-
-def facet_plot_ds(
-    gwf,
-    model_ds,
-    figdir,
-    plot_var="bot",
-    plot_time=None,
-    plot_bc=("CHD",),
-    color="k",
-    grid=False,
-    xlim=None,
-    ylim=None,
-):
-    """make a 2d plot of every modellayer, store them in a grid.
+def set_ds_attrs(ds, model_name, model_ws, mfversion="mf6", exe_name=None):
+    """set the attribute of a model dataset.
 
     Parameters
     ----------
-    gwf : Groundwater flow
-        Groundwaterflow model.
-    model_ds : xr.DataSet
-        model data.
-    figdir : str
-        file path figures.
-    plot_var : str, optional
-        variable in model_ds. The default is 'bot'.
-    plot_time : int, optional
-        time step if plot_var is time variant. The default is None.
-    plot_bc : list of str, optional
-        name of packages of which boundary conditions are plot. The default
-        is ['CHD'].
-    color : str, optional
-        color. The default is 'k'.
-    grid : bool, optional
-        if True a grid is plotted. The default is False.
-    xlim : tuple, optional
-        xlimits. The default is None.
-    ylim : tuple, optional
-        ylimits. The default is None.
+    ds : xarray dataset
+        An existing model dataset
+    model_name : str
+        name of the model.
+    model_ws : str or None
+        workspace of the model. This is where modeldata is saved to.
+    mfversion : str, optional
+        modflow version. The default is "mf6".
+    exe_name: str, optional
+        path to modflow executable, default is None, which assumes binaries
+        are available in nlmod/bin directory. Binaries can be downloaded
+        using `nlmod.util.download_mfbinaries()`.
 
     Returns
     -------
-    fig : TYPE
-        DESCRIPTION.
-    axes : TYPE
-        DESCRIPTION.
+    ds : xarray dataset
+        model dataset.
     """
-    for key in plot_bc:
-        if key not in gwf.get_package_list():
-            raise ValueError(
-                f"cannot plot boundary condition {key} because it is not in the package list"
-            )
-
-    nlay = len(model_ds.layer)
-
-    plots_per_row = int(np.ceil(np.sqrt(nlay)))
-    plots_per_col = nlay // plots_per_row + 1
-
-    fig, axes = plt.subplots(
-        plots_per_col,
-        plots_per_row,
-        figsize=(11, 10),
-        sharex=True,
-        sharey=True,
-        dpi=150,
-    )
-    if plot_time is None:
-        plot_arr = model_ds[plot_var]
-    else:
-        plot_arr = model_ds[plot_var][plot_time]
-
-    vmin = plot_arr.min()
-    vmax = plot_arr.max()
-    for ilay in range(nlay):
-        iax = axes.ravel()[ilay]
-        mp = flopy.plot.PlotMapView(model=gwf, layer=ilay, ax=iax)
-        # mp.plot_grid()
-        qm = mp.plot_array(plot_arr[ilay].values, cmap="viridis", vmin=vmin, vmax=vmax)
-        # qm = mp.plot_array(hf[-1], cmap="viridis", vmin=-0.1, vmax=0.1)
-        # mp.plot_ibound()
-        # plt.colorbar(qm)
-        for bc_var in plot_bc:
-            mp.plot_bc(bc_var, kper=0, color=color)
-
-        iax.set_aspect("equal", adjustable="box")
-        iax.set_title(f"Layer {ilay}")
-
-        iax.grid(grid)
-        if xlim is not None:
-            iax.set_xlim(xlim)
-        if ylim is not None:
-            iax.set_ylim(ylim)
-
-    for iax in axes.ravel()[nlay:]:
-        iax.set_visible(False)
-
-    cb = fig.colorbar(qm, ax=axes, shrink=1.0)
-    cb.set_label(f"{plot_var}", rotation=270)
-    fig.suptitle(f"{plot_var} Time = {(model_ds.nper*model_ds.perlen)/365} year")
-    fig.tight_layout()
-    fig.savefig(
-        os.path.join(figdir, f"{plot_var}_per_layer.png"),
-        dpi=150,
-        bbox_inches="tight",
-    )
-
-    return fig, axes
-
-
-def plot_array(gwf, array, figsize=(8, 8), colorbar=True, ax=None, **kwargs):
-    warnings.warn(
-        "The 'plot.plot_array' function is deprecated please use"
-        "'plot.data_array' instead",
-        DeprecationWarning,
-    )
-    if ax is None:
-        _, ax = plt.subplots(figsize=figsize)
-
-    yticklabels = ax.yaxis.get_ticklabels()
-    plt.setp(yticklabels, rotation=90, verticalalignment="center")
-    ax.axis("scaled")
-    pmv = flopy.plot.PlotMapView(modelgrid=gwf.modelgrid, ax=ax)
-    pcm = pmv.plot_array(array, **kwargs)
-    if colorbar:
-        fig = ax.get_figure()
-        fig.colorbar(pcm, ax=ax, orientation="vertical")
-        # plt.colorbar(pcm)
-    if hasattr(array, "name"):
-        ax.set_title(array.name)
-    # set rotation of y ticks to zero
-    plt.setp(ax.yaxis.get_majorticklabels(), rotation=0)
-    return ax
 
+    if model_name is not None and len(model_name) > 16 and mfversion == "mf6":
+        raise ValueError("model_name can not have more than 16 characters")
+    ds.attrs["model_name"] = model_name
+    ds.attrs["mfversion"] = mfversion
+    fmt = "%Y%m%d_%H:%M:%S"
+    ds.attrs["model_dataset_created_on"] = dt.datetime.now().strftime(fmt)
+
+    if exe_name is None:
+        exe_name = util.get_exe_path(mfversion)
+
+    ds.attrs["exe_name"] = exe_name
+
+    # add some directories
+    if model_ws is not None:
+        figdir, cachedir = util.get_model_dirs(model_ws)
+        ds.attrs["model_ws"] = model_ws
+        ds.attrs["figdir"] = figdir
+        ds.attrs["cachedir"] = cachedir
+
+    return ds
+
+
+def to_model_ds(
+    ds,
+    model_name=None,
+    model_ws=None,
+    extent=None,
+    delr=100.0,
+    delc=None,
+    fill_nan=True,
+    extrapolate=True,
+    anisotropy=10,
+    fill_value_kh=1.0,
+    fill_value_kv=0.1,
+    xorigin=0.0,
+    yorigin=0.0,
+    angrot=0.0,
+    drop_attributes=True,
+    transport=False,
+):
+    """Transform an input dataset to a groundwater model dataset.
 
-def plot_vertex_array(da, vertices, ax=None, gridkwargs=None, **kwargs):
-    """plot dataarray with gridtype vertex.
+    Optionally select a different grid size.
 
     Parameters
     ----------
-    da : xarray.Datarray
-        plot data with dimension(icell2d).
-    vertices : xarray.Datarray or numpy.ndarray
-        Vertex coördinates per cell with dimensions(icell2d, 4, 2)
-    ax : TYPE, optional
-        DESCRIPTION. The default is None.
-    gridkwargs : dict or None, optional
-        layout parameters to plot the cells. For example
-        {'edgecolor':'k'} to create black cell lines. The default is None.
-    **kwargs :
-        passed to quadmesh.set().
+    ds : xarray.dataset
+        A layer model dataset.
+    model_name : str, optional
+        name of the model. The default is None
+    model_ws : str, optional
+        workspace of the model. This is where modeldata is saved to. The
+        default is None
+    extent : list or tuple of length 4, optional
+        The extent of the new grid. Get from ds when None. The default is None.
+    delr : int, float, list, tuple or array, optional
+        The gridsize along columns (dx). The default is 100. meter.
+    delc : None, int, float, list, tuple or array, optional
+        The gridsize along rows (dy). Set to delr when None. If None delc=delr
+        The default is None.
+    fill_nan : bool, optional
+        if True nan values in the top, botm, kh and kv are filled using the
+        fill_nan_top_botm_kh_kv function. Layers with only nan values in the
+        botm are removed.
+    extrapolate : bool, optional
+        When true, extrapolate data-variables, into the sea or other areas with
+        only nans. The default is True
+    anisotropy : int or float
+        factor to calculate kv from kh or the other way around
+    fill_value_kh : int or float, optional
+        use this value for kh if there is no data. The default is 1.0.
+    fill_value_kv : int or float, optional
+        use this value for kv if there is no data. The default is 0.1.
+    xorigin : int or float, optional
+        lower left x coordinate of the model grid only used if angrot != 0.
+        Default is 0.0.
+    yorigin : int or float, optional
+        lower left y coordinate of the model grid only used if angrot != 0.
+        Default is 0.0.
+    angrot : int or float, optinal
+        the rotation of the grid in counter clockwise degrees, default is 0.0
+    drop_attributes : bool, optional
+        if True drop the attributes from the layer model dataset. Otherwise
+        keep the attributes. Default is True.
+    transport : bool, optional
+        flag indicating whether dataset includes data for a groundwater
+        transport model (GWT). Default is False, no transport.
 
     Returns
     -------
-    ax : TYPE
-        DESCRIPTION.
+    ds : xarray.dataset
+        the model Dataset.
     """
-    DeprecationWarning("plot.plot_vertex_array is deprecated. Use plot.data_array.")
-
-    if isinstance(vertices, xr.Dataset):
-        vertices = get_vertices(vertices)
-    if isinstance(vertices, xr.DataArray):
-        vertices = vertices.values
-
-    if ax is None:
-        _, ax = plt.subplots()
-
-    patches = [Polygon(vert) for vert in vertices]
-    if gridkwargs is None:
-        pc = PatchCollection(patches)
-    else:
-        pc = PatchCollection(patches, **gridkwargs)
-    pc.set_array(da)
+    if extent is None:
+        extent = ds.attrs["extent"]
 
-    # set max and min
-    if "vmin" in kwargs:
-        vmin = kwargs.pop("vmin")
-    else:
-        vmin = da.min()
+    # drop attributes
+    if drop_attributes:
+        ds = ds.copy()
+        for attr in list(ds.attrs):
+            del ds.attrs[attr]
+
+    # convert dataset to grid
+    logger.info("resample layer model data to structured modelgrid")
+    ds = resample.ds_to_structured_grid(
+        ds, extent, delr, delc, xorigin=xorigin, yorigin=yorigin, angrot=angrot
+    )
 
-    if "vmax" in kwargs:
-        vmax = kwargs.pop("vmax")
+    # add cell area variable
+    if delc is None:
+        delc = delr
+    if isinstance(delr, (numbers.Number)) and isinstance(delc, (numbers.Number)):
+        ds["area"] = ("y", "x"), ds.delr * ds.delc * np.ones(
+            (ds.dims["y"], ds.dims["x"])
+        )
+    elif isinstance(delr, np.ndarray) and isinstance(delc, np.ndarray):
+        ds["area"] = ("y", "x"), np.outer(delc, delr)
+        ds["delr"] = ("x"), delr
+        ds["delc"] = ("y"), delc
     else:
-        vmax = da.max()
+        raise TypeError("unexpected type for delr and/or delc")
 
-    # limit the color range
-    pc.set_clim(vmin=vmin, vmax=vmax)
-    pc.set(**kwargs)
+    if extrapolate:
+        ds = extrapolate_ds(ds)
 
-    ax.add_collection(pc)
-    ax.set_xlim(vertices[:, :, 0].min(), vertices[:, :, 0].max())
-    ax.set_xlabel("x")
-    ax.set_ylabel("y")
-    ax.set_ylim(vertices[:, :, 1].min(), vertices[:, :, 1].max())
-    ax.set_aspect("equal")
+    # add attributes
+    ds = set_ds_attrs(ds, model_name, model_ws)
+    ds.attrs["transport"] = int(transport)
+
+    # fill nan's and add idomain
+    if fill_nan:
+        ds = fill_nan_top_botm_kh_kv(
+            ds,
+            anisotropy=anisotropy,
+            fill_value_kh=fill_value_kh,
+            fill_value_kv=fill_value_kv,
+        )
+    else:
+        ds = set_idomain(ds, remove_nan_layers=False)
 
-    ax.get_figure().colorbar(pc, ax=ax, orientation="vertical")
-    if hasattr(da, "name"):
-        ax.set_title(da.name)
+    return ds
 
-    return ax
 
+def extrapolate_ds(ds, mask=None):
+    """Fill missing data in layermodel based on nearest interpolation.
 
-def data_array(da, ds=None, ax=None, rotated=False, edgecolor=None, **kwargs):
-    """Plot an xarray DataArray, using information from the model Dataset ds.
+    Used for ensuring layer model contains data everywhere. Useful for
+    filling in data beneath the sea for coastal groundwater models, or models
+    near the border of the Netherlands.
 
     Parameters
     ----------
-    da : xarray.DataArray
-        The DataArray (structured or vertex) you like to plot.
-    ds : xarray.DataSet, optional
-        Needed when the gridtype is vertex or rotated is True. The default is None.
-    ax : matplotlib.Axes, optional
-        The axes used for plotting. Set to current axes when None. The default is None.
-    rotated : bool, optional
-        Plot the data-array in rotated coordinates
-    **kwargs : cit
-        Kwargs are passed to PatchCollection (vertex) or pcolormesh (structured).
+    ds : xarray.DataSet
+        Model layer DataSet
+    mask: np.ndarray, optional
+        Boolean mask for each cell, with a value of True if its value needs to
+        be determined. When mask is None, it is determined from the botm-
+        variable. The default is None.
 
     Returns
     -------
-    matplotlib QuadMesh or PatchCollection
-        The object containing the cells.
+    ds : xarray.DataSet
+        filled layermodel
     """
-    if ax is None:
-        ax = plt.gca()
-    if "icell2d" in da.dims:
-        if ds is None:
-            raise (Exception("Supply model dataset (ds) for grid information"))
-        if isinstance(ds, list):
-            patches = ds
-        else:
-            patches = get_patches(ds, rotated=rotated)
-        if edgecolor is None:
-            edgecolor = "face"
-        pc = PatchCollection(patches, edgecolor=edgecolor, **kwargs)
-        pc.set_array(da)
-        ax.add_collection(pc)
-        if ax.get_autoscale_on():
-            extent = get_extent(ds, rotated=rotated)
-            ax.axis(extent)
-        return pc
-    else:
-        x = da.x
-        y = da.y
-        if rotated:
-            if ds is None:
-                raise (Exception("Supply model dataset (ds) for grid information"))
-            if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
-                affine = get_affine_mod_to_world(ds)
-                x, y = affine * np.meshgrid(x, y)
-        return ax.pcolormesh(x, y, da, shading="nearest", edgecolor=edgecolor, **kwargs)
-
-
-def get_patches(ds, rotated=False):
-    """Get the matplotlib patches for a vertex grid, which can be used in
-    da()"""
-    assert "icell2d" in ds.dims
-    xy = np.column_stack((ds["xv"].data, ds["yv"].data))
-    if rotated and "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
-        affine = get_affine_mod_to_world(ds)
-        xy[:, 0], xy[:, 1] = affine * (xy[:, 0], xy[:, 1])
-    icvert = ds["icvert"].data
-    if "_FillValue" in ds["icvert"].attrs:
-        nodata = ds["icvert"].attrs["_FillValue"]
+    if mask is None:
+        mask = np.isnan(ds["botm"]).all("layer").data
+    if not mask.any():
+        # all of the model cells are is inside the known area
+        return ds
+    if mask.all():
+        raise (Exception("The model only contains NaNs"))
+    if "gridtype" in ds.attrs and ds.gridtype == "vertex":
+        x = ds.x.data
+        y = ds.y.data
+        dims = ("icell2d",)
     else:
-        nodata = -1
-        icvert = icvert.copy()
-        icvert[np.isnan(icvert)] = nodata
-        icvert = icvert.astype(int)
-    patches = []
-    for icell2d in ds.icell2d.data:
-        patches.append(Polygon(xy[icvert[icell2d, icvert[icell2d] != nodata]]))
-    return patches
-
-
-def get_map(
-    extent,
-    figsize=10.0,
-    nrows=1,
-    ncols=1,
-    base=1000.0,
-    fmt="{:.0f}",
-    sharex=False,
-    sharey=True,
-    crs=28992,
-    background=False,
-    alpha=0.5,
+        x, y = np.meshgrid(ds.x, ds.y)
+        dims = ("y", "x")
+    points = np.stack((x[~mask], y[~mask]), axis=1)
+    xi = np.stack((x[mask], y[mask]), axis=1)
+    # geneterate the tree only once, to increase speed
+    tree = cKDTree(points)
+    _, i = tree.query(xi)
+    for key in ds:
+        if not np.any([dim in ds[key].dims for dim in dims]):
+            continue
+        data = ds[key].data
+        if ds[key].dims == dims:
+            data[mask] = data[~mask][i]
+        elif ds[key].dims == ("layer",) + dims:
+            for lay in range(len(ds["layer"])):
+                data[lay][mask] = data[lay][~mask][i]
+        else:
+            raise (Exception(f"Dimensions {ds[key].dims} not supported"))
+        # make sure to set the data (which for some reason is sometimes needed)
+        ds[key].data = data
+    return ds
+
+
+def _get_structured_grid_ds(
+    xedges,
+    yedges,
+    nlay=1,
+    top=np.nan,
+    botm=np.nan,
+    xorigin=0.0,
+    yorigin=0.0,
+    angrot=0,
+    attrs=None,
+    crs=None,
 ):
-    """Generate a motplotlib Figure with a map with the axis set to extent.
+    """Create an xarray dataset with structured grid geometry.
 
     Parameters
     ----------
-    extent : list of 4 floats
-        The model extent .
-    figsize : float or list of 2 floats, optional
-        The size of the figure, in inches. The default is 10, which means the
-        figsize is determined automatically.
-    nrows : int, optional
-        The number of rows. The default is 1.
-    ncols : int, optional
-        The number of columns. The default is 1.
-    base : float, optional
-        The interval for ticklabels on the x- and y-axis. The default is 1000.
-        m.
-    fmt : string, optional
-        The format of the ticks on the x- and y-axis. The default is "{:.0f}".
-    sharex : bool, optional
-        Only display the ticks on the lowest x-axes, when nrows > 1. The
-        default is False.
-    sharey : bool, optional
-        Only display the ticks on the left y-axes, when ncols > 1. The default
-        is True.
-    background : bool or str, optional
-        Draw a background using contextily when True or when background is a string.
-        When background is a string it repesents the map-provider. Use
-        nlmod.plot._list_contextily_providers().keys() to show possible map-providers.
-        THe defaults is False.
-    alpha: float, optional
-        The alpha value of the background. The default is 0.5.
+    xedges : array_like
+        A 1D array of the x coordinates of the grid edges.
+    yedges : array_like
+        A 1D array of the y coordinates of the grid edges.
+    nlay : int, optional
+        The number of layers in the grid. Default is 1.
+    top : array_like, optional
+        A 2D array of the top elevation of the grid cells. Default is NaN.
+    botm : array_like, optional
+        A 3D array of the bottom elevation of the grid cells. Default is NaN.
+    xorigin : float, optional
+        The x-coordinate origin of the grid. Default is 0.0.
+    yorigin : float, optional
+        The y-coordinate origin of the grid. Default is 0.0.
+    angrot : float, optional
+        The counter-clockwise rotation angle of the grid, in degrees.
+        Default is 0.
+    attrs : dict, optional
+        A dictionary of attributes to add to the xarray dataset. Default is an
+        empty dictionary.
+    crs : dict or str, optional
+        A dictionary or string describing the coordinate reference system of
+        the grid. Default is None.
 
     Returns
     -------
-    f : matplotlib.Figure
-        The resulting figure.
-    axes : matplotlib.Axes or numpy array of matplotlib.Axes
-        the ax or axes (when ncols/nrows > 1).
-    """
-    if isinstance(figsize, (float, int)):
-        xh = 0.0
-        if base is None:
-            xh = 0.0
-        figsize = get_figsize(extent, nrows=nrows, ncols=ncols, figw=figsize, xh=xh)
-    f, axes = plt.subplots(
-        figsize=figsize, nrows=nrows, ncols=ncols, sharex=sharex, sharey=sharey
-    )
-    if isinstance(background, bool) and background is True:
-        background = "nlmaps.standaard"
+    ds : xarray.Dataset
+        An xarray dataset with the following data variables and coordinates:
 
-    def set_ax_in_map(ax):
-        ax.axis("scaled")
-        ax.axis(extent)
-        rotate_yticklabels(ax)
-        if base is None:
-            ax.set_xticks([])
-            ax.set_yticks([])
-        else:
-            rd_ticks(ax, base=base, fmt=fmt)
-        if background:
-            add_background_map(ax, crs=crs, map_provider=background, alpha=alpha)
-
-    if nrows == 1 and ncols == 1:
-        set_ax_in_map(axes)
-    else:
-        for ax in axes.ravel():
-            set_ax_in_map(ax)
-    f.tight_layout(pad=0.0)
-    return f, axes
-
-
-def _list_contextily_providers():
-    """List contextily providers.
-
-    Taken from contextily notebooks.
-
-    Returns
-    -------
-    providers : dict
-        dictionary containing all providers. See keys for names
-        that can be passed as map_provider arguments.
+        - top : a 2D array of the top elevation of the grid cells
+        - botm : a 3D array of the bottom elevation of the grid cells
+        - x : a 1D array of the x coordinates of the grid cell centers
+        - y : a 1D array of the y coordinates of the grid cell centers
+        - layer : a 1D array of the layer indices
+        - xc : a 2D array of the x coordinates of the grid cell centers, after
+          rotation if `angrot` is not 0.0 (optional)
+        - yc : a 2D array of the y coordinates of the grid cell centers, after
+          rotation if `angrot` is not 0.0 (optional)
+
+        The dataset also includes the attributes specified in the `attrs`
+        dictionary, and a coordinate reference system specified by `crs`, if
+        provided.
     """
-    import contextily as ctx
 
-    providers = {}
-
-    def get_providers(provider):
-        if "url" in provider:
-            providers[provider["name"]] = provider
-        else:
-            for prov in provider.values():
-                get_providers(prov)
+    if attrs is None:
+        attrs = {}
+    attrs.update({"gridtype": "structured"})
+
+    # get extent from local grid edge coordinates
+    extent = [
+        np.min(xedges),
+        np.max(xedges),
+        np.min(yedges),
+        np.max(yedges),
+    ]
+
+    # calculate centers
+    xcenters = xedges[:-1] + np.diff(xedges) / 2.0
+    ycenters = yedges[:-1] + np.diff(yedges) / 2.0
+
+    resample._set_angrot_attributes(extent, xorigin, yorigin, angrot, attrs)
+
+    coords = {
+        "x": xcenters,
+        "y": ycenters,
+        "layer": range(nlay),
+    }
+    if angrot != 0.0:
+        affine = resample.get_affine_mod_to_world(attrs)
+        xc, yc = affine * np.meshgrid(xcenters, ycenters)
+        coords["xc"] = (("y", "x"), xc)
+        coords["yc"] = (("y", "x"), yc)
+
+    dims = ("layer", "y", "x")
+    ds = xr.Dataset(
+        data_vars={
+            "top": (dims[1:], top),
+            "botm": (dims, botm),
+        },
+        coords=coords,
+        attrs=attrs,
+    )
+    # set delr and delc
+    delr = np.diff(xedges)
+    if len(np.unique(delr)) == 1:
+        ds.attrs["delr"] = np.unique(delr)[0]
+    else:
+        ds["delr"] = ("x"), delr
+    delc = -np.diff(yedges)
+    if len(np.unique(delc)) == 1:
+        ds.attrs["delc"] = np.unique(delc)[0]
+    else:
+        ds["delc"] = ("y"), delc
 
-    get_providers(ctx.providers)
-    return providers
+    if crs is not None:
+        ds.rio.set_crs(crs)
+    return ds
 
 
-def add_background_map(ax, crs=28992, map_provider="nlmaps.standaard", **kwargs):
-    """Add background map to axes using contextily.
+def _get_vertex_grid_ds(
+    x,
+    y,
+    xv,
+    yv,
+    cell2d,
+    extent,
+    nlay=1,
+    top=np.nan,
+    botm=np.nan,
+    xorigin=0.0,
+    yorigin=0.0,
+    angrot=0.0,
+    attrs=None,
+    crs=None,
+):
+    """Create an xarray dataset with vertex-based grid geometry.
 
     Parameters
     ----------
-    ax: matplotlib.Axes
-        axes to add background map to
-    map_provider: str, optional
-        name of map provider, see `contextily.providers` for options.
-        Default is 'nlmaps.standaard'
-    proj: pyproj.Proj or str, optional
-        projection for background map, default is 'epsg:28992'
-        (RD Amersfoort, a projection for the Netherlands)
-    """
-    import contextily as ctx
-
-    if isinstance(crs, (str, int)):
-        import pyproj
-
-        proj = pyproj.Proj(crs)
-
-    providers = _list_contextily_providers()
-    ctx.add_basemap(ax, source=providers[map_provider], crs=proj.srs, **kwargs)
-
-
-def get_figsize(extent, figw=10.0, nrows=1, ncols=1, xh=0.2):
-    """Get a figure size in inches, calculated from a model extent."""
-    w = extent[1] - extent[0]
-    h = extent[3] - extent[2]
-    axh = (figw / ncols) * (h / w) + xh
-    figh = nrows * axh
-    figsize = (figw, figh)
-    return figsize
+    x : array_like
+        A 1D array of the x coordinates of the grid cell centers.
+    y : array_like
+        A 1D array of the y coordinates of the grid cell centers.
+    xv : array_like
+        A 1D array of the x coordinates of the grid vertices.
+    yv : array_like
+        A 1D array of the y coordinates of the grid vertices.
+    cell2d : array-like
+        array-like with vertex grid cell2d info
+    extent : list
+        A list of [xmin, xmax, ymin, ymax] defining the extent of the model grid.
+    nlay : int or sequence of ints, optional
+        The number of layers in the grid, or a sequence of layer indices.
+        Default is 1.
+    top : array_like, optional
+        A 2D array of the top elevation of the grid cells. Default is NaN.
+    botm : array_like, optional
+        A 3D array of the bottom elevation of the grid cells. Default is NaN.
+    xorigin : float, optional
+        The x-coordinate origin of the grid. Default is 0.0.
+    yorigin : float, optional
+        The y-coordinate origin of the grid. Default is 0.0.
+    angrot : float, optional
+        The counter-clockwise rotation angle of the grid, in degrees.
+        Default is 0.0.
+    attrs : dict, optional
+        A dictionary of attributes to add to the xarray dataset. Default is an
+        empty dictionary.
+    crs : dict or str, optional
+        A dictionary or string describing the coordinate reference system of
+        the grid. Default is None.
 
+    Returns
+    -------
+    ds : xarray.Dataset
+        An xarray dataset with the following data variables and coordinates:
 
-def rotate_yticklabels(ax):
-    """Rotate the labels on the y-axis 90 degrees to save space."""
-    yticklabels = ax.yaxis.get_ticklabels()
-    plt.setp(yticklabels, rotation=90, verticalalignment="center")
+        - top : a 2D array of the top elevation of the grid cells
+        - botm : a 3D array of the bottom elevation of the grid cells
+        - x : a 1D array of the x coordinates of the grid cell centers
+        - y : a 1D array of the y coordinates of the grid cell centers
+        - layer : a 1D array of the layer indices
+        - xv : a 1D array of the x coordinates of the grid vertices
+        - yv : a 1D array of the y coordinates of the grid vertices
+
+        The dataset also includes the attributes specified in the `attrs`
+        dictionary, and a coordinate reference system specified by `crs`, if
+        provided.
+    """
+    if attrs is None:
+        attrs = {}
 
+    attrs.update(
+        {
+            "extent": extent,
+            "angrot": angrot,
+            "xorigin": xorigin,
+            "yorigin": yorigin,
+            "gridtype": "vertex",
+        }
+    )
 
-def rd_ticks(ax, base=1000.0, fmt_base=1000.0, fmt="{:.0f}"):
-    """Add ticks every 1000 (base) m, and divide ticklabels by 1000
-    (fmt_base)"""
+    if isinstance(nlay, int):
+        layers = range(nlay)
+    else:
+        layers = nlay
 
-    def fmt_rd_ticks(x, _):
-        return fmt.format(x / fmt_base)
+    coords = {"x": x, "y": y, "layer": layers}
+    dims = ("layer", "icell2d")
+    ds = xr.Dataset(
+        data_vars=dict(
+            top=(dims[1:], top),
+            botm=(dims, botm),
+        ),
+        coords=coords,
+        attrs=attrs,
+    )
 
-    if base is not None:
-        ax.xaxis.set_major_locator(MultipleLocator(base))
-        ax.yaxis.set_major_locator(MultipleLocator(base))
-    ax.xaxis.set_major_formatter(FuncFormatter(fmt_rd_ticks))
-    ax.yaxis.set_major_formatter(FuncFormatter(fmt_rd_ticks))
+    # add extra modelgrid information to ds
+    ds["xv"] = ("iv", xv)
+    ds["yv"] = ("iv", yv)
+
+    # set extra grid information
+    nodata = -1
+    ncpl = len(x)
+    ncvert_max = np.max([x[3] for x in cell2d])
+    icvert = np.full((ncpl, ncvert_max), nodata)
+    for i in range(ncpl):
+        icvert[i, : cell2d[i][3]] = cell2d[i][4:]
+    ds["icvert"] = ("icell2d", "icv"), icvert
+    ds["icvert"].attrs["_FillValue"] = nodata
+
+    if crs is not None:
+        ds.rio.set_crs(crs)
+    return ds
 
 
-def colorbar_inside(
-    mappable=None, ax=None, norm=None, cmap=None, bounds=None, bbox_labels=True, **kw
-):
-    """Place a colorbar inside an axes."""
-    if ax is None:
-        ax = plt.gca()
-    if bounds is None:
-        bounds = [0.95, 0.05, 0.02, 0.9]
-    cax = ax.inset_axes(bounds, facecolor="none")
-    if mappable is None and norm is not None and cmap is not None:
-        # make an empty dataset...
-        mappable = plt.cm.ScalarMappable(norm=norm, cmap=cmap)
-        mappable._A = []
-    cb = plt.colorbar(mappable, cax=cax, ax=ax, **kw)
-    if bounds[0] > 0.5:
-        cax.yaxis.tick_left()
-        cax.yaxis.set_label_position("left")
-    if isinstance(bbox_labels, bool) and bbox_labels is True:
-        bbox_labels = dict(facecolor="w", alpha=0.5)
-    if isinstance(bbox_labels, dict):
-        for label in cb.ax.yaxis.get_ticklabels():
-            label.set_bbox(bbox_labels)
-        cb.ax.yaxis.get_label().set_bbox(bbox_labels)
-    return cb
-
-
-def title_inside(
-    title,
-    ax=None,
-    x=0.5,
-    y=0.98,
-    horizontalalignment="center",
-    verticalalignment="top",
-    bbox=True,
+def get_ds(
+    extent,
+    delr=100.0,
+    delc=None,
+    model_name=None,
+    model_ws=None,
+    layer=None,
+    top=0.0,
+    botm=None,
+    kh=10.0,
+    kv=1.0,
+    crs=28992,
+    xorigin=0.0,
+    yorigin=0.0,
+    angrot=0.0,
+    attrs=None,
+    extrapolate=True,
+    fill_nan=True,
+    transport=False,
     **kwargs,
 ):
-    """Place a title inside a matplotlib axes, at the top."""
-    if ax is None:
-        ax = plt.gca()
-    if isinstance(bbox, bool):
-        if bbox:
-            bbox = dict(facecolor="w", alpha=0.5)
-        else:
-            bbox = None
-    return ax.text(
-        x,
-        y,
-        title,
-        horizontalalignment=horizontalalignment,
-        verticalalignment=verticalalignment,
-        transform=ax.transAxes,
-        bbox=bbox,
-        **kwargs,
-    )
-
-
-def geotop_lithok_in_cross_section(
-    line, gt=None, ax=None, legend=True, legend_loc=None, lithok_props=None, **kwargs
-):
-    """
-    PLot the lithoclass-data of GeoTOP in a cross-section
+    """Create a model dataset from scratch.
 
     Parameters
     ----------
-    line : sahpely.LineString
-        The line along which the GeoTOP data is plotted
-    gt : xr.Dataset, optional
-        The voxel-dataset from GeoTOP. It is downloaded with the method
-        nlmod.read.geaotop.get_geotop_raw_within_extent if None. The default is None.
-    ax : matplotlib.Axes, optional
-        The axes in whcih the cross-section is plotted. Will default to the current axes
-        if None. The default is None.
-    legend : bool, optional
-        When True, add a legend to the plot with the lithology-classes. The default is
-        True.
-    legend_loc : None or str, optional
-        The location of the legend. See matplotlib documentation. The default is None.
-    lithok_props : pd.DataFrame, optional
-        A DataFrame containing the properties of the lithoclasses.
-        Will call nlmod.read.geotop.get_lithok_props() when None. The default is None.
+    extent : list, tuple or np.array
+        desired model extent (xmin, xmax, ymin, ymax)
+    delr : int, float, list, tuple or array, optional
+        The gridsize along columns (dx). The default is 100. meter.
+    delc : None, int, float, list, tuple or array, optional
+        The gridsize along rows (dy). Set to delr when None. If None delc=delr. The
+        default is None.
+    model_name : str, optional
+        name of the model. The default is None
+    model_ws : str, optional
+        workspace of the model. This is where modeldata is saved to. The default is
+        None.
+    layer : int, list, tuple or ndarray, optional
+        The names or index of the layers of the model. When layer is an integer it is
+        the number of layers. When layer is None, the number of layers is caluclated
+        from botm. When botm is None as well, the number of layers is set to 10. The
+        default is None.
+    top : float, list or ndarray, optional
+        The top of the model. It has to be of shape (len(y), len(x)) or it is
+        transformed into that shape if top is a float. The default is 0.0.
+    botm : list or ndarray, optional
+        The botm of the model layers. It has to be of shape
+        (len(layer), len(y), len(x)) or it is transformed to that shape if botm
+        is or a list/array of len(layer). When botm is None, a botm is
+        generated with a constant layer thickness of 10 meter. The default is
+        None.
+    kh : float, list or ndarray, optional
+        The horizontal conductivity of the model layers. It has to be of shape
+        (len(layer), len(y), len(x)) or it is transformed to that shape if kh
+        is a float or a list/array of len(layer). The default is 10.0.
+    kv : float, list or ndarray, optional
+        The vertical conductivity of the model layers. It has to be of shape
+        (len(layer), len(y), len(x)) or it is transformed to that shape if kv
+        is a float or a list/array of len(layer). The default is 1.0.
+    crs : int, optional
+        The coordinate reference system of the model. The default is 28992.
+    xorigin : float, optional
+        x-position of the lower-left corner of the model grid. Only used when angrot is
+        not 0. The defauls is 0.0.
+    yorigin : float, optional
+        y-position of the lower-left corner of the model grid. Only used when angrot is
+        not 0. The defauls is 0.0.
+    angrot : float, optional
+        counter-clockwise rotation angle (in degrees) of the lower-left corner of the
+        model grid. The default is 0.0
+    attrs : dict, optional
+        Attributes of the model dataset. The default is None.
+    extrapolate : bool, optional
+        When true, extrapolate data-variables, into the sea or other areas with
+        only nans. The default is True
+    fill_nan : bool, optional
+        if True nan values in the top, botm, kh and kv are filled using the
+        fill_nan_top_botm_kh_kv function. Layers with only nan values in the
+        botm are removed.
+    transport : bool, optional
+        flag indicating whether dataset includes data for a groundwater
+        transport model (GWT). Default is False, no transport.
+
 
     **kwargs : dict
-        kwargs are passed onto DatasetCrossSection.
+        Kwargs are passed into mbase.to_ds. These can be the model_name
+        or ds.
 
     Returns
     -------
-    cs : DatasetCrossSection
-        The instance of DatasetCrossSection that is used to plot the cross-section.
-
+    xr.Dataset
+        The model dataset.
     """
-    if ax is None:
-        ax = plt.gca()
+    if delc is None:
+        delc = delr
+
+    if isinstance(delr, (tuple, list)):
+        delr = np.asarray(delr)
 
-    if gt is None:
-        # download geotop
-        x = [coord[0] for coord in line.coords]
-        y = [coord[1] for coord in line.coords]
-        extent = [min(x), max(x), min(y), max(y)]
-        gt = geotop.get_geotop_raw_within_extent(extent)
-
-    if "top" not in gt or "botm" not in gt:
-        gt = geotop.add_top_and_botm(gt)
-
-    if lithok_props is None:
-        lithok_props = geotop.get_lithok_props()
-
-    cs = DatasetCrossSection(gt, line, layer="z", ax=ax, **kwargs)
-    lithoks = gt["lithok"].data
-    lithok_un = np.unique(lithoks[~np.isnan(lithoks)])
-    array = np.full(lithoks.shape, np.NaN)
-
-    colors = []
-    for i, lithok in enumerate(lithok_un):
-        lithok = int(lithok)
-        array[lithoks == lithok] = i
-        colors.append(lithok_props.at[lithok, "color"])
-    cmap = ListedColormap(colors)
-    norm = Normalize(-0.5, np.nanmax(array) + 0.5)
-    cs.plot_array(array, norm=norm, cmap=cmap)
-    if legend:
-        # make a legend with dummy handles
-        handles = []
-        for i, lithok in enumerate(lithok_un):
-            label = lithok_props.at[int(lithok), "name"]
-            handles.append(Patch(facecolor=colors[i], label=label))
-        ax.legend(handles=handles, loc=legend_loc)
+    if isinstance(delc, (tuple, list)):
+        delc = np.asarray(delc)
 
-    return cs
+    if attrs is None:
+        attrs = {}
+
+    if layer is None:
+        if botm is None:
+            layer = 10
+        else:
+            layer = len(botm)
+    if isinstance(layer, int):
+        layer = np.arange(0, layer)
+    if botm is None:
+        botm = top - 10 * np.arange(1.0, len(layer) + 1)
+
+    # check for nan
+    for par in [top, botm, kh, kv]:
+        if isinstance(par, numbers.Number):
+            if np.isnan(par) and (extrapolate or fill_nan):
+                raise ValueError(
+                    "'extrapolate' and 'remove_nan_layer' should be "
+                    "False when setting model parameters to NaN"
+                )
+
+    resample._set_angrot_attributes(extent, xorigin, yorigin, angrot, attrs)
+    x, y = resample.get_xy_mid_structured(attrs["extent"], delr, delc)
+    coords = dict(x=x, y=y, layer=layer)
+    if angrot != 0.0:
+        affine = resample.get_affine_mod_to_world(attrs)
+        xc, yc = affine * np.meshgrid(x, y)
+        coords["xc"] = (("y", "x"), xc)
+        coords["yc"] = (("y", "x"), yc)
+
+    def check_variable(var, shape):
+        if isinstance(var, int):
+            # the variable is a single integer
+            var = float(var)
+        if isinstance(var, float):
+            # the variable is a single float
+            var = np.full(shape, var)
+        else:
+            # assume the variable is an array of some kind
+            if not isinstance(var, np.ndarray):
+                var = np.array(var)
+            if var.dtype != float:
+                var = var.astype(float)
+            if len(var.shape) == 1 and len(shape) == 3:
+                # the variable is defined per layer
+                assert len(var) == shape[0]
+                var = var[:, np.newaxis, np.newaxis]
+                var = np.repeat(np.repeat(var, shape[1], 1), shape[2], 2)
+            else:
+                assert var.shape == shape
+        return var
+
+    shape = (len(y), len(x))
+    top = check_variable(top, shape)
+    shape = (len(layer),) + shape
+    botm = check_variable(botm, shape)
+    kh = check_variable(kh, shape)
+    kv = check_variable(kv, shape)
+
+    dims = ["layer", "y", "x"]
+    ds = xr.Dataset(
+        data_vars=dict(
+            top=(dims[1:], top),
+            botm=(dims, botm),
+            kh=(dims, kh),
+            kv=(dims, kv),
+        ),
+        coords=coords,
+        attrs=attrs,
+    )
+    ds = to_model_ds(
+        ds,
+        model_name=model_name,
+        model_ws=model_ws,
+        extent=extent,
+        delr=delr,
+        delc=delc,
+        drop_attributes=False,
+        extrapolate=extrapolate,
+        fill_nan=fill_nan,
+        transport=transport,
+        **kwargs,
+    )
+    ds.rio.set_crs(crs)
+    return ds
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nlmod-0.5.3/nlmod/read/ahn.py` & `nlmod-0.6.0/nlmod/read/ahn.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,17 +203,18 @@
     )
     return da
 
 
 def get_ahn2_tiles(extent=None):
     """Get the tiles (kaartbladen) of AHN3 as a GeoDataFrame.
 
-    The links in the tiles are cuurently incorrect. Thereore get_ahn3_tiles is used in
-    get_ahn2 and get_ahn1, as the tiles from get_ahn3_tiles also contain information
-    about the tiles of ahn1 and ahn2
+    The links in the tiles are cuurently incorrect. Thereore
+    get_ahn3_tiles is used in get_ahn2 and get_ahn1, as the tiles from
+    get_ahn3_tiles also contain information about the tiles of ahn1 and
+    ahn2
     """
     url = "https://services.arcgis.com/nSZVuSZjHpEZZbRo/arcgis/rest/services/Kaartbladen_AHN2/FeatureServer"
     layer = 0
     gdf = arcrest(url, layer, extent)
     if not gdf.empty:
         gdf = gdf.set_index("Kaartblad")
     return gdf
@@ -330,15 +331,15 @@
         DataArray (if as_data_array is True) or Rasterio MemoryFile of the AHN
     """
     tiles = get_ahn4_tiles(extent)
     return _download_and_combine_tiles(tiles, identifier, extent, as_data_array)
 
 
 def _download_and_combine_tiles(tiles, identifier, extent, as_data_array):
-    """Internal method to download and combine ahn-data"""
+    """Internal method to download and combine ahn-data."""
     if tiles.empty:
         raise (Exception(f"{identifier} has no data for requested extent"))
     datasets = []
     for name in tqdm(tiles.index, desc=f"Downloading tiles of {identifier}"):
         url = tiles.at[name, identifier]
         path = url.split("/")[-1].replace(".zip", ".TIF")
         if path.lower().endswith(".tif.tif"):
```

### Comparing `nlmod-0.5.3/nlmod/read/bgt.py` & `nlmod-0.6.0/nlmod/read/bgt.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,15 @@
     geometry=None,
     files=None,
     cut_by_extent=True,
     make_valid=False,
     extent=None,
     remove_expired=True,
 ):
-    """
-    Read data from a zipfile that was downloaded using get_bgt().
+    """Read data from a zipfile that was downloaded using get_bgt().
 
     Parameters
     ----------
     fname : string
         The filename of the zip-file containing the BGT-data.
     geometry : str, optional
         DESCRIPTION. The default is None.
@@ -155,15 +154,14 @@
         Remove expired items (that contain a value for 'eindRegistratie') when True. The
         default is True.
 
     Returns
     -------
     gdf : dict of GeoPandas GeoDataFrame
         A dict of GeoDataFrames containing all geometries and properties.
-
     """
     zf = ZipFile(fname)
     gdf = {}
     if files is None:
         files = zf.namelist()
     elif isinstance(files, str):
         files = [files]
```

### Comparing `nlmod-0.5.3/nlmod/read/brp.py` & `nlmod-0.6.0/nlmod/read/brp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/nlmod/read/geotop.py` & `nlmod-0.6.0/nlmod/read/geotop.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,17 @@
 
 
 def convert_geotop_to_ml_layers(
     geotop_ds_raw,
     strat_props=None,
     **kwargs,
 ):
-    """
-    Convert geotop voxel data to layers using the Stratography-data.
+    """Convert geotop voxel data to layers using the stratigraphy-data.
 
-    It gets the top and botm of each stratographic unit in the geotop dataset.
+    It gets the top and botm of each stratigraphic unit in the geotop dataset.
 
     Parameters
     ----------
     geotop_ds_raw: xr.Dataset
         dataset with geotop voxel data
     strat_props: pandas.DataFrame
         The properties of the stratigraphic unit. Load with get_strat_props() when None.
@@ -179,29 +178,29 @@
         geo_eenheden[(geo_eenheden == 2000.0) + (geo_eenheden == 1130.0)] = [
             2000.0,
             1130.0,
         ]
 
     strat_codes = []
     for geo_eenh in geo_eenheden:
-        if geo_eenh in strat_props.index:
-            code = strat_props.at[geo_eenh, "code"]
+        if int(geo_eenh) in strat_props.index:
+            code = strat_props.at[int(geo_eenh), "code"]
         else:
             logger.warning(f"Unknown strat-value: {geo_eenh}")
             code = str(geo_eenh)
         strat_codes.append(code)
 
     # fill top and bot
     shape = (len(strat_codes), len(geotop_ds_raw.y), len(geotop_ds_raw.x))
     top = np.full(shape, np.nan)
     bot = np.full(shape, np.nan)
     lay = 0
     logger.info("creating top and bot per geo eenheid")
     for geo_eenheid in geo_eenheden:
-        logger.debug(geo_eenheid)
+        logger.debug(int(geo_eenheid))
 
         mask = geotop_ds_raw.strat == geo_eenheid
         geo_z = xr.where(mask, geotop_ds_raw.z, np.NaN)
 
         top[lay] = geo_z.max(dim="z") + 0.25
         bot[lay] = geo_z.min(dim="z") - 0.25
 
@@ -229,30 +228,28 @@
     if "kh" in geotop_ds_raw and "kv" in geotop_ds_raw:
         aggregate_to_ds(geotop_ds_raw, geotop_ds_mod, **kwargs)
 
     return geotop_ds_mod
 
 
 def add_top_and_botm(ds):
-    """
-    Add the top and bottom of the voxels to the GeoTOP Dataset.
+    """Add the top and bottom of the voxels to the GeoTOP Dataset.
 
     This makes sure the structure of the geotop dataset is more like regis, and we can
     use the cross-section class (DatasetCrossSection from nlmod.
 
     Parameters
     ----------
     ds : xr.Dataset
         The geotop-dataset.
 
     Returns
     -------
     ds : xr.Dataset
         The geotop-dataset, with added variables "top" and "botm".
-
     """
     # make ready for DataSetCrossSection
     # ds = ds.transpose("z", "y", "x")
     # ds = ds.sortby("z", ascending=False)
 
     bottom = np.expand_dims(ds.z.data - 0.25, axis=(1, 2))
     bottom = np.repeat(np.repeat(bottom, len(ds.y), 1), len(ds.x), 2)
@@ -274,16 +271,15 @@
     kv_method="harmonic_mean",
     anisotropy=1.0,
     kh="kh",
     kv="kv",
     kh_df="kh",
     kv_df="kv",
 ):
-    """
-    Add kh and kv variables to the voxels of the GeoTOP Dataset.
+    """Add kh and kv variables to the voxels of the GeoTOP Dataset.
 
     Parameters
     ----------
     gt : xr.Dataset
         The geotop dataset, at least with variable lithok.
     df : pd.DataFrame
         A DataFrame with information about the kh and optionally kv, for different
@@ -321,15 +317,14 @@
 
         DESCRIPTION.
 
     Returns
     -------
     gt : xr.Dataset
         Datset with voxel-data, with the added variables 'kh' and 'kv'.
-
     """
     if isinstance(stochastic, bool):
         if stochastic:
             stochastic = "linear"
         else:
             stochastic = None
     if kh_method not in ["arithmetic_mean", "harmonic_mean"]:
@@ -475,17 +470,16 @@
             kv = np.inf
     return kh, kv
 
 
 def aggregate_to_ds(
     gt, ds, kh="kh", kv="kv", kd="kD", c="c", kh_gt="kh", kv_gt="kv", add_kd_and_c=False
 ):
-    """
-    Aggregate voxels from GeoTOP to layers in a model DataSet with top and botm, to
-    calculate kh and kv
+    """Aggregate voxels from GeoTOP to layers in a model DataSet with top and
+    botm, to calculate kh and kv.
 
     Parameters
     ----------
     gt : xr.Dataset
         A Dataset containing the Geotop voxel data.
     ds : xr.Dataset
         A Dataset containing the top and botm of the layers.
@@ -510,15 +504,14 @@
     add_kd_and_c : bool, optional
         Add the variables kd and c to ds. The default is False.
 
     Returns
     -------
     ds : xr.Dataset
         The Dataset ds, with added variables kh and kv (and optionally kd and c).
-
     """
     assert (ds.x == gt.x).all() and (ds.y == gt.y).all()
     msg = "Please add {} to geotop-Dataset first, using add_kh_and_kv()"
     if kh_gt not in gt:
         raise (Exception(msg.format(kh_gt)))
     if kv_gt not in gt:
         raise (Exception(msg.format(kv_gt)))
```

### Comparing `nlmod-0.5.3/nlmod/read/jarkus.py` & `nlmod-0.6.0/nlmod/read/jarkus.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,27 +163,26 @@
                     )
             tiles = tiles_left
     z_dataset = xr.combine_by_coords(tiles, combine_attrs="drop")
     return z_dataset
 
 
 def get_jarkus_tilenames(extent, kind="jarkus"):
-    """Find all Jarkus tilenames within a certain extent
+    """Find all Jarkus tilenames within a certain extent.
 
     Parameters
     ----------
     extent : list, tuple or np.array
         extent (xmin, xmax, ymin, ymax) of the desired grid. Should be RD-new
         coördinates (EPSG:28992)
 
     Returns
     -------
     netcdf_urls : list of str
         list of the urls of all netcdf files of the tiles with Jarkus data.
-
     """
     if kind == "jarkus":
         url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc"
     elif kind == "kusthoogte":
         url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/kusthoogte/catalog.nc"
     elif kind == "vaklodingen":
         url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/vaklodingen/catalog.nc"
```

### Comparing `nlmod-0.5.3/nlmod/read/knmi.py` & `nlmod-0.6.0/nlmod/read/knmi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import datetime as dt
 import logging
 
 import hydropandas as hpd
 import numpy as np
 import pandas as pd
+from hydropandas.io import knmi as hpd_knmi
 
 from .. import cache, util
 from ..dims.layers import get_first_active_layer
 from ..dims.resample import get_affine_mod_to_world
 
 logger = logging.getLogger(__name__)
 
 
 @cache.cache_netcdf
-def get_recharge(ds, method="linear"):
+def get_recharge(ds, method="linear", most_common_station=False):
     """add multiple recharge packages to the groundwater flow model with knmi
     data by following these steps:
 
        1. check for each cell (structured or vertex) which knmi measurement
           stations (prec and evap) are the closest.
        2. download precipitation and evaporation data for all knmi stations that
           were found at 1
@@ -37,25 +38,28 @@
     ----------
     ds : xr.DataSet
         dataset containing relevant model grid information
     method : bool, optional
         If 'linear', calculate recharge by subtracting evaporation from precipitation.
         If 'separate', add precipitation as 'recharge' and evaporation as 'evaporation'.
         The defaults is 'linear'.
+    most_common_station : bool, optional
+        When True, only download data from the station that is most common in the model
+        area. The default is False
 
     Returns
     -------
     ds : xr.DataSet
         dataset with spatial model data including the rch raster
     """
 
     if "time" not in ds:
         raise (
             AttributeError(
-                "'Dataset' object has no attribute 'time'. "
+                "'Dataset' object has no 'time' dimension. "
                 "Please run nlmod.time.set_ds_time()"
             )
         )
     start = pd.Timestamp(ds.time.attrs["start"])
     end = pd.Timestamp(ds.time.data[-1])
 
     ds_out = util.get_ds_empty(ds)
@@ -67,60 +71,53 @@
     elif ds.gridtype == "vertex":
         dims = ("icell2d",)
     dims = ("time",) + dims
 
     shape = [len(ds_out[dim]) for dim in dims]
 
     locations, oc_knmi_prec, oc_knmi_evap = get_knmi_at_locations(
-        ds, start=start, end=end
-    )
-
-    # add closest precipitation and evaporation measurement station to each cell
-    locations[["prec_point", "distance"]] = locations.geo.get_nearest_point(
-        oc_knmi_prec
-    )
-    locations[["evap_point", "distance"]] = locations.geo.get_nearest_point(
-        oc_knmi_evap
+        ds, start=start, end=end, most_common_station=most_common_station
     )
 
     if method in ["linear"]:
         ds_out["recharge"] = dims, np.zeros(shape)
 
         # find unique combination of precipitation and evaporation station
-        unique_combinations = locations.drop_duplicates(["prec_point", "evap_point"])[
-            ["prec_point", "evap_point"]
+        unique_combinations = locations.drop_duplicates(["stn_rd", "stn_ev24"])[
+            ["stn_rd", "stn_ev24"]
         ].values
 
-        for prec_stn, evap_stn in unique_combinations:
+        for stn_rd, stn_ev24 in unique_combinations:
             # get locations with the same prec and evap station
-            loc_sel = locations.loc[
-                (locations["prec_point"] == prec_stn)
-                & (locations["evap_point"] == evap_stn)
-            ]
+            mask = (locations["stn_rd"] == stn_rd) & (locations["stn_ev24"] == stn_ev24)
+            loc_sel = locations.loc[mask]
 
             # calculate recharge time series
-            prec = oc_knmi_prec.loc[prec_stn,
-                                    "obs"]["RD"].resample('D').nearest()
-            evap = oc_knmi_evap.loc[evap_stn,
-                                    "obs"]["EV24"].resample('D').nearest()
+            index = oc_knmi_prec.index[oc_knmi_prec.station == stn_rd][0]
+            prec = oc_knmi_prec.loc[index, "obs"]["RD"].resample("D").nearest()
+            index = oc_knmi_evap.index[oc_knmi_evap.station == stn_ev24][0]
+            evap = oc_knmi_evap.loc[index, "obs"]["EV24"].resample("D").nearest()
             ts = (prec - evap).dropna()
             ts.name = f"{prec.name}-{evap.name}"
 
             _add_ts_to_ds(ts, loc_sel, "recharge", ds_out)
 
     elif method == "separate":
         ds_out["recharge"] = dims, np.zeros(shape)
-        for stn in locations["prec_point"].unique():
-            ts = oc_knmi_prec.loc[stn, "obs"]["RD"]
-            loc_sel = locations.loc[(locations["prec_point"] == stn)]
+        for stn in locations["stn_rd"].unique():
+            index = oc_knmi_prec.index[oc_knmi_prec.station == stn][0]
+            ts = oc_knmi_prec.loc[index, "obs"]["RD"].resample("D").nearest()
+            loc_sel = locations.loc[(locations["stn_rd"] == stn)]
             _add_ts_to_ds(ts, loc_sel, "recharge", ds_out)
+
         ds_out["evaporation"] = dims, np.zeros(shape)
-        for stn in locations["evap_point"].unique():
-            ts = oc_knmi_evap.loc[stn, "obs"]["EV24"]
-            loc_sel = locations.loc[(locations["evap_point"] == stn)]
+        for stn in locations["stn_ev24"].unique():
+            index = oc_knmi_evap.index[oc_knmi_evap.station == stn][0]
+            ts = oc_knmi_evap.loc[index, "obs"]["EV24"].resample("D").nearest()
+            loc_sel = locations.loc[(locations["stn_ev24"] == stn)]
             _add_ts_to_ds(ts, loc_sel, "evaporation", ds_out)
     else:
         raise (Exception(f"Unknown method: {method}"))
     for datavar in ds_out:
         ds_out[datavar].attrs["source"] = "KNMI"
         ds_out[datavar].attrs["date"] = dt.datetime.now().strftime("%Y%m%d")
         ds_out[datavar].attrs["units"] = "m/day"
@@ -128,16 +125,15 @@
     return ds_out
 
 
 def _add_ts_to_ds(timeseries, loc_sel, variable, ds):
     """Add a timeseries to a variable at location loc_sel in model DataSet."""
     end = pd.Timestamp(ds.time.data[-1])
     if timeseries.index[-1] < end:
-        raise ValueError(
-            f"no recharge available at {timeseries.name} for date {end}")
+        raise ValueError(f"no recharge available at {timeseries.name} for date {end}")
 
     # fill recharge data array
     model_recharge = pd.Series(index=ds.time, dtype=float)
     for j, ts in enumerate(model_recharge.index):
         if j == 0:
             start = ds.time.start
         else:
@@ -148,16 +144,15 @@
         # when the model frequency is higher than the timeseries-frequency,
         # there will be NaN's, which we fill by backfill
         model_recharge = model_recharge.fillna(method="bfill")
         if model_recharge.isna().any():
             raise (Exception("There are NaN-values in {variable}"))
 
     # add data to ds
-    values = np.repeat(
-        model_recharge.values[:, np.newaxis], loc_sel.shape[0], 1)
+    values = np.repeat(model_recharge.values[:, np.newaxis], loc_sel.shape[0], 1)
     if ds.gridtype == "structured":
         ds[variable].data[:, loc_sel.row, loc_sel.col] = values
     elif ds.gridtype == "vertex":
         ds[variable].data[:, loc_sel.index] = values
 
 
 def get_locations_vertex(ds):
@@ -225,15 +220,15 @@
             data={"x": x, "y": y, "row": rows, "col": columns, "layer": layers}
         )
     )
 
     return locations
 
 
-def get_knmi_at_locations(ds, start="2010", end=None):
+def get_knmi_at_locations(ds, start="2010", end=None, most_common_station=False):
     """get knmi data at the locations of the active grid cells in ds.
 
     Parameters
     ----------
     ds : xr.DataSet
         dataset containing relevant model grid information
     start : str or datetime, optional
@@ -258,18 +253,33 @@
     # get locations
     if ds.gridtype == "structured":
         locations = get_locations_structured(ds)
     elif ds.gridtype == "vertex":
         locations = get_locations_vertex(ds)
     else:
         raise ValueError("gridtype should be structured or vertex")
+    locations["stn_rd"] = hpd_knmi.get_nearest_station_df(locations, meteo_var="RD")
+    locations["stn_ev24"] = hpd_knmi.get_nearest_station_df(locations, meteo_var="EV24")
+    if most_common_station:
+        if ds.gridtype == "structured":
+            # set the most common station to all locations
+            locations["stn_rd"] = locations["stn_rd"].value_counts().idxmax()
+            locations["stn_ev24"] = locations["stn_ev24"].value_counts().idxmax()
+        else:
+            # set the station with the largest area to all locations
+            locations["area"] = ds["area"].loc[locations.index]
+            locations["stn_rd"] = locations.groupby("stn_rd").sum()["area"].idxmax()
+            locations["stn_ev24"] = locations.groupby("stn_ev24").sum()["area"].idxmax()
+
+    stns_rd = locations["stn_rd"].unique()
+    stns_ev24 = locations["stn_ev24"].unique()
 
     # get knmi data stations closest to any grid cell
     oc_knmi_prec = hpd.ObsCollection.from_knmi(
-        locations=locations, starts=[start], ends=[end], meteo_vars=["RD"]
+        stns=stns_rd, starts=[start], ends=[end], meteo_vars=["RD"]
     )
 
     oc_knmi_evap = hpd.ObsCollection.from_knmi(
-        locations=locations, starts=[start], ends=[end], meteo_vars=["EV24"]
+        stns=stns_ev24, starts=[start], ends=[end], meteo_vars=["EV24"]
     )
 
     return locations, oc_knmi_prec, oc_knmi_evap
```

### Comparing `nlmod-0.5.3/nlmod/read/meteobase.py` & `nlmod-0.6.0/nlmod/read/meteobase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import re
-from pandas import Timestamp
 from enum import Enum
 from io import FileIO
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 from zipfile import ZipFile
 
 import numpy as np
+from pandas import Timestamp
 from xarray import DataArray
 
 
 class MeteobaseType(Enum):
-    """Enum class to couple folder names to observation type (from in LEESMIJ.txt)"""
+    """Enum class to couple folder names to observation type (from in
+    LEESMIJ.txt)"""
 
     NEERSLAG = "Neerslagradargegevens in Arc/Info-formaat."
     MAKKINK = "Verdampingsgegevens volgens Makkink."
     PENMAN = "Verdampingsgegevens volgens Penman-Monteith."
     EVAPOTRANSPIRATIE = "Actuele evapotranspiratie volgens SATDATA 3.0."
     VERDAMPINGSTEKORT = "Verdampingstekort (Epot - Eact) volgens SATDATA 3.0."
 
 
 def read_leesmij(fo: FileIO) -> Dict[str, Dict[str, str]]:
-    """Read LEESMIJ.TXT file
+    """Read LEESMIJ.TXT file.
 
     Parameters
     ----------
     fo : FileIO
         File object
 
     Returns
@@ -51,15 +52,16 @@
             meta[meta_idx] = submeta  # sla submeta op in meta
             submeta = {}
         line = str(fo.readline(), encoding="utf-8")
     return meta
 
 
 def get_timestamp_from_fname(fname: str) -> Timestamp:
-    """Get the Timestamp from a filename (with some assumptions about the formatting)"""
+    """Get the Timestamp from a filename (with some assumptions about the
+    formatting)"""
     datestr = re.search("([0-9]{8})", fname)  # assumes YYYYMMDD
     if datestr is not None:
         match = datestr.group(0)
         year = int(match[0:4])
         month = int(match[4:6])
         day = int(match[6:8])
 
@@ -71,59 +73,70 @@
         hour = int(match.replace("_", ""))
 
     dtime = Timestamp(year=year, month=month, day=day, hour=hour)
     return dtime
 
 
 def read_ascii(fo: FileIO) -> Union[np.ndarray, dict]:
-    """Read Esri ASCII raster format file
+    """Read Esri ASCII raster format file.
 
     Parameters
     ----------
     fo : FileIO
         File object
 
     Returns
     -------
     Union[np.ndarray, dict]
         Numpy array with data and header meta
-
     """
+    ascii_header_keys = [
+        "ncols",
+        "nrows",
+        "nodata_value",
+        "xllcorner",
+        "yllcorner",
+        "cellsize",
+        "xllcenter",
+        "yllcenter",
+    ]
+
     # read file
     lines = fo.readlines()
 
     # extract header
     meta = {}
-    for line in lines[0:6]:
-        l1, l2 = str(line, encoding="utf-8").split()
+    line_cnt = 0
+    for line in lines:
+        linestr = str(line, encoding="utf-8").lower()
+        if not any((x for x in ascii_header_keys if x in str(linestr))):
+            break
+        l1, l2 = linestr.split()
         if l1.lower() in ("ncols", "nrows", "nodata_value"):
-            l2 = int(l2)
+            meta[l1] = int(l2)
         elif l1.lower() in (
             "xllcorner",
             "yllcorner",
             "cellsize",
             "xllcenter",
             "yllcenter",
         ):
-            l2 = float(l2)
-        else:
-            raise ValueError(f"Found unknown key '{l1}' in ASCII header")
-
-        meta[l1.lower()] = l2
+            meta[l1] = float(l2)
+        line_cnt += 1
 
     # extract data
-    data = np.array([x.split() for x in lines[6:]], dtype=float)
+    data = np.array([x.split() for x in lines[line_cnt:]], dtype=float)
 
     return data, meta
 
 
 def get_xy_from_ascii_meta(
     meta: Dict[str, Union[int, float]]
 ) -> Tuple[np.ndarray, np.ndarray]:
-    """Get the xy coordinates Esri ASCII raster format header
+    """Get the xy coordinates Esri ASCII raster format header.
 
     Parameters
     ----------
     meta : dict
         dictonary with the following keys and value types:
         {cellsize: int,
          nrows: int,
@@ -131,17 +144,15 @@
          xllcorner/xllcenter: float,
          yllcorner/yllcenter: float}
 
     Returns
     -------
     Tuple[np.ndarray, np.ndarray]
         Tuple with the the x and y coordinates as numpy array
-
     """
-
     if "xllcorner" in meta.keys():
         xstart = meta["xllcorner"] + meta["cellsize"] / 2
     elif "xllcenter" in meta.keys():
         xstart = meta["xllcenter"]
 
     x = np.linspace(
         xstart,
@@ -151,90 +162,111 @@
     )
 
     if "yllcorner" in meta.keys():
         ystart = meta["yllcorner"] + meta["cellsize"] / 2
     elif "yllcenter" in meta.keys():
         ystart = meta["yllcenter"]
 
-    y = np.linspace(
-        ystart,
-        ystart + meta["cellsize"] * meta["nrows"],
-        meta["nrows"],
-        endpoint=False,
+    y = np.flip(
+        np.linspace(
+            ystart,
+            ystart + meta["cellsize"] * meta["nrows"],
+            meta["nrows"],
+            endpoint=True,
+        )
     )
     return x, y
 
 
 def read_meteobase_ascii(
-    zfile: ZipFile, foldername: str, meta: Dict[str, str]
+    zfile: ZipFile, foldername: str, meta: Dict[str, str], replace_na: bool = True
 ) -> DataArray:
-    """Read list of .asc files in a meteobase zipfile
+    """Read list of .asc files in a meteobase zipfile.
 
     Parameters
     ----------
     zfile : ZipFile
         meteobase zipfile
     foldername : str
         foldername where specific observation type is stored
     meta : Dict[str, str]
         relevant metadata for DataArray
+    replace_na : bool
+        replace nodata_value with numpy.nan
 
     Returns
     -------
     DataArray
     """
-    fnames = [x for x in zfile.namelist() if f"{foldername}/" in x]
+    fnames = [
+        x
+        for x in zfile.namelist()
+        if f"{foldername}/" in x and x.upper().endswith(".ASC")
+    ]
     if meta["Bestandsformaat"] == ".ASC (Arc/Info-raster)":
         times = []
+        data_array = None
         for i, fname in enumerate(fnames):
-            data_array = None
             with zfile.open(fname) as fo:
                 data, ascii_meta = read_ascii(fo)
+
                 if data_array is None:
-                    meta = meta | ascii_meta
+                    meta.update(ascii_meta)
                     data_array = np.zeros(
                         shape=(len(fnames), ascii_meta["nrows"], ascii_meta["ncols"]),
                         dtype=float,
                     )
                 data_array[i] = data
 
                 times.append(get_timestamp_from_fname(fname))
 
+        if "Eenheid gegevens" in meta.keys():
+            meta["units"] = meta["Eenheid gegevens"]
+
+        if "nodata_value" in meta.keys() and replace_na:
+            data_array[data_array == meta["nodata_value"]] = np.nan
+            meta["nodata_value"] = str(np.nan)
+
         x, y = get_xy_from_ascii_meta(ascii_meta)
 
         da = DataArray(
             data_array,
             dims=["time", "y", "x"],
             coords=dict(
                 time=times,
                 x=x,
                 y=y,
             ),
             attrs=meta,
             name=foldername,
         )
+
         return da
 
     else:
         raise ValueError(f"Can't read bestandsformaat '{meta['Bestandsformaat']}'")
 
 
 def read_meteobase(
-    path: Union[Path, str], meteobase_type: Optional[str] = None
+    path: Union[Path, str],
+    meteobase_type: Optional[str] = None,
+    replace_na: bool = True,
 ) -> List[DataArray]:
-    """Read Meteobase zipfile with ASCII data
+    """Read Meteobase zipfile with ASCII data.
 
     Parameters
     ----------
     path : Union[Path,str]
         Path to meteobase .zipfile
     meteobase_type : Optional[str], optional
         Must be one of 'NEERSLAG', 'MAKKINK', 'PENMAN', 'EVAPOTRANSPIRATIE',
         'VERDAMPINGSTEKORT', by default None which reads all data from the
         zipfile.
+    replace_na : bool
+        replace nodata_value with numpy.nan
 
     Returns
     -------
     List[DataArray]
     """
 
     with ZipFile(Path(path)) as zfile:
@@ -242,11 +274,22 @@
             meta = read_leesmij(fo)
 
         if meteobase_type is None:
             meteo_basetype = list(meta.keys())
 
         da_list = []
         for mb_type in meteo_basetype:
-            da = read_meteobase_ascii(zfile, mb_type.upper(), meta[mb_type.upper()])
+            da = read_meteobase_ascii(
+                zfile, mb_type.upper(), meta[mb_type.upper()], replace_na=replace_na
+            )
+            if "Projectie" in meta[mb_type.upper()].keys():
+                if (
+                    meta[mb_type.upper()]["Projectie"]
+                    == "RD new (Amersfoort, rijksdriehoekstelsel)"
+                ):
+                    import rioxarray  # noqa # pylint: disable=unused-import
+
+                    da.rio.write_crs("EPSG:28992", inplace=True)
+
             da_list.append(da)
 
     return da_list
```

### Comparing `nlmod-0.5.3/nlmod/read/regis.py` & `nlmod-0.6.0/nlmod/read/regis.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,16 @@
 
     return ds
 
 
 def add_geotop_to_regis_layers(
     rg, gt, layers="HLc", geotop_k=None, remove_nan_layers=True
 ):
-    """Combine geotop and regis in such a way that the one or more layers in Regis are
-    replaced by the geo_eenheden of geotop.
+    """Combine geotop and regis in such a way that the one or more layers in
+    Regis are replaced by the geo_eenheden of geotop.
 
     Parameters
     ----------
     rg : xarray.DataSet
         regis dataset
     gt : xarray.DataSet
         geotop dataset
@@ -263,16 +263,18 @@
 
     layer_names = xr.open_dataset(REGIS_URL).layer.astype(str).values
 
     return layer_names
 
 
 def get_legend():
-    """Get a legend (DataFrame) with the colors of REGIS-layers. These colors can
-    mainly be used in cross-sections."""
+    """Get a legend (DataFrame) with the colors of REGIS-layers.
+
+    These colors can be used when plotting cross-sections.
+    """
     dir_path = os.path.dirname(os.path.realpath(__file__))
     fname = os.path.join(dir_path, "..", "data", "regis_2_2.gleg")
     leg = pd.read_csv(
         fname,
         sep="\t",
         header=None,
         names=["naam", "beschrijving", "r", "g", "b", "a", "x"],
```

### Comparing `nlmod-0.5.3/nlmod/read/rws.py` & `nlmod-0.6.0/nlmod/read/rws.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,37 +27,37 @@
 
     Returns
     -------
     gdf_opp_water : GeoDataframe
         surface water geodataframe.
     """
     # laad bestanden in
-    fname = os.path.join(nlmod.NLMOD_DATADIR, "opp_water.shp")
+    fname = os.path.join(nlmod.NLMOD_DATADIR, "shapes", "opp_water.shp")
     gdf_swater = gpd.read_file(fname)
     extent = dims.get_extent(ds)
     gdf_swater = util.gdf_within_extent(gdf_swater, extent)
 
     return gdf_swater
 
 
 @cache.cache_netcdf
-def get_surface_water(ds, da_name):
+def get_surface_water(ds, da_basename):
     """create 3 data-arrays from the shapefile with surface water:
 
-    - area: with the area of the shape in the cell
-    - cond: with the conductance based on the area and bweerstand column in shapefile
-    - peil: with the surface water lvl based on the peil column in the shapefile
+    - area: area of the shape in the cell
+    - cond: conductance based on the area and "bweerstand" column in shapefile
+    - stage: surface water level based on the "peil" column in the shapefile
 
     Parameters
     ----------
     ds : xr.DataSet
         xarray with model data
-    da_name : str
-        name of the polygon shapes, name is used to store data arrays in
-        ds
+    da_basename : str
+        name of the polygon shapes, name is used as a prefix
+        to store data arrays in ds
 
     Returns
     -------
     ds : xarray.Dataset
         dataset with modelgrid data.
     """
 
@@ -75,20 +75,20 @@
             ds.gridtype,
         )
         cond = xr.where(area_pol > area, area_pol / row["bweerstand"], cond)
         peil = xr.where(area_pol > area, row["peil"], peil)
         area = xr.where(area_pol > area, area_pol, area)
 
     ds_out = util.get_ds_empty(ds)
-    ds_out[f"{da_name}_area"] = area
-    ds_out[f"{da_name}_area"].attrs["units"] = "m2"
-    ds_out[f"{da_name}_cond"] = cond
-    ds_out[f"{da_name}_cond"].attrs["units"] = "m2/day"
-    ds_out[f"{da_name}_peil"] = peil
-    ds_out[f"{da_name}_peil"].attrs["units"] = "mNAP"
+    ds_out[f"{da_basename}_area"] = area
+    ds_out[f"{da_basename}_area"].attrs["units"] = "m2"
+    ds_out[f"{da_basename}_cond"] = cond
+    ds_out[f"{da_basename}_cond"].attrs["units"] = "m2/day"
+    ds_out[f"{da_basename}_stage"] = peil
+    ds_out[f"{da_basename}_stage"].attrs["units"] = "mNAP"
 
     for datavar in ds_out:
         ds_out[datavar].attrs["source"] = "RWS"
         ds_out[datavar].attrs["date"] = dt.datetime.now().strftime("%Y%m%d")
 
     return ds_out
 
@@ -129,23 +129,27 @@
 
     ds_out = dims.gdf_to_bool_ds(swater_zee, ds, da_name)
 
     return ds_out
 
 
 def add_northsea(ds, cachedir=None):
-    """a) get cells from modelgrid that are within the northsea, add data
-    variable 'northsea' to ds b) fill top, bot, kh and kv add northsea cell by
-    extrapolation c) get bathymetry (northsea depth) from jarkus.
+    """Add datavariable bathymetry to model dataset.
 
-    Add datavariable bathymetry to model dataset
+    Performs the following steps:
+
+    a) get cells from modelgrid that are within the northsea, add data
+       variable 'northsea' to ds
+    b) fill top, bot, kh and kv add northsea cell by extrapolation
+    c) get bathymetry (northsea depth) from jarkus.
     """
 
     logger.info(
-        "nan values at the northsea are filled using the bathymetry from jarkus"
+        "Filling NaN values in top/botm and kh/kv in "
+        "North Sea using bathymetry data from jarkus"
     )
 
     # find grid cells with northsea
     ds.update(get_northsea(ds, cachedir=cachedir, cachename="sea_ds.nc"))
 
     # fill top, bot, kh, kv at sea cells
     fal = dims.get_first_active_layer(ds)
```

### Comparing `nlmod-0.5.3/nlmod/read/waterboard.py` & `nlmod-0.6.0/nlmod/read/waterboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,15 +221,21 @@
             "url": "https://kaarten.hhnk.nl/arcgis/rest/services/NHFLO/Peilafwijking_gebied/MapServer"
         },
     }
 
     config["Hollandse Delta"] = {
         "bgt_code": "W0655",
         "watercourses": {
-            "url": "https://geoportaal.wshd.nl/arcgis/rest/services/Geoportaal/Legger2014waterbeheersing_F_transparant/FeatureServer",
+            # "url": "https://geoportaal.wshd.nl/arcgis/rest/services/Geoportaal/Legger2014waterbeheersing_F_transparant/FeatureServer",
+            "url": "https://geoportaal.wshd.nl/arcgis/rest/services/Watersysteem/Watersysteem/MapServer",
+            "layer": 15,  # Waterlopen
+            "bottom_height": [
+                ["BODEMHOOGTE_BOVENSTROOMS", "BODEMHOOGTE_BENEDENSTROOMS"]
+            ],
+            "bottom_width": "BODEMBREEDTE",
         },
         "level_areas": {
             "url": "https://geoportaal.wshd.nl/arcgis/rest/services/Watersysteem/Peilgebieden/MapServer",
             "layer": 31,
             "f": "json",
             "summer_stage": [
                 "REKENPEIL_ZOMER",
@@ -283,17 +289,31 @@
             # "layer": 12,
             # "index": "OWAIDENT",
             # "layer": 11,
             # "index": "OBJECTID",
             "layer": 10,
             "index": "OVKIDENT",
             # "f": "json",
-            "bottom_height": ["IWS_AVVHOBOS_L", "IWS_AVVHOBES_L"],
+            "bottom_height": [["IWS_AVVHOBOS_L", "IWS_AVVHOBES_L"]],
             "bottom_width": "AVVBODDR",
         },
+        "culverts": {
+            "url": "https://opengeo.wrij.nl/arcgis/rest/services/VigerendeLegger/MapServer",
+            "layer": 7,
+            "index": "KDUIDENT",
+            "bottom_height": [["KDUBOKBO_L", "KDUBOKBE_L"]],
+            "bottom_width": "KDUBREED_L",
+        },
+        "weirs": {
+            "url": "https://opengeo.wrij.nl/arcgis/rest/services/VigerendeLegger/MapServer",
+            "layer": 5,
+            "index": "KSTIDENT",
+            "summer_stage": "IWS_KSTZMRPL",
+            "winter_stage": "IWS_KSTWTPL",
+        },
     }
 
     config["Rijnland"] = {
         "bgt_code": "W0616",
         "watercourses": {
             "url": "https://rijnland.enl-mcs.nl/arcgis/rest/services/Leggers/Legger_Oppervlaktewater_Vigerend/MapServer",
             "layer": 1,
@@ -342,21 +362,22 @@
             ],
         },
     }
 
     config["Scheldestromen"] = {
         "bgt_code": "W0661",
         "watercourses": {
-            "url": "https://geo.scheldestromen.nl/arcgis/rest/services/Extern/EXT_WB_Legger_Oppervlaktewaterlichamen_Vastgesteld/MapServer",
+            "url": "http://geo.scheldestromen.nl/arcgis/rest/services/Extern/EXT_WB_Legger_Oppervlaktewaterlichamen_Vastgesteld/MapServer",
             "layer": 6,
             "index": "OAFIDENT",
             "bottom_height": "OAFBODHG",
+            "bottom_width": "OAFBODBR",
         },
         "level_areas": {
-            "url": "https://geo.scheldestromen.nl/arcgis/rest/services/Extern/EXT_WB_Waterbeheer/FeatureServer",
+            "url": "http://geo.scheldestromen.nl/arcgis/rest/services/Extern/EXT_WB_Waterbeheer/FeatureServer",
             "layer": 14,  # Peilgebieden (praktijk)
             "index": "GPGIDENT",
             # "layer": 15,  # Peilgebieden (juridisch)
             # "index": "GJPIDENT",
             "f": "json",  # geojson does not return GPGZP and GPGWP
             "summer_stage": "GPGZP",
             "winter_stage": "GPGWP",
@@ -402,26 +423,42 @@
     }
 
     config["Vechtstromen"] = {
         "bgt_code": "W0663",
         "watercourses": {
             "url": "https://services1.arcgis.com/3RkP6F5u2r7jKHC9/arcgis/rest/services/Legger_publiek_Vastgesteld_Openbaar/FeatureServer",
             "layer": 11,
-            "index": "GLOBALID",
+            "index": "OVKIDENT",
+            "bottom_height": [["IWS_AVVHOBES_L", "IWS_AVVHOBOS_L"]],
+            "bottom_width": "AVVBODDR",
         },
         "level_areas": {
             "url": "https://services1.arcgis.com/3RkP6F5u2r7jKHC9/arcgis/rest/services/WBP_Peilen/FeatureServer",
             "layer": 0,  # Peilgebieden voormalig Velt en Vecht
             "index": "GPG_ID",
             "summer_stage": "GPGZMRPL",
             "winter_stage": "GPGWNTPL",
             "nan_values": 0,
             # "layer": 1,  # Peilregister voormalig Regge en Dinkel
             # "index": None,
         },
+        "weirs": {
+            "url": "https://services1.arcgis.com/3RkP6F5u2r7jKHC9/arcgis/rest/services/Legger_publiek_Vastgesteld_Openbaar/FeatureServer",
+            "layer": 5,
+            "index": "KSTIDENT",
+            "summer_stage": "IWS_KSTZMRPL",
+            "winter_stage": "IWS_KSTWTPL",
+        },
+        "culverts": {
+            "url": "https://services1.arcgis.com/3RkP6F5u2r7jKHC9/arcgis/rest/services/Legger_publiek_Vastgesteld_Openbaar/FeatureServer",
+            "layer": 8,
+            "index": "KDUIDENT",
+            "bottom_height": [["KDUBHBO", "KDUBHBE"]],
+            "bottom_width": "KDUBREED_L",
+        },
     }
 
     config["Zuiderzeeland"] = {
         "bgt_code": "W0650",
         "watercourses": {
             # "url": "https://services.arcgis.com/84oM5NriBghHdQ3Z/ArcGIS/rest/services/leggerkavelsloten/FeatureServer",
             "url": "https://services.arcgis.com/84oM5NriBghHdQ3Z/arcgis/rest/services/legger_concept/FeatureServer",
@@ -511,37 +548,40 @@
         )
     elif server_kind == "wfs":
         gdf = webservices.wfs(
             url, layer, extent, max_record_count=max_record_count, **kwargs
         )
     else:
         raise (Exception("Unknown server-kind: {server_kind}"))
+    if len(gdf) == 0:
+        return gdf
+
+    # set index
     if index is not None:
         if index not in gdf:
             logger.warning(f"Cannot find {index} in {data_kind} of {wb}")
         else:
             gdf = gdf.set_index(index)
-    if data_kind == "level_areas":
-        summer_stage = []
-        if "summer_stage" in conf:
-            summer_stage = conf["summer_stage"]
-        gdf = _set_column_from_columns(gdf, "summer_stage", summer_stage)
-        winter_stage = []
-        if "winter_stage" in conf:
-            winter_stage = conf["winter_stage"]
-        gdf = _set_column_from_columns(gdf, "winter_stage", winter_stage)
-    elif data_kind == "watercourses":
-        bottom_height = []
-        if "bottom_height" in conf:
-            bottom_height = conf["bottom_height"]
-        gdf = _set_column_from_columns(gdf, "bottom_height", bottom_height)
-        water_depth = []
-        if "water_depth" in conf:
-            water_depth = conf["water_depth"]
-        gdf = _set_column_from_columns(gdf, "water_depth", water_depth)
+
+    # set a value for summer_stage and winter_stage or bottom_height and water_depth
+    if data_kind in ["level_areas", "weirs"]:
+        set_columns = ["summer_stage", "winter_stage"]
+    elif data_kind in ["watercourses", "culverts"]:
+        set_columns = ["bottom_height", "water_depth"]
+    else:
+        set_columns = []
+    nan_values = None
+    if "nan_values" in conf:
+        nan_values = conf["nan_values"]
+
+    for set_column in set_columns:
+        from_columns = conf[set_column] if set_column in conf else []
+        gdf = _set_column_from_columns(
+            gdf, set_column, from_columns, nan_values=nan_values
+        )
     return gdf
 
 
 def _set_column_from_columns(gdf, set_column, from_columns, nan_values=None):
     """Retrieve values from one or more Geo)DataFrame-columns and set these
     values as another column."""
     if set_column in gdf.columns:
```

### Comparing `nlmod-0.5.3/nlmod/sim/sim.py` & `nlmod-0.6.0/nlmod/sim/sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     # Create the Flopy temporal discretization object
     tdis = flopy.mf6.modflow.mftdis.ModflowTdis(
         sim,
         pname=pname,
         time_units=ds.time.time_units,
         nper=len(ds.time),
-        # start_date_time=ds.time.start, # disable until fix in modpath
+        start_date_time=pd.Timestamp(ds.time.start).isoformat(),
         perioddata=tdis_perioddata,
     )
 
     return tdis
 
 
 def ims(sim, complexity="MODERATE", pname="ims", **kwargs):
```

### Comparing `nlmod-0.5.3/nlmod/util.py` & `nlmod-0.6.0/nlmod/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 import sys
 import warnings
 from typing import Dict, Optional
 
 import flopy
 import geopandas as gpd
-import numpy as np
 import requests
 import xarray as xr
 from colorama import Back, Fore, Style
 from shapely.geometry import box
 
 logger = logging.getLogger(__name__)
 
@@ -383,103 +382,14 @@
         if os.path.isdir(destination):
             filename = get_google_drive_filename(fid)
             destination = os.path.join(destination, filename)
 
     save_response_content(response, destination)
 
 
-def get_heads_dataarray(ds, fill_nans=False, fname_hds=None):
-    """reads the heads from a modflow .hds file and returns an xarray
-    DataArray.
-
-    Parameters
-    ----------
-    ds : TYPE
-        DESCRIPTION.
-    fill_nans : bool, optional
-        if True the nan values are filled with the heads in the cells below
-    fname_hds : TYPE, optional
-        DESCRIPTION. The default is None.
-
-    Returns
-    -------
-    head_ar : TYPE
-        DESCRIPTION.
-    """
-    logger.warning(
-        "nlmod.util.get_heads_dataarray is deprecated. "
-        "Please use nlmod.gwf.get_heads_da instead"
-    )
-
-    if fname_hds is None:
-        fname_hds = os.path.join(ds.model_ws, ds.model_name + ".hds")
-
-    head = get_heads_array(fname_hds, fill_nans=fill_nans)
-
-    if ds.gridtype == "vertex":
-        head_ar = xr.DataArray(
-            data=head[:, :, 0],
-            dims=("time", "layer", "icell2d"),
-            coords={
-                "icell2d": ds.icell2d,
-                "layer": ds.layer,
-                "time": ds.time,
-            },
-        )
-    elif ds.gridtype == "structured":
-        head_ar = xr.DataArray(
-            data=head,
-            dims=("time", "layer", "y", "x"),
-            coords={
-                "x": ds.x,
-                "y": ds.y,
-                "layer": ds.layer,
-                "time": ds.time,
-            },
-        )
-
-    return head_ar
-
-
-def get_heads_array(fname_hds, fill_nans=False):
-    """reads the heads from a modflow .hds file and returns a numpy array.
-
-    assumes the dimensions of the heads file are:
-        structured: time, layer, icell2d
-        vertex: time, layer, nrow, ncol
-
-
-    Parameters
-    ----------
-    fname_hds : TYPE, optional
-        DESCRIPTION. The default is None.
-    fill_nans : bool, optional
-        if True the nan values are filled with the heads in the cells below
-
-    Returns
-    -------
-    head_ar : np.ndarray
-        heads array.
-    """
-    logger.warning(
-        "nlmod.util.get_heads_array is deprecated. "
-        "Please use nlmod.gwf.get_heads_da instead"
-    )
-    hdobj = flopy.utils.HeadFile(fname_hds)
-    head = hdobj.get_alldata()
-    head[head == 1e30] = np.nan
-
-    if fill_nans:
-        for lay in range(head.shape[1] - 2, -1, -1):
-            head[:, lay] = np.where(
-                np.isnan(head[:, lay]), head[:, lay + 1], head[:, lay]
-            )
-    return head
-
-
 def download_mfbinaries(bindir=None):
     """Download and unpack platform-specific modflow binaries.
 
     Source: USGS
 
     Parameters
     ----------
@@ -491,14 +401,30 @@
     """
 
     if bindir is None:
         bindir = os.path.join(os.path.dirname(__file__), "bin")
     if not os.path.isdir(bindir):
         os.makedirs(bindir)
     flopy.utils.get_modflow(bindir)
+    if sys.platform.startswith("win"):
+        # download the provisional version of modpath from Github
+        download_modpath_provisional_exe(bindir)
+
+
+def download_modpath_provisional_exe(bindir=None, timeout=120):
+    """Downlaod the provisional version of modpath to the folder with binaries"""
+    if bindir is None:
+        bindir = os.path.join(os.path.dirname(__file__), "bin")
+    if not os.path.isdir(bindir):
+        os.makedirs(bindir)
+    url = "https://github.com/MODFLOW-USGS/modpath-v7/raw/develop/msvs/bin_PROVISIONAL/mpath7_PROVISIONAL_2022-08-23_9ac760f.exe"
+    r = requests.get(url, allow_redirects=True, timeout=timeout)
+    fname = os.path.join(bindir, "mp7_2_002_provisional.exe")
+    with open(fname, "wb") as file:
+        file.write(r.content)
 
 
 def check_presence_mfbinaries(exe_name="mf6", binpath=None):
     """Check if exe_name is present in the binpath folder.
 
     Parameters
     ----------
@@ -561,7 +487,114 @@
     logger = logging.getLogger()
     logger.handlers[:] = []
     logger.addHandler(handler)
     logger.setLevel(getattr(logging, level))
 
     logging.captureWarnings(True)
     return logger
+
+
+def _get_value_from_ds_attr(ds, varname, attr=None, value=None, warn=True):
+    """Internal function to get value from dataset attributes.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        dataset containing model data
+    varname : str
+        name of the variable in flopy package
+    attr : str, optional
+        name of the attribute in dataset (is sometimes different to varname)
+    value : Any, optional
+        variable value, by default None
+    warn : bool, optional
+        log warning if value not found
+
+    Returns
+    -------
+    value : Any
+        returns variable value, if value was None, attempts to obtain
+        variable from dataset attributes.
+    """
+    if attr is None:
+        attr = varname
+
+    if value is not None and (attr in ds.attrs):
+        logger.info(
+            f"Using user-provided '{varname}' and not stored attribute 'ds.{attr}'"
+        )
+    elif value is None and (attr in ds.attrs):
+        logger.debug(f"Using stored data attribute '{attr}' for '{varname}'")
+        value = ds.attrs[attr]
+    elif value is None:
+        if warn:
+            msg = (
+                f"No value found for '{varname}', returning None. "
+                f"To fix this error pass '{varname}' to function or set 'ds.{attr}'."
+            )
+            logger.warning(msg)
+        # raise ValueError(msg)
+    return value
+
+
+def _get_value_from_ds_datavar(ds, varname, datavar=None, warn=True):
+    """Internal function to get value from dataset data variables.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        dataset containing model data
+    varname : str
+        name of the variable in flopy package
+    datavar : Any, optional
+        if str, treated as the name of the data variable (which can be
+        different to varname) in dataset, if not provided is assumed to be
+        the same as varname. If not passed as string, it is treated as data
+    warn : bool, optional
+        log warning if value not found
+
+    Returns
+    -------
+    value : Any
+        returns variable value, if value is None or str, attempts to obtain
+        variable from dataset data variables.
+
+    Note
+    ----
+    For optional data, use warn=False, e.g.::
+
+        _get_value_from_ds_datavar(ds, "ss", datavar=None, warn=False)
+    """
+    # parsing datavar to check things:
+    # - varname is the name of the variable in the original function/flopy package
+    # - datavar is converted to str or None, used to check for presence in dataset
+    # - value is used to store value
+    if isinstance(datavar, xr.DataArray):
+        value = datavar
+        datavar = datavar.name
+    elif isinstance(datavar, str):
+        value = datavar
+    else:
+        value = datavar
+        datavar = None
+
+    # inform user that user-provided variable is used over stored copy
+    if (value is not None and not isinstance(value, str)) and (datavar in ds):
+        logger.info(
+            f"Using user-provided '{varname}' and not"
+            f" stored data variable 'ds.{datavar}'"
+        )
+    # get datavar from dataset if value is None or value is string
+    elif ((value is None) or isinstance(value, str)) and (datavar in ds):
+        logger.debug(f"Using stored data variable '{datavar}' for '{varname}'")
+        value = ds[datavar]
+    # warn if value is None
+    elif isinstance(value, str):
+        value = None
+        if warn:
+            msg = (
+                f"No value found for '{varname}', returning None. "
+                f"To silence this warning pass '{varname}' data directly "
+                f"to function or check whether 'ds.{datavar}' was set correctly."
+            )
+            logger.warning(msg)
+    return value
```

### Comparing `nlmod-0.5.3/nlmod/version.py` & `nlmod-0.6.0/nlmod/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib import metadata
 from platform import python_version
 
-__version__ = "0.5.3"
+__version__ = "0.6.0"
 
 
 def show_versions() -> None:
     """Method to print the version of dependencies."""
 
     msg = (
         f"Python version: {python_version()}\n"
```

### Comparing `nlmod-0.5.3/nlmod.egg-info/SOURCES.txt` & `nlmod-0.6.0/nlmod.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
+docs/conf.py
+docs/examples/cache_example.py
+docs/examples/generate_logo.py
+docs/examples/run_all_notebooks.py
 nlmod/__init__.py
 nlmod/cache.py
-nlmod/dcs.py
 nlmod/gis.py
-nlmod/plot.py
+nlmod/mfoutput.py
 nlmod/util.py
 nlmod/version.py
 nlmod.egg-info/PKG-INFO
 nlmod.egg-info/SOURCES.txt
 nlmod.egg-info/dependency_links.txt
 nlmod.egg-info/requires.txt
 nlmod.egg-info/top_level.txt
-nlmod/data/opp_water.cpg
-nlmod/data/opp_water.dbf
-nlmod/data/opp_water.prj
-nlmod/data/opp_water.qpj
-nlmod/data/opp_water.shp
-nlmod/data/opp_water.shx
+nlmod/bin/mp7_2_002_provisional
 nlmod/data/regis_2_2.gleg
 nlmod/data/geotop/geo_eenheden.csv
 nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
 nlmod/data/geotop/litho_eenheden.csv
+nlmod/data/shapes/opp_water.cpg
+nlmod/data/shapes/opp_water.dbf
+nlmod/data/shapes/opp_water.prj
+nlmod/data/shapes/opp_water.qpj
+nlmod/data/shapes/opp_water.shp
+nlmod/data/shapes/opp_water.shx
 nlmod/dims/__init__.py
 nlmod/dims/base.py
 nlmod/dims/grid.py
 nlmod/dims/layers.py
 nlmod/dims/rdp.py
 nlmod/dims/resample.py
 nlmod/dims/time.py
@@ -40,21 +44,27 @@
 nlmod/gwf/wells.py
 nlmod/gwt/__init__.py
 nlmod/gwt/gwt.py
 nlmod/gwt/output.py
 nlmod/gwt/prepare.py
 nlmod/modpath/__init__.py
 nlmod/modpath/modpath.py
+nlmod/plot/__init__.py
+nlmod/plot/dcs.py
+nlmod/plot/flopy.py
+nlmod/plot/plot.py
+nlmod/plot/plotutil.py
 nlmod/read/__init__.py
 nlmod/read/ahn.py
 nlmod/read/bgt.py
 nlmod/read/brp.py
 nlmod/read/geotop.py
 nlmod/read/jarkus.py
 nlmod/read/knmi.py
+nlmod/read/knmi_data_platform.py
 nlmod/read/meteobase.py
 nlmod/read/regis.py
 nlmod/read/rws.py
 nlmod/read/waterboard.py
 nlmod/read/webservices.py
 nlmod/sim/__init__.py
 nlmod/sim/sim.py
@@ -70,8 +80,10 @@
 tests/test_010_wells.py
 tests/test_011_dcs.py
 tests/test_012_plot.py
 tests/test_013_surface_water.py
 tests/test_014_gis.py
 tests/test_015_gwf_output.py
 tests/test_016_time.py
-tests/test_017_metbase.py
+tests/test_017_metbase.py
+tests/test_018_knmi_data_platform.py
+tests/util.py
```

### Comparing `nlmod-0.5.3/tests/test_001_model.py` & `nlmod-0.6.0/tests/test_001_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import tempfile
 
-import nlmod
 import pytest
 import xarray as xr
 
+import nlmod
+
 tmpdir = tempfile.gettempdir()
 tst_model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data")
 
 
 def test_model_directories(tmpdir):
     model_ws = os.path.join(tmpdir, "test_model")
     figdir, cachedir = nlmod.util.get_model_dirs(model_ws)
@@ -174,23 +175,23 @@
 
     # Create the output control package
     _ = nlmod.gwf.oc(ds, gwf)
 
     # voeg grote oppervlaktewaterlichamen toe
     da_name = "surface_water"
     ds.update(nlmod.read.rws.get_surface_water(ds, da_name))
-    _ = nlmod.gwf.ghb(ds, gwf, da_name)
+    _ = nlmod.gwf.ghb(ds, gwf, bhead=f"{da_name}_stage", cond=f"{da_name}_cond")
 
     # surface level drain
     ds.update(nlmod.read.ahn.get_ahn(ds))
     _ = nlmod.gwf.surface_drain_from_ds(ds, gwf, 0.1)
 
     # add constant head cells at model boundaries
     ds.update(nlmod.grid.mask_model_edge(ds, ds["idomain"]))
-    _ = nlmod.gwf.chd(ds, gwf, chd="edge_mask", head="starting_head")
+    _ = nlmod.gwf.chd(ds, gwf, mask="edge_mask", head="starting_head")
 
     # add knmi recharge to the model datasets
     ds.update(nlmod.read.knmi.get_recharge(ds))
     # create recharge package
     _ = nlmod.gwf.rch(ds, gwf)
 
     _ = nlmod.sim.write_and_run(sim, ds)
@@ -245,23 +246,23 @@
 
     # Create the output control package
     nlmod.gwf.oc(ds, gwf)
 
     # voeg grote oppervlaktewaterlichamen toe
     da_name = "surface_water"
     ds.update(nlmod.read.rws.get_surface_water(ds, da_name))
-    nlmod.gwf.ghb(ds, gwf, da_name)
+    nlmod.gwf.ghb(ds, gwf, bhead=f"{da_name}_stage", cond=f"{da_name}_cond")
 
     # surface level drain
     ds.update(nlmod.read.ahn.get_ahn(ds))
     nlmod.gwf.surface_drain_from_ds(ds, gwf, 1.0)
 
     # add constant head cells at model boundaries
     ds.update(nlmod.grid.mask_model_edge(ds, ds["idomain"]))
-    nlmod.gwf.chd(ds, gwf, chd="edge_mask", head="starting_head")
+    nlmod.gwf.chd(ds, gwf, mask="edge_mask", head="starting_head")
 
     # add knmi recharge to the model datasets
     ds.update(nlmod.read.knmi.get_recharge(ds))
     # create recharge package
     nlmod.gwf.rch(ds, gwf)
 
     nlmod.sim.write_and_run(sim, ds)
@@ -316,23 +317,23 @@
 
     # Create the output control package
     nlmod.gwf.oc(ds, gwf)
 
     # voeg grote oppervlaktewaterlichamen toe
     da_name = "surface_water"
     ds.update(nlmod.read.rws.get_surface_water(ds, da_name))
-    nlmod.gwf.ghb(ds, gwf, da_name)
+    nlmod.gwf.ghb(ds, gwf, bhead=f"{da_name}_stage", cond=f"{da_name}_cond")
 
     # surface level drain
     ds.update(nlmod.read.ahn.get_ahn(ds))
     nlmod.gwf.surface_drain_from_ds(ds, gwf, 1.0)
 
     # add constant head cells at model boundaries
     ds.update(nlmod.grid.mask_model_edge(ds, ds["idomain"]))
-    nlmod.gwf.chd(ds, gwf, chd="edge_mask", head="starting_head")
+    nlmod.gwf.chd(ds, gwf, mask="edge_mask", head="starting_head")
 
     # add knmi recharge to the model datasets
     ds.update(nlmod.read.knmi.get_recharge(ds))
     # create recharge package
     nlmod.gwf.rch(ds, gwf)
 
     nlmod.sim.write_and_run(sim, ds)
```

### Comparing `nlmod-0.5.3/tests/test_002_regis_geotop.py` & `nlmod-0.6.0/tests/test_002_regis_geotop.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.3/tests/test_004_northsea.py` & `nlmod-0.6.0/tests/test_004_northsea.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-import nlmod
-
 import test_001_model
 
+import nlmod
+
 
 def test_get_gdf_opp_water():
     ds = test_001_model.get_ds_from_cache()
     nlmod.read.rws.get_gdf_surface_water(ds)
 
 
 def test_surface_water_to_dataset():
```

### Comparing `nlmod-0.5.3/tests/test_005_external_data.py` & `nlmod-0.6.0/tests/test_005_external_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-import nlmod
-
 import test_001_model
 
+import nlmod
+
 
 def test_get_recharge():
     # model with sea
     ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # add knmi recharge to the model dataset
     ds.update(nlmod.read.knmi.get_recharge(ds))
 
 
+def test_get_reacharge_most_common():
+    # model with sea
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
+
+    # add knmi recharge to the model dataset
+    ds.update(nlmod.read.knmi.get_recharge(ds, most_common_station=True))
+
+
 def test_get_recharge_steady_state():
     # model with sea
     ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # modify mtime
     ds = ds.drop_dims("time")
     ds = nlmod.time.set_ds_time(ds, start_time="2000-1-1", perlen=3650)
```

### Comparing `nlmod-0.5.3/tests/test_006_caching.py` & `nlmod-0.6.0/tests/test_006_caching.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 """Created on Mon Jan 11 12:26:16 2021.
 
 @author: oebbe
 """
 
 import tempfile
 
-import nlmod
 import pytest
-
 import test_001_model
 
+import nlmod
+
 tmpdir = tempfile.gettempdir()
 
 
 def test_ds_check_true():
     # two models with the same grid and time dicretisation
     ds = test_001_model.get_ds_from_cache("small_model")
     ds2 = ds.copy()
```

### Comparing `nlmod-0.5.3/tests/test_007_run_notebooks.py` & `nlmod-0.6.0/tests/test_007_run_notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,16 @@
 
 @pytest.mark.notebooks
 def test_run_notebook_05_caching():
     _run_notebook(nbdir, "05_caching.ipynb")
 
 
 @pytest.mark.notebooks
-def test_run_notebook_06_compare_layermodels():
-    _run_notebook(nbdir, "06_compare_layermodels.ipynb")
-
-
-@pytest.mark.notebooks
-def test_run_notebook_07_gridding_vector_data():
-    _run_notebook(nbdir, "07_gridding_vector_data.ipynb")
+def test_run_notebook_06_gridding_vector_data():
+    _run_notebook(nbdir, "06_gridding_vector_data.ipynb")
 
 
 @pytest.mark.notebooks
 def test_run_notebook_07_resampling():
     _run_notebook(nbdir, "07_resampling.ipynb")
```

### Comparing `nlmod-0.5.3/tests/test_008_waterschappen.py` & `nlmod-0.6.0/tests/test_008_waterschappen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 """Created on Tue Aug 16 10:29:13 2022.
 
 @author: Ruben
 """
 
-import nlmod
 import pytest
 
+import nlmod
+
 
 def test_download_polygons():
     nlmod.read.waterboard.get_polygons()
 
 
 def test_get_config():
     nlmod.read.waterboard.get_configuration()
```

### Comparing `nlmod-0.5.3/tests/test_009_layers.py` & `nlmod-0.6.0/tests/test_009_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
+
 import matplotlib.pyplot as plt
-import nlmod
-from nlmod.dcs import DatasetCrossSection
 from shapely.geometry import LineString
 
+import nlmod
+from nlmod.plot import DatasetCrossSection
+
 
 def get_regis_horstermeer():
     extent = [131000, 136800, 471500, 475700]
     cachedir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data")
     if not os.path.isdir(cachedir):
         os.makedirs(cachedir)
     regis = nlmod.read.get_regis(
```

### Comparing `nlmod-0.5.3/tests/test_010_wells.py` & `nlmod-0.6.0/tests/test_010_wells.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+
 import nlmod
 
 
 def get_model_ds():
     kh = [10, 0.1, 20]
     kv = [0.5 * k for k in kh]
```

### Comparing `nlmod-0.5.3/tests/test_012_plot.py` & `nlmod-0.6.0/tests/test_012_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import nlmod
 import util
 
+import nlmod
+
 
 def test_plot_modelgrid():
     ds = util.get_ds_structured()
     nlmod.plot.modelgrid(ds)
 
 
 def test_plot_surface_water_empty():
```

### Comparing `nlmod-0.5.3/tests/test_015_gwf_output.py` & `nlmod-0.6.0/tests/test_015_gwf_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import tempfile
+
+import numpy as np
 import test_001_model
 
 import nlmod
-import numpy as np
-from nlmod.gwf import get_heads_da
 from nlmod.dims.grid import refine
+from nlmod.gwf import get_heads_da
 
 tmpdir = tempfile.gettempdir()
 tst_model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data")
 
 
 def test_create_small_model_grid_only(tmpdir, model_name="test"):
     model_name = "test"
@@ -51,15 +52,15 @@
     nlmod.gwf.npf(ds, gwf)
 
     # Create the initial conditions package
     nlmod.gwf.ic(ds, gwf, starting_head=1.0)
     nlmod.gwf.oc(ds, gwf)
 
     ds.update(nlmod.grid.mask_model_edge(ds, ds["idomain"]))
-    nlmod.gwf.chd(ds, gwf, chd="edge_mask", head="starting_head")
+    nlmod.gwf.chd(ds, gwf, mask="edge_mask", head="starting_head")
 
     nlmod.sim.write_and_run(sim, ds)
 
     heads_correct = np.ones((3, 5, 2, 3))
     heads_correct[:, 3, :, 1:] = np.nan
 
     da = get_heads_da(ds=ds, gwf=None, fname_hds=None)
@@ -105,15 +106,15 @@
     nlmod.gwf.npf(ds_unstr, gwf_unstr)
 
     # Create the initial conditions package
     nlmod.gwf.ic(ds_unstr, gwf_unstr, starting_head=1.0)
     nlmod.gwf.oc(ds_unstr, gwf_unstr)
 
     ds_unstr.update(nlmod.grid.mask_model_edge(ds_unstr, ds_unstr["idomain"]))
-    nlmod.gwf.chd(ds_unstr, gwf_unstr, chd="edge_mask", head="starting_head")
+    nlmod.gwf.chd(ds_unstr, gwf_unstr, mask="edge_mask", head="starting_head")
 
     nlmod.sim.write_and_run(sim, ds_unstr)
 
     heads_correct = np.ones((3, 5, 6))
     heads_correct[:, 3, [1, 2, 4, 5]] = np.nan
 
     da = get_heads_da(ds=ds_unstr, gwf=None, fname_hds=None)
```

