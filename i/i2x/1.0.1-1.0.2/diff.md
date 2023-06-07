# Comparing `tmp/i2x-1.0.1.tar.gz` & `tmp/i2x-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2x-1.0.1.tar", last modified: Wed Jun  7 18:29:51 2023, max compression
+gzip compressed data, was "i2x-1.0.2.tar", last modified: Wed Jun  7 18:41:55 2023, max compression
```

## Comparing `i2x-1.0.1.tar` & `i2x-1.0.2.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.295109 i2x-1.0.1/
--rw-rw-rw-   0        0        0     2030 2023-01-31 18:24:18.000000 i2x-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3372 2023-06-07 18:29:51.295109 i2x-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2548 2023-06-01 15:55:15.000000 i2x-1.0.1/README.md
--rw-rw-rw-   0        0        0     1270 2023-06-07 18:29:51.297212 i2x-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-05-25 20:44:25.000000 i2x-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.665863 i2x-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.777083 i2x-1.0.1/src/i2x/
--rw-rw-rw-   0        0        0       34 2023-06-01 15:49:30.000000 i2x-1.0.1/src/i2x/__init__.py
--rw-rw-rw-   0        0        0     1284 2023-06-07 15:37:29.000000 i2x-1.0.1/src/i2x/api.py
--rw-rw-rw-   0        0        0     2652 2023-06-07 17:36:49.000000 i2x-1.0.1/src/i2x/der_choices.py
--rw-rw-rw-   0        0        0    24682 2023-01-25 19:53:16.000000 i2x-1.0.1/src/i2x/der_monitor.py
--rw-rw-rw-   0        0        0    32715 2023-06-07 17:38:36.000000 i2x-1.0.1/src/i2x/der_panel.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.675836 i2x-1.0.1/src/i2x/models/
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.136534 i2x-1.0.1/src/i2x/models/ieee9500/
--rw-rw-rw-   0        0        0   156349 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/BalancedLoads.dss
--rw-rw-rw-   0        0        0    96658 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/BusCoords.dss
--rw-rw-rw-   0        0        0      262 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/CableData.dss
--rw-rw-rw-   0        0        0     2141 2023-01-09 14:52:20.000000 i2x-1.0.1/src/i2x/models/ieee9500/CapControls.dss
--rw-rw-rw-   0        0        0      934 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/Capacitors.dss
--rw-rw-rw-   0        0        0      489 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/EnergyStorage.dss
--rw-rw-rw-   0        0        0     3601 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/Generators.dss
--rw-rw-rw-   0        0        0     2468 2023-06-07 17:25:58.000000 i2x-1.0.1/src/i2x/models/ieee9500/HCABase.dss
--rw-rw-rw-   0        0        0   171399 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LatLongCoords.dss
--rw-rw-rw-   0        0        0    12436 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LineCodes.dss
--rw-rw-rw-   0        0        0    14548 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LineGeometry.dss
--rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss
--rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss
--rw-rw-rw-   0        0        0   128092 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/LoadXfmrCodes.dss
--rw-rw-rw-   0        0        0     2903 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/Master-bal-initial-config.dss
--rw-rw-rw-   0        0        0     3105 2022-11-22 00:41:33.000000 i2x-1.0.1/src/i2x/models/ieee9500/Master-unbal-initial-config.dss
--rw-rw-rw-   0        0        0  4120960 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/ieee9500/Network.json
--rw-rw-rw-   0        0        0  4383678 2022-12-21 15:25:32.000000 i2x-1.0.1/src/i2x/models/ieee9500/PNNL-33471.pdf
--rw-rw-rw-   0        0        0     7444 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss
--rw-rw-rw-   0        0        0     6724 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss
--rw-rw-rw-   0        0        0     2566 2023-01-23 21:37:50.000000 i2x-1.0.1/src/i2x/models/ieee9500/README.md
--rw-rw-rw-   0        0        0     3735 2023-01-09 14:46:11.000000 i2x-1.0.1/src/i2x/models/ieee9500/Regulators.dss
--rw-rw-rw-   0        0        0     4728 2023-01-09 17:53:54.000000 i2x-1.0.1/src/i2x/models/ieee9500/Transformers.dss
--rw-rw-rw-   0        0        0      786 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/TriplexLineCodes.dss
--rw-rw-rw-   0        0        0   139322 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/TriplexLines.dss
--rw-rw-rw-   0        0        0   361982 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/UnbalancedLoads.dss
--rw-rw-rw-   0        0        0    15618 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/WireData.dss
--rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.1/src/i2x/models/ieee9500/clean.bat
--rw-rw-rw-   0        0        0       40 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/ieee9500bal.dss
--rw-rw-rw-   0        0        0       42 2022-11-21 21:45:09.000000 i2x-1.0.1/src/i2x/models/ieee9500/ieee9500unbal.dss
--rw-rw-rw-   0        0        0     5190 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/protection.dss
--rw-rw-rw-   0        0        0     2801 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/reclosers.dss
--rw-rw-rw-   0        0        0     1082 2023-06-01 15:55:15.000000 i2x-1.0.1/src/i2x/models/ieee9500/switches.dss
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.268181 i2x-1.0.1/src/i2x/models/ieee_lvn/
--rw-rw-rw-   0        0        0      835 2023-06-07 17:26:09.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/HCABase.dss
--rw-rw-rw-   0        0        0   164108 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/Master.dss
--rw-rw-rw-   0        0        0   316030 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/Network.json
--rw-rw-rw-   0        0        0      878 2023-01-23 21:38:04.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/README.md
--rw-rw-rw-   0        0        0    87814 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/SecPar.dss
--rw-rw-rw-   0        0        0     6023 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/buscoords.dat
--rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/clean.bat
--rw-rw-rw-   0        0        0     6555 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/energy_meters.dss
--rw-rw-rw-   0        0        0    12451 2023-01-07 23:18:01.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors.dss
--rw-rw-rw-   0        0        0     7153 2023-02-05 01:47:30.000000 i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors_reverse.dss
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:51.292116 i2x-1.0.1/src/i2x/models/support/
--rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/support/cdaily.dat
--rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/support/ldaily.dat
--rw-rw-rw-   0        0        0     2666 2023-06-07 17:33:16.000000 i2x-1.0.1/src/i2x/models/support/loadshapes_and_xycurves.dss
--rw-rw-rw-   0        0        0   512867 2022-11-30 15:56:42.000000 i2x-1.0.1/src/i2x/models/support/pclear.dat
--rw-rw-rw-   0        0        0   337498 2022-11-30 15:56:42.000000 i2x-1.0.1/src/i2x/models/support/pcloud.dat
--rw-rw-rw-   0        0        0    36988 2022-11-30 15:56:42.000000 i2x-1.0.1/src/i2x/models/support/pvloadshape-1sec-2900pts.dat
--rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/models/support/qdaily.dat
--rw-rw-rw-   0        0        0    16020 2023-06-06 18:30:36.000000 i2x-1.0.1/src/i2x/opendss_graph.py
--rw-rw-rw-   0        0        0    14526 2023-06-05 21:59:21.000000 i2x-1.0.1/src/i2x/opendss_interface.py
--rw-rw-rw-   0        0        0     1134 2023-06-07 16:46:17.000000 i2x-1.0.1/src/i2x/pcc_analysis.py
--rw-rw-rw-   0        0        0    13958 2023-06-06 22:31:15.000000 i2x-1.0.1/src/i2x/plot_opendss_feeder.py
--rw-rw-rw-   0        0        0       23 2023-06-06 22:32:45.000000 i2x-1.0.1/src/i2x/version.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:29:50.831511 i2x-1.0.1/src/i2x.egg-info/
--rw-rw-rw-   0        0        0     3372 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2516 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-23 20:58:26.000000 i2x-1.0.1/src/i2x.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       75 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-07 18:29:50.000000 i2x-1.0.1/src/i2x.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:55.078631 i2x-1.0.2/
+-rw-rw-rw-   0        0        0     2030 2023-01-31 18:24:18.000000 i2x-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3372 2023-06-07 18:41:55.079081 i2x-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2548 2023-06-01 15:55:15.000000 i2x-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1289 2023-06-07 18:41:55.082077 i2x-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2021-05-25 20:44:25.000000 i2x-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:54.780258 i2x-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:54.839271 i2x-1.0.2/src/i2x/
+-rw-rw-rw-   0        0        0       34 2023-06-01 15:49:30.000000 i2x-1.0.2/src/i2x/__init__.py
+-rw-rw-rw-   0        0        0     1284 2023-06-07 15:37:29.000000 i2x-1.0.2/src/i2x/api.py
+-rw-rw-rw-   0        0        0     2652 2023-06-07 17:36:49.000000 i2x-1.0.2/src/i2x/der_choices.py
+-rw-rw-rw-   0        0        0    24682 2023-01-25 19:53:16.000000 i2x-1.0.2/src/i2x/der_monitor.py
+-rw-rw-rw-   0        0        0    32715 2023-06-07 17:38:36.000000 i2x-1.0.2/src/i2x/der_panel.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:54.793711 i2x-1.0.2/src/i2x/models/
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:54.999297 i2x-1.0.2/src/i2x/models/ieee9500/
+-rw-rw-rw-   0        0        0   156349 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/BalancedLoads.dss
+-rw-rw-rw-   0        0        0    96658 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/BusCoords.dss
+-rw-rw-rw-   0        0        0      262 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/CableData.dss
+-rw-rw-rw-   0        0        0     2141 2023-01-09 14:52:20.000000 i2x-1.0.2/src/i2x/models/ieee9500/CapControls.dss
+-rw-rw-rw-   0        0        0      934 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/Capacitors.dss
+-rw-rw-rw-   0        0        0      489 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/EnergyStorage.dss
+-rw-rw-rw-   0        0        0     3601 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/Generators.dss
+-rw-rw-rw-   0        0        0     2468 2023-06-07 17:25:58.000000 i2x-1.0.2/src/i2x/models/ieee9500/HCABase.dss
+-rw-rw-rw-   0        0        0   171399 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/LatLongCoords.dss
+-rw-rw-rw-   0        0        0    12436 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/LineCodes.dss
+-rw-rw-rw-   0        0        0    14548 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/LineGeometry.dss
+-rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss
+-rw-rw-rw-   0        0        0   511727 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss
+-rw-rw-rw-   0        0        0   128092 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/LoadXfmrCodes.dss
+-rw-rw-rw-   0        0        0     2903 2023-06-01 15:55:15.000000 i2x-1.0.2/src/i2x/models/ieee9500/Master-bal-initial-config.dss
+-rw-rw-rw-   0        0        0     3105 2022-11-22 00:41:33.000000 i2x-1.0.2/src/i2x/models/ieee9500/Master-unbal-initial-config.dss
+-rw-rw-rw-   0        0        0  4120960 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/models/ieee9500/Network.json
+-rw-rw-rw-   0        0        0  4383678 2022-12-21 15:25:32.000000 i2x-1.0.2/src/i2x/models/ieee9500/PNNL-33471.pdf
+-rw-rw-rw-   0        0        0     7444 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss
+-rw-rw-rw-   0        0        0     6724 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss
+-rw-rw-rw-   0        0        0     2566 2023-01-23 21:37:50.000000 i2x-1.0.2/src/i2x/models/ieee9500/README.md
+-rw-rw-rw-   0        0        0     3735 2023-01-09 14:46:11.000000 i2x-1.0.2/src/i2x/models/ieee9500/Regulators.dss
+-rw-rw-rw-   0        0        0     4728 2023-01-09 17:53:54.000000 i2x-1.0.2/src/i2x/models/ieee9500/Transformers.dss
+-rw-rw-rw-   0        0        0      786 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/TriplexLineCodes.dss
+-rw-rw-rw-   0        0        0   139322 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/TriplexLines.dss
+-rw-rw-rw-   0        0        0   361982 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/UnbalancedLoads.dss
+-rw-rw-rw-   0        0        0    15618 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/WireData.dss
+-rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.2/src/i2x/models/ieee9500/clean.bat
+-rw-rw-rw-   0        0        0       40 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/ieee9500bal.dss
+-rw-rw-rw-   0        0        0       42 2022-11-21 21:45:09.000000 i2x-1.0.2/src/i2x/models/ieee9500/ieee9500unbal.dss
+-rw-rw-rw-   0        0        0     5190 2023-06-01 15:55:15.000000 i2x-1.0.2/src/i2x/models/ieee9500/protection.dss
+-rw-rw-rw-   0        0        0     2801 2023-06-01 15:55:15.000000 i2x-1.0.2/src/i2x/models/ieee9500/reclosers.dss
+-rw-rw-rw-   0        0        0     1082 2023-06-01 15:55:15.000000 i2x-1.0.2/src/i2x/models/ieee9500/switches.dss
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:55.032208 i2x-1.0.2/src/i2x/models/ieee_lvn/
+-rw-rw-rw-   0        0        0      835 2023-06-07 17:26:09.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/HCABase.dss
+-rw-rw-rw-   0        0        0   164108 2023-01-07 23:18:01.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/Master.dss
+-rw-rw-rw-   0        0        0   316030 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/Network.json
+-rw-rw-rw-   0        0        0      878 2023-01-23 21:38:04.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/README.md
+-rw-rw-rw-   0        0        0    87814 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/SecPar.dss
+-rw-rw-rw-   0        0        0     6023 2023-01-07 23:18:01.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/buscoords.dat
+-rwxrwxrwx   0        0        0       60 2023-01-27 04:35:54.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/clean.bat
+-rw-rw-rw-   0        0        0     6555 2023-01-07 23:18:01.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/energy_meters.dss
+-rw-rw-rw-   0        0        0    12451 2023-01-07 23:18:01.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/network_protectors.dss
+-rw-rw-rw-   0        0        0     7153 2023-02-05 01:47:30.000000 i2x-1.0.2/src/i2x/models/ieee_lvn/network_protectors_reverse.dss
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:55.045189 i2x-1.0.2/src/i2x/models/radial/
+-rw-rw-rw-   0        0        0     2004 2023-06-06 18:08:43.000000 i2x-1.0.2/src/i2x/models/radial/Buscoords.dat
+-rw-rw-rw-   0        0        0    17839 2023-06-07 17:25:47.000000 i2x-1.0.2/src/i2x/models/radial/HCABase.dss
+-rw-rw-rw-   0        0        0    81691 2023-06-06 20:08:13.000000 i2x-1.0.2/src/i2x/models/radial/Network.json
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:55.075092 i2x-1.0.2/src/i2x/models/support/
+-rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/models/support/cdaily.dat
+-rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/models/support/ldaily.dat
+-rw-rw-rw-   0        0        0     2666 2023-06-07 17:33:16.000000 i2x-1.0.2/src/i2x/models/support/loadshapes_and_xycurves.dss
+-rw-rw-rw-   0        0        0   512867 2022-11-30 15:56:42.000000 i2x-1.0.2/src/i2x/models/support/pclear.dat
+-rw-rw-rw-   0        0        0   337498 2022-11-30 15:56:42.000000 i2x-1.0.2/src/i2x/models/support/pcloud.dat
+-rw-rw-rw-   0        0        0    36988 2022-11-30 15:56:42.000000 i2x-1.0.2/src/i2x/models/support/pvloadshape-1sec-2900pts.dat
+-rw-rw-rw-   0        0        0   691208 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/models/support/qdaily.dat
+-rw-rw-rw-   0        0        0    16020 2023-06-06 18:30:36.000000 i2x-1.0.2/src/i2x/opendss_graph.py
+-rw-rw-rw-   0        0        0    14526 2023-06-05 21:59:21.000000 i2x-1.0.2/src/i2x/opendss_interface.py
+-rw-rw-rw-   0        0        0     1134 2023-06-07 16:46:17.000000 i2x-1.0.2/src/i2x/pcc_analysis.py
+-rw-rw-rw-   0        0        0    13958 2023-06-06 22:31:15.000000 i2x-1.0.2/src/i2x/plot_opendss_feeder.py
+-rw-rw-rw-   0        0        0       23 2023-06-07 18:40:39.000000 i2x-1.0.2/src/i2x/version.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:41:54.878043 i2x-1.0.2/src/i2x.egg-info/
+-rw-rw-rw-   0        0        0     3372 2023-06-07 18:41:54.000000 i2x-1.0.2/src/i2x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-06-07 18:41:54.000000 i2x-1.0.2/src/i2x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 18:41:54.000000 i2x-1.0.2/src/i2x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 18:41:54.000000 i2x-1.0.2/src/i2x.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-01-23 20:58:26.000000 i2x-1.0.2/src/i2x.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       75 2023-06-07 18:41:54.000000 i2x-1.0.2/src/i2x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-07 18:41:54.000000 i2x-1.0.2/src/i2x.egg-info/top_level.txt
```

### Comparing `i2x-1.0.1/LICENSE.txt` & `i2x-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/PKG-INFO` & `i2x-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2x
-Version: 1.0.1
+Version: 1.0.2
 Summary: i2x: Interconnection Innovation e-Xchange Open Test Systems.
 Home-page: https://github.com/pnnl/i2x
 Author: Tom McDermott, Eran Schweitzer, and Jessica Kerby
 Author-email: Thomas.McDermott@PNNL.gov
 License: BSD
 Project-URL: Bug Tracker, https://github.com/pnnl/i2x/issues
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `i2x-1.0.1/README.md` & `i2x-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/setup.cfg` & `i2x-1.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,17 @@
 00000400: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
 00000410: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
 00000420: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
 00000430: 6174 615d 0d0a 2a20 3d20 6d6f 6465 6c73  ata]..* = models
 00000440: 2f73 7570 706f 7274 2f2a 2e2a 2c20 6d6f  /support/*.*, mo
 00000450: 6465 6c73 2f69 6565 6539 3530 302f 2a2e  dels/ieee9500/*.
 00000460: 2a2c 206d 6f64 656c 732f 6965 6565 5f6c  *, models/ieee_l
-00000470: 766e 2f2a 2e2a 0d0a 0d0a 5b6f 7074 696f  vn/*.*....[optio
-00000480: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000490: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-000004a0: 7320 3d20 0d0a 0969 3278 2d64 6572 203d  s = ...i2x-der =
-000004b0: 2069 3278 2e61 7069 3a73 686f 775f 6465   i2x.api:show_de
-000004c0: 725f 636f 6e66 6967 0d0a 0d0a 5b65 6767  r_config....[egg
-000004d0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000004e0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004f0: 2030 0d0a 0d0a                            0....
+00000470: 766e 2f2a 2e2a 2c20 6d6f 6465 6c73 2f72  vn/*.*, models/r
+00000480: 6164 6961 6c2f 2a2e 2a0d 0a0d 0a5b 6f70  adial/*.*....[op
+00000490: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000004a0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000004b0: 6970 7473 203d 200d 0a09 6932 782d 6465  ipts = ...i2x-de
+000004c0: 7220 3d20 6932 782e 6170 693a 7368 6f77  r = i2x.api:show
+000004d0: 5f64 6572 5f63 6f6e 6669 670d 0a0d 0a5b  _der_config....[
+000004e0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000004f0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000500: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `i2x-1.0.1/src/i2x/api.py` & `i2x-1.0.2/src/i2x/api.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/der_choices.py` & `i2x-1.0.2/src/i2x/der_choices.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/der_monitor.py` & `i2x-1.0.2/src/i2x/der_monitor.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/der_panel.py` & `i2x-1.0.2/src/i2x/der_panel.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/BalancedLoads.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/BalancedLoads.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/BusCoords.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/BusCoords.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/CapControls.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/CapControls.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Capacitors.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/Capacitors.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Generators.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/Generators.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/HCABase.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/HCABase.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/LatLongCoords.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/LatLongCoords.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/LineCodes.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/LineCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/LineGeometry.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/LineGeometry.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/LinesSwitchesGeometry.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/LinesSwitchesLineCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/LoadXfmrCodes.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/LoadXfmrCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Master-bal-initial-config.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/Master-bal-initial-config.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Master-unbal-initial-config.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/Master-unbal-initial-config.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Network.json` & `i2x-1.0.2/src/i2x/models/ieee9500/Network.json`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/PNNL-33471.pdf` & `i2x-1.0.2/src/i2x/models/ieee9500/PNNL-33471.pdf`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/PV_10pen_DSSPV.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/PV_NN_100_DSSPV.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/README.md` & `i2x-1.0.2/src/i2x/models/ieee9500/README.md`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Regulators.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/Regulators.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/Transformers.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/Transformers.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/TriplexLineCodes.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/TriplexLineCodes.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/TriplexLines.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/TriplexLines.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/UnbalancedLoads.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/UnbalancedLoads.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/WireData.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/WireData.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/protection.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/protection.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/reclosers.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/reclosers.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee9500/switches.dss` & `i2x-1.0.2/src/i2x/models/ieee9500/switches.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/HCABase.dss` & `i2x-1.0.2/src/i2x/models/ieee_lvn/HCABase.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/Master.dss` & `i2x-1.0.2/src/i2x/models/ieee_lvn/Master.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/Network.json` & `i2x-1.0.2/src/i2x/models/ieee_lvn/Network.json`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/README.md` & `i2x-1.0.2/src/i2x/models/ieee_lvn/README.md`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/SecPar.dss` & `i2x-1.0.2/src/i2x/models/ieee_lvn/SecPar.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/buscoords.dat` & `i2x-1.0.2/src/i2x/models/ieee_lvn/buscoords.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/energy_meters.dss` & `i2x-1.0.2/src/i2x/models/ieee_lvn/energy_meters.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors.dss` & `i2x-1.0.2/src/i2x/models/ieee_lvn/network_protectors.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/ieee_lvn/network_protectors_reverse.dss` & `i2x-1.0.2/src/i2x/models/ieee_lvn/network_protectors_reverse.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/cdaily.dat` & `i2x-1.0.2/src/i2x/models/support/cdaily.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/ldaily.dat` & `i2x-1.0.2/src/i2x/models/support/ldaily.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/loadshapes_and_xycurves.dss` & `i2x-1.0.2/src/i2x/models/support/loadshapes_and_xycurves.dss`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/pclear.dat` & `i2x-1.0.2/src/i2x/models/support/pclear.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/pcloud.dat` & `i2x-1.0.2/src/i2x/models/support/pcloud.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/pvloadshape-1sec-2900pts.dat` & `i2x-1.0.2/src/i2x/models/support/pvloadshape-1sec-2900pts.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/models/support/qdaily.dat` & `i2x-1.0.2/src/i2x/models/support/qdaily.dat`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/opendss_graph.py` & `i2x-1.0.2/src/i2x/opendss_graph.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/opendss_interface.py` & `i2x-1.0.2/src/i2x/opendss_interface.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/pcc_analysis.py` & `i2x-1.0.2/src/i2x/pcc_analysis.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x/plot_opendss_feeder.py` & `i2x-1.0.2/src/i2x/plot_opendss_feeder.py`

 * *Files identical despite different names*

