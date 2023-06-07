# Comparing `tmp/i2x-1.0.0.tar.gz` & `tmp/i2x-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2x-1.0.0.tar", last modified: Mon Jun  5 22:00:39 2023, max compression
+gzip compressed data, was "i2x-1.0.1.tar", last modified: Wed Jun  7 18:29:51 2023, max compression
```

## Comparing `i2x-1.0.0.tar` & `i2x-1.0.1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:39.260446 i2x-1.0.0/
--rw-rw-rw-   0        0        0     2030 2023-01-31 18:24:18.000000 i2x-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3372 2023-06-05 22:00:39.261421 i2x-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2548 2023-06-01 15:55:15.000000 i2x-1.0.0/README.md
--rw-rw-rw-   0        0        0     1270 2023-06-05 22:00:39.263465 i2x-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-05-25 20:44:25.000000 i2x-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:38.566383 i2x-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:38.678123 i2x-1.0.0/src/i2x/
--rw-rw-rw-   0        0        0       34 2023-06-01 15:49:30.000000 i2x-1.0.0/src/i2x/__init__.py
--rw-rw-rw-   0        0        0     1242 2023-06-01 15:55:15.000000 i2x-1.0.0/src/i2x/api.py
--rw-rw-rw-   0        0        0     2504 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/der_choices.py
--rw-rw-rw-   0        0        0    24682 2023-01-25 19:53:16.000000 i2x-1.0.0/src/i2x/der_monitor.py
--rw-rw-rw-   0        0        0    32598 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/der_panel.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:38.568381 i2x-1.0.0/src/i2x/models/
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:39.090788 i2x-1.0.0/src/i2x/models/ieee9500/
--rw-rw-rw-   0        0        0   156349 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/BalancedLoads.dss
--rw-rw-rw-   0        0        0    96658 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/BusCoords.dss
--rw-rw-rw-   0        0        0      262 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/CableData.dss
--rw-rw-rw-   0        0        0     2141 2023-01-09 14:52:20.000000 i2x-1.0.0/src/i2x/models/ieee9500/CapControls.dss
--rw-rw-rw-   0        0        0      934 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/Capacitors.dss
--rw-rw-rw-   0        0        0      489 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/EnergyStorage.dss
--rw-rw-rw-   0        0        0     3601 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/Generators.dss
--rw-rw-rw-   0        0        0     3027 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/ieee9500/HCABase.dss
--rw-rw-rw-   0        0        0   171399 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/LatLongCoords.dss
--rw-rw-rw-   0        0        0    12436 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/LineCodes.dss
--rw-rw-rw-   0        0        0    14548 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/LineGeometry.dss
--rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss
--rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss
--rw-rw-rw-   0        0        0   128092 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/LoadXfmrCodes.dss
--rw-rw-rw-   0        0        0     2903 2023-06-01 15:55:15.000000 i2x-1.0.0/src/i2x/models/ieee9500/Master-bal-initial-config.dss
--rw-rw-rw-   0        0        0     3105 2022-11-22 00:41:33.000000 i2x-1.0.0/src/i2x/models/ieee9500/Master-unbal-initial-config.dss
--rw-rw-rw-   0        0        0  4120960 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/ieee9500/Network.json
--rw-rw-rw-   0        0        0  4383678 2022-12-21 15:25:32.000000 i2x-1.0.0/src/i2x/models/ieee9500/PNNL-33471.pdf
--rw-rw-rw-   0        0        0     7444 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss
--rw-rw-rw-   0        0        0     6724 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss
--rw-rw-rw-   0        0        0     2566 2023-01-23 21:37:50.000000 i2x-1.0.0/src/i2x/models/ieee9500/README.md
--rw-rw-rw-   0        0        0     3735 2023-01-09 14:46:11.000000 i2x-1.0.0/src/i2x/models/ieee9500/Regulators.dss
--rw-rw-rw-   0        0        0     4728 2023-01-09 17:53:54.000000 i2x-1.0.0/src/i2x/models/ieee9500/Transformers.dss
--rw-rw-rw-   0        0        0      786 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/TriplexLineCodes.dss
--rw-rw-rw-   0        0        0   139322 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/TriplexLines.dss
--rw-rw-rw-   0        0        0   361982 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/UnbalancedLoads.dss
--rw-rw-rw-   0        0        0    15618 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/WireData.dss
--rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.0/src/i2x/models/ieee9500/clean.bat
--rw-rw-rw-   0        0        0       40 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/ieee9500bal.dss
--rw-rw-rw-   0        0        0       42 2022-11-21 21:45:09.000000 i2x-1.0.0/src/i2x/models/ieee9500/ieee9500unbal.dss
--rw-rw-rw-   0        0        0     5190 2023-06-01 15:55:15.000000 i2x-1.0.0/src/i2x/models/ieee9500/protection.dss
--rw-rw-rw-   0        0        0     2801 2023-06-01 15:55:15.000000 i2x-1.0.0/src/i2x/models/ieee9500/reclosers.dss
--rw-rw-rw-   0        0        0     1082 2023-06-01 15:55:15.000000 i2x-1.0.0/src/i2x/models/ieee9500/switches.dss
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:39.212934 i2x-1.0.0/src/i2x/models/ieee_lvn/
--rw-rw-rw-   0        0        0     1404 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/HCABase.dss
--rw-rw-rw-   0        0        0   164108 2023-01-07 23:18:01.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/Master.dss
--rw-rw-rw-   0        0        0   316030 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/Network.json
--rw-rw-rw-   0        0        0      878 2023-01-23 21:38:04.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/README.md
--rw-rw-rw-   0        0        0    87814 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/SecPar.dss
--rw-rw-rw-   0        0        0     6023 2023-01-07 23:18:01.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/buscoords.dat
--rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/clean.bat
--rw-rw-rw-   0        0        0     6555 2023-01-07 23:18:01.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/energy_meters.dss
--rw-rw-rw-   0        0        0    12451 2023-01-07 23:18:01.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/network_protectors.dss
--rw-rw-rw-   0        0        0     7153 2023-02-05 01:47:30.000000 i2x-1.0.0/src/i2x/models/ieee_lvn/network_protectors_reverse.dss
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:39.258429 i2x-1.0.0/src/i2x/models/support/
--rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/support/cdaily.dat
--rw-rw-rw-   0        0        0     1981 2023-02-09 01:33:35.000000 i2x-1.0.0/src/i2x/models/support/inverters.dss
--rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/support/ldaily.dat
--rw-rw-rw-   0        0        0   512867 2022-11-30 15:56:42.000000 i2x-1.0.0/src/i2x/models/support/pclear.dat
--rw-rw-rw-   0        0        0   337498 2022-11-30 15:56:42.000000 i2x-1.0.0/src/i2x/models/support/pcloud.dat
--rw-rw-rw-   0        0        0    36988 2022-11-30 15:56:42.000000 i2x-1.0.0/src/i2x/models/support/pvloadshape-1sec-2900pts.dat
--rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/models/support/qdaily.dat
--rw-rw-rw-   0        0        0    15581 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/opendss_graph.py
--rw-rw-rw-   0        0        0    14526 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/opendss_interface.py
--rw-rw-rw-   0        0        0    13102 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/plot_opendss_feeder.py
--rw-rw-rw-   0        0        0       23 2023-06-05 21:59:21.000000 i2x-1.0.0/src/i2x/version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:00:38.715088 i2x-1.0.0/src/i2x.egg-info/
--rw-rw-rw-   0        0        0     3372 2023-06-05 22:00:38.000000 i2x-1.0.0/src/i2x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2478 2023-06-05 22:00:38.000000 i2x-1.0.0/src/i2x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 22:00:38.000000 i2x-1.0.0/src/i2x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 22:00:38.000000 i2x-1.0.0/src/i2x.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-23 20:58:26.000000 i2x-1.0.0/src/i2x.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       75 2023-06-05 22:00:38.000000 i2x-1.0.0/src/i2x.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-05 22:00:38.000000 i2x-1.0.0/src/i2x.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.295109 i2x-1.0.1/
+-rw-rw-rw-   0        0        0     2030 2023-01-31 18:24:18.000000 i2x-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3372 2023-06-07 18:29:51.295109 i2x-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2548 2023-06-01 15:55:15.000000 i2x-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1270 2023-06-07 18:29:51.297212 i2x-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2021-05-25 20:44:25.000000 i2x-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.665863 i2x-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.777083 i2x-1.0.1/src/i2x/
+-rw-rw-rw-   0        0        0       34 2023-06-01 15:49:30.000000 i2x-1.0.1/src/i2x/__init__.py
+-rw-rw-rw-   0        0        0     1284 2023-06-07 15:37:29.000000 i2x-1.0.1/src/i2x/api.py
+-rw-rw-rw-   0        0        0     2652 2023-06-07 17:36:49.000000 i2x-1.0.1/src/i2x/der_choices.py
+-rw-rw-rw-   0        0        0    24682 2023-01-25 19:53:16.000000 i2x-1.0.1/src/i2x/der_monitor.py
+-rw-rw-rw-   0        0        0    32715 2023-06-07 17:38:36.000000 i2x-1.0.1/src/i2x/der_panel.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.675836 i2x-1.0.1/src/i2x/models/
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.136534 i2x-1.0.1/src/i2x/models/ieee9500/
+-rw-rw-rw-   0        0        0   156349 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/BalancedLoads.dss
+-rw-rw-rw-   0        0        0    96658 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/BusCoords.dss
+-rw-rw-rw-   0        0        0      262 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/CableData.dss
+-rw-rw-rw-   0        0        0     2141 2023-01-09 14:52:20.000000 i2x-1.0.1/src/i2x/models/ieee9500/CapControls.dss
+-rw-rw-rw-   0        0        0      934 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/Capacitors.dss
+-rw-rw-rw-   0        0        0      489 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/EnergyStorage.dss
+-rw-rw-rw-   0        0        0     3601 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/Generators.dss
+-rw-rw-rw-   0        0        0     2468 2023-06-07 17:25:58.000000 i2x-1.0.1/src/i2x/models/ieee9500/HCABase.dss
+-rw-rw-rw-   0        0        0   171399 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LatLongCoords.dss
+-rw-rw-rw-   0        0        0    12436 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LineCodes.dss
+-rw-rw-rw-   0        0        0    14548 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LineGeometry.dss
+-rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss
+-rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss
+-rw-rw-rw-   0        0        0   128092 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LoadXfmrCodes.dss
+-rw-rw-rw-   0        0        0     2903 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/Master-bal-initial-config.dss
+-rw-rw-rw-   0        0        0     3105 2022-11-22 00:41:33.000000 i2x-1.0.1/src/i2x/models/ieee9500/Master-unbal-initial-config.dss
+-rw-rw-rw-   0        0        0  4120960 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/ieee9500/Network.json
+-rw-rw-rw-   0        0        0  4383678 2022-12-21 15:25:32.000000 i2x-1.0.1/src/i2x/models/ieee9500/PNNL-33471.pdf
+-rw-rw-rw-   0        0        0     7444 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss
+-rw-rw-rw-   0        0        0     6724 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss
+-rw-rw-rw-   0        0        0     2566 2023-01-23 21:37:50.000000 i2x-1.0.1/src/i2x/models/ieee9500/README.md
+-rw-rw-rw-   0        0        0     3735 2023-01-09 14:46:11.000000 i2x-1.0.1/src/i2x/models/ieee9500/Regulators.dss
+-rw-rw-rw-   0        0        0     4728 2023-01-09 17:53:54.000000 i2x-1.0.1/src/i2x/models/ieee9500/Transformers.dss
+-rw-rw-rw-   0        0        0      786 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/TriplexLineCodes.dss
+-rw-rw-rw-   0        0        0   139322 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/TriplexLines.dss
+-rw-rw-rw-   0        0        0   361982 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/UnbalancedLoads.dss
+-rw-rw-rw-   0        0        0    15618 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/WireData.dss
+-rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.1/src/i2x/models/ieee9500/clean.bat
+-rw-rw-rw-   0        0        0       40 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/ieee9500bal.dss
+-rw-rw-rw-   0        0        0       42 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/ieee9500unbal.dss
+-rw-rw-rw-   0        0        0     5190 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/protection.dss
+-rw-rw-rw-   0        0        0     2801 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/reclosers.dss
+-rw-rw-rw-   0        0        0     1082 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/switches.dss
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.268181 i2x-1.0.1/src/i2x/models/ieee_lvn/
+-rw-rw-rw-   0        0        0      835 2023-06-07 17:26:09.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/HCABase.dss
+-rw-rw-rw-   0        0        0   164108 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/Master.dss
+-rw-rw-rw-   0        0        0   316030 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/Network.json
+-rw-rw-rw-   0        0        0      878 2023-01-23 21:38:04.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/README.md
+-rw-rw-rw-   0        0        0    87814 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/SecPar.dss
+-rw-rw-rw-   0        0        0     6023 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/buscoords.dat
+-rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/clean.bat
+-rw-rw-rw-   0        0        0     6555 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/energy_meters.dss
+-rw-rw-rw-   0        0        0    12451 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors.dss
+-rw-rw-rw-   0        0        0     7153 2023-02-05 01:47:30.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors_reverse.dss
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.292116 i2x-1.0.1/src/i2x/models/support/
+-rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/support/cdaily.dat
+-rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/support/ldaily.dat
+-rw-rw-rw-   0        0        0     2666 2023-06-07 17:33:16.000000 i2x-1.0.1/src/i2x/models/support/loadshapes_and_xycurves.dss
+-rw-rw-rw-   0        0        0   512867 2022-11-30 15:56:42.000000 i2x-1.0.1/src/i2x/models/support/pclear.dat
+-rw-rw-rw-   0        0        0   337498 2022-11-30 15:56:42.000000 i2x-1.0.1/src/i2x/models/support/pcloud.dat
+-rw-rw-rw-   0        0        0    36988 2022-11-30 15:56:42.000000 i2x-1.0.1/src/i2x/models/support/pvloadshape-1sec-2900pts.dat
+-rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/support/qdaily.dat
+-rw-rw-rw-   0        0        0    16020 2023-06-06 18:30:36.000000 i2x-1.0.1/src/i2x/opendss_graph.py
+-rw-rw-rw-   0        0        0    14526 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/opendss_interface.py
+-rw-rw-rw-   0        0        0     1134 2023-06-07 16:46:17.000000 i2x-1.0.1/src/i2x/pcc_analysis.py
+-rw-rw-rw-   0        0        0    13958 2023-06-06 22:31:15.000000 i2x-1.0.1/src/i2x/plot_opendss_feeder.py
+-rw-rw-rw-   0        0        0       23 2023-06-06 22:32:45.000000 i2x-1.0.1/src/i2x/version.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.831511 i2x-1.0.1/src/i2x.egg-info/
+-rw-rw-rw-   0        0        0     3372 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2516 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-01-23 20:58:26.000000 i2x-1.0.1/src/i2x.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       75 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/top_level.txt
```

### Comparing `i2x-1.0.0/LICENSE.txt` & `i2x-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/PKG-INFO` & `i2x-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2x
-Version: 1.0.0
+Version: 1.0.1
 Summary: i2x: Interconnection Innovation e-Xchange Open Test Systems.
 Home-page: https://github.com/pnnl/i2x
 Author: Tom McDermott, Eran Schweitzer, and Jessica Kerby
 Author-email: Thomas.McDermott@PNNL.gov
 License: BSD
 Project-URL: Bug Tracker, https://github.com/pnnl/i2x/issues
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `i2x-1.0.0/README.md` & `i2x-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/setup.cfg` & `i2x-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/api.py` & `i2x-1.0.1/src/i2x/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .opendss_graph import make_builtin_graph
 from .plot_opendss_feeder import plot_opendss_feeder
 from .plot_opendss_feeder import load_opendss_graph
 from .plot_opendss_feeder import load_builtin_graph
 from .plot_opendss_feeder import parse_opendss_graph
 from .opendss_interface import print_opendss_interface
 from .opendss_interface import run_opendss, initialize_opendss, opendss_output, get_basekv, check_element_status
+from .pcc_analysis import trace_pcc_path
 
 from .der_choices import feederChoices
 from .der_choices import solarChoices
 from .der_choices import loadChoices
 from .der_choices import inverterChoices
 from .der_choices import solutionModeChoices
 from .der_choices import controlModeChoices
```

