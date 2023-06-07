# Comparing `tmp/geoslurp-2.0.0.tar.gz` & `tmp/geoslurp-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoslurp-2.0.0.tar", last modified: Fri Sep  3 15:44:33 2021, max compression
+gzip compressed data, was "geoslurp-2.1.1.tar", last modified: Wed Jun  7 11:59:05 2023, max compression
```

## Comparing `geoslurp-2.0.0.tar` & `geoslurp-2.1.1.tar`

### file list

```diff
@@ -1,132 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-09-03 15:44:25.000000 geoslurp-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-09-03 15:44:33.631714 geoslurp-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      706 2021-09-03 15:44:25.000000 geoslurp-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.623714 geoslurp-2.0.0/clitools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:25.000000 geoslurp-2.0.0/clitools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17934 2021-09-03 15:44:25.000000 geoslurp-2.0.0/clitools/geoslurper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.623714 geoslurp-2.0.0/geoslurp/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.623714 geoslurp-2.0.0/geoslurp/config/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13407 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/config/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)     8116 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/config/localsettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/config/slurplogger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.623714 geoslurp-2.0.0/geoslurp/datapull/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/ftp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/geodesyunr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5563 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/github.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/icgem.py
--rw-r--r--   0 runner    (1001) docker     (121)     9478 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/motu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/rsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     9745 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/thredds.py
--rw-r--r--   0 runner    (1001) docker     (121)     8633 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/uri.py
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/datapull/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/ArcticDEM.py
--rw-r--r--   0 runner    (1001) docker     (121)     9265 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/Argo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/CSVBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/DuacsGriddedDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7932 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/EasyCora.py
--rw-r--r--   0 runner    (1001) docker     (121)     6086 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/GRACEDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/GSHHGDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/Hydrosheds.py
--rw-r--r--   0 runner    (1001) docker     (121)     4877 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/IceSatDrainDiv.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/OGRBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     5551 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/PSMSL.py
--rw-r--r--   0 runner    (1001) docker     (121)     6922 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/RGIDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     9242 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/RadsDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7869 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/RasterBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     8008 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/TUGRAZDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8497 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/avisoRefOrbits.py
--rw-r--r--   0 runner    (1001) docker     (121)    13164 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/dataSetBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/datasetgeneric.py
--rw-r--r--   0 runner    (1001) docker     (121)    16337 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/deg1n2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5037 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/era5.py
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/geodesyunr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/geoshapes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/icgemDsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/motuGridsBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/mss_cnes_cls2015.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/naturalearth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/orsiFronts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6578 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/pandasbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     4130 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/snrei.py
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/wgms_fog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dataset/wribasin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/db/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/connectorbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     5829 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/geoslurpdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)    12727 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/db/tabletools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/dbfunc/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dbfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dbfunc/dbfunc.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dbfunc/maskgeom.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dbfunc/radsfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/dbfunc/readfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/discover/
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/discover/fesom/
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/fesom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/fesom/extractprofiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/fesom/fesomQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/discover/generic/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/generic/getTableData.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/generic/regexQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.627714 geoslurp-2.0.0/geoslurp/discover/gravity/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/gravity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/gravity/graceQuery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/gravity/gravQuery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/gravity/staticQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/geoslurp/discover/oceanobs/
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oceanobs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      366 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oceanobs/argoProfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oceanobs/argoQuery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oceanobs/awipiesQuery.py
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oceanobs/coraQuery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oceanobs/psmsl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/geoslurp/discover/oras/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/discover/oras/orasQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/geoslurp/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     4310 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/Bounds.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5794 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/gravity.py
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/netcdftools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/ogrgeom.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/shapelytools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/tools/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/geoslurp/types/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/types/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/types/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/geoslurp/view/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/view/graceviews.py
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2021-09-03 15:44:25.000000 geoslurp-2.0.0/geoslurp/view/viewBase.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/geoslurp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-09-03 15:44:33.000000 geoslurp-2.0.0/geoslurp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-09-03 15:44:33.000000 geoslurp-2.0.0/geoslurp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-03 15:44:33.000000 geoslurp-2.0.0/geoslurp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-09-03 15:44:33.000000 geoslurp-2.0.0/geoslurp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-09-03 15:44:33.000000 geoslurp-2.0.0/geoslurp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-03 15:44:33.631714 geoslurp-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2021-09-03 15:44:25.000000 geoslurp-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 15:44:33.631714 geoslurp-2.0.0/userplugins/
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2021-09-03 15:44:25.000000 geoslurp-2.0.0/userplugins/AWIPIES.py
--rw-r--r--   0 runner    (1001) docker     (121)    10420 2021-09-03 15:44:25.000000 geoslurp-2.0.0/userplugins/FESOM.py
--rw-r--r--   0 runner    (1001) docker     (121)     7488 2021-09-03 15:44:25.000000 geoslurp-2.0.0/userplugins/ORAS5.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-09-03 15:44:25.000000 geoslurp-2.0.0/userplugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10347 2021-09-03 15:44:25.000000 geoslurp-2.0.0/userplugins/grdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.456416 geoslurp-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-07 11:58:54.000000 geoslurp-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-07 11:59:05.456416 geoslurp-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 11:58:54.000000 geoslurp-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.436415 geoslurp-2.1.1/clitools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:58:54.000000 geoslurp-2.1.1/clitools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19296 2023-06-07 11:58:54.000000 geoslurp-2.1.1/clitools/geoslurper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.436415 geoslurp-2.1.1/geoslurp/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.436415 geoslurp-2.1.1/geoslurp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/localsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/slurplogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/datapull/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/geodesyunr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/icgem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/motu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/thredds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/CSVBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/OGRBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/RasterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/cdsbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/dataSetBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/datasetgeneric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/era5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/motuGridsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/pandasbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/snrei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/xarraybase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/connectorbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/geoslurpdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/tabletools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/dbfunc/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/dbfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/maskgeom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/radsfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/readfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/earthmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/earthmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/earthmodels/getlove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/fesom/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/fesom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/fesom/extractprofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/fesom/fesomQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/generic/getTableData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/generic/regexQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/gravity/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/graceQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/gravQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/staticQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/oceanobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/argoProfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/argoQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/awipiesQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/coraQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/psmsl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/oras/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oras/orasQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.448416 geoslurp-2.1.1/geoslurp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/Bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/netcdftools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/ogrgeom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/shapelytools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/spatiallite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/tarsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.448416 geoslurp-2.1.1/geoslurp/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/columnmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/xar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.448416 geoslurp-2.1.1/geoslurp/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/view/graceviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/view/viewBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.456416 geoslurp-2.1.1/geoslurp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:59:05.456416 geoslurp-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-07 11:58:54.000000 geoslurp-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.456416 geoslurp-2.1.1/userplugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/AWIPIES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/ArcticDEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/Argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/DuacsGriddedDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/EasyCora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/FESOM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/GRACEDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/GSHHGDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/Hydrosheds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/IceSatDrainDiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/ORAS5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/PSMSL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/RGIDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/RadsDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/TUGRAZDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/avisoRefOrbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/deg1n2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/geodesyunr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/geoshapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/gleam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/glofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/gracefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/icgemDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/imerg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/loadlove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/mss_cnes_cls2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/naturalearth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/orsiFronts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/sebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/sentinelreforbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/wgms_fog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/wribasin.py
```

### Comparing `geoslurp-2.0.0/LICENSE` & `geoslurp-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/PKG-INFO` & `geoslurp-2.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: geoslurp
-Version: 2.0.0
+Version: 2.1.1
 Summary: Python postgreSQL-PostGIS client for managing earth science datasets
 Home-page: https://github.com/strawpants/geoslurp
 Author: Roelof Rietbroek
 Author-email: roelof@wobbly.earth
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
+Provides-Extra: SH
 License-File: LICENSE
 
 # Download and manage datasets in a PostGreSQL database with the PostGIS
 The idea is that this tool contains script to download (i.e. **slurp**) commonly used datasets and to register them in a postgresql+postgis database. This database can then be queried allowing the retrieval of the relevant data or datafiles. 
 
 The main documentation lives at [wobbly.earth/geoslurp](https://wobbly.earth/geoslurp)
 
@@ -26,9 +25,7 @@
 The geoslurp module itself is a pure python module, which acts as a client. For this to work one needs to [set up a running PostGreSQL database](https://github.com/strawpants/docker-geoslurp).
 
 ![Image of geoslurp clients versus database server](docsrc/graphics/geoslurp_network.svg)
 
 
 
 
-
-
```

### Comparing `geoslurp-2.0.0/README.md` & `geoslurp-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/clitools/geoslurper.py` & `geoslurp-2.1.1/clitools/geoslurper.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     parser=addCommandLineArgs()
     args = parser.parse_args(argv[1:])
     args=check_args(args,parser)
 
 
     # We need a point of contact to communicate with the database
     try:
-        DbConn=GeoslurpConnector(args.host,args.user,args.password,cache=args.cache,dataroot=args.dataroot)
+        DbConn=GeoslurpConnector(args.host,args.user,args.password,cache=args.cache,dataroot=args.dataroot,plugindir=args.plugindir)
     except Exception as e:
         print(e)
         print("Cannot connect to postgresql database, quitting")
         sys.exit(1)
 
 
     # # Process common options
@@ -59,25 +59,43 @@
         addUser(DbConn,args.add_readonly_user,True)
 
 
 
     #print registered datasets (i.e. tables)
     if args.info:
         slurpInvent=Inventory(DbConn)
-        print("Registered datasets (scheme.dataset, owner, lastupdate):")
+        print("Registered entries:")
         if args.dset:
             #print a summary of the inventory
             dsetpat=re.compile(args.dset)
             for entry in slurpInvent:
-                if dsetpat.fullmatch(entry.scheme+'.'+entry.dataset):
-                    print("%s.%s %s %s"%(entry.scheme,entry.dataset,entry.owner,entry.lastupdate.isoformat()))
-        else:
+                if entry.dataset is not None and dsetpat.fullmatch(entry.scheme+'.'+entry.dataset):
+                    print({ky:val for ky,val in entry.__dict__.items() if ky not in ['_sa_instance_state','view','pgfunc']})
+        
+        elif args.view:
+            #print a summary of the inventory
+            viewpat=re.compile(args.view)
+            for entry in slurpInvent:
+                if entry.view is not None and viewpat.fullmatch(entry.scheme+'.'+entry.view):
+                    print({ky:val for ky,val in entry.__dict__.items() if ky not in ['_sa_instance_state','dataset','pgfunc']})
+        elif args.func:
             #print a summary of the inventory
+            funcpat=re.compile(args.func)
             for entry in slurpInvent:
-                print("%s.%s %s %s"%(entry.scheme,entry.dataset,entry.owner,entry.lastupdate.isoformat()))
+                if entry.pgfunc is not None and funcpat.fullmatch(entry.scheme+'.'+entry.pgfunc):
+                    print({ky:val for ky,val in entry.__dict__.items() if ky not in ['_sa_instance_state','dataset','view']})
+        else:
+            #print a summary of the inventory (registered datasets, views, functions)
+            for entry in slurpInvent:
+                if entry.dataset is not None:
+                    print("DATASET: %s.%s %s %s"%(entry.scheme,entry.dataset,entry.owner,entry.lastupdate.isoformat()))
+                elif entry.view is not None:
+                    print("VIEW: %s.%s %s %s"%(entry.scheme,entry.view,entry.owner,entry.lastupdate.isoformat()))
+                elif entry.pgfunc is not None:
+                    print("FUNCTION: %s.%s %s %s"%(entry.scheme,entry.pgfunc,entry.owner,entry.lastupdate.isoformat()))
         sys.exit(0) 
     
     #change settings in the database
     
     # Initializes an object which holds the current settings
     conf=Settings(DbConn)
     if args.config:
@@ -351,14 +369,16 @@
                             help='Select password for the postgresql user')
 
         parser.add_argument("--port",metavar="port",type=int, default=5432,
                             help='Select the port where the database is served')
 
         parser.add_argument("--dataroot",metavar="DATAROOT",nargs="?",type=str, help="Specify the local root of the data directory. Defaults to ${HOME}/geoslurp_data")
 
+        parser.add_argument("--plugindir",metavar="DIREC",nargs="?",type=str, help="Append a directory where dataset implementations can be found.")
+
 
         parser.add_argument("--dbalias",metavar="DBALIAS",nargs="?",type=str, help="Specify the database alias to connect to. Each database alias can have a different host,port,user,password,dataroot,etc (see the localsettings file")
         # parser.add_argument("--usekeyring",action='store_true',
         #                     help='Set and get the system keyring to store the database password (alternatives are '
         #                          'using --password or the environment variable GEOSLURP_PGPASS')
         parser.add_argument("--keyring","--no-keyring",dest="usekeyring",action=NegateAction, nargs=0,
                             help=" Use/don't use the system keyring to store and retrieve the database password (alternatives are "
```

### Comparing `geoslurp-2.0.0/geoslurp/config/catalogue.py` & `geoslurp-2.1.1/geoslurp/config/catalogue.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import yaml
 import inspect
 from datetime import datetime
 from geoslurp.config.slurplogger import slurplog
 from geoslurp.db import Inventory
 from importlib import import_module
 
+from geoslurp.dataset.datasetgeneric import DataSetGeneric
+
 class DatasetCatalogue:
     #holds dataset classes (not initiated!)
     __dsets__=[]
     __dbfuncs__=[]
     __dviews__=[]
     # holds factory methods for dyanamically building datasets
     __dsetfac__=[]
@@ -40,20 +42,19 @@
     
     @staticmethod 
     def getCacheFile(conf):
         return os.path.join(conf.getCacheDir("Dset"),"Dset_Catalogue.yaml")
     
     @staticmethod 
     def addUserPlugPaths(conf,loadmod=False):
-        if 'userplugins' in conf.userentry.conf:
-            for upath in conf.userentry.conf["userplugins"].split(";"):
-                if sys.path.count(upath) == 0:
-                    sys.path.append(upath)
-                    if loadmod:
-                        mod=__import__(os.path.basename(upath))
+        for upath in conf.db.plugindir.split(";"):
+            if sys.path.count(upath) == 0:
+                sys.path.append(upath)
+                if loadmod:
+                    mod=__import__(os.path.basename(upath))
 
     def addDataset(self, datasetcls):
         self.__dsets__.append(datasetcls)
     
     def addDatasetFactory(self, datasetclsfac):
         self.__dsetfac__.append(datasetclsfac)
     
@@ -139,27 +140,26 @@
     def registerAllDataSets(self,conf):
         """load all dataset classes (but don't construct them)"""
         if self.__dsets__:
             #already loaded (quick return)
             return
         
         #dynamically import all relevant datasets and class factories (including userplugin datasets)
-        modgeo=__import__("geoslurp.dataset")
+        # modgeo=__import__("geoslurp.dataset")
        
         #dynamically load functions
         modgeof=__import__("geoslurp.dbfunc")
 
         #dynamically load views
         modgeov=__import__("geoslurp.view")
 
         #also load userplugins
         self.addUserPlugPaths(conf,True)
 
 
-
     def listDataSets(self,conf):
         self.loadCatalogue(conf)
         return self.__catalogue__["datasets"]
 
     def listFunctions(self,conf):
         self.loadCatalogue(conf)
         return self.__catalogue__["functions"]
@@ -245,16 +245,16 @@
                         ds=type(tbl,(dsbase,),{"scheme":scheme})
                     outdsets=[ds]
         
         if not outdsets and singleEntry:
             #fall back with a generic type
 
             scheme,tbl=regex.split(".")
-            dsgen=self.getDsetClass(conf,"anyscheme.DataSetGeneric")
-            outdsets.append(type(tbl,(dsgen,),{"scheme":scheme}))
+            # dsgen=self.getDsetClass(conf,"anyscheme.DataSetGeneric")
+            outdsets.append(type(tbl,(DataSetGeneric,),{"scheme":scheme}))
 
         return outdsets
         
     def getDFuncClass(self,conf,name):
         """Loads a database function as an class (but check cache first)"""
         if name in self.__dfcache__:
             return self.__dfcache__[name]
```

### Comparing `geoslurp-2.0.0/geoslurp/config/localsettings.py` & `geoslurp-2.1.1/geoslurp/config/localsettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
     local_settings=None
     """(str): Alternative local settings file (instead of ${HOME}/.geoslurp_lastused.yaml)"""
 
     cache=None
     write_local_settings=False
     dbalias=None
-
-    def __init__(self,host=None,user=None,usekeyring=False,password=None,port=None,dataroot=None,cache=None,dbalias=None):
+    plugindir=None
+    def __init__(self,host=None,user=None,usekeyring=False,password=None,port=None,dataroot=None,cache=None,dbalias=None,plugindir=None):
         if host:
             self.host=host
 
         if user:
             self.user=user
 
         if usekeyring:
@@ -61,18 +61,24 @@
         if port:
             self.port=port
         
         if dataroot:
             self.dataroot=dataroot
         if cache:
             self.cache=cache
+
         if dbalias:
             self.dbalias=dbalias
+        
+        if plugindir:
+            self.plugindir=plugindir
 
-defaultdbdict={"host":None,"user":"geoslurp","port":5432,"readonlyUser":"slurpy","cache":"/tmp/geoslurp_cache","dataroot":os.path.join(os.path.expanduser('~'),'geoslurp_data')}
+defaultdbdict={"host":None,"user":"geoslurp","port":5432,"readonlyUser":"slurpy",
+        "cache":"/tmp/geoslurp_cache","dataroot":os.path.join(os.path.expanduser('~'),'geoslurp_data'),
+        "plugindir":os.path.abspath(os.path.dirname(__file__)+"../../../userplugins")}
 
 
 def readLocalSettings(args=settingsArgs(),readonlyuser=True,dbalias=None):
     """Retrieves/updates last used settings from the local settings file .geoslurp_lastused.yaml"""
 
     #We need a deepcopy to properly separate input from output, and funny behavior
     argsout=copy.deepcopy(args)
@@ -214,14 +220,22 @@
     if argsout.cache:
         lastOpts[dbalias]["cache"]=argsout.cache
     else:
         if "cache"  in lastOpts[dbalias]:
             argsout.cache=lastOpts[dbalias]["cache"]
         else:
             argsout.cache="/tmp/geoslurp_cache"
+    
+    if argsout.plugindir:
+        lastOpts[dbalias]["plugindir"]=argsout.plugindir
+    else:
+        if "plugindir" in lastOpts[dbalias]:
+            argsout.plugindir=lastOpts[dbalias]["plugindir"]
+        else:
+            argsout.plugindir=defaultdbdict["plugindir"]
 
     #write out  options to file to store these settings
     if isUpdated and argsout.write_local_settings:
         lastOpts["lastupdate"]=datetime.now()
         with open(settingsFile,'w') as fid:
             yaml.dump(lastOpts, fid, default_flow_style=False)
```

### Comparing `geoslurp-2.0.0/geoslurp/config/slurplogger.py` & `geoslurp-2.1.1/geoslurp/config/slurplogger.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/datapull/crawler.py` & `geoslurp-2.1.1/geoslurp/datapull/crawler.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/datapull/ftp.py` & `geoslurp-2.1.1/geoslurp/datapull/ftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         regexdir=re.compile(b'^d[\-r][\-w][\-x]')
         url=os.path.join(self.rooturl,subdirs)
         if url[-1] != '/':
             url+='/'
 
         buf=Uri(url,auth=self.auth).buffer()
 
+        #import pdb;pdb.set_trace() 
         for ln in buf.getvalue().splitlines():
             t=None
             #try to parse the date from the buffer line
             match=regexdate.search(ln)
             if match:
                 t=datetime.strptime(match.group(1).decode('utf-8'),'%b %d %Y')
             else:
@@ -60,25 +61,23 @@
                 if match:
                     t=datetime.strptime(match.group(1).decode('utf-8'),'%b %d %H:%M')
                     if t.month <= datetime.now().month:
                         t=t.replace(year=datetime.now().year)
                     else:
                         #last year
                         t=t.replace(year=datetime.now().year-1)
-
             name=ln.decode('utf-8').split()[-1]
             if regexdir.match(ln):
                 #append /
                 name+='/'
 
             yield name,t
 
     def uris(self, check=False,subdirs=''):
         """Generate a list files in a directory and return a list of uri"""
-
         for name,t in self.ls(subdirs):
             #only apply the pattern to the last column
             if re.search(self.pattern,name):
                 uri=Uri(os.path.join(self.rooturl,subdirs,name),lastmod=t,subdirs=subdirs,auth=self.auth)
 
                 if uri.lastmod == None:
                     #one can try to get this information through the header informatio too (slower and not always working)
```

### Comparing `geoslurp-2.0.0/geoslurp/datapull/geodesyunr.py` & `geoslurp-2.1.1/geoslurp/datapull/geodesyunr.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/datapull/github.py` & `geoslurp-2.1.1/geoslurp/datapull/github.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/datapull/http.py` & `geoslurp-2.1.1/geoslurp/discover/gravity/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,14 @@
 
 # geoslurp is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public
-# License along with Frommle; if not, write to the Free Software
+# License along with geoslurp; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
-# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
-import re
-import os
-from geoslurp.datapull import UriBase
-
-class Uri(UriBase):
-    def __init__(self,url,lastmod=None,auth=None,headers=None):
-        super().__init__(url=url,lastmod=lastmod,auth=auth,headers=headers)
-        if not bool(re.match('^https?://',url)):
-            raise Exception("URL does not seem to be a valid http(s) address")
-
+# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
 
+from .staticQuery import *
+from .graceQuery import *
```

### Comparing `geoslurp-2.0.0/geoslurp/datapull/icgem.py` & `geoslurp-2.1.1/geoslurp/datapull/icgem.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/datapull/motu.py` & `geoslurp-2.1.1/geoslurp/datapull/motu.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/datapull/rsync.py` & `geoslurp-2.1.1/geoslurp/datapull/rsync.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,34 +14,43 @@
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
 
 from geoslurp.datapull import CrawlerBase,  UriFile
 import subprocess
 import re
-
+import os
 class Crawler(CrawlerBase):
     """Crawler wrapper around the rsync program calls the linux rsync utility"""
     def __init__(self,url,auth):
         super().__init__(url)
         self.auth=auth
 
-    def parallelDownload(self,outdir,check=False):
+    def parallelDownload(self,outdir,check=False,includes=None,dryrun=False):
         updated=[]
+        cmd=['rsync', '-avz', '--del']
         if check:
-            cmd=['rsync', '-avz', '--del','--update', self.auth.user +"@"+self.rooturl,outdir]
-        else:
-            cmd=['rsync', '-avz', '--del', self.auth.user +"@"+self.rooturl,outdir]
-
+            cmd.append('--update')
+        if dryrun:
+            cmd.append('--dry-run')
+        if includes:
+            cmd.extend([f'--include={inc}' for inc in includes]) 
+            # inclist='{"'+'","'.join(includes)+'"}'
+            # cmd.append(f'--include={inclist}')
+            #exclude everything else which is not obeying the include filters
+            cmd.append('--exclude=*')
+            
+        cmd.append(self.auth.user +"@"+self.rooturl)
+        cmd.append(outdir)
         for file in self.startrsync(cmd):
-             updated.append(UriFile(file))
+             updated.append(UriFile(os.path.join(outdir,file)))
         return updated
 
     def startrsync(self,cmd):
-        """Start rsync and returns the lsit of files as a generator"""
+        """Start rsync and returns the list of files as a generator"""
         #start command and catch output
         dryrun=subprocess.Popen(cmd,stdout=subprocess.PIPE, env={"RSYNC_PASSWORD":self.auth.passw})
         buf,stderr=dryrun.communicate()
         #skip rsync output, and directories
         skipregex=re.compile(b'(/$)|(receiving incremental)|(^$)|(sent.*bytes.*received)|(total size)')
         for ln in buf.splitlines():
 
@@ -50,12 +59,11 @@
             yield ln.decode('utf-8')
 
     def  uris(self):
         pass
 
     def ls(self):
         """list remote content (using dry run)"""
-        #write a tempoary passowrd file to /tmp
         cmd=['rsync', '-avz', '--del','--dry-run', self.auth.user +"@"+self.rooturl,'.']
         for file in self.startrsync(cmd):
             yield file
```

### Comparing `geoslurp-2.0.0/geoslurp/datapull/thredds.py` & `geoslurp-2.1.1/geoslurp/datapull/thredds.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 from geoslurp.datapull import UriBase,CrawlerBase
 
 
 class Uri(UriBase):
     """Thredds URI class"""
     suburl=None
     opendap=None
-    def __init__(self,dataxml,services):
+    def __init__(self,dataxml,services,auth=None):
         self.suburl=dataxml.attrib['urlPath']
 
         self.opendap=services.baseurl+services.opendap+self.suburl
         #set the main url to the http version
-        super().__init__(services.baseurl+services.http+self.suburl,lastmod=getDate(dataxml))
+        super().__init__(services.baseurl+services.http+self.suburl,lastmod=getDate(dataxml),auth=auth)
 
 
 
 
 class ThreddsFilter():
     """Helper class to aid traversing to opendap xml elements"""
     def __init__(self,xmltyp="*",attr=None,regex=None):
@@ -134,23 +134,24 @@
     for ky,val in xml.attrib.items():
         if re.search(regex,ky):
             return val
     return None
 
 class Crawler(CrawlerBase):
     """A class to work with an Opendap server"""
-    def __init__(self, catalogurl, filter=ThreddsFilter("dataset", attr="urlPath"), followfilter=ThreddsFilter("catalogRef").OR("dataset")):
+    def __init__(self, catalogurl, filter=ThreddsFilter("dataset", attr="urlPath"), followfilter=ThreddsFilter("catalogRef").OR("dataset"),auth=None):
         super().__init__(url=catalogurl)
         #load the root catalog
         self._catalogurl=catalogurl
         self._rootxml=self.getCatalog(catalogurl)
         self.services=self.getServices(self._rootxml,self._catalogurl)
         self._filt=filter
         self._followFilt=followfilter
         self.resuming=False
+        self.auth=auth
     def setResumePoint(self,filter,followfilt=None):
         """Sets the filters after which the normal filters will be applied."""
         # stores a copy of the normal filter and set the resume filter to the normal filter
         self._filtcopy=self._filt
         self._filt=filter
 
         if followfilt:
@@ -168,26 +169,26 @@
 
         if self._followFiltcopy:
             self._followFilt=self._followFiltcopy
             self._followFiltcopy=None
         self.resuming=False
 
     @staticmethod
-    def getCatalog(url):
+    def getCatalog(url,auth=None):
         """Retrieve a catalogue"""
         slurplogger().info("getting Thredds catalog: %s"%(url))
-        buf=http(url).buffer()
+        buf=http(url,auth=auth).buffer()
         return XMLTree.fromstring(buf.getvalue())
 
 
     @staticmethod
     def getServices(catalog,rooturl,depth=2):
         """Retrieves the root for serving files over http url from a catalogue"""
         compoundfilt=ThreddsFilter("service", attr="serviceType", regex="Compound")
-        opendapfilt=ThreddsFilter("service", attr="serviceType", regex="(OpenDAP)|(OPENDAP)|(DODS)")
+        opendapfilt=ThreddsFilter("service", attr="serviceType", regex="(OpenDAP)|(OPENDAP)|(DODS)|(OPeNDAP)")
         httpfilt=ThreddsFilter("service", attr="serviceType", regex="HTTPServer")
         # possibly add other serices if deemed usefull
         servtuple=namedtuple("Service","baseurl opendap catalog http")
 
         proto,url=rooturl.split('://')
         #also strip off trailing directory to retrieve the root
         baseurl, tmp=url.split('/', 1)
@@ -265,13 +266,13 @@
                     suburl=url
                     subxml=xelem
 
                 yield from self.xmlitems(subxml, suburl, depth)
 
     def uris(self,depth=10):
         """Generates a list of threddsURI's (makes use of xmlitems())"""
-        urlFilt=ThreddsFilter("dataset", attr="urlPath")
+        # urlFilt=ThreddsFilter("dataset", attr="urlPath")
         for xelem in self.xmlitems(depth=depth):
-            if urlFilt.isValid(xelem):
+            if self._filt.isValid(xelem):
                 yield Uri(xelem,self.services)
```

### Comparing `geoslurp-2.0.0/geoslurp/datapull/uri.py` & `geoslurp-2.1.1/geoslurp/datapull/uri.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 def setFtime(file,modTime=None):
     """change modification and access time of a file"""
     if modTime:
         mtime=time.mktime(modTime.timetuple())
         os.utime(file,(mtime,mtime))
 
-def curlDownload(url,fileorfid,mtime=None,gzip=False,gunzip=False,auth=None,restdict=None,headers=None,customRequest=None,upfid=None):
+def curlDownload(url,fileorfid,mtime=None,gzip=False,gunzip=False,auth=None,restdict=None,headers=None,customRequest=None,upfid=None,cookiefile=None):
     """
     Download  the content of an url to an open file or buffer using pycurl
     :param url: url to download from
     :param fileorfid: filename or open file or buffer
     :param mtime: explicitly set the modification time to this (usefull when modification times are not supported
     b the server)
     :param gzip: additionally gzip the file on disk (note this routine does not append \*.gz to the file name)
@@ -87,42 +87,71 @@
             fid=gz.open(tmpfile,'wb')
         else:
             fid=open(tmpfile,'wb')
     else:
         fid=fileorfid
 
     crl=pycurl.Curl()
+    #crl.setopt(pycurl.VERBOSE,1)
     crl.setopt(pycurl.USERAGENT,"curl/7.72.0")
     crl.setopt(pycurl.URL,url.replace(' ','%20'))
     crl.setopt(pycurl.FOLLOWLOCATION, 1)
     crl.setopt(pycurl.WRITEDATA,fid)
      
     if customRequest:
         crl.setopt(pycurl.CUSTOMREQUEST,customRequest)
 
-    if headers:
-        crl.setopt(pycurl.HTTPHEADER,headers)
+    
+    if cookiefile:
+        if os.path.exists(cookiefile):
+            crl.setopt(pycurl.COOKIEFILE, cookiefile)
+
+        crl.setopt(pycurl.COOKIEJAR, cookiefile)
+
 
     if auth:
-        #use authentification
-        crl.setopt(pycurl.USERPWD,auth.user+":"+auth.passw)
+        if hasattr(auth,"ftptls"):
+            #enable explicit ftp over tls
+            if auth.ftptls:
+    #            crl.setopt(pycurl.HTTPPROXYTUNNEL,1)
+                crl.setopt(pycurl.FTP_SSL, pycurl.FTPSSL_ALL)
+                crl.setopt(pycurl.FTPSSLAUTH,pycurl.FTPAUTH_TLS)
+        if hasattr(auth,"trusted"):
+            if auth.trusted:
+                crl.setopt(pycurl.UNRESTRICTED_AUTH,1)
+        if hasattr(auth,'oauthtoken'):
+            #use oauth in a header to authenticate
+            oauthhead=f"Authorization: Bearer {auth.oauthtoken}"
+            if headers:
+                headers.append(oauthead)
+            else:
+                headers=[oauthhead]
+
+
+        else:
+            #use basic authentication
+            crl.setopt(pycurl.USERPWD,auth.user+":"+auth.passw)
+
+    if headers:
+        crl.setopt(pycurl.HTTPHEADER,headers)
     
     if restdict:
         crl.setopt(crl.POSTFIELDS,urlencode(restdict))
     
     if upfid:
         crl.setopt(pycurl.UPLOAD,1)
         crl.setopt(pycurl.READDATA,upfid)
 
     try:
         crl.perform()
     except pycurl.error as pyexc:
         # possibly remove a partly downloaded file
-        if os.path.exists(tmpfile):
-            os.remove(tmpfile)
+        if type(fileorfid) == str:       
+            if os.path.exists(tmpfile):
+                os.remove(tmpfile)
         raise pyexc
 
     modtime=timeFromStamp(crl.getinfo(pycurl.INFO_FILETIME))
     if mtime:
         #force the modification time to that provided
         modtime=mtime
 
@@ -147,20 +176,21 @@
 class UriBase():
     """Base class to store uri resource"""
     url=None
     lastmod=None
     auth=None #link to a certain authentification alias
     subdirs='' #create these subdrectories when downloading the file
     headers=None 
-    def __init__(self,url,lastmod=None,auth=None,subdirs='',headers=None):
+    def __init__(self,url,lastmod=None,auth=None,subdirs='',headers=None,cookiefile=None):
         self.url=url
         self.lastmod=lastmod
         self.auth=auth
         self.subdirs=subdirs
         self.headers=headers
+        self.cookiefile=cookiefile
 
     def updateModTime(self):
         """Tries to retrieve the last modification time of a file
         Note: his is often not supported by the server"""
         crl=pycurl.Curl()
         crl.setopt(pycurl.URL,self.url)
         #note: not all servers support this query with NOBODY set to 1
@@ -189,28 +219,28 @@
             else:
                 outf=os.path.join(direc,self.subdirs,os.path.basename(self.url))
 
 
 
         #create directory if it does not exist
         if not os.path.exists(os.path.dirname(outf)):
-            os.makedirs(os.path.dirname(outf))
+            os.makedirs(os.path.dirname(outf),exist_ok=True)
 
         uri=UriFile(url=outf)
         if check and self.lastmod and uri.lastmod:
             if self.lastmod <= uri.lastmod:
                 #no need to download the file
                 slurplog.info("Already Downloaded, skipping %s"%(uri.url))
                 return uri,False
         slurplog.info("Downloading %s"%(uri.url))
         try:
             if self.lastmod:
-                curlDownload(self.url,uri.url,self.lastmod,gzip=gzip,gunzip=gunzip,auth=self.auth,restdict=restdict,headers=self.headers)
+                curlDownload(self.url,uri.url,self.lastmod,gzip=gzip,gunzip=gunzip,auth=self.auth,restdict=restdict,headers=self.headers,cookiefile=self.cookiefile)
             else:
-                self.lastmod=curlDownload(self.url,uri.url,gzip=gzip,gunzip=gunzip,auth=self.auth,restdict=restdict,headers=self.headers)
+                self.lastmod=curlDownload(self.url,uri.url,gzip=gzip,gunzip=gunzip,auth=self.auth,restdict=restdict,headers=self.headers,cookiefile=self.cookiefile)
         except pycurl.error as pyexc:
             slurplog.info("Download failed, skipping %s"%(uri.url))
             if not continueonError:
                 raise pyexc
         except Exception as e:
             raise e
         uri.lastmod=self.lastmod
```

### Comparing `geoslurp-2.0.0/geoslurp/datapull/webdav.py` & `geoslurp-2.1.1/geoslurp/datapull/webdav.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/ArcticDEM.py` & `geoslurp-2.1.1/userplugins/ArcticDEM.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/Argo.py` & `geoslurp-2.1.1/userplugins/Argo.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/CSVBase.py` & `geoslurp-2.1.1/geoslurp/dataset/CSVBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/DuacsGriddedDsets.py` & `geoslurp-2.1.1/userplugins/DuacsGriddedDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/EasyCora.py` & `geoslurp-2.1.1/userplugins/EasyCora.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Authors Roelof Rietbroek (r.rietbroek@utwente.nl) and Alisa Yakhontova, 2021
 
 from geoslurp.dataset.dataSetBase import DataSet
 from geoslurp.datapull.ftp import Crawler as ftpCrawler
 import tarfile
+from geoslurp.tools.tarsafe import tar_safe_extractall
 from geoslurp.tools.netcdftools import ncStr
 from geoslurp.datapull import findFiles
 from geoslurp.datapull import UriFile
 from geoalchemy2.types import Geometry,Geography
 from geoalchemy2.elements import WKBElement
 from sqlalchemy import Column,Integer,String, Boolean, ARRAY
 from sqlalchemy.dialects.postgresql import TIMESTAMP
@@ -178,15 +179,15 @@
                 #check if the files need unpacking (only unpack when needed)
                     #check if the last file is already extracted
                     if os.path.exists(succesfile):
                         slurplogger().info(f"{tarf.url} is already extracted, skipping")
                     else:
                         with tarfile.open(tarf.url,"r:gz") as tf:
                             slurplogger().info(f"Extracting trajectory files from {tarf.url}")
-                            tf.extractall(datadir)
+                            tar_safe_extractall(tf,datadir)
                             #touch the sucessfile to indcate this archive has been sucessfully extracted
                         Path(succesfile).touch()
             except tarfile.ReadError as exc:
                 raise exc
 
     def register(self,pattern='.*\.nc$'):
         """Register downloaded trajectory files from CORA
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/GRACEDsets.py` & `geoslurp-2.1.1/userplugins/GRACEDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/GSHHGDsets.py` & `geoslurp-2.1.1/userplugins/GSHHGDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/Hydrosheds.py` & `geoslurp-2.1.1/userplugins/Hydrosheds.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/IceSatDrainDiv.py` & `geoslurp-2.1.1/userplugins/IceSatDrainDiv.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/OGRBase.py` & `geoslurp-2.1.1/geoslurp/dataset/OGRBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from geoslurp.dataset.dataSetBase import DataSet
 from osgeo import gdal,osr
 from geoslurp.config.slurplogger import slurplogger
 from geoalchemy2 import WKBElement,Geography,Geometry
 from sqlalchemy import Column, Integer, String, Float, BigInteger,Date,DateTime
 from geoslurp.db import tableMapFactory
 import re
-
+from zipfile import ZipFile
+import os
 
 
 
 class OGRBase(DataSet):
     """Base class which downloads a single OGR layer (e.g. shapefile) and registers it as a postgis table"""
     table=None
     gtype=None
@@ -135,17 +136,26 @@
         :returns nothing (but sets the internal qlalchemy table)
         """
         # currently we can only cope with updating the entire table as a whole
         self.db.dropTable(self.name,self.scheme)
 
         slurplogger().info("Filling POSTGIS table %s.%s with data from %s" % (self.scheme, self.name, self.ogrfile))
         
-        #open shapefile directory
+        #open shapefile directory or ogr file
+        if self.ogrfile.endswith('.kmz') and not gdal.GetDriverByName('LIBKML'): 
+            #unzip the kmz file
+            cache=self.cacheDir()
+            with ZipFile(self.ogrfile,'r') as zp:
+                kmlf=zp.namelist()[0]#take the first zip file only 
+                zp.extract(kmlf,cache)
+            kmlfile=os.path.join(cache,kmlf)
+            shpf=gdal.OpenEx(kmlfile,0)
 
-        shpf=gdal.OpenEx(self.ogrfile,0)
+        else:
+            shpf=gdal.OpenEx(self.ogrfile,0)
         
         count=0
         for ithlayer in range(shpf.GetLayerCount()):
             shpflayer=shpf.GetLayer(ithlayer)
             if self.layerregex:
                 if not re.search(self.layerregex,shpflayer.GetName()):
                     continue
@@ -161,15 +171,15 @@
             # print(sourceprj.IsSame(self.targetprj))
             for feat in shpflayer:
                 count+=1
                 if self.table == None:
                     cols=self.columnsFromOgrFeat(feat)
                     self.createTable(cols)
                 values=self.valuesFromOgrFeat(feat,transform)
-#                 import pdb;pdb.set_trace()
+                # import pdb;pdb.set_trace()
                 try:
                     self.addEntry(values)
                 except:
                     pass
                 #commit every X times
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/PSMSL.py` & `geoslurp-2.1.1/userplugins/PSMSL.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/RGIDsets.py` & `geoslurp-2.1.1/userplugins/RGIDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/RadsDsets.py` & `geoslurp-2.1.1/userplugins/grdc.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,239 +9,261 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public
 # License along with Frommle; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
-# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
+# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2020
 
-from geoslurp.dataset import DataSet
-from geoalchemy2.elements import WKBElement
-from geoalchemy2.types import Geography
-from sqlalchemy import Column,Integer,String, Boolean
-from sqlalchemy.dialects.postgresql import TIMESTAMP, JSONB
-from sqlalchemy import MetaData
-from geoslurp.datapull import UriFile
-from geoslurp.datapull.rsync import Crawler as rsync
-from geoslurp.datapull.uri import findFiles
+
+from geoslurp.datapull.ftp import Uri as ftp
+from geoslurp.config.slurplogger import slurplogger
+from geoslurp.datapull.webdav import Crawler as webdav
+from zipfile import ZipFile
 import os
+from geoslurp.config.catalogue import geoslurpCatalogue
+from geoslurp.dataset.pandasbase import PandasBase
+from geoslurp.dataset.OGRBase import OGRBase
+from geoslurp.dataset.dataSetBase import DataSet
+from geoslurp.datapull import findFiles,UriFile
+from geoalchemy2 import Geography,WKTElement,WKBElement
+from sqlalchemy import MetaData
 from sqlalchemy.ext.declarative import declared_attr, as_declarative
-from netCDF4 import Dataset as ncDset
-from osgeo import ogr
-from datetime import datetime,timedelta
-from glob import glob
-from geoslurp.config.slurplogger import slurplogger
+from sqlalchemy import Column,Integer,String, Boolean,Float
+from sqlalchemy.dialects.postgresql import TIMESTAMP
+from shapely.wkt import dumps as wktdump
+from shapely.wkb import dumps as wkbdump
+from shapely.geometry import Point
 import re
-from geoslurp.config.catalogue import geoslurpCatalogue
-from geoslurp.db.settings import getCreateDir
-geotracktype = Geography(geometry_type="MULTILINESTRINGZ", srid='4326', spatial_index=True, dimension=3)
+import gzip
+from datetime import datetime
+
+scheme='grdc'
+
+def pullGRDC(downloaddir,auth,pattern,unzip=True):
+    """Pulls various GRDC datasets from a webdav folder"""
+    gissource=webdav(auth.url,auth=auth,pattern=pattern)
+    for uri in gissource.uris():
+        urif,upd=uri.download(downloaddir,check=True)
+        #unzip if newly updated
+        if upd and unzip:
+            with ZipFile(urif.url,'r') as zp:
+                    zp.extractall(downloaddir)
+
+class grdc_gis_base(OGRBase):
+    """Base class for the shapefiles from the grdc station data. Note """
+    scheme=scheme
+    filename=''
+    def __init__(self,dbconn):
+        super().__init__(dbconn)
+        if not self._dbinvent.cache:
+                self._dbinvent.cache=self.conf.getCacheDir(self.scheme,subdirs='GIS_layers')
+        self.ogrfile=os.path.join(self._dbinvent.cache,self.filename)
+    
+    def pull(self):
+        """Pulls the GIS_Layers.zip file from the web and unzip it in the cache"""
+        try:
+            cred=self.conf.authCred("grdcgis")
+        except:
+            raise RuntimeError("No Authentification data found. The GRDC GIS data is unfortunately only available after agreeing with the grdc user policy, please visit https://www.bafg.de/GRDC/EN/04_spcldtbss/43_GRfN/refDataset_node.html") 
+        
+        pullGRDC(self._dbinvent.cache,cred,pattern="GIS_layers\.zip")
+
+geoPointtype = Geography(geometry_type="POINTZ", srid='4326', spatial_index=True,dimension=3)
+class grdc_catalogue(PandasBase):
+    scheme=scheme
+    ftype='excel'
+    dtypes={"geom":geoPointtype}
+    pdfile='GRDC_Stations.xlsx'
+    def __init__(self,dbconn):
+        super().__init__(dbconn)
+        if not self._dbinvent.cache:
+                self._dbinvent.cache=self.conf.getCacheDir(self.scheme)
+        self.pdfile=os.path.join(self.cacheDir(),self.pdfile)
+
+    def pull(self):
+        """pulls the station catalogue as excel file """
+        downloaddir=self.cacheDir()
+        urif,upd=ftp("ftp://ftp.bafg.de/pub/REFERATE/GRDC/catalogue/grdc_stations.zip").download(downloaddir)
+        if upd:
+            with ZipFile(urif.url,'r') as zp:
+                    zp.extractall(downloaddir)
+
+        #also download the time series in the data directory
+    
+    def modify_df(self,df):
+        """Adds a geometry column TODO: converts day,month,year column to proper dates"""
+
+        #make a geometry column with points
+        df.altitude=df.altitude.replace(-999,0)
+        df['geom']=[WKTElement(wktdump(Point(lon,lat,h)),srid=4326,extended=True) for lon,lat,h in zip(df.long,df.lat,df.altitude)] 
+        
+
+        # gdf = gpd.GeoDataFrame(
+                    # df, geometry=gpd.points_from_xy(df.Longitude, df.Latitude))
+        
+        return df
+
+
 
-@as_declarative(metadata=MetaData(schema='altim'))
-class RadsTBase(object):
+@as_declarative(metadata=MetaData(schema=scheme))
+class grdcTBase(object):
     @declared_attr
     def __tablename__(cls):
         #strip of the 'Table' from the class name
-        return cls.__name__[:-5].lower()
-    id = Column(Integer, primary_key=True)
+        return cls.__name__[:-5].replace("-","_").lower()
+    id=Column(Integer,primary_key=True)
+    grdc_no=Column(Integer,unique=True)
     lastupdate=Column(TIMESTAMP)
     tstart=Column(TIMESTAMP,index=True)
     tend=Column(TIMESTAMP,index=True)
-    cycle=Column(Integer)
-    apass=Column(Integer)
-    uri=Column(String, unique=True,index=True)
-    data=Column(JSONB)
-    geom=Column(geotracktype)
-
-def is_set(x,n):
-    """Check if the nth bit of x is set to True"""
-    return x & 1 << n != 0
-
-def flag4_isonLand(x):
-    return is_set(x,4)
-
-def radsMetaDataExtractor(uri):
-    """Extract a dictionary with rads entries for the database"""
-    slurplogger().info("extracting data from %s"%(uri.url))
-    ncrads=ncDset(uri.url)
-    track=ogr.Geometry(ogr.wkbMultiLineString)
-    data={"segments":[]}
-   
-
-    if ncrads.dimensions['time'].size <3:
-       #no point trying to index empty files
-       return {}
-    #reference time 
-    t0=datetime(1985,1,1)
-    
-    # We need to compare some values fromt he previous loop which we store in the follwoing variables 
-    lonprev=ncrads["lon"][0]
-    if lonprev > 180:
-        lonprev-=360
-    
-    tprev=ncrads["time"][0]
-    onlandprev=flag4_isonLand(ncrads["flags"][0])
-   
-   #initiate first linestring segment 
-    trackseg=ogr.Geometry(ogr.wkbLineString)
-    #we also store some bookkeeping information on each track segment
-    segment={"tstart":(t0+timedelta(seconds=float(tprev))).isoformat(),"tend":None,"istart":0,"iend":0,"land":int(flag4_isonLand(ncrads["flags"][0]))}
-   
-    
-    for i,(t,lon,lat,flag) in enumerate(zip(ncrads["time"][:],ncrads["lon"][:],ncrads["lat"][:],ncrads['flags'][:])):
-        dt=t0+timedelta(seconds=float(t))
-        onland=flag4_isonLand(flag)
-        if lon > 180:
-            #make sure longitude goes from -180 to 180
-            lon-=360
-            #create a new segment when: (a) crossing the 180 d line, (b) a gap larger than 100 seconds is occurred, (c) or when ocean/land flag changes
-        if abs(lonprev-lon) > 180 or t-tprev > 100 or (onlandprev != onland):
-            #start a new segment upon crossing the 180 line or when a time gap occurredi, or when crossing from land to ocean or lake
-            #Segments which have more than a single point will be added:
-            if trackseg.GetPointCount() > 1:
-                #gather some end bookkeeping on the previous segment
-                segment["tend"]=dt.isoformat()
-                segment["iend"]=i
-   
-                #append segment and bookkeeping data
-                data["segments"].append(segment.copy())
-                # import pdb;pdb.set_trace()
-                track.AddGeometry(trackseg)
-            #initialize new segment
-            segment["tstart"]=dt.isoformat()
-            segment["istart"]=i
-            segment["land"]=int(onland)
-            trackseg=ogr.Geometry(ogr.wkbLineString)
-        
-        trackseg.AddPoint(float(lon),float(lat),0)
-        lonprev=lon
-        tprev=t
-        onlandprev=onland
-    
-    #also add the last segment
-    if trackseg.GetPointCount() > 1:
-        #gather some end bookkeeping on the previous segment
-        segment["tend"]=dt.isoformat()
-        segment["iend"]=i
-
-        #append segment and bookkeeping data
-        data["segments"].append(segment)
-        track.AddGeometry(trackseg)
-   
-    if not data["segments"]:
-       #return an empty dict when no segments are found
-       return {}
-
-    #reference time for rads
-    mtch=re.search("p([0-9]+)c([0-9]+).nc",uri.url)
-    meta={"lastupdate":uri.lastmod,
-          "tstart":t0+timedelta(seconds=float(ncrads['time'][0])),
-          "tend":t0+timedelta(seconds=float(ncrads['time'][-1])),
-          "cycle":int(mtch.group(2)),
-          "apass":int(mtch.group(1)),
-          "uri":uri.url,
-          "data":data,
-          "geom":WKBElement(track.ExportToIsoWkb(),srid=4326,extended=True)
-          }
+    area=Column(Float)
+    altitude=Column(Float)
+    river=Column(String)
+    statname=Column(String)
+    country=Column(String)
+    nextstation=Column(Integer)
+    uri=Column(String)
+    remarks=Column(String)
+    geom=Column(geoPointtype)
+
+def GRDCmetaExtractor(uri):
+    encoding='iso-8859-1'
+    meta={}
+    headerregex=re.compile(b"^#")
+    dataregex=re.compile(b"^[0-9]")
+    header={}
+    epoch=[]
+    slurplogger().info("Extracting meta info from: %s"%(uri.url))
+    with gzip.open(uri.url,'r') as gzid:
+        for ln in gzid:
+            if headerregex.search(ln):
+                #parse header
+                lnspl=ln[1:].split(b":",1)
+                if len(lnspl) == 2:
+                    ky=lnspl[0].lstrip(b" ").rstrip(b" ").decode(encoding)
+                    val=lnspl[1].lstrip(b" ").rstrip(b"\r\n ").decode(encoding)
+                    if not val:
+                        #get the nextline as a value
+                        val=gzid.readline()[1:].lstrip(b" ").rstrip(b"\r\n ").decode(encoding)
+                    header[ky]=val
+                continue
+            if dataregex.search(ln):
+                #parse data line
+                lnspl=ln.decode(encoding).split(";")
+                datestr=lnspl[0]+lnspl[1].replace("--:--",":00:00")
+                epoch.append(datetime.strptime(datestr, '%Y-%m-%d:%H:%S'))
+    
+    nextdownstream=header["Next downstream station"]
 
-    return meta
+    if "-" in nextdownstream:
+        nextdownstream=None
+    else:
+        nextdownstream=int(nextdownstream)
+    
+    area=float(header["Catchment area (km²)"])
+    if area == -999.0:
+        area=None
+
+    alt=float(header["Altitude (m ASL)"])
+    if alt == -999.0:
+        alt=None
+        location=Point(float(header["Longitude (DD)"]),float(header["Latitude (DD)"]),0)
+    else:
+        location=Point(float(header["Longitude (DD)"]),float(header["Latitude (DD)"]),alt)
+    # import pdb;pdb.set_trace()
+    try:
+        meta={"grdc_no":int(header["GRDC-No."]),
+                "tstart":epoch[0],
+                "tend":epoch[-1],
+                "lastupdate":datetime.strptime(header["Last update"],"%Y-%m-%d"),
+                "area":area,
+                "altitude":alt,
+                "river":header["River"],
+                "statname":header["Station"],
+                "country":header["Country"],
+                "nextstation":nextdownstream,
+                "uri":uri.url,
+                "geom":WKTElement(wktdump(location),srid=4326,extended=True)}
+                # "geom":WKBElement(wkbdump(location),srid=4326,extended=True)}
+    except KeyError as e:
+        import pdb;pdb.set_trace()
+        raise(e)
 
 
-class RadsBase(DataSet):
-    """Base class for a satellite + phase in the rads database
-    """
-    table=None
-    sat=None
-    phase=None
-    scheme='altim'
-    def __init__(self,dbconn):
-        super().__init__(dbconn)
-        self.updated=None
+    return meta
 
-        if not self._dbinvent.datadir:
-            if 'RADSDATAROOT' in os.environ:
-                self._dbinvent.datadir=getCreateDir(os.environ['RADSDATAROOT'])
-            else:
-                self._dbinvent.datadir=self.conf.getDataDir(self.scheme,subdirs="RADS")
-            self.updateInvent(False)
-        #initialize postgreslq table
-        self.table.__table__.create(self.db.dbeng,checkfirst=True)
-        # RadsTBase.metadata.tables[".".join([self.scheme.lower(),self.name])].create(self.db.dbeng,checkfirst=True)
-        # RadsTBase.metadata.create_all(self.db.dbeng, checkfirst=True)
-
-    def pull(self, cycle=None):
-        """Pulls the data from the rads server
-        :param cycle: only pulls data from a specific cycle
-        """
-        cred=self.conf.authCred("rads")
-
-        url="rads.tudelft.nl::rads/data"
-
-        #pull configuration data (xml files)
-        rsync(url+"/conf",auth=cred).parallelDownload(self._dbinvent.datadir,True)
-
-        srcurl=os.path.join(url,self.sat,self.phase)
-        desturl=os.path.join(self._dbinvent.datadir,self.sat)
-        if cycle:
-            srcurl=os.path.join(srcurl,"c%03d"%(cycle))
-            desturl=os.path.join(desturl,self.phase)
-        getCreateDir(desturl)
-        self.updated=rsync(srcurl,auth=cred).parallelDownload(desturl,True)
-
-    def register(self,cycle=None,since=None):
-        if since:
-           since=datetime.strptime(since,"%Y-%m-%d")
-           print(since)
-        else:
-           since=self._dbinvent.lastupdate
-        #create a list of files which need to be (re)registered
-        if self.updated:
-            files=self.updated
+class grdc_DSBase(DataSet):
+    """Holdings of the daily and monthly discharge files"""
+    """GRDC river discharge holdings"""
+    version=(0,0,0)
+    scheme=scheme
+    def __init__(self,dbcon):
+        super().__init__(dbcon)
+        if re.search("monthly",self.name):
+            self.zipname="DATA_MON.ZIP"
         else:
-            slurplogger().info("Listing files to process (this can take a while)...")
+            self.zipname="DATA_DAY.ZIP"
 
-            if cycle:
-                # import pdb; pdb.set_trace()
-                files=[UriFile(file) for file in findFiles(os.path.join(self._dbinvent.datadir,self.sat,self.phase,"c%03d"%(cycle)),'.*\.nc$',since=since)]
-            else:
-                files=[UriFile(file) for file in findFiles(os.path.join(self._dbinvent.datadir,self.sat,self.phase),'.*\.nc$',since=since)]
-        if not files:
-           slurplogger().info("No updated files found")
-           return
-
-        newfiles=self.retainnewUris(files)
-        if not newfiles:
-            slurplogger().info("Nothing to update")
+    def pull(self):
+        try:
+            cred=self.conf.authCred("grdcgis")
+        except:
+            raise RuntimeError("No Authentification data found. The GRDC data is unfortunately only available after agreeing with the grdc user policy, please visit https://www.bafg.de/GRDC/EN/04_spcldtbss/43_GRfN/refDataset_node.html") 
+        #pull the data but rezip it with gzip to save space 
+        pullGRDC(self.cacheDir(),cred,pattern=self.zipname,unzip=False)
+
+        datadir=self.dataDir()
+        #rezip data in the datadirectory
+        with ZipFile(os.path.join(self.cacheDir(),self.zipname),'r') as zp:
+            for member in zp.namelist():
+                #open file and gzip it into the datadir
+                with zp.open(member) as fid:
+                    slurplogger().info("re-gzipping file %s"%member)
+                    with gzip.open(os.path.join(datadir,member+".gz"),'wb') as gzid:
+                            gzid.write(fid.read())
+
+                     
+    def register(self):
+        slurplogger().info("Building file list..")
+        files=[UriFile(file) for file in findFiles(self.dataDir(),'.*gz',self._dbinvent.lastupdate)]
+        # import pdb;pdb.set_trace() 
+        filesnew=self.retainnewUris(files)
+        if len(filesnew) == 0:
+            slurplogger().info("GRDC: No database update needed")
             return
-
-        for uri in newfiles:
-            meta=radsMetaDataExtractor(uri)
-            if not meta:
-               #don't register empty entries
-               continue
-
+        # filesnew=[UriFile(os.path.join(self.dataDir(),"4208270_Q_Month.txt.gz"))]
+        #loop over files
+        for uri in filesnew:
+            meta=GRDCmetaExtractor(uri)
             self.addEntry(meta)
-
+        
         self.updateInvent()
 
 
+def GRDCClassFactory(clsName):
+    table=type(clsName +"Table", (grdcTBase,), {})
+    return type(clsName, (grdc_DSBase,), {"table":table})
 
+# Factory method to dynamically create classes
+def GRDCGISClassFactory(fileName):
+    splt=fileName.split(".")
+    return type(splt[0], (grdc_gis_base,), {"filename":fileName,"gtype":"GEOMETRY","swapxy":True})
 
 
+def getGRDCDsets(conf):
+    """Automatically create all classes contained within the GRDC tables"""
+    GISshapes=['GRDC_405_basins_from_mouth.shp','GRDC_687_rivers.shp','GRDC_687_rivers_class.shp','GRDC_lakes_join_rivers.shp','grdc_basins_smoothed.shp']
+    
+    out=[GRDCGISClassFactory(name) for name in GISshapes]
+    
+    #also add the monthly and daily  datasets
+    for name in ["grdc_monthly","grdc_daily"]:
+        out.append(GRDCClassFactory(name))
 
-# Factory method to dynamically create classes
-def radsclassFactory(clnm):
-    dum,sat,phase=clnm.split("_")
-    table=type(clnm+"Table",(RadsTBase,),{})
-    return type(clnm, (RadsBase,), {"sat":sat,"phase":phase,"table":table})
-
-def getRADSDsets(conf):
-    """Create all tables for all satellite missions and phases"""
-    satphases={"j1":["a","b","c"],"j2":["a","b","c"],"j3":["a"],"3a":["a"],"c2":["a"],"n1":["b","c"],"sa":["a","b"],"tx":["a","b","n"],"3a":["a"]}
-    out=[]
-    for sat,phases in satphases.items():
-        for  phase in phases:
-            clname="rads_"+sat+"_"+phase
-            out.append(radsclassFactory(clname))
     return out
 
-geoslurpCatalogue.addDatasetFactory(getRADSDsets)
+
+
+geoslurpCatalogue.addDatasetFactory(getGRDCDsets)
+geoslurpCatalogue.addDataset(grdc_catalogue)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/RasterBase.py` & `geoslurp-2.1.1/geoslurp/dataset/RasterBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,48 +15,50 @@
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
 
 
 from geoslurp.dataset.dataSetBase import DataSet
 from geoslurp.config.slurplogger import slurplogger
 from geoslurp.datapull.uri import findFiles, UriFile
+from geoslurp.config.slurplogger import slurplog
 from sqlalchemy import Column,Integer,String,Float
 from geoalchemy2 import Raster
 from sqlalchemy import func,select,text
 import rasterio as rio
 from rasterio.io import MemoryFile
 from rasterio.crs import CRS
+from affine import Affine
 import numpy as np
-
 class RasterBase(DataSet):
     """Base class to load raster (tiles) into the postgis database"""
-    srid=None #will try to find out the srid autmatically (but it's better to explicitly set this)
     srcdir=None
     rastregex=".*"
     auxcolumns=None
     outofdb=False
     regularblocking=False
     tiles=None
     srid=4326 #default but can be overruled
     bandname=None
     overviews=None
     #[ulx,xres,xskew,uly,yskew,yres]
-    geotransform=None
+    # geotransform=None
+    swapxy=False #transpose data (affine transformation)
     preview={} #creates a raster which is a preview of the complete rasterdataset only
     def __init__(self,dbcon):
         super().__init__(dbcon)
         if self.outofdb and not self.srcdir:
             #expects stuff in the datadirectory
             self.srcdir=self.dataDir()
         elif self.preview and not self.srcdir:
             self.srcdir=self.dataDir()
         elif not self.outofdb and not self.srcdir:
             #use the cacheDir
             self.srcdir=self.cacheDir()
-
+        if self.swapxy and self.outofdb:
+            slurplog.warning("Swapxy requested on an outofdb file:your rasters will likely be trasnposed")
 
     def columns(self):
         #construct the columns
         cols=[Column("id",Integer,primary_key=True),Column("uri",String),Column("add_offset",Float),Column("scale_factor",Float)]
         # possibly add auxiliary columns
         if self.auxcolumns:
             cols.extend(self.auxcolumns)
@@ -128,61 +130,95 @@
                 self._ses.execute(text("select ST_CreateOverview('%s.%s'::regclass, 'rast', %d, 'Lanczos')"%(self.scheme,self.name,factor)))
 
         self.updateInvent()
 
     def rastExtract(self,uri):
         """How things are extracted from the raster file (this may be overloaded in derived classes for more granular access"""
         slurplogger().info("Extracting info from raster: %s"%(uri.url))
+        #check file type
+        if uri.url.endswith(".nc"):
+            raw=False
+        else:
+            raw=True
+
+        if self.preview or not raw:
+            meta=self.rastFromRio(uri)
+        else:
+            meta=self.rastFromGDAL(uri)
+
+        return meta
+
+    def rastFromGDAL(self,uri):
+            #read the entire thing directly from gdal format
+            with open(uri.url,'rb') as fid:
+                fbytes=fid.read()
+                return {"rast":func.ST_FromGDALRaster(fbytes,srid=self.srid)}
+
+    def rastFromRio(self,uri):
+        
+        if uri.url.endswith(".nc"):
+            prefix="NETCDF:"
+        else:
+            prefix=""
         
         if self.preview:
-            bandnr=self.preview["bandnr"]
+            bandnrs=[self.preview["bandnr"]]
             bandname=self.preview["bandname"]
-            
-            #explicitly open the gdal file to get the bounding box info
-            if uri.url.endswith(".nc"):
-                prefix="NETCDF:"
-            else:
-                prefix=""
-
-            if bandname:
-                suffix=":"+bandname
-            else:
-                suffix=""
+        else:
+            bandnrs=None
+            bandname=self.bandname
+        
+        if bandname:
+            suffix=f":{bandname}"
+        else:
+            suffix=""
 
-            rdata=rio.open(prefix+uri.url+suffix)
+        #explicitly open the gdal file to get the bounding box info
+        rdata=rio.open(prefix+uri.url+suffix)
+        nodata=rdata.nodata
+        if self.swapxy:
+            nx=rdata.height
+            ny=rdata.width
+            transform=rdata.transform
+            transform=Affine(transform[4],transform[3],transform[5],transform[1],transform[0],transform[2])
+        else:
             nx=rdata.width
             ny=rdata.height
-            nodata=rdata.nodata
-            scale=rdata.scales[bandnr]
-            offset=rdata.offsets[bandnr]
             transform=rdata.transform
-            dtype=rdata.dtypes[bandnr]
 
-            if self.outofdb:
-                #create an out of db rasterband
-                ulx,uly,xres,yres,xskew,yskew=[transform[2],transform[5],transform[0],transform[4],transform[1],transform[3]]
-                emptyrast=func.ST_MakeEmptyRaster(nx,ny,ulx,uly,xres,yres,xskew,yskew,self.srid)
-                outdbfile=self.conf.get_PG_path(uri.url)
-                meta={"rast":func.ST_AddBand(emptyrast,prefix+outdbfile+suffix,[bandnr],0,nodata),
-                      "uri":uri.url,"add_offset":offset,"scale_factor":scale}
-            else:
-                with MemoryFile() as memfile:
-                    with memfile.open(driver='GTiff', count=1,
-                            width=nx,height=ny,
-                            dtype=dtype, nodata=nodata,
-                            crs=CRS.from_epsg(self.srid),transform=transform) as dataset:
-                        dataset.write(np.expand_dims(rdata.read(bandnr),0))
-                    
-                    meta={"rast":func.ST_FromGDALRaster(bytes(memfile.getbuffer()),srid=self.srid),
-                        "uri":uri.url,"add_offset":offset,"scale_factor":scale}
-        else:
-            if self.outofdb:
-                raise NotImplementedError("Can currently only work with outofdb previews, not entire bandsets")
-            
-            #read the entire thing directly from gdal format
-            with open(uri.url,'rb') as fid:
-                fbytes=fid.read()
-                meta={"rast":func.ST_FromGDALRaster(fbytes,srid=self.srid),"uri":uri.url}
+        if not bandnrs:
+            bandnrs=[nr+1 for nr in range(rdata.count)]
+        
+        #OK we're assuming these are the same for all requested bands
+        refband=bandnrs[0]-1
+        scale=rdata.scales[refband]
+        offset=rdata.offsets[refband]
+        dtype=rdata.dtypes[refband]
+
+        if self.outofdb:
+            #create an out of db rasterband
+            ulx,uly,xres,yres,xskew,yskew=[transform[2],transform[5],transform[0],transform[4],transform[1],transform[3]]
+            currentrast=func.ST_MakeEmptyRaster(nx,ny,ulx,uly,xres,yres,xskew,yskew,self.srid)
+            outdbfile=self.conf.get_PG_path(uri.url)
+            for i,bandn in enumerate(bandnrs):
+                currentrast=func.ST_AddBand(currentrast,prefix+outdbfile+suffix,[bandn],i+1,nodata)
 
+            meta={"rast":currentrast,"uri":uri.url,"add_offset":offset,"scale_factor":scale}
+        else:
+            #write to gdalformat and stuff the bytes in the raster 
+            with MemoryFile() as memfile:
+                with memfile.open(driver='GTiff', count=len(bandnrs),
+                        width=nx,height=ny,
+                        dtype=dtype, nodata=nodata,
+                        crs=CRS.from_epsg(self.srid),transform=transform) as dataset:
+                    
+                    for bandn in bandnrs:
+                        if self.swapxy:
+                            data=np.expand_dims(rdata.read(bandn).transpose(),0)
+                        else:
+                            data=np.expand_dims(rdata.read(bandn),0)
+                        dataset.write(data)
+                
+                meta={"rast":func.ST_FromGDALRaster(bytes(memfile.getbuffer()),srid=self.srid), "uri":uri.url,"add_offset":offset,"scale_factor":scale}
+        
         return meta
 
-
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/TUGRAZDsets.py` & `geoslurp-2.1.1/userplugins/TUGRAZDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/__init__.py` & `geoslurp-2.1.1/userplugins/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# NOTE: only list the files which contain actual registration calls for the datasets here
 from .naturalearth import *
 from .Argo import *
 from .GSHHGDsets import *
 from .PSMSL import *
 from .wribasin import *
 from .DuacsGriddedDsets import *
 from .GRACEDsets import *
@@ -11,16 +10,24 @@
 from .TUGRAZDsets import *
 from .RGIDsets import *
 from .geodesyunr import *
 from .deg1n2 import *
 from .orsiFronts import *
 from .ArcticDEM import *
 from .geoshapes import *
-from .snrei import *
+from .loadlove import *
 from .wgms_fog import *
 from .avisoRefOrbits import *
 from .mss_cnes_cls2015 import *
 from .IceSatDrainDiv import *
 from .Hydrosheds import *
 from .EasyCora import *
-# datasetgeneric should always be to last one to load(!)
-from .datasetgeneric import *
+from .gracefilters import *
+from .glofas import *
+from .sentinelreforbits import *
+from .FESOM import *
+from .grdc import *
+from .AWIPIES import *
+from .ORAS5 import *
+from .sebs import *
+from .gleam import *
+from .imerg import *
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/avisoRefOrbits.py` & `geoslurp-2.1.1/userplugins/avisoRefOrbits.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/dataSetBase.py` & `geoslurp-2.1.1/geoslurp/dataset/dataSetBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from abc import ABC, abstractmethod
 import os
 from geoslurp.config.slurplogger import slurplogger
 import shutil
 import re
 from geoslurp.db import Inventory,Settings
 from sqlalchemy.orm.exc import NoResultFound
-from datetime import datetime
+from datetime import datetime,timedelta
 from sqlalchemy import Table,Column,Integer,String
 from sqlalchemy.dialects.postgresql import TIMESTAMP
 from geoslurp.datapull import UriFile
 from sqlalchemy import and_
 from geoslurp.db.settings import getCreateDir
 from geoslurp.db import tableMapFactory
 
@@ -100,24 +100,35 @@
 
     def updateInvent(self,updateTime=True):
         if updateTime:
             self._dbinvent.lastupdate=datetime.now()
         self._dbinvent.updatefreq=self.updatefreq
         
         #see if there are custom columns defined inthe table
-        for col in self.table.__table__.columns:
-            if re.search('geoslurp\.types\.',str(col.type.__class__)):
-                if not "customcolumns" in self._dbinvent.data:
-                    self._dbinvent.data["customcolumns"]={}
-                self._dbinvent.data["customcolumns"][col.name]={"type":col.type.__repr__(),"class":str(col.type.__class__)}
+        if self.table:
+            for col in self.table.__table__.columns:
+                if re.search('geoslurp\.types\.',str(col.type.__class__)):
+                    if not "customcolumns" in self._dbinvent.data:
+                        self._dbinvent.data["customcolumns"]={}
+                    self._dbinvent.data["customcolumns"][col.name]={"type":col.type.__repr__(),"class":str(col.type.__class__)}
 
         self._ses.commit()
 
-    def info(self):
-        return self._dbinvent
+    # def info(self):
+        # return self._dbinvent
+
+    def isExpired(self):
+        """Checks whether the table data is expired relative to to the updatefrequency"""
+        if not self._dbinvent.updatefreq:
+            #ten years if not specified
+            updatefreq=timedelta(days=10*365)
+        else:
+            updatefreq=timedelta(days=self._dbinvent.updatefreq)
+
+        return (self._dbinvent.lastupdate + updatefreq ) < datetime.today()
 
     def dataDir(self,subdirs=None):
         """Returns the specialized data directory of this scheme and dataset
         The directory will be created if it does not exist"""
         
         if self._dbinvent.datadir:
             return getCreateDir(self._dbinvent.datadir)
@@ -128,17 +139,17 @@
         self._dbinvent.datadir=ddir
         self.updateInvent(False)
 
     def cacheDir(self,subdirs=None):
         """returns the cache directory of this scheme and dataset"""
         if self._dbinvent.cache:
             if subdirs:
-                return getCreateDir(os.path.join(self._dbinvent.cache,subdirs),self.conf.mirrorMap)
+                return getCreateDir(os.path.join(self._dbinvent.cache,subdirs))
             else:
-                return getCreateDir(self._dbinvent.cache,self.conf.mirrorMap)
+                return getCreateDir(self._dbinvent.cache)
 
         return self.conf.getCacheDir(self.scheme, dataset=self.name,subdirs=subdirs)
     
     def setCacheDir(self,cdir):
         self._dbinvent.cache=cdir
         self.updateInvent(False)
 
@@ -202,46 +213,47 @@
         """Filters those uris which have table entries which are too old or are not present in the database"""
         #create a temporary table with uri and lastmodification time entries
         cols=[Column('id', Integer, primary_key=True),Column('uri',String),Column('lastmod',TIMESTAMP)]
 
         #setup a seperate session  and transaction in order to work with a temporary table
         trans,ses=self.db.transsession()
         
-        tmptable=self.db.createTable('tmpuris',cols,temporary=True,bind=ses.get_bind())
+        tmptable=self.db.createTable('tmpuris',cols,temporary=False,bind=ses.get_bind())
         # tmptable=self.db.createTable('tmpuris',cols,temporary=False,bind=ses.get_bind())
         # import pdb;pdb.set_trace()
         #fill the table with the file list and last modification timsstamps
         count=0
         for uri in urilist:
-            url=self.conf.generalize_path(uri.url)
+            if self.stripuri:
+                url=self.conf.generalize_path(uri.url)
+            else:
+                url=uri.url
+
             entry=tmptable(uri=url,lastmod=uri.lastmod)
             ses.add(entry)
             count+=1
             if count > self.commitperN:
                 ses.commit()
                 count=0
 
         ses.commit()
-
         #delete all entries which require updating
         # first gather all the ids of i entries which are expired 
         subqry=ses.query(self.table.id).join(tmptable, and_(tmptable.uri == self.table.uri,tmptable.lastmod > self.table.lastupdate)).subquery()
         # #then delete those entries from the table
-        # import pdb;pdb.set_trace()
-        
         delqry=self.table.__table__.delete().where(self.table.id.in_(subqry))
         ses.execute(delqry)
-
-
+        ses.commit()
         #now make a list of new uris
         qrynew=ses.query(tmptable).outerjoin(self.table,self.table.uri == tmptable.uri).filter(self.table.uri == None)
 
         #submit transaction
         trans.commit()
 
+        # import pdb;pdb.set_trace()
         #return entried which need updating he entries in the original table which need updating
         return [UriFile(self.conf.get_local_path(x.uri),x.lastmod) for x in qrynew]
 
 
     def entryNeedsUpdate(self,likestr,lastmod,col=None):
         """Query for a Columns in the table based on a alike string and delete the entry when older than lastmod"""
         needsupdate=True
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/datasetgeneric.py` & `geoslurp-2.1.1/geoslurp/dataset/datasetgeneric.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,17 @@
 # License along with Frommle; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (r.rietbroek@utwente.nl), 2021
 
 from geoslurp.dataset.dataSetBase import DataSet
 
-from geoslurp.config.catalogue import geoslurpCatalogue
-
 class DataSetGeneric(DataSet):
     scheme="anyscheme"
     def __init__(self,dbcon):
         super().__init__(dbcon)
 
     def pull(self):
         raise NotImplementedError("No pull method defined for a generic dataset")
     def register(self):
         raise NotImplementedError("No register method defined for a generic dataset")
 
-
-geoslurpCatalogue.addDataset(DataSetGeneric)
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/deg1n2.py` & `geoslurp-2.1.1/userplugins/deg1n2.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,18 @@
                     cnmv.append(float(snm))
                     sigcnmv.append(float(sigsnm))
 
                 if m == 1: 
                     #register the accumulated entry
                     tstart=parseGSMDate(ts)
                     tend=parseGSMDate(te)
-                    #snap the central epoch to the 15th of the month
-                    tcent=datetime(tstart.year,tstart.month,15)
+                    #get the central time
+                    tcent=tstart+(tend-tstart)/2
+                    #snap the central epoch to the 15th of the month of the central time
+                    # tcent=datetime(tstart.year,tstart.month,15)
                 
                     meta={"type":"GSM","time":tcent,"tstart":tstart,"tend":tend,"lastupdate":lastupdate,"nmax":1,"omax":1,"origin":"CF","format":"JSONB","gm":0.3986004415e+15,"re":0.6378136460e+07}
                     meta["data"]=xr.Dataset(data_vars=dict(cnm=(["shg"],cnmv),sigcnm=(["shg"],sigcnmv)),coords=dict(n=(["shg"],nv),m=(["shg"],mv),t=(["shg"],tv)))
                     
                     self.addEntry(meta)
                     nv=[]
                     mv=[]
@@ -277,37 +279,40 @@
                 
                 mjd0,decy0,c20,dc20,sigc20,c30,dc30,sigc30,mjd1,decyr1=ln.split()
                 
                 nv=[]
                 mv=[]
                 tv=[]
                 cnmv=[]
+                dcnmv=[]
                 sigcnmv=[]
                 
                 #Append c20 coefficients
                 nv.append(2)
                 mv.append(0)
                 tv.append(0)
                 cnmv.append(float(c20))
+                dcnmv.append(float(dc20)*1e-10)
                 sigcnmv.append(float(sigc20))
                 if c30 != "NaN":
                     nmax=3
                     nv.append(3)
                     mv.append(0)
                     tv.append(0)
                     cnmv.append(float(c30))
+                    dcnmv.append(float(dc30)*1e-10)
                     sigcnmv.append(float(sigc30))
 
                 #register the accumulated entry
                 tstart=mjd00+timedelta(days=float(mjd0))
                 tend=mjd00+timedelta(days=float(mjd1))
                 tcent=tstart+(tend-tstart)/2
             
                 meta={"type":"GSM","time":tcent,"tstart":tstart,"tend":tend,"lastupdate":lastupdate,"nmax":nmax,"omax":omax,"format":"JSONB","gm":0.3986004415e+15,"re":0.6378136460e+07}
-                meta["data"]=xr.Dataset(data_vars=dict(cnm=(["shg"],cnmv),sigcnm=(["shg"],sigcnmv)),coords=dict(n=(["shg"],nv),m=(["shg"],mv),t=(["shg"],tv)))
+                meta["data"]=xr.Dataset(data_vars=dict(cnm=(["shg"],cnmv),dcnm=(["shg"],dcnmv),sigcnm=(["shg"],sigcnmv)),coords=dict(n=(["shg"],nv),m=(["shg"],mv),t=(["shg"],tv)))
                 
                 self.addEntry(meta)
             self.updateInvent()
 
 
 geoslurpCatalogue.addDataset(TN14_SLR_GSFC)
 # class Sun2017Comb(LowdegreeSource):
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/era5.py` & `geoslurp-2.1.1/geoslurp/dataset/cdsbase.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,103 +15,125 @@
 
 # Author Roelof Rietbroek (r.rietbroek@utwente.nl), 2021
 
 
 from sqlalchemy import Column, Integer, String, DateTime,JSON
 from geoslurp.dataset import DataSet
 from geoslurp.datapull import findFiles, UriFile
+from geoslurp.datapull.cds import Cds
 from geoslurp.config.slurplogger import slurplogger
-import cdsapi
 import os
 import numpy as np
 from geoalchemy2 import Geography
 from shapely.geometry import Polygon
 from shapely.wkt import dumps as wktdumps
 from netCDF4 import Dataset as ncDset
 from netCDF4 import num2date
+import time
 
 envelopType = Geography(geometry_type="POLYGON", srid='4326')
 
-def ERA5MetaExtractor(ncuri):
-    name=os.path.basename(ncuri.url).split('_')[-1][0:-3]
-    ncid=ncDset(ncuri.url)
-    data={"dimensions":{ky:val.size for ky,val in ncid.dimensions.items()},
-            "variables":{ky:{"long_name":val.long_name,"dimensions":val.dimensions} for ky,val in ncid.variables.items()}}
-    tstart=num2date(ncid["time"][0],units=ncid['time'].units,only_use_cftime_datetimes=False)
-    tend=num2date(ncid["time"][-1],units=ncid['time'].units,only_use_cftime_datetimes=False)
-    latmin=np.min(ncid["latitude"])
-    latmax=np.max(ncid["latitude"])
-    lonmin=np.min(ncid["longitude"])
-    lonmax=np.max(ncid["longitude"])
-    bbox=Polygon([(lonmin,latmin),(lonmin,latmax),(lonmax,latmax),(lonmax,latmin)])
-    return {"name":name,"lastupdate":ncuri.lastmod,"tstart":tstart,"tend":tend,"uri":ncuri.url,"data":data,
-            "geom":wktdumps(bbox)}
-
-class ERA5Base(DataSet):
-    """Provides a Base class from which subclasses can inherit to download a subset of the data per area"""
-    scheme="atmo"
-    dset='reanalysis-era5-pressure-levels-monthly-means'
-    productType='monthly_averaged_reanalysis'
-    yrstart=2000
-    yrend=2000
-    variables={}
-    time="00:00"
+class CDSBase(DataSet):
+    """Provides a Base class from which subclasses can inherit to download CDS hosted data"""
+    scheme="cds" 
+    # The following need to be set in hte derived class
+    resource=None
+    productType=None
+    variables=[]
+    #may be overruled in derived classes
     columns=[Column('id',Integer,primary_key=True),Column("name",String,unique=True),
             Column("lastupdate",DateTime),Column("tstart",DateTime),Column("tend",DateTime),
             Column("uri", String),Column("data",JSON),Column("geom",envelopType)]
-
+    
+    #entries of the form {name:jsondict,..}
+    reqdicts={}
+    oformat='netcdf'
+    description="CDS subset downloaded from cds.climate.copernicus.eu"
+    res=0.0 # resolution of the pixels in the grid (used for adding a margin around the downloaded area when not 0)
     def __init__(self,dbconn):
         super().__init__(dbconn)
-        self.areas_nwse={}
+        if not "cds_jobs" in self._dbinvent.data:
+            self._dbinvent.data["cds_jobs"]={}
+    
+        if self.oformat == 'netcdf':
+            self.app=".nc"
+        elif self.oformat == 'grib':
+            self.app=".grb"
+        elif self.oformat =='tgz':
+            self.app=".tgz"
+
+    def metaExtractor(self,uri):
+        """implement this function in derived class"""
+        raise NotImplementedError("MetaExtractor(self,uri) not implemented")
+        return {}
 
-    def appendRequest(self,name,area):
-        bb=area.envelope.exterior.xy
+    def pull(self,maxreq=100):
+        dout=self.dataDir()
+        
+        cdsQueue=Cds(self.resource,self._dbinvent.data["cds_jobs"])
+        #add requests to the CDS queue
+        #Not it is expected that the derived class adds these requestdictionaries in one way or the other (default will be empty)
+        
+        #only submit maxreq at once
+        nreq=0
+        for name,reqdict in self.reqdicts.items():
+
+            fout=os.path.join(dout,self.resource+"_"+name+self.app)
+            cdsQueue.queueRequest(fout,reqdict)
+            nreq+=1
+            if nreq > maxreq:
+                #do an intermediate download before submitting more requests
+                #Sync the possibly updated queueinfo to the database
+                self._dbinvent.data["cds_jobs"]=cdsQueue.jobqueue
+                self._ses.commit()
         
-        self.areas_nwse[name]=[np.max(bb[1]),np.min(bb[0]),np.min(bb[1]),np.max(bb[0])]
+                #wait for tasks to finish and download results to files
+                cdsQueue.downloadQueue()
+                cdsQueue.clearRequests()
+                nreq=0
+
+        #download outstanding jobs
+        self._dbinvent.data["cds_jobs"]=cdsQueue.jobqueue
+        self._ses.commit()
 
-    def pull(self):
+        #wait for tasks to finish and download results to files
+        cdsQueue.downloadQueue()
 
-        if not os.path.exists(os.path.join(os.path.expanduser("~"),".cdsapirc")):
-            raise RuntimeError("Before using the cdsapi please visit https://cds.climate.copernicus.eu/api-how-to to obtain a token and setup your ~/.cdsapirc file")
-        dout=self.dataDir()
-        #start a client
-        c = cdsapi.Client()
-        for name,area in self.areas_nwse.items():
-            fout=os.path.join(dout,self.dset+"_"+name+".nc")
-            if os.path.exists(fout):
-                slurplogger().info(f"Already downloaded ERA5 data for area {name}")
-                continue
-            requestdict=self.getRequestDict(area)
-            slurplogger().info(f"Downloading ERA5 for {name}")
-            c.retrieve(self.dset,requestdict,fout)
-
-    def getRequestDict(self,area):
-        """Builds a dictionary for the cdsapi
-        :param area (shapely geometry) geometry which will be used to compute the bounding box to download data for"""
-        reqdict={
-                'format': 'netcdf',
-                'product_type': self.productType,
-                'variable': self.variables,
-                'pressure_level':self.plevels,
-                'year': [f"{yr}" for yr in range(self.yrstart,self.yrend+1)],
-                'month':[f"{mn:02d}" for mn in range(1,13)],
-                'time': self.time,
-                'area': area}
-        return reqdict
+        cdsQueue.clearRequests()
 
     def register(self):
         if not self.table:
             #create a new table on the fly
             self.createTable(self.columns)
+        
         #create a list of files which need to be (re)registered
-        newfiles=self.retainnewUris([UriFile(file) for file in findFiles(self.dataDir(),".*\.nc$")])
+        newfiles=self.retainnewUris([UriFile(file) for file in findFiles(self.dataDir(),f".*\{self.app}$")])
         for uri in newfiles:
-            meta=ERA5MetaExtractor(uri)
+            meta=self.metaExtractor(uri)
             if not meta:
                 #don't register empty entries
                 continue
+            slurplogger().info(f"Adding metadata from {uri.url}")
             self.addEntry(meta)
-        self._dbinvent.data["Description"]="ERA5 subset downloaded from cds.climate.copernicus.eu"
+        self._dbinvent.data["Description"]=self.description
         self.updateInvent()
 
+    def getDefaultDict(self,geomshape=None):
+        #return a default cdsapi dictionary with common parameters
+        
+        reqdict={
+                'format': self.oformat,
+                'variable': self.variables,
+                }
+        
+        if self.productType:
+            reqdict["product_type"]=self.productType
+
+        if geomshape:
+            bb=geomshape.envelope.exterior.xy
+            hres=self.res/2
+            if np.min(bb[0]) > 180 or np.min(bb[0]) < 0:
+                breakpoint()
+            reqdict["area"]=[np.max(bb[1])+hres,np.min(bb[0])-hres,np.min(bb[1])-hres,np.max(bb[0])+hres]
+        return reqdict
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/geodesyunr.py` & `geoslurp-2.1.1/userplugins/geodesyunr.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/geoshapes.py` & `geoslurp-2.1.1/userplugins/geoshapes.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/icgemDsets.py` & `geoslurp-2.1.1/userplugins/icgemDsets.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
 # provides a dataset and table for static gravity fields from the icgem website
 
 
 
-from geoslurp.dataset import DataSet,GravitySHTBase
+from geoslurp.dataset import DataSet
+from geoslurp.tools.gravity import GravitySHTBase
 from geoslurp.datapull.icgem import  Crawler as IcgemCrawler
 from geoslurp.datapull.uri import findFiles
 import re
 import gzip as gz
 from geoslurp.config.slurplogger import slurplogger
 from glob import glob
 from geoslurp.datapull import UriFile
@@ -37,14 +38,15 @@
     scheme='gravity'
     stripuri=True
     def __init__(self, dbconn):
         super().__init__(dbconn)
         #initialize postgreslq table
         GravitySHTBase.metadata.create_all(self.db.dbeng, checkfirst=True)
         self.updated=[]
+    
     def pull(self,pattern=None,list=False):
         """Pulls static gravity fields from the icgem website
         :param pattern: only download files whose name obeys this regular expression
         :param list (bool): only list available models"""
         self.updated=[]
         crwl=IcgemCrawler()
         if pattern:
@@ -61,14 +63,17 @@
                 print("%-12s %5d %4d"%(uri.name,uri.nmax,uri.lastmod.year))
             else:
                 tmp,upd=uri.download(outdir,check=True, gzip=True)
                 if upd:
                     self.updated.append(tmp)
 
     def register(self,pattern=None):
+        """Register static gravity fields donwloaded in the data director
+        :param pattern: only register files whose filename obeys this regular expression
+        """
         if not pattern:
             pattern='.*\.gz'
         #create a list of files which need to be (re)registered
         if self.updated:
             files=self.updated
         else:
             files=[UriFile(file) for file in findFiles(self.dataDir(),pattern)]
@@ -77,15 +82,14 @@
         for uri in files:
             urilike=os.path.basename(uri.url)
 
             if not self.uriNeedsUpdate(urilike,uri.lastmod):
                 continue
 
             meta=icgemMetaExtractor(uri)
-
             self.addEntry(meta)
 
         self.updateInvent()
 
 
 geoslurpCatalogue.addDataset(ICGEM_static)
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/motuGridsBase.py` & `geoslurp-2.1.1/geoslurp/dataset/motuGridsBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
 
 from geoslurp.dataset import DataSet
 from geoslurp.datapull.motu import Uri as MotuUri
 from geoslurp.datapull.motu import MotuOpts, MotuRecursive
 from geoslurp.tools.Bounds import BtdBox
 from geoslurp.tools.netcdftools import ncSwapLongitude,stackNcFiles
-from geoslurp.config.catalogue import geoslurpCatalogue
 
 import os
 from geoalchemy2.types import Geography
 from sqlalchemy import Column,Integer,String, Boolean,ARRAY
 from sqlalchemy.dialects.postgresql import TIMESTAMP, JSONB
 from sqlalchemy import MetaData
 from sqlalchemy.ext.declarative import declarative_base
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/mss_cnes_cls2015.py` & `geoslurp-2.1.1/userplugins/mss_cnes_cls2015.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/naturalearth.py` & `geoslurp-2.1.1/userplugins/naturalearth.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/orsiFronts.py` & `geoslurp-2.1.1/userplugins/orsiFronts.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/pandasbase.py` & `geoslurp-2.1.1/geoslurp/dataset/pandasbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from geoalchemy2.types import Geography,Raster
 from geoalchemy2.elements import WKBElement,RasterElement
 import shapely.wkb
 from sqlalchemy import func
 import numpy as np
 from collections import namedtuple
 from geoslurp.types.zarr import OutDBZarrType
+from geoslurp.types.numpy import datetime64Type
 import xarray as xr
 import os
 from datetime import datetime
 #geoinfo=namedtuple("geoinfo",["srid","geoname","geomtype","dims","rastname"],defaults=(4326,"geom","GEOMETRY",2,"rast",))
 #make compatible with 3.6
 geoinfo=namedtuple("geoinfo",["srid","geoname","geomtype","dims","rastname"])
 geoinfo.__new__.__defaults__=(4326,"geom","GEOMETRY",2,"rast",)
@@ -41,14 +42,16 @@
     """Base class which reads in a pandas compatible table (CSV, excel, or in memory dataframe are currently supported) it in a db table"""
     pdfile=None
     skipfooter=0
     ftype="csv"
     encoding=None
     geoinfo=geoinfo()
     inbulk=False
+    #how to treat series which have xarray dataarrays or datasets
+    xrappend_dim=None
     def __init__(self,dbconn):
         super().__init__(dbconn)
     
 
     def setGeoInfo(self,df):
         """Try to extract srid, geometry type from a geopandas geodataframe"""
 
@@ -80,18 +83,20 @@
         """Returns a list of columns from a dataframe)"""
         Map = {str: String, np.dtype(int): Integer, 
                 np.dtype(float):Float,dict:JSON,
                 np.int64:BIGINT,
                 float:Float,np.float64:Float,
                 "string": String, "integer": Integer, 
                 "floating":Float,
-                xr.DataArray:OutDBZarrType(defaultZstore=self.outdbArchiveName()),
-                "datetime64":DateTime}
+                xr.DataArray:OutDBZarrType(defaultZstore=self.outdbArchiveName(),modifyUri=self.conf.generalize_path,append_dim=self.xrappend_dim),
+                xr.Dataset:OutDBZarrType(defaultZstore=self.outdbArchiveName(),modifyUri=self.conf.generalize_path,append_dim=self.xrappend_dim),
+                "datetime64":DateTime,
+                np.dtype('<M8[ns]'):datetime64Type}
         cols = [Column('id', Integer, primary_key=True)]
-        
+         
         for name,col in df.iteritems():
             if name == "id":
                 #already added
                 continue
             
             elif name == self.geoinfo.rastname:
                 cType=Raster(spatial_index=False)
@@ -170,8 +175,12 @@
 
     def pull(self):
         """overload when needed"""
         pass
 
 
     def outdbArchiveName(self):
-        return os.path.join(self.dataDir(),self.name+"_data.zarr")
+        # if self.stripuri:
+            # arname=self.conf.generalize_path(os.path.join(self.dataDir(),self.name+"_data.zarr"))
+        # else:
+        arname=os.path.join(self.dataDir(),self.name+"_data.zarr")
+        return arname
```

### Comparing `geoslurp-2.0.0/geoslurp/dataset/wgms_fog.py` & `geoslurp-2.1.1/userplugins/wgms_fog.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dataset/wribasin.py` & `geoslurp-2.1.1/userplugins/wribasin.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # You should have received a copy of the GNU Lesser General Public
 # License along with Frommle; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
 
-from geoslurp.dataset import OGRBase
+from geoslurp.dataset.OGRBase import OGRBase
 from geoslurp.datapull.http import Uri as http
 from geoslurp.config.catalogue import geoslurpCatalogue
 import urllib.request
 from zipfile import ZipFile
 import os
 
 class WriBasin(OGRBase):
```

### Comparing `geoslurp-2.0.0/geoslurp/db/connector.py` & `geoslurp-2.1.1/geoslurp/db/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 
 # You should have received a copy of the GNU Lesser General Public
 # License along with Frommle; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2018
 
-from sqlalchemy import create_engine, MetaData,and_
+from sqlalchemy import create_engine, MetaData,and_,inspect
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.sql import exists,select,column,table,text
 from sqlalchemy.schema import CreateSchema, DropSchema
 from sqlalchemy import Table,func
 from geoslurp.db.tabletools import tableMapFactory
 import re
 from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
 from geoslurp.config.slurplogger import  slurplogger, debugging
 import getpass
 from geoslurp.db.connectorbase import GeoslurpConnectorBase
 
 class GeoslurpConnector(GeoslurpConnectorBase):
     """Holds a connector to a geoslurp database"""
-    def __init__(self, host, user, passwd=None, port=5432,dataroot=None,cache=None):
+    def __init__(self, host, user, passwd=None, port=5432,dataroot=None,cache=None,plugindir=None):
         """
         establishes a database engine whoch provides the base
         for creating sessions (ORM) or connections (SQL expressions)
         :param dburl: url of the database e.g.: postgresql+psycopg2://geoslurp:password@host/geoslurp
         """
-        super().__init__(dataroot=dataroot,cache=cache)
+        super().__init__(dataroot=dataroot,cache=cache,plugindir=plugindir)
 
 
         self.user=user
         if passwd:
             self.passw=passwd
         else:
             self.passw=getpass.getpass(prompt='Please enter password for %s: '%(user))
@@ -122,16 +122,19 @@
 
     def dropTable(self, tablename, schema=None):
         if schema:
             self.dbeng.execute('DROP TABLE IF EXISTS %s."%s";' % (schema.lower(), tablename.lower()))
         else:
             self.dbeng.execute('DROP TABLE IF EXISTS "%s";' % (tablename.lower()))
     
-    def hasTable(self,tablename):
-        return self.dbeng.has_table(tablename)
+    def tableExists(self,tablename):
+        insp=inspect(self.dbeng)
+        sch,tbl=tablename.split(".")
+        return insp.has_table(tbl,sch)
+
 
     def getTable(self,tname,scheme="public",customcolumns=None):
         mdata=MetaData(bind=self.dbeng,schema=scheme)
         if customcolumns:
             return Table(tname, mdata, *customcolumns,autoload=True, autoload_with=self.dbeng)
         else:
             return Table(tname, mdata, autoload=True, autoload_with=self.dbeng)
```

### Comparing `geoslurp-2.0.0/geoslurp/db/connectorbase.py` & `geoslurp-2.1.1/geoslurp/db/connectorbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,32 @@
     fname=inspect.stack()[1].function
     raise NotImplementedError(f"Sorry {fname} is not (yet) implemented for this database type")
 
 class GeoslurpConnectorBase():
     """Holds the base class for a connector to a geoslurp database"""
     cache=None
     localdataroot=None
-    def __init__(self,cache=None,dataroot=None):
+    plugindir=None
+    def __init__(self,cache=None,dataroot=None,plugindir=None):
         """
         Sets the variables which all connectors have in common"""
 
         if dataroot:
             self.localdataroot=dataroot
         else:
             self.localdataroot=os.path.join(os.path.expanduser('~'),'geoslurp_data')
+        
         if cache:
             self.cache=cache
         else:
             #default when not specified
             self.cache="/tmp/geoslurp_cache"
+        
+        if plugindir:
+            self.plugindir=plugindir
 
 
     def transsession(self):
         raiseNotImpl()
     
     def vacuumAnalyze(self, tableName, schema):
         """vacuum and analyze a certain table"""
```

### Comparing `geoslurp-2.0.0/geoslurp/db/exporter.py` & `geoslurp-2.1.1/geoslurp/db/exporter.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/db/geoslurpdb.py` & `geoslurp-2.1.1/geoslurp/db/geoslurpdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,30 @@
 # License along with geoslurp; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
 from geoslurp.config.localsettings import readLocalSettings,settingsArgs
 from geoslurp.db.connector import GeoslurpConnector
 
-def geoslurpConnect(args=None,readonly_user=True,update=False,local_settings=None,dbalias=None):
+
+def geoslurpConnect(args=None,readonly_user=True,update=False,local_settings=None,dbalias=None,plugindir=None):
     """Convenience wrapper to start a connection with a geoslurpdatabase. Returns a database connection while taking use of stored settings from the users 
     configuration file ($HOME/.geoslurp_lastused.yaml).
     :param args: Class which encapsulates different connection parameters
     :type args: geoslurp.localsettings.settingsArgs"""
    
     if not args:
         args=settingsArgs()
 
     if local_settings:
         args.local_settings=local_settings
 
     if dbalias:
         args.dbalias=dbalias
+    
+    if plugindir:
+        args.plugindir=plugindir
 
     userSettings=readLocalSettings(args=args,readonlyuser=readonly_user)
-    return GeoslurpConnector(host=userSettings.host,user=userSettings.user,passwd=userSettings.password,cache=userSettings.cache,dataroot=userSettings.dataroot)
+    return GeoslurpConnector(host=userSettings.host,user=userSettings.user,passwd=userSettings.password,
+            cache=userSettings.cache,dataroot=userSettings.dataroot,
+            plugindir=userSettings.plugindir)
```

### Comparing `geoslurp-2.0.0/geoslurp/db/inventory.py` & `geoslurp-2.1.1/geoslurp/db/inventory.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/db/settings.py` & `geoslurp-2.1.1/geoslurp/db/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,27 +52,30 @@
     for serv,dsub in d.items():
         # print(serv)
         for ky,v in dsub.items():
             if ky == "passw" or ky == "oauthtoken":
                 d[serv][ky]="*****"
     return d
 
-Credentials=namedtuple("Credentials","user passw alias oauthtoken url")
+Credentials=namedtuple("Credentials","user passw alias oauthtoken url ftptls trusted")
 """A named tuple to store authentication credentials
 
 Attributes:
     user (str): Username for the service
     alias (str): (obligatory) The short name of this service
     passw (str): The password associated with the username
     oauthtoken (str): An oauth2 token
     url (str): The root url which is linked to this service
+    ftptls(bool): Use Explicit ftp over tls for this host and user
+    trusted(bool): Allow forwarding password and username
 """
 
 Credentials.__new__.__defaults__ = (None,) * len(Credentials._fields)
 
+commonCredentials={"podaac":["user","passw","trusted"]}
 
 
 
 
 
 
 GSBase=declarative_base(metadata=MetaData(schema='admin'))
@@ -162,21 +165,27 @@
         print(self.userentry.conf)
         #also shows the registered authentification services (but don't show passwords
         if hideflag == "nohide":
             print(self.auth)
         else:
             print(stripPasswords(self.auth))
 
-    def authCred(self,service,qryfields=["user","passw"]):
+    def authCred(self,service,qryfields=None):
         """obtains username credentials for a certain service
         :param service: name of the service
+        :param qryfields: prompt for input for these fields when service is not present
         :returns a namedtuple with credentials"""
 
         if service not in self.auth:
             #prompt for the necessary fields and store in database
+            if qryfields is not None and service in commonCredentials:
+                qryfields=commonCredentials[service]
+            else:
+                qryfields=["user","passw"]
+
             creddict={"alias":service}
             for key in qryfields:
                 if key == "passw":
                     val=getpass.getpass(prompt='Please enter passw for authentication service %s\n'%service)
                 else:
                     val=input('Please enter %s for authentication service %s\n'%(key,service))
                 creddict[key]=val
```

### Comparing `geoslurp-2.0.0/geoslurp/db/tabletools.py` & `geoslurp-2.1.1/geoslurp/db/tabletools.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dbfunc/dbfunc.py` & `geoslurp-2.1.1/geoslurp/dbfunc/dbfunc.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,16 +70,26 @@
         """Delete pgfunction entry in the database"""
         slurplogger().info("Deleting %s function entry"%(self.name))
         self._ses.delete(self._dbinvent)
         self._ses.commit()
         
         dropexec=text("DROP FUNCTION IF EXISTS %s.%s;"%(self.scheme,self.name))
         self.db.dbeng.execute(dropexec) 
-    
     def register(self):
-        """Creates/replaces the  pgfunction in the database"""
-        pgheader="CREATE OR REPLACE FUNCTION %s(%s) RETURNS %s AS $dbff$\n"%(self.name,self.inargs,self.outargs)
-        pgbody=self.pgbody
+        #iterate over overloaded functions
+        if type(self.inargs) == list and type(self.pgbody) == list:
+            #iterate over mutile function overloads
+            for inargs,pgbody in zip(self.inargs,self.pgbody):
+                self.register_overload(inargs,pgbody)
+        else:
+                self.register_overload(self.inargs,self.pgbody)
+
+        self.updateInvent()
+    
+
+    def register_overload(self,inargs,pgbody):
+        """Creates/replaces the (overloaded) pgfunction in the database"""
+        slurplogger().info("Registering (overload) of %s function"%(self.name))
+        pgheader="CREATE OR REPLACE FUNCTION %s(%s) RETURNS %s AS $dbff$\n"%(self.name,inargs,self.outargs)
         pgfooter=";\n$dbff$ LANGUAGE %s;"%(self.language)
-        print(str(pgheader+pgbody+pgfooter))
+        # print(str(pgheader+pgbody+pgfooter))
         self.db.dbeng.execute(text(pgheader+pgbody+pgfooter)) 
-        self.updateInvent()
```

### Comparing `geoslurp-2.0.0/geoslurp/dbfunc/radsfuncs.py` & `geoslurp-2.1.1/geoslurp/dbfunc/radsfuncs.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/dbfunc/readfile.py` & `geoslurp-2.1.1/geoslurp/dbfunc/readfile.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/__init__.py` & `geoslurp-2.1.1/geoslurp/discover/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/fesom/__init__.py` & `geoslurp-2.1.1/geoslurp/discover/fesom/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/fesom/extractprofiles.py` & `geoslurp-2.1.1/geoslurp/discover/fesom/extractprofiles.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/fesom/fesomQuery.py` & `geoslurp-2.1.1/geoslurp/discover/fesom/fesomQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/generic/getTableData.py` & `geoslurp-2.1.1/geoslurp/discover/generic/getTableData.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/generic/regexQuery.py` & `geoslurp-2.1.1/geoslurp/discover/generic/regexQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/gravity/__init__.py` & `geoslurp-2.1.1/geoslurp/discover/oceanobs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,11 +9,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public
 # License along with geoslurp; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
-# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
-
-from .staticQuery import *
-from .graceQuery import *
+# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
```

### Comparing `geoslurp-2.0.0/geoslurp/discover/gravity/graceQuery.py` & `geoslurp-2.1.1/geoslurp/discover/gravity/graceQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/gravity/gravQuery.py` & `geoslurp-2.1.1/geoslurp/discover/gravity/gravQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/gravity/staticQuery.py` & `geoslurp-2.1.1/geoslurp/discover/gravity/staticQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/oceanobs/__init__.py` & `geoslurp-2.1.1/userplugins/loadlove.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public
 # License along with geoslurp; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
-# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019  
+# Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
+from geoslurp.config.catalogue import geoslurpCatalogue
+from geoslurp.dataset.snrei import LLove
+
+geoslurpCatalogue.addDataset(LLove)
```

### Comparing `geoslurp-2.0.0/geoslurp/discover/oceanobs/argoQuery.py` & `geoslurp-2.1.1/geoslurp/discover/oceanobs/argoQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/oceanobs/awipiesQuery.py` & `geoslurp-2.1.1/geoslurp/discover/oceanobs/awipiesQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/oceanobs/coraQuery.py` & `geoslurp-2.1.1/geoslurp/discover/oceanobs/coraQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/oceanobs/psmsl.py` & `geoslurp-2.1.1/geoslurp/discover/oceanobs/psmsl.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/oras/__init__.py` & `geoslurp-2.1.1/geoslurp/discover/oras/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/discover/oras/orasQuery.py` & `geoslurp-2.1.1/geoslurp/discover/oras/orasQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/tools/Bounds.py` & `geoslurp-2.1.1/geoslurp/tools/Bounds.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/tools/csv.py` & `geoslurp-2.1.1/geoslurp/tools/csv.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/tools/gravity.py` & `geoslurp-2.1.1/geoslurp/tools/gravity.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from sqlalchemy.ext.declarative import declared_attr, as_declarative
 from sqlalchemy import MetaData
 from sqlalchemy import Column,Integer,String, Boolean,Float
 from sqlalchemy.dialects.postgresql import TIMESTAMP, JSONB
 import gzip as gz
 from geoslurp.config.slurplogger import slurplogger
-from geoslurp.types import DataArrayJSONType
+from geoslurp.types.json import DataArrayJSONType
 import re
 from datetime import datetime
 from enum import Enum
 
 #define a declarative baseclass for spherical harmonics gravity  data
 @as_declarative(metadata=MetaData(schema='gravity'))
 class GravitySHTBase(object):
```

### Comparing `geoslurp-2.0.0/geoslurp/tools/netcdftools.py` & `geoslurp-2.1.1/geoslurp/tools/netcdftools.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/tools/ogrgeom.py` & `geoslurp-2.1.1/geoslurp/tools/ogrgeom.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/tools/shapelytools.py` & `geoslurp-2.1.1/geoslurp/tools/shapelytools.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,21 @@
 # You should have received a copy of the GNU Lesser General Public
 # License along with geoslurp; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 # Author Roelof Rietbroek (roelof@geod.uni-bonn.de), 2019
 
 
+from rasterio.io import MemoryFile
 import shapely.wkb
 
 def shpextract(entry):
     """ extract a shapely object from the database entry"""
     return shapely.wkb.loads(str(entry['geom']), hex=True)
 
 
 # def closestDistance():
-    
+def wkb2shapely(geom):
+    return shapely.wkb.loads(str(geom),hex=True)
+
+def gdal2rastio(rast):
+    return MemoryFile(rast.tobytes())
```

### Comparing `geoslurp-2.0.0/geoslurp/tools/time.py` & `geoslurp-2.1.1/geoslurp/tools/time.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/types/json.py` & `geoslurp-2.1.1/geoslurp/types/json.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/types/zarr.py` & `geoslurp-2.1.1/geoslurp/types/zarr.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,58 +15,74 @@
 
 # Author Roelof Rietbroek (r.rietbroek@utwente.nl), 2021
 
 
 from sqlalchemy.types import UserDefinedType
 import xarray as xr
 from psycopg2.extras import Json
-from geoslurp.tools.xarray import XarGeoslurp
 import os
 
+def getAttr(ds,key):
+    if key in ds.attrs:
+        return ds.attrs[key]
+    else:
+        return None
+
+def get_storage(ds):
+    return getAttr(ds,"gslrp_storage")
+
+def get_append_dim(ds):
+    return getAttr(ds,"gslrp_append_dim")
+
 class OutDBZarrType(UserDefinedType):
     """Converts a column of xarray Dataarrays to an out-of-db data representation"""
-    def __init__(self,defaultZstore=None):
+    def __init__(self,defaultZstore=None,modifyUri=None,append_dim=None):
         self.defaultZstore=defaultZstore
+        self.modifyUri=modifyUri
+        self.append_dim=append_dim
 
     def get_col_spec(self, **kw):
         return "JSONB"
 
     def bind_processor(self, dialect):
         def process(value):
             """Stores an xarray DataArray to a zarr-archive and return a JSON with meta info"""
-            if type(value) != xr.DataArray:
-                raise TypeError(f"Expected a xarrayDataArray got {type(value)}")
-            
-            if value.gslrp.storage:
-                #possibly overrule storage location (could be different per dataarray)
-                storage=value.gslrp.storage
-            else:
-                storage=self.defaultZstore
+            if type(value) != xr.DataArray and type(value) != xr.Dataset:
+                raise TypeError(f"Expected a xarrayDataArray/Dataset got {type(value)}")
+           
+            storage=self.defaultZstore
             
             #find out whether this dataset needs to be appended to an existing
-            append_dim=value.gslrp.append_dim
-            if not append_dim:
+            append_dim=get_append_dim(value)
+            if not self.append_dim:
                 #Expand a dimension and add a coordinate for lookup
                 append_dim="gslrp"
                 value=value.expand_dims({append_dim:1})
-            value=value.to_dataset()
+            else:
+                append_dim=self.append_dim
+            vname=value.name
+
+            if type(value) == xr.DataArray:
+                value=value.to_dataset()
 
             if os.path.exists(storage):
                 #append
                 zstore=xr.open_zarr(storage)
                 iappend=zstore.sizes[append_dim]+1
                 value.to_zarr(storage,mode='a',append_dim=append_dim)
             else:
                 #start with a new file
                 iappend=1
                 value.to_zarr(storage,mode='w')
-            
-            metadict=Json({"uri":storage,"slice":{append_dim:iappend}})
+            if self.modifyUri:
+                storage=self.modifyUri(storage)
+                
+            metadict=Json({"uri":storage,"varnames":[vname],"slice":{append_dim:iappend}})
             return metadict
         return process
 
     def result_processor(self, dialect, coltype):
         def process(value):
-            return self.zstore
+            return value
         return process
```

### Comparing `geoslurp-2.0.0/geoslurp/view/graceviews.py` & `geoslurp-2.1.1/geoslurp/view/graceviews.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp/view/viewBase.py` & `geoslurp-2.1.1/geoslurp/view/viewBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/geoslurp.egg-info/PKG-INFO` & `geoslurp-2.1.1/geoslurp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: geoslurp
-Version: 2.0.0
+Version: 2.1.1
 Summary: Python postgreSQL-PostGIS client for managing earth science datasets
 Home-page: https://github.com/strawpants/geoslurp
 Author: Roelof Rietbroek
 Author-email: roelof@wobbly.earth
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
+Provides-Extra: SH
 License-File: LICENSE
 
 # Download and manage datasets in a PostGreSQL database with the PostGIS
 The idea is that this tool contains script to download (i.e. **slurp**) commonly used datasets and to register them in a postgresql+postgis database. This database can then be queried allowing the retrieval of the relevant data or datafiles. 
 
 The main documentation lives at [wobbly.earth/geoslurp](https://wobbly.earth/geoslurp)
 
@@ -26,9 +25,7 @@
 The geoslurp module itself is a pure python module, which acts as a client. For this to work one needs to [set up a running PostGreSQL database](https://github.com/strawpants/docker-geoslurp).
 
 ![Image of geoslurp clients versus database server](docsrc/graphics/geoslurp_network.svg)
 
 
 
 
-
-
```

### Comparing `geoslurp-2.0.0/geoslurp.egg-info/SOURCES.txt` & `geoslurp-2.1.1/geoslurp.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,71 +5,55 @@
 ./clitools/geoslurper.py
 ./geoslurp/__init__.py
 ./geoslurp/config/__init__.py
 ./geoslurp/config/catalogue.py
 ./geoslurp/config/localsettings.py
 ./geoslurp/config/slurplogger.py
 ./geoslurp/datapull/__init__.py
+./geoslurp/datapull/cds.py
 ./geoslurp/datapull/crawler.py
 ./geoslurp/datapull/ftp.py
 ./geoslurp/datapull/geodesyunr.py
 ./geoslurp/datapull/github.py
 ./geoslurp/datapull/http.py
 ./geoslurp/datapull/icgem.py
 ./geoslurp/datapull/motu.py
 ./geoslurp/datapull/rsync.py
+./geoslurp/datapull/sftp.py
 ./geoslurp/datapull/thredds.py
 ./geoslurp/datapull/uri.py
 ./geoslurp/datapull/webdav.py
-./geoslurp/dataset/ArcticDEM.py
-./geoslurp/dataset/Argo.py
 ./geoslurp/dataset/CSVBase.py
-./geoslurp/dataset/DuacsGriddedDsets.py
-./geoslurp/dataset/EasyCora.py
-./geoslurp/dataset/GRACEDsets.py
-./geoslurp/dataset/GSHHGDsets.py
-./geoslurp/dataset/Hydrosheds.py
-./geoslurp/dataset/IceSatDrainDiv.py
 ./geoslurp/dataset/OGRBase.py
-./geoslurp/dataset/PSMSL.py
-./geoslurp/dataset/RGIDsets.py
-./geoslurp/dataset/RadsDsets.py
 ./geoslurp/dataset/RasterBase.py
-./geoslurp/dataset/TUGRAZDsets.py
 ./geoslurp/dataset/__init__.py
-./geoslurp/dataset/avisoRefOrbits.py
+./geoslurp/dataset/cdsbase.py
 ./geoslurp/dataset/dataSetBase.py
 ./geoslurp/dataset/datasetgeneric.py
-./geoslurp/dataset/deg1n2.py
 ./geoslurp/dataset/era5.py
-./geoslurp/dataset/geodesyunr.py
-./geoslurp/dataset/geoshapes.py
-./geoslurp/dataset/icgemDsets.py
 ./geoslurp/dataset/motuGridsBase.py
-./geoslurp/dataset/mss_cnes_cls2015.py
-./geoslurp/dataset/naturalearth.py
-./geoslurp/dataset/orsiFronts.py
 ./geoslurp/dataset/pandasbase.py
 ./geoslurp/dataset/snrei.py
-./geoslurp/dataset/wgms_fog.py
-./geoslurp/dataset/wribasin.py
+./geoslurp/dataset/xarraybase.py
 ./geoslurp/db/__init__.py
 ./geoslurp/db/connector.py
 ./geoslurp/db/connectorbase.py
 ./geoslurp/db/exporter.py
 ./geoslurp/db/geoslurpdb.py
 ./geoslurp/db/inventory.py
 ./geoslurp/db/settings.py
 ./geoslurp/db/tabletools.py
 ./geoslurp/dbfunc/__init__.py
 ./geoslurp/dbfunc/dbfunc.py
 ./geoslurp/dbfunc/maskgeom.py
 ./geoslurp/dbfunc/radsfuncs.py
 ./geoslurp/dbfunc/readfile.py
 ./geoslurp/discover/__init__.py
+./geoslurp/discover/earthmodels/__init__.py
+./geoslurp/discover/earthmodels/getlove.py
 ./geoslurp/discover/fesom/__init__.py
 ./geoslurp/discover/fesom/extractprofiles.py
 ./geoslurp/discover/fesom/fesomQuery.py
 ./geoslurp/discover/generic/__init__.py
 ./geoslurp/discover/generic/getTableData.py
 ./geoslurp/discover/generic/regexQuery.py
 ./geoslurp/discover/gravity/__init__.py
@@ -82,31 +66,67 @@
 ./geoslurp/discover/oceanobs/awipiesQuery.py
 ./geoslurp/discover/oceanobs/coraQuery.py
 ./geoslurp/discover/oceanobs/psmsl.py
 ./geoslurp/discover/oras/__init__.py
 ./geoslurp/discover/oras/orasQuery.py
 ./geoslurp/tools/Bounds.py
 ./geoslurp/tools/__init__.py
+./geoslurp/tools/cf.py
 ./geoslurp/tools/csv.py
 ./geoslurp/tools/gravity.py
 ./geoslurp/tools/netcdftools.py
 ./geoslurp/tools/ogrgeom.py
+./geoslurp/tools/pandas.py
 ./geoslurp/tools/shapelytools.py
+./geoslurp/tools/spatiallite.py
+./geoslurp/tools/tarsafe.py
 ./geoslurp/tools/time.py
 ./geoslurp/tools/xarray.py
 ./geoslurp/types/__init__.py
+./geoslurp/types/columnmapper.py
 ./geoslurp/types/json.py
+./geoslurp/types/numpy.py
+./geoslurp/types/xar.py
 ./geoslurp/types/zarr.py
 ./geoslurp/view/__init__.py
 ./geoslurp/view/graceviews.py
 ./geoslurp/view/viewBase.py
 ./userplugins/AWIPIES.py
+./userplugins/ArcticDEM.py
+./userplugins/Argo.py
+./userplugins/DuacsGriddedDsets.py
+./userplugins/EasyCora.py
 ./userplugins/FESOM.py
+./userplugins/GRACEDsets.py
+./userplugins/GSHHGDsets.py
+./userplugins/Hydrosheds.py
+./userplugins/IceSatDrainDiv.py
 ./userplugins/ORAS5.py
+./userplugins/PSMSL.py
+./userplugins/RGIDsets.py
+./userplugins/RadsDsets.py
+./userplugins/TUGRAZDsets.py
 ./userplugins/__init__.py
+./userplugins/avisoRefOrbits.py
+./userplugins/deg1n2.py
+./userplugins/geodesyunr.py
+./userplugins/geoshapes.py
+./userplugins/gleam.py
+./userplugins/glofas.py
+./userplugins/gracefilters.py
 ./userplugins/grdc.py
+./userplugins/icgemDsets.py
+./userplugins/imerg.py
+./userplugins/loadlove.py
+./userplugins/mss_cnes_cls2015.py
+./userplugins/naturalearth.py
+./userplugins/orsiFronts.py
+./userplugins/sebs.py
+./userplugins/sentinelreforbits.py
+./userplugins/wgms_fog.py
+./userplugins/wribasin.py
 clitools/geoslurper.py
 geoslurp.egg-info/PKG-INFO
 geoslurp.egg-info/SOURCES.txt
 geoslurp.egg-info/dependency_links.txt
 geoslurp.egg-info/requires.txt
 geoslurp.egg-info/top_level.txt
```

### Comparing `geoslurp-2.0.0/setup.py` & `geoslurp-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,24 @@
     long_description = fh.read()
 
 
 setuptools.setup(
     name="geoslurp",
     author="Roelof Rietbroek",
     author_email="roelof@wobbly.earth",
-    version="2.0.0",
+    version="2.1.1",
     description="Python postgreSQL-PostGIS client for managing earth science datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/strawpants/geoslurp",
     packages=find_packages("."),
     package_dir={"":"."},
     scripts=['clitools/geoslurper.py'],
     install_requires=['numpy','SQLAlchemy','pycurl','cryptography','PyYAML','lxml','keyring','pandas','motuclient','netCDF4','GDAL','Shapely','GeoAlchemy2','psycopg2'],
-    extra_requires=["pyshtools"],
+    extras_require={"SH":["pyshtools"]},
     classifiers=["Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: POSIX :: Linux",
         "Topic :: Scientific/Engineering",
         "Intended Audience :: Science/Research",
         "Development Status :: 4 - Beta"]
```

### Comparing `geoslurp-2.0.0/userplugins/AWIPIES.py` & `geoslurp-2.1.1/userplugins/AWIPIES.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def pull(self):
         """Pulls the OBP matlab file from the cloud"""
         cred=self.conf.authCred("awipies",['url','user','passw'])
         obpsource=http(cred.url,auth=cred)
         obpsource.download(self.dataDir(),outfile=self.obpfile)
 
     def register(self):
-
+        self.truncateTable()
         obpfile=os.path.join(self.dataDir(),self.obpfile)
 
         for meta in extractMetaPies(obpfile):
             self.addEntry(meta)
 
         self.updateInvent()
```

### Comparing `geoslurp-2.0.0/userplugins/FESOM.py` & `geoslurp-2.1.1/userplugins/FESOM.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.0.0/userplugins/ORAS5.py` & `geoslurp-2.1.1/userplugins/ORAS5.py`

 * *Files identical despite different names*