### Comparing `i2x-1.0.1/src/i2x.egg-info/PKG-INFO` & `i2x-1.0.2/src/i2x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2x
-Version: 1.0.1
+Version: 1.0.2
 Summary: i2x: Interconnection Innovation e-Xchange Open Test Systems.
 Home-page: https://github.com/pnnl/i2x
 Author: Tom McDermott, Eran Schweitzer, and Jessica Kerby
 Author-email: Thomas.McDermott@PNNL.gov
 License: BSD
 Project-URL: Bug Tracker, https://github.com/pnnl/i2x/issues
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `i2x-1.0.1/src/i2x.egg-info/SOURCES.txt` & `i2x-1.0.2/src/i2x.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 src/i2x/models/ieee_lvn/README.md
 src/i2x/models/ieee_lvn/SecPar.dss
 src/i2x/models/ieee_lvn/buscoords.dat
 src/i2x/models/ieee_lvn/clean.bat
 src/i2x/models/ieee_lvn/energy_meters.dss
 src/i2x/models/ieee_lvn/network_protectors.dss
 src/i2x/models/ieee_lvn/network_protectors_reverse.dss
+src/i2x/models/radial/Buscoords.dat
+src/i2x/models/radial/HCABase.dss
+src/i2x/models/radial/Network.json
 src/i2x/models/support/cdaily.dat
 src/i2x/models/support/ldaily.dat
 src/i2x/models/support/loadshapes_and_xycurves.dss
 src/i2x/models/support/pclear.dat
 src/i2x/models/support/pcloud.dat
 src/i2x/models/support/pvloadshape-1sec-2900pts.dat
 src/i2x/models/support/qdaily.dat
```