### Comparing `i2x-1.0.0/src/i2x/der_choices.py` & `i2x-1.0.1/src/i2x/der_choices.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 """Configuration data for DER test feeders
 """
 
 # TODO: consider migration to a JSON file for customization
 
 feederChoices = {
   'ieee9500':{'path':'models/ieee9500/', 'base':'Master-bal-initial-config.dss', 'network':'Network.json'},
-  'ieee_lvn':{'path':'models/ieee_lvn/', 'base':'SecPar.dss', 'network':'Network.json'}
+  'ieee_lvn':{'path':'models/ieee_lvn/', 'base':'SecPar.dss', 'network':'Network.json'},
+  'radial':{'path':'models/radial/', 'base':'HCABase.dss', 'network':'Network.json'}
   }
 
 solarChoices = {
   'pclear':{'dt':1.0, 'file':'pclear.dat', 'npts':0, 'data':None},
   'pcloud':{'dt':1.0, 'file':'pcloud.dat', 'npts':0, 'data':None},
-  'pvduty':{'dt':1.0, 'file':'pvloadshape-1sec-2900pts.dat', 'npts':0, 'data':None}
+  'pvduty':{'dt':1.0, 'file':'pvloadshape-1sec-2900pts.dat', 'npts':0, 'data':None},
+  'step':{'t':[0,6,6.003,18,18.003,24], 'p':[0,0,1,1,0,0]}
   }
 
 # this is the original OpenDSS data for piece-wise constant interpolation
 #  we are now using a quadratic interpolant at 1-second interfals
 #'default':{'t':[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24],
 #           'p':[0.677,0.6256,0.6087,0.5833,0.58028,0.6025,0.657,0.7477,0.832,0.88,0.94,0.989,0.985,0.98,0.9898,0.999,1,0.958,0.936,0.913,0.876,0.876,0.828,0.756,0.677]},
```

### Comparing `i2x-1.0.0/src/i2x/der_monitor.py` & `i2x-1.0.1/src/i2x/der_monitor.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/der_panel.py` & `i2x-1.0.1/src/i2x/der_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,20 @@
     self.nb = ttk.Notebook(master)
     self.nb.pack(fill='both', expand='yes')
 
     s = ttk.Style()
     s.configure('.', font=fontchoice)
 
     for key, row in i2x.solarChoices.items():
-      fname = pkg_resources.resource_filename (__name__, support_dir + row['file'])
-      row['data'] = np.loadtxt (fname)
-      row['npts'] = row['data'].shape[0]
-      peak = max(np.abs(row['data']))
-      row['data'] /= peak
+      if 'file' in row:
+        fname = pkg_resources.resource_filename (__name__, support_dir + row['file'])
+        row['data'] = np.loadtxt (fname)
+        row['npts'] = row['data'].shape[0]
+        peak = max(np.abs(row['data']))
+        row['data'] /= peak
     for key, row in i2x.loadChoices.items():
       if 'file' in row:
         fname = pkg_resources.resource_filename (__name__, support_dir + row['file'])
         row['data'] = np.loadtxt (fname)
         row['npts'] = row['data'].shape[0]
         peak = max(np.abs(row['data']))
         row['data'] /= peak
@@ -573,19 +574,23 @@
                              ax=self.ax_feeder, fig=self.fig_feeder)
     self.canvas_feeder.draw()
     self.ResetDERPage()
 
   def UpdateSolarProfile(self, event):
     key = self.cb_solar.get()
     row = i2x.solarChoices[key]
-    dt = row['dt']
-    npts = row['npts']
-    tmax = dt * (npts - 1)
-    y = row['data']
-    t = np.linspace (0.0, tmax, npts) / 3600.0
+    if 'dt' in row:
+      dt = row['dt']
+      npts = row['npts']
+      tmax = dt * (npts - 1)
+      y = row['data']
+      t = np.linspace (0.0, tmax, npts) / 3600.0
+    else:
+      t = row['t']
+      y = row['p']
     self.ax_solar.cla()
     self.ax_solar.plot(t, y, color='blue')
     self.ax_solar.set_xlabel('Time [hr]')
     self.ax_solar.set_ylabel('Power [pu]')
     self.ax_solar.grid()
     self.canvas_solar.draw()
```

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/BalancedLoads.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/BalancedLoads.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/BusCoords.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/BusCoords.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/CapControls.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/CapControls.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Capacitors.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/Capacitors.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Generators.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/Generators.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/HCABase.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/Master-bal-initial-config.dss`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+// Master file for 9500-Node IEEE Test Feeder Case
+// Unbalanced Load Case
+// Line definitions can use either geometry or lineconstants matrices.
+
 Clear
-set eventlogdefault=yes
 
-New Circuit.hca9500node pu=1.05  r1=0  x1=0.001  r0=0  x0=0.001  
+New Circuit.final9500node
 
-new Loadshape.pclear npts=86401 sinterval=1 csvfile=../support/pclear.dat action=normalize
-new Loadshape.pcloud npts=86401 sinterval=1 csvfile=../support/pcloud.dat action=normalize
-new Loadshape.ldaily npts=86401 sinterval=1 csvfile=../support/ldaily.dat action=normalize
-new Loadshape.qdaily npts=86401 sinterval=1 csvfile=../support/qdaily.dat action=normalize
-new Loadshape.cdaily npts=86401 sinterval=1 csvfile=../support/cdaily.dat action=normalize
-new Loadshape.pvduty npts=2900 sinterval=1 mult=(file=../support/pvloadshape-1sec-2900pts.dat) action=normalize
-redirect ../support/inverters.dss
+! Make the source stiff with small impedance
+~ pu=1.05  r1=0  x1=0.001  r0=0  x0=0.001  
 
 Redirect  WireData.dss
 Redirect  CableData.dss
+! Use either LineGeometry or LineConstantsCodes
 Redirect  LineGeometry.dss
+!Redirect  LineCodes.dss
 Redirect  TriplexLineCodes.dss
+
+! Use either LineGeometry or LineConstantsCodes
 Redirect  LinesSwitchesGeometry.dss
+!Redirect  LinesSwitchesLineCodes.dss
 Redirect  Transformers.dss
 Redirect  LoadXfmrCodes.dss
 Redirect  TriplexLines.dss
 Redirect  BalancedLoads.dss
 Redirect  Capacitors.dss
 Redirect  CapControls.dss
 Redirect  Regulators.dss
@@ -48,29 +51,29 @@
 setkvbase m1089-LNG1    kVll=0.480
 setkvbase m1089DER480-1 kVll=0.480
 setkvbase m1089-DIES1   kVll=0.480
 setkvbase m1069DER480-1 kVll=0.480
 setkvbase m1069-MT1     kVll=0.480
 
 ! Load in bus coordintes now that bus list is established
+!Buscoords  BusCoords.dss
 LatLongCoords LatLongCoords.dss
 
-New Energymeter.m1 Element=Line.HVMV115B1_sw Terminal=1 // Element=Line.LN5710794-3 Terminal=1
+New Energymeter.m1 Element=Line.LN5710794-3 Terminal=1
 
 
 Set Maxiterations=30     ! Sometimes the solution takes more than the default 15 iterations
 Set MaxControlIter=100
 
 Set loadmult=1.0
 
 ! Generator Configuration
 ! CHP at 30% capacity, MT-1 at 25%, MT-2 at 50%, all other DG off.
-! generator PV model (3) is not compatible with InvControl and ExpControl
-edit Generator.SteamGen1 model=1 kw=1000 vpu=1.00 pf=-0.68
-//edit Generator.SteamGen1 kw=1000 vpu=1.00
+Generator.SteamGen1.kw=1000
+Generator.SteamGen1.vpu=1.00
 Generator.MicroTurb-1.kw=50
 Generator.MicroTurb-2.kw=0
 Generator.MicroTurb-3.kw=0
 Generator.WindTurb-1.kw=20
 Generator.WindTurb-2.kw=20
 Generator.WindTurb-3.kw=20
 Generator.MicroTurb-4.kw=100
@@ -79,9 +82,17 @@
 Generator.LNGEngine100.kw=0
 Generator.LNGEngine1800.kw=0
 
 
 ! Set normal feeder configuration
 redirect switches.dss
 
-// include reclosers and their monitors
+set MarkPVSystems=true PVMarkerCode=18
+set Markswitches=true SwitchMarkerCode=9
+set MarkRegulators=true RegMarkerCode=15         
+set MarkCapacitors=true CapMarkerCode=38
+set MarkStorage=true StoreMarkerCode=36
+set MarkTransformers=true TransmarkerCode=14
+
 redirect reclosers.dss
+
+//Plot daisy Power Max=1000 dots=n labels=n 1ph=3
```

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/LatLongCoords.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/LatLongCoords.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/LineCodes.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/LineCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/LineGeometry.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/LineGeometry.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/LoadXfmrCodes.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/LoadXfmrCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Master-bal-initial-config.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/Master-unbal-initial-config.dss`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ! Use either LineGeometry or LineConstantsCodes
 Redirect  LinesSwitchesGeometry.dss
 !Redirect  LinesSwitchesLineCodes.dss
 Redirect  Transformers.dss
 Redirect  LoadXfmrCodes.dss
 Redirect  TriplexLines.dss
-Redirect  BalancedLoads.dss
+Redirect  UnbalancedLoads.dss
 Redirect  Capacitors.dss
 Redirect  CapControls.dss
 Redirect  Regulators.dss
 
 Redirect  Generators.dss
 Redirect  EnergyStorage.dss
 Redirect  PV_10pen_DSSPV.dss
@@ -80,19 +80,28 @@
 Generator.Diesel620.kw=0
 Generator.Diesel590.kw=0
 Generator.LNGEngine100.kw=0
 Generator.LNGEngine1800.kw=0
 
 
 ! Set normal feeder configuration
-redirect switches.dss
+open Line.WF856_48332_sw
+open Line.WG127_48332_sw
+open LINE.LN0653457_SW
+open LINE.V7173_48332_SW
+open LINE.TSW803273_SW 
+open LINE.A333_48332_SW 
+//solve
+open LINE.TSW320328_SW  
+open LINE.A8645_48332_SW
+open LINE.TSW568613_SW
+//solve
+
 
 set MarkPVSystems=true PVMarkerCode=18
 set Markswitches=true SwitchMarkerCode=9
 set MarkRegulators=true RegMarkerCode=15         
 set MarkCapacitors=true CapMarkerCode=38
 set MarkStorage=true StoreMarkerCode=36
 set MarkTransformers=true TransmarkerCode=14
 
-redirect reclosers.dss
-
 //Plot daisy Power Max=1000 dots=n labels=n 1ph=3
```

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Master-unbal-initial-config.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/HCABase.dss`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-// Master file for 9500-Node IEEE Test Feeder Case
-// Unbalanced Load Case
-// Line definitions can use either geometry or lineconstants matrices.
-
 Clear
+set eventlogdefault=yes
 
-New Circuit.final9500node
+New Circuit.hca9500node pu=1.05  r1=0  x1=0.001  r0=0  x0=0.001  
 
-! Make the source stiff with small impedance
-~ pu=1.05  r1=0  x1=0.001  r0=0  x0=0.001  
+redirect ../support/loadshapes_and_xycurves.dss
 
 Redirect  WireData.dss
 Redirect  CableData.dss
-! Use either LineGeometry or LineConstantsCodes
 Redirect  LineGeometry.dss
-!Redirect  LineCodes.dss
 Redirect  TriplexLineCodes.dss
-
-! Use either LineGeometry or LineConstantsCodes
 Redirect  LinesSwitchesGeometry.dss
-!Redirect  LinesSwitchesLineCodes.dss
 Redirect  Transformers.dss
 Redirect  LoadXfmrCodes.dss
 Redirect  TriplexLines.dss
-Redirect  UnbalancedLoads.dss
+Redirect  BalancedLoads.dss
 Redirect  Capacitors.dss
 Redirect  CapControls.dss
 Redirect  Regulators.dss
 
 Redirect  Generators.dss
 Redirect  EnergyStorage.dss
 Redirect  PV_10pen_DSSPV.dss
@@ -51,57 +42,40 @@
 setkvbase m1089-LNG1    kVll=0.480
 setkvbase m1089DER480-1 kVll=0.480
 setkvbase m1089-DIES1   kVll=0.480
 setkvbase m1069DER480-1 kVll=0.480
 setkvbase m1069-MT1     kVll=0.480
 
 ! Load in bus coordintes now that bus list is established
-!Buscoords  BusCoords.dss
 LatLongCoords LatLongCoords.dss
 
-New Energymeter.m1 Element=Line.LN5710794-3 Terminal=1
+New Energymeter.m1 Element=Line.HVMV115B1_sw Terminal=1 // Element=Line.LN5710794-3 Terminal=1
 
 
 Set Maxiterations=30     ! Sometimes the solution takes more than the default 15 iterations
 Set MaxControlIter=100
 
 Set loadmult=1.0
 
 ! Generator Configuration
 ! CHP at 30% capacity, MT-1 at 25%, MT-2 at 50%, all other DG off.
-Generator.SteamGen1.kw=1000
-Generator.SteamGen1.vpu=1.00
+! generator PV model (3) is not compatible with InvControl and ExpControl
+edit Generator.SteamGen1 model=1 kw=1000 vpu=1.00 pf=-0.68
+//edit Generator.SteamGen1 kw=1000 vpu=1.00
 Generator.MicroTurb-1.kw=50
 Generator.MicroTurb-2.kw=0
 Generator.MicroTurb-3.kw=0
 Generator.WindTurb-1.kw=20
 Generator.WindTurb-2.kw=20
 Generator.WindTurb-3.kw=20
 Generator.MicroTurb-4.kw=100
 Generator.Diesel620.kw=0
 Generator.Diesel590.kw=0
 Generator.LNGEngine100.kw=0
 Generator.LNGEngine1800.kw=0
 
 
 ! Set normal feeder configuration
-open Line.WF856_48332_sw
-open Line.WG127_48332_sw
-open LINE.LN0653457_SW
-open LINE.V7173_48332_SW
-open LINE.TSW803273_SW 
-open LINE.A333_48332_SW 
-//solve
-open LINE.TSW320328_SW  
-open LINE.A8645_48332_SW
-open LINE.TSW568613_SW
-//solve
-
-
-set MarkPVSystems=true PVMarkerCode=18
-set Markswitches=true SwitchMarkerCode=9
-set MarkRegulators=true RegMarkerCode=15         
-set MarkCapacitors=true CapMarkerCode=38
-set MarkStorage=true StoreMarkerCode=36
-set MarkTransformers=true TransmarkerCode=14
+redirect switches.dss
 
-//Plot daisy Power Max=1000 dots=n labels=n 1ph=3
+// include reclosers and their monitors
+redirect reclosers.dss
```

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Network.json` & `i2x-1.0.1/src/i2x/models/ieee9500/Network.json`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/PNNL-33471.pdf` & `i2x-1.0.1/src/i2x/models/ieee9500/PNNL-33471.pdf`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/README.md` & `i2x-1.0.1/src/i2x/models/ieee9500/README.md`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Regulators.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/Regulators.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/Transformers.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/Transformers.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/TriplexLineCodes.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/TriplexLineCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/TriplexLines.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/TriplexLines.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/UnbalancedLoads.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/UnbalancedLoads.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/WireData.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/WireData.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/protection.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/protection.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/reclosers.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/reclosers.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee9500/switches.dss` & `i2x-1.0.1/src/i2x/models/ieee9500/switches.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/Master.dss` & `i2x-1.0.1/src/i2x/models/ieee_lvn/Master.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/Network.json` & `i2x-1.0.1/src/i2x/models/ieee_lvn/Network.json`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/README.md` & `i2x-1.0.1/src/i2x/models/ieee_lvn/README.md`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/SecPar.dss` & `i2x-1.0.1/src/i2x/models/ieee_lvn/SecPar.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/buscoords.dat` & `i2x-1.0.1/src/i2x/models/ieee_lvn/buscoords.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/energy_meters.dss` & `i2x-1.0.1/src/i2x/models/ieee_lvn/energy_meters.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/network_protectors.dss` & `i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/ieee_lvn/network_protectors_reverse.dss` & `i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors_reverse.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/support/cdaily.dat` & `i2x-1.0.1/src/i2x/models/support/cdaily.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/support/inverters.dss` & `i2x-1.0.1/src/i2x/models/support/loadshapes_and_xycurves.dss`

 * *Files 23% similar despite different names*

```diff
@@ -23,8 +23,16 @@
 
 // volt-watt settings to start limiting at 1.03 pu, with sentinel, can't absorb P 
 //   note that minimum V1 is 1.05 and maximum V2 is 1.10 per IEEE 1547, so V1=1.03 below is outside the standard
 //   OpenDSS will screen for V1 >= 1.00 and V2 <= 1.10
 New XYcurve.voltwatt1547pv npts=4 Yarray=[1.0,1.0,0.0,0.0] Xarray=[0.0,1.03,1.06,2.00]
 
 new loadshape.flat npts=2 interval=0 hour=[0.00,24.00] mult=[1.00,1.00] action=normalize
+new loadshape.step npts=6 interval=0 hour=[0.00,6.00,6.003,18.00,18.003,24.00] 
+~                                    mult=[0.00,0.00,1.000, 1.00, 0.000, 0.00] action=normalize
+new Loadshape.pclear npts=86401 sinterval=1 csvfile=pclear.dat action=normalize
+new Loadshape.pcloud npts=86401 sinterval=1 csvfile=pcloud.dat action=normalize
+new Loadshape.ldaily npts=86401 sinterval=1 csvfile=ldaily.dat action=normalize
+new Loadshape.qdaily npts=86401 sinterval=1 csvfile=qdaily.dat action=normalize
+new Loadshape.cdaily npts=86401 sinterval=1 csvfile=cdaily.dat action=normalize
+new Loadshape.pvduty npts=2900 sinterval=1 mult=(file=pvloadshape-1sec-2900pts.dat) action=normalize
```

### Comparing `i2x-1.0.0/src/i2x/models/support/ldaily.dat` & `i2x-1.0.1/src/i2x/models/support/ldaily.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/support/pclear.dat` & `i2x-1.0.1/src/i2x/models/support/pclear.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/support/pcloud.dat` & `i2x-1.0.1/src/i2x/models/support/pcloud.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/support/pvloadshape-1sec-2900pts.dat` & `i2x-1.0.1/src/i2x/models/support/pvloadshape-1sec-2900pts.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/models/support/qdaily.dat` & `i2x-1.0.1/src/i2x/models/support/qdaily.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/opendss_graph.py` & `i2x-1.0.1/src/i2x/opendss_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,17 @@
                             ['bus1', 'bus2'])
   relays = dict_from_file (os.path.join (saved_path, 'Relay.dss'),
                           ['MonitoredObj', 'type', 'MonitoredTerm'], 
                           ['MonitoredObj', 'type'])
   reclosers = dict_from_file (os.path.join (saved_path, 'Recloser.dss'),
                           ['MonitoredObj', 'MonitoredTerm', 'PhaseTrip', 'GroundTrip'], 
                           ['MonitoredObj'])
+  fuses = dict_from_file (os.path.join (saved_path, 'Fuse.dss'),
+                          ['MonitoredObj', 'MonitoredTerm', 'RatedCurrent'], 
+                          ['MonitoredObj'])
   regulators = dict_from_file (os.path.join (saved_path, 'RegControl.dss'),
                             ['transformer', 'winding', 'tapwinding', 'ptratio', 'vreg', 'band', 
                              'reversible', 'revvreg', 'revband','revThreshold', 'delay', 'revDelay'], 
                             ['transformer', 'reversible'])
   swtcontrols = dict_from_file (os.path.join (saved_path, 'SwtControl.dss'),
                           ['SwitchedObj', 'State', 'Normal', 'SwitchedTerm'], 
                           ['SwitchedObj', 'State', 'Normal'])
@@ -268,14 +271,18 @@
     if 'line.' in row['MonitoredObj']:
       branch = row['MonitoredObj'][5:]
       lines[branch]['Relay'] = True
   for key, row in reclosers.items():
     if 'line.' in row['MonitoredObj']:
       branch = row['MonitoredObj'][5:]
       lines[branch]['Recloser'] = True
+  for key, row in fuses.items():
+    if 'line.' in row['MonitoredObj']:
+      branch = row['MonitoredObj'][5:]
+      lines[branch]['Fuse'] = True
   for key, row in swtcontrols.items():
     if 'line.' in row['SwitchedObj']:
       branch = row['SwitchedObj'][5:]
       lines[branch]['SwtControl'] = True
       lines[branch]['SwitchedTerminal'] = int(row['SwitchedTerm'])
       SwtOpen = False
       if 'State' in row:
@@ -317,14 +324,15 @@
 
   print ('read {:4d} transformers'.format (len(transformers)))
   print ('read {:4d} regulators (as transformers)'.format (len(regulators)))
   print ('read {:4d} lines'.format (len(lines)))
   print ('read {:4d} switches (in lines)'.format (nswitch))
   print ('read {:4d} switch controls'.format (len(swtcontrols)))
   print ('read {:4d} reclosers'.format (len(reclosers)))
+  print ('read {:4d} fuses'.format (len(fuses)))
   print ('read {:4d} relays'.format (len(relays)))
   print ('read {:4d} reactors'.format (len(reactors)))
   print ('read {:4d} sources'.format (len(sources)))
   print ('read {:4d} bus_xy_kv'.format (len(bus_xy_kv)))
 
   # construct a graph of the model, starting with all known buses that have XY coordinates
   G = nx.DiGraph()
@@ -336,14 +344,16 @@
 
   # add series power delivery branches (not handling series capacitors)
   for key, data in lines.items():
     if 'Relay' in data:
       eclass = 'nwp'
     elif 'Recloser' in data:
       eclass = 'recloser'
+    elif 'Fuse' in data:
+      eclass = 'fuse'
     elif data['Switch']:
       if data['SwtControl']:
         eclass = 'swtcontrol'
       else:
         eclass = 'switch'
     else:
       eclass = 'line'
```

### Comparing `i2x-1.0.0/src/i2x/opendss_interface.py` & `i2x-1.0.1/src/i2x/opendss_interface.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.0/src/i2x/plot_opendss_feeder.py` & `i2x-1.0.1/src/i2x/plot_opendss_feeder.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,32 +91,46 @@
   'ieee9500':{'path':'models/ieee9500/', 'base':'Master-bal-initial-config.dss', 'network':'Network.json'},
   'ieee_lvn':{'path':'models/ieee_lvn/', 'base':'SecPar.dss', 'network':'Network.json'}
   }
 
 lblDeltaY = 0.0 # 0.35
 
 edgeTypes = {
-  'line':        {'color':'gray',   'tag':'LN'},
-  'transformer': {'color':'orange', 'tag':'XFM'},
-  'regulator':   {'color':'red',    'tag':'REG'},
-  'switch':      {'color':'cornflowerblue',   'tag':'SWT'},
-  'swtcontrol':  {'color':'blue',   'tag':'CTL'},
-  'nwp':         {'color':'magenta','tag':'NWP'},
-  'recloser':    {'color':'lime',   'tag':'REC'},
-  'reactor':     {'color':'green',  'tag':'RCT'}
+  'line':        {'color':'gray',   'tag':'LN', 'count':0},
+  'transformer': {'color':'orange', 'tag':'XFM', 'count':0},
+  'regulator':   {'color':'red',    'tag':'REG', 'count':0},
+  'switch':      {'color':'cornflowerblue',   'tag':'SWT', 'count':0},
+  'swtcontrol':  {'color':'blue',   'tag':'CTL', 'count':0},
+  'nwp':         {'color':'magenta','tag':'NWP', 'count':0},
+  'recloser':    {'color':'lime',   'tag':'REC', 'count':0},
+  'reactor':     {'color':'green',  'tag':'RCT', 'count':0},
+  'fuse':        {'color':'magenta','tag':'FUS', 'count':0}
   }
 
 nodeTypes = {
-  'source':     {'color':'cyan',   'tag':'SUB', 'size':10, 'lblDeltaY': -lblDeltaY},
-  'generator':  {'color':'red',    'tag':'GEN', 'size':10, 'lblDeltaY':  lblDeltaY},
-  'solar':      {'color':'gold',   'tag':'PV',  'size':25, 'lblDeltaY': -lblDeltaY},
-  'capacitor':  {'color':'blue',   'tag':'CAP', 'size':15, 'lblDeltaY': -lblDeltaY},
-  'storage':    {'color':'green',  'tag':'BAT', 'size':35, 'lblDeltaY': -lblDeltaY}
+  'source':     {'color':'cyan',   'tag':'SUB', 'size':25, 'lblDeltaY': -lblDeltaY, 'count':0},
+  'generator':  {'color':'red',    'tag':'GEN', 'size':25, 'lblDeltaY':  lblDeltaY, 'count':0},
+  'solar':      {'color':'gold',   'tag':'PV',  'size':25, 'lblDeltaY': -lblDeltaY, 'count':0},
+  'capacitor':  {'color':'blue',   'tag':'CAP', 'size':15, 'lblDeltaY': -lblDeltaY, 'count':0},
+  'storage':    {'color':'green',  'tag':'BAT', 'size':25, 'lblDeltaY': -lblDeltaY, 'count':0}
   }
 
+def filter_types_used(d):
+  ret = {}
+  for key, val in d.items():
+    if val['count'] > 0:
+      ret[key] = val
+  return ret
+
+def reset_type_counts():
+  for key, val in edgeTypes.items():
+    val['count'] = 0
+  for key, val in nodeTypes.items():
+    val['count'] = 0
+
 def get_node_mnemonic(nclass):
   if nclass in nodeTypes:
     return nodeTypes[nclass]['tag']
   return nodeTypes['other']['tag']
 
 def get_node_size(nclass):
   if nclass in nodeTypes:
@@ -126,28 +140,35 @@
 def get_node_offset(nclass):
   if nclass in nodeTypes:
     return nodeTypes[nclass]['lblDeltaY']
   return -lblDeltaY
 
 def get_node_color(nclass):
   if nclass in nodeTypes:
+    nodeTypes[nclass]['count'] += 1
     return nodeTypes[nclass]['color']
   return 'black'
 
 def get_edge_width(nphs, eclass):
-  if eclass in ['recloser', 'swtcontrol']:
-    return 10.0
+  if eclass != 'line':
+    return 4.0
   if nphs == 1:
-    return 2.0 # 1.0
+    return 1.0
   if nphs == 2:
-    return 2.0 # 1.5
+    return 1.5
   return 2.0
 
+def get_edge_marker(eclass):
+  if eclass == 'line':
+    return None
+  return None # 's'
+
 def get_edge_color(eclass):
   if eclass in edgeTypes:
+    edgeTypes[eclass]['count'] += 1
     return edgeTypes[eclass]['color']
   print ('unknown edge class', eclass)
   return edgeTypes['unknown']['color']
 
 def get_edge_mnemonic(eclass):
   if eclass in edgeTypes:
     return edgeTypes[eclass]['tag']
@@ -170,14 +191,15 @@
   row = feederChoices[feeder_name]
   fname = pkg_resources.resource_filename (__name__, row['path'] + row['network'])
   return load_opendss_graph (fname)
 
 def plot_opendss_feeder (G, plot_labels = False, pdf_name = None, fig = None, 
                          ax = None, title=None, on_canvas=False, plot_comps=False, legend_loc='lower right'):
 
+  reset_type_counts()
   # extract the XY coordinates available for plotting
   xy = {}
   xyLbl = {}
   lblNode = {}
   plotNodes = []
   nodeColors = []
   nodeSizes = []
@@ -238,19 +260,22 @@
     nx.draw_networkx_labels (G, xyLbl, lblNode, font_size=8, font_color='k', 
                  horizontalalignment='left', verticalalignment='baseline', ax=ax)
   if title is not None:
     plt.title (title)
   plt.xlabel ('X coordinate [k]')
   plt.ylabel ('Y coordinate [k]')
   ax.grid(linestyle='dotted')
+  # plot a legend containing only the node and edge types that were actually used
+  legendEdges = filter_types_used (edgeTypes)
+  legendNodes = filter_types_used (nodeTypes)
   xdata = [0, 1]
   ydata = [1, 0]
-  lns = [lines.Line2D(xdata, ydata, color=get_edge_color(e)) for e in edgeTypes] + \
-    [lines.Line2D(xdata, ydata, color=get_node_color(n), marker='o') for n in nodeTypes]
-  labs = [get_edge_mnemonic (e) for e in edgeTypes] + [get_node_mnemonic (n) for n in nodeTypes]
+  lns = [lines.Line2D(xdata, ydata, color=get_edge_color(e), marker=get_edge_marker(e)) for e in legendEdges] + \
+    [lines.Line2D(xdata, ydata, color=get_node_color(n), marker='o') for n in legendNodes]
+  labs = [get_edge_mnemonic (e) for e in legendEdges] + [get_node_mnemonic (n) for n in legendNodes]
   ax.tick_params(left=True, bottom=True, labelleft=True, labelbottom=True)
   ax.legend(lns, labs, loc=legend_loc)
   if pdf_name is not None:
     plt.savefig (pdf_name)
   if not on_canvas:
     plt.show()
```

### Comparing `i2x-1.0.0/src/i2x.egg-info/PKG-INFO` & `i2x-1.0.1/src/i2x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2x
-Version: 1.0.0
+Version: 1.0.1
 Summary: i2x: Interconnection Innovation e-Xchange Open Test Systems.
 Home-page: https://github.com/pnnl/i2x
 Author: Tom McDermott, Eran Schweitzer, and Jessica Kerby
 Author-email: Thomas.McDermott@PNNL.gov
 License: BSD
 Project-URL: Bug Tracker, https://github.com/pnnl/i2x/issues
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `i2x-1.0.0/src/i2x.egg-info/SOURCES.txt` & `i2x-1.0.1/src/i2x.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/i2x/__init__.py
 src/i2x/api.py
 src/i2x/der_choices.py
 src/i2x/der_monitor.py
 src/i2x/der_panel.py
 src/i2x/opendss_graph.py
 src/i2x/opendss_interface.py
+src/i2x/pcc_analysis.py
 src/i2x/plot_opendss_feeder.py
 src/i2x/version.py
 src/i2x.egg-info/PKG-INFO
 src/i2x.egg-info/SOURCES.txt
 src/i2x.egg-info/dependency_links.txt
 src/i2x.egg-info/entry_points.txt
 src/i2x.egg-info/not-zip-safe
@@ -58,13 +59,13 @@
 src/i2x/models/ieee_lvn/SecPar.dss
 src/i2x/models/ieee_lvn/buscoords.dat
 src/i2x/models/ieee_lvn/clean.bat
 src/i2x/models/ieee_lvn/energy_meters.dss
 src/i2x/models/ieee_lvn/network_protectors.dss
 src/i2x/models/ieee_lvn/network_protectors_reverse.dss
 src/i2x/models/support/cdaily.dat
-src/i2x/models/support/inverters.dss
 src/i2x/models/support/ldaily.dat
+src/i2x/models/support/loadshapes_and_xycurves.dss
 src/i2x/models/support/pclear.dat
 src/i2x/models/support/pcloud.dat
 src/i2x/models/support/pvloadshape-1sec-2900pts.dat
 src/i2x/models/support/qdaily.dat
```

