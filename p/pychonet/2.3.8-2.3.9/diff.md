# Comparing `tmp/pychonet-2.3.8.tar.gz` & `tmp/pychonet-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pychonet-2.3.8.tar", last modified: Fri Sep 30 15:15:03 2022, max compression
+gzip compressed data, was "dist/pychonet-2.3.9.tar", last modified: Thu Oct  6 12:05:22 2022, max compression
```

## Comparing `pychonet-2.3.8.tar` & `pychonet-2.3.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-09-30 15:15:03.763047 pychonet-2.3.8/
--rwxr--r--   0 vaio       (500) vaio       (500)     2601 2022-09-30 14:47:09.000000 pychonet-2.3.8/CHANGES.txt
--rw-r--r--   0 vaio       (500) vaio       (500)       56 2022-06-17 04:53:25.000000 pychonet-2.3.8/MANIFEST.in
--rw-r--r--   0 vaio       (500) vaio       (500)     7010 2022-09-30 15:15:03.763047 pychonet-2.3.8/PKG-INFO
--rw-r--r--   0 vaio       (500) vaio       (500)     5406 2022-09-02 00:16:39.000000 pychonet-2.3.8/README.md
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-09-30 15:15:03.761047 pychonet-2.3.8/pychonet/
--rwxr--r--   0 vaio       (500) vaio       (500)     5634 2022-09-26 07:33:30.000000 pychonet-2.3.8/pychonet/DistributionPanelMeter.py
--rwxr--r--   0 vaio       (500) vaio       (500)     9846 2022-09-02 05:40:23.000000 pychonet-2.3.8/pychonet/EchonetInstance.py
--rw-r--r--   0 vaio       (500) vaio       (500)     1734 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/ElectricBlind.py
--rw-r--r--   0 vaio       (500) vaio       (500)      785 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/ElectricEnergyMeter.py
--rw-r--r--   0 vaio       (500) vaio       (500)     1941 2022-07-04 08:56:51.000000 pychonet-2.3.8/pychonet/ElectricLock.py
--rw-r--r--   0 vaio       (500) vaio       (500)      471 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/ElectricVehicleCharger.py
--rw-r--r--   0 vaio       (500) vaio       (500)      733 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/GasMeter.py
--rw-r--r--   0 vaio       (500) vaio       (500)     2926 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/GeneralLighting.py
--rw-r--r--   0 vaio       (500) vaio       (500)     3592 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/HomeAirCleaner.py
--rwxr--r--   0 vaio       (500) vaio       (500)    11013 2022-09-26 07:13:17.000000 pychonet-2.3.8/pychonet/HomeAirConditioner.py
--rw-r--r--   0 vaio       (500) vaio       (500)     1599 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/HomeSolarPower.py
--rw-r--r--   0 vaio       (500) vaio       (500)     3970 2022-06-20 11:49:01.000000 pychonet-2.3.8/pychonet/HotWaterGenerator.py
--rw-r--r--   0 vaio       (500) vaio       (500)     2709 2022-06-20 11:49:01.000000 pychonet-2.3.8/pychonet/HybridWaterHeater.py
--rw-r--r--   0 vaio       (500) vaio       (500)      804 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/StorageBattery.py
--rw-r--r--   0 vaio       (500) vaio       (500)      599 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/TemperatureSensor.py
--rw-r--r--   0 vaio       (500) vaio       (500)     2076 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/WaterFlowMeter.py
--rw-r--r--   0 vaio       (500) vaio       (500)     1993 2022-09-03 01:09:18.000000 pychonet-2.3.8/pychonet/__init__.py
--rwxr--r--   0 vaio       (500) vaio       (500)     9884 2022-09-30 14:42:10.000000 pychonet-2.3.8/pychonet/echonetapiclient.py
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-09-30 15:15:03.763047 pychonet-2.3.8/pychonet/lib/
--rw-r--r--   0 vaio       (500) vaio       (500)        0 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/lib/__init__.py
--rwxr--r--   0 vaio       (500) vaio       (500)     9490 2022-09-25 05:29:36.000000 pychonet-2.3.8/pychonet/lib/const.py
--rw-r--r--   0 vaio       (500) vaio       (500)     8031 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/lib/eojx.py
--rw-r--r--   0 vaio       (500) vaio       (500)    66754 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/lib/epc.py
--rw-r--r--   0 vaio       (500) vaio       (500)     3726 2022-07-16 05:23:39.000000 pychonet-2.3.8/pychonet/lib/epc_functions.py
--rw-r--r--   0 vaio       (500) vaio       (500)     3686 2022-06-17 04:53:25.000000 pychonet-2.3.8/pychonet/lib/functions.py
--rw-r--r--   0 vaio       (500) vaio       (500)     3907 2022-07-18 01:15:36.000000 pychonet-2.3.8/pychonet/lib/udpserver.py
--rwxr--r--   0 vaio       (500) vaio       (500)       80 2022-09-30 14:47:16.000000 pychonet-2.3.8/pychonet/version.py
-drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-09-30 15:15:03.762047 pychonet-2.3.8/pychonet.egg-info/
--rw-r--r--   0 vaio       (500) vaio       (500)     7010 2022-09-30 15:15:03.000000 pychonet-2.3.8/pychonet.egg-info/PKG-INFO
--rw-r--r--   0 vaio       (500) vaio       (500)      879 2022-09-30 15:15:03.000000 pychonet-2.3.8/pychonet.egg-info/SOURCES.txt
--rw-r--r--   0 vaio       (500) vaio       (500)        1 2022-09-30 15:15:03.000000 pychonet-2.3.8/pychonet.egg-info/dependency_links.txt
--rw-r--r--   0 vaio       (500) vaio       (500)        9 2022-09-30 15:15:03.000000 pychonet-2.3.8/pychonet.egg-info/top_level.txt
--rw-r--r--   0 vaio       (500) vaio       (500)      265 2022-09-30 15:15:03.764047 pychonet-2.3.8/setup.cfg
--rw-r--r--   0 vaio       (500) vaio       (500)      625 2022-09-03 01:09:18.000000 pychonet-2.3.8/setup.py
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-10-06 12:05:22.138416 pychonet-2.3.9/
+-rwxr--r--   0 vaio       (500) vaio       (500)     2703 2022-10-06 11:48:58.000000 pychonet-2.3.9/CHANGES.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)       56 2022-06-17 04:53:25.000000 pychonet-2.3.9/MANIFEST.in
+-rw-r--r--   0 vaio       (500) vaio       (500)     7549 2022-10-06 12:05:22.138416 pychonet-2.3.9/PKG-INFO
+-rw-r--r--   0 vaio       (500) vaio       (500)     5897 2022-10-01 13:10:27.000000 pychonet-2.3.9/README.md
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-10-06 12:05:22.135416 pychonet-2.3.9/pychonet/
+-rwxr--r--   0 vaio       (500) vaio       (500)     5634 2022-09-26 07:33:30.000000 pychonet-2.3.9/pychonet/DistributionPanelMeter.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     9845 2022-10-03 13:56:41.000000 pychonet-2.3.9/pychonet/EchonetInstance.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     1734 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/ElectricBlind.py
+-rw-r--r--   0 vaio       (500) vaio       (500)      785 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/ElectricEnergyMeter.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     1941 2022-07-04 08:56:51.000000 pychonet-2.3.9/pychonet/ElectricLock.py
+-rw-r--r--   0 vaio       (500) vaio       (500)      471 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/ElectricVehicleCharger.py
+-rw-r--r--   0 vaio       (500) vaio       (500)      733 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/GasMeter.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     2926 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/GeneralLighting.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     3592 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/HomeAirCleaner.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    11013 2022-09-26 07:13:17.000000 pychonet-2.3.9/pychonet/HomeAirConditioner.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     1599 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/HomeSolarPower.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     3970 2022-06-20 11:49:01.000000 pychonet-2.3.9/pychonet/HotWaterGenerator.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     2709 2022-06-20 11:49:01.000000 pychonet-2.3.9/pychonet/HybridWaterHeater.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     5122 2022-10-06 11:16:27.000000 pychonet-2.3.9/pychonet/LowVoltageSmartElectricEnergyMeter.py
+-rw-r--r--   0 vaio       (500) vaio       (500)      804 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/StorageBattery.py
+-rw-r--r--   0 vaio       (500) vaio       (500)      599 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/TemperatureSensor.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     2076 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/WaterFlowMeter.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     2138 2022-10-03 08:45:58.000000 pychonet-2.3.9/pychonet/__init__.py
+-rwxr--r--   0 vaio       (500) vaio       (500)    10665 2022-10-01 12:57:46.000000 pychonet-2.3.9/pychonet/echonetapiclient.py
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-10-06 12:05:22.137416 pychonet-2.3.9/pychonet/lib/
+-rw-r--r--   0 vaio       (500) vaio       (500)        0 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/lib/__init__.py
+-rwxr--r--   0 vaio       (500) vaio       (500)     9490 2022-09-25 05:29:36.000000 pychonet-2.3.9/pychonet/lib/const.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     8031 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/lib/eojx.py
+-rw-r--r--   0 vaio       (500) vaio       (500)    66754 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/lib/epc.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     3726 2022-07-16 05:23:39.000000 pychonet-2.3.9/pychonet/lib/epc_functions.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     3686 2022-06-17 04:53:25.000000 pychonet-2.3.9/pychonet/lib/functions.py
+-rw-r--r--   0 vaio       (500) vaio       (500)     4144 2022-10-06 11:46:34.000000 pychonet-2.3.9/pychonet/lib/udpserver.py
+-rwxr--r--   0 vaio       (500) vaio       (500)       80 2022-10-06 12:00:12.000000 pychonet-2.3.9/pychonet/version.py
+drwxr-xr-x   0 vaio       (500) vaio       (500)        0 2022-10-06 12:05:22.136416 pychonet-2.3.9/pychonet.egg-info/
+-rw-r--r--   0 vaio       (500) vaio       (500)     7549 2022-10-06 12:05:21.000000 pychonet-2.3.9/pychonet.egg-info/PKG-INFO
+-rw-r--r--   0 vaio       (500) vaio       (500)      926 2022-10-06 12:05:21.000000 pychonet-2.3.9/pychonet.egg-info/SOURCES.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)        1 2022-10-06 12:05:21.000000 pychonet-2.3.9/pychonet.egg-info/dependency_links.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)        9 2022-10-06 12:05:21.000000 pychonet-2.3.9/pychonet.egg-info/top_level.txt
+-rw-r--r--   0 vaio       (500) vaio       (500)      265 2022-10-06 12:05:22.139416 pychonet-2.3.9/setup.cfg
+-rw-r--r--   0 vaio       (500) vaio       (500)      625 2022-09-03 01:09:18.000000 pychonet-2.3.9/setup.py
```

### Comparing `pychonet-2.3.8/CHANGES.txt` & `pychonet-2.3.9/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,7 +29,8 @@
 v2.3.2, 30 Jul 2022 -- Discover process optimization and request success/failure detection.
 v2.3.3, 03 Aug 2022 -- Fixed a bug in judging the success or failure of the data set request.
 v2.3.4, 04 Aug 2022 -- Fix data handling issues in process_discovery_data().
 v2.3.5, 25 Sep 2022 -- Ignore not-yet-supported notifications of node profile class.
 v2.3.6, 26 Sep 2022 -- Added some ENL codes for HomeAirConditioner and DistributionPanelMeter.
 v2.3.7, 28 Sep 2022 -- Added _discover_callback to echonetapiclient.
 v2.3.8, 30 Sep 2022 -- Bug fix of calling _discover_callback().
+v2.3.9, 06 Aug 2022 -- Added LowVoltageSmartElectricEnergyMeter, Create a another socket for sending.
```

### Comparing `pychonet-2.3.8/PKG-INFO` & `pychonet-2.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychonet
-Version: 2.3.8
+Version: 2.3.9
 Summary: A library for interfacing via the ECHONETlite protocol.
 Home-page: http://pypi.python.org/pypi/pychonet/
 Author: Scott Phillips
 Author-email: scotty.phillips@hotmail.com
 License: LICENSE.txt
 Description: # Pychonet
         
@@ -141,14 +141,20 @@
         Thanks to Jeffro Carr who inspired me to write my own native Python ECHONET
         library for Home Assistant.
         
         Thanks to Futomi Hatano for open sourcing a well-documented ECHONET Lite
         library in Node JS.
         (https://github.com/futomi/node-echonet-lite)
         
+        ## References for ECHONET specifications
+        
+        - [ECHONET Lite Specification, Version 1.13](https://echonet.jp/spec_v113_lite_en/)
+          - [Part 2 ECHONET Lite Communications Middleware Specifications](https://echonet.jp/wp/wp-content/uploads/pdf/General/Standard/ECHONET_lite_V1_13_en/ECHONET-Lite_Ver.1.13(02)_E.pdf)
+        - [APPENDIX, Detailed Requirements for ECHONET Device objects, Release Q](https://echonet.jp/wp/wp-content/uploads/pdf/General/Standard/Release/Release_Q/Appendix_Release_Q_E.pdf)
+        
         ## License
         
         This application is licensed under an MIT license, refer to LICENSE-MIT for details.
         
         Portions of 'ECHONET Lite Device Emulator' (Copyright 2020 Kanagawa Institute of Technology)
         have been used in this application. This code was licensed under the MIT licence.
```

### Comparing `pychonet-2.3.8/README.md` & `pychonet-2.3.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -133,14 +133,20 @@
 Thanks to Jeffro Carr who inspired me to write my own native Python ECHONET
 library for Home Assistant.
 
 Thanks to Futomi Hatano for open sourcing a well-documented ECHONET Lite
 library in Node JS.
 (https://github.com/futomi/node-echonet-lite)
 
+## References for ECHONET specifications
+
+- [ECHONET Lite Specification, Version 1.13](https://echonet.jp/spec_v113_lite_en/)
+  - [Part 2 ECHONET Lite Communications Middleware Specifications](https://echonet.jp/wp/wp-content/uploads/pdf/General/Standard/ECHONET_lite_V1_13_en/ECHONET-Lite_Ver.1.13(02)_E.pdf)
+- [APPENDIX, Detailed Requirements for ECHONET Device objects, Release Q](https://echonet.jp/wp/wp-content/uploads/pdf/General/Standard/Release/Release_Q/Appendix_Release_Q_E.pdf)
+
 ## License
 
 This application is licensed under an MIT license, refer to LICENSE-MIT for details.
 
 Portions of 'ECHONET Lite Device Emulator' (Copyright 2020 Kanagawa Institute of Technology)
 have been used in this application. This code was licensed under the MIT licence.
```

### Comparing `pychonet-2.3.8/pychonet/DistributionPanelMeter.py` & `pychonet-2.3.9/pychonet/DistributionPanelMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/EchonetInstance.py` & `pychonet-2.3.9/pychonet/EchonetInstance.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         if response is not False:
             for epc in attributes:
                 if epc not in list(
                     self._api._state[self._host]["instances"][self._eojgc][self._eojcc][
                         self._eojci
                     ].keys()
                 ):
-                    returned_json_data.update({epc: False})
+                    returned_json_data.update({epc: None})
                     continue
                 elif epc in list(
                     EPC_SUPER_FUNCTIONS.keys()
                 ):  # check if function is defined in the superset
                     returned_json_data.update(
                         {
                             epc: EPC_SUPER_FUNCTIONS[epc](
```

### Comparing `pychonet-2.3.8/pychonet/ElectricBlind.py` & `pychonet-2.3.9/pychonet/ElectricBlind.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/ElectricEnergyMeter.py` & `pychonet-2.3.9/pychonet/ElectricEnergyMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/ElectricLock.py` & `pychonet-2.3.9/pychonet/ElectricLock.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/GasMeter.py` & `pychonet-2.3.9/pychonet/GasMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/GeneralLighting.py` & `pychonet-2.3.9/pychonet/GeneralLighting.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/HomeAirCleaner.py` & `pychonet-2.3.9/pychonet/HomeAirCleaner.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/HomeAirConditioner.py` & `pychonet-2.3.9/pychonet/HomeAirConditioner.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/HomeSolarPower.py` & `pychonet-2.3.9/pychonet/HomeSolarPower.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/HotWaterGenerator.py` & `pychonet-2.3.9/pychonet/HotWaterGenerator.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/HybridWaterHeater.py` & `pychonet-2.3.9/pychonet/HybridWaterHeater.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/StorageBattery.py` & `pychonet-2.3.9/pychonet/StorageBattery.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/TemperatureSensor.py` & `pychonet-2.3.9/pychonet/TemperatureSensor.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/WaterFlowMeter.py` & `pychonet-2.3.9/pychonet/WaterFlowMeter.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/__init__.py` & `pychonet-2.3.9/pychonet/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .GeneralLighting import GeneralLighting
 from .HomeAirCleaner import HomeAirCleaner
 from .HomeAirConditioner import HomeAirConditioner
 from .HomeSolarPower import HomeSolarPower
 from .StorageBattery import StorageBattery
 from .TemperatureSensor import TemperatureSensor
 from .DistributionPanelMeter import DistributionPanelMeter
+from .LowVoltageSmartElectricEnergyMeter import LowVoltageSmartElectricEnergyMeter
 from .HybridWaterHeater import HybridWaterHeater
 from .HotWaterGenerator import HotWaterGenerator
 from .GasMeter import GasMeter
 from .ElectricEnergyMeter import ElectricEnergyMeter
 from .WaterFlowMeter import WaterFlowMeter
 
 
@@ -37,14 +38,15 @@
         f"{0x02}-{0x79}": HomeSolarPower,
         f"{0x02}-{0x7D}": StorageBattery,
         f"{0x02}-{0x7E}": ElectricVehicleCharger,
         f"{0x02}-{0x80}": ElectricEnergyMeter,
         f"{0x02}-{0x81}": WaterFlowMeter,
         f"{0x02}-{0x82}": GasMeter,
         f"{0x02}-{0x87}": DistributionPanelMeter,
+        f"{0x02}-{0x88}": LowVoltageSmartElectricEnergyMeter,
         f"{0x02}-{0x90}": GeneralLighting,
         f"{0x02}-{0xA6}": HybridWaterHeater,
         None: None,
     }
     instance_object = instances.get(instance, None)
     if instance_object is not None:
         return instance_object(host, server, eojci)
```

### Comparing `pychonet-2.3.8/pychonet/echonetapiclient.py` & `pychonet-2.3.9/pychonet/echonetapiclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,31 @@
 
         key = f"{host}-{seojgc}-{seojcc}-{seojci}"
         esv_set = esv in [SETRES, SETC_SND]
         esv_get = esv in [GETRES, GET_SNA, INF, INF_SNA, INFC]
         # handle discovery message response
         for opc in processed_data["OPC"]:
             epc = opc["EPC"]
-            if seojgc == 0x0E and seojcc == 0xF0:
+            if seojgc == 0x0E and seojcc == 0xF0: # Node Profile Class Response
                 if (epc in [INSTANCE_LIST, ENL_MANUFACTURER, ENL_UID]): # process discovery data
                     await self.process_discovery_data(host, opc)
                 else:
-                    # @todo handling others (0x05: Notify of change instance list, etc...)
+                    # @todo handling others
+                    '''
+                    Ex. 0x05: Instance list notification
+                    A property to announce the configuration of instances to be disclosed to the network at startup.
+                    This property also announces instances held at the self-node each time the configuration of
+                    instances disclosed to the network is changed during system operation, such as instance
+                    addition or deletion.
+                    '''
+                    '''
+                    It is desirable to dynamically add and delete entities when there is an increase
+                    or decrease in the number of instances within a device already configured with HA,
+                    but that will be an issue for the future.
+                    '''
                     continue
             else: # process each EPC in order
                 if epc == ENL_SETMAP or epc == ENL_GETMAP or epc == ENL_STATMAP:
                     map = EPC_SUPER_FUNCTIONS[epc](opc["EDT"])
                     self._state[host]["instances"][seojgc][seojcc][seojci][epc] = map
                 elif epc in (ENL_UID, ENL_MANUFACTURER):
                     self._state[host]["instances"][seojgc][seojcc][seojci][
```

### Comparing `pychonet-2.3.8/pychonet/lib/const.py` & `pychonet-2.3.9/pychonet/lib/const.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/lib/eojx.py` & `pychonet-2.3.9/pychonet/lib/eojx.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/lib/epc.py` & `pychonet-2.3.9/pychonet/lib/epc.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/lib/epc_functions.py` & `pychonet-2.3.9/pychonet/lib/epc_functions.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/lib/functions.py` & `pychonet-2.3.9/pychonet/lib/functions.py`

 * *Files identical despite different names*

### Comparing `pychonet-2.3.8/pychonet/lib/udpserver.py` & `pychonet-2.3.9/pychonet/lib/udpserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
         self._download_speed = download_speed
         self._recv_max_size = recv_max_size
 
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, 0)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setblocking(False)
 
+        self._send_sock = None
+
         # enable multicast
         mreq = struct.pack("=4sl", socket.inet_aton("224.0.23.0"), socket.INADDR_ANY)
         self._sock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
 
         self._send_event = asyncio.Event()
         self._send_queue = deque()
 
@@ -70,35 +72,41 @@
             self._socket_error(e)
         else:
             fut.set_result((data, addr))
 
         return fut
 
     def _sock_send(self, data, addr, fut=None, registered=False):
-        fd = self._sock.fileno()
+        if registered == False:
+            self._send_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, 0)
+            self._send_sock.setblocking(False)
+
+        fd = self._send_sock.fileno()
 
         if fut is None:
             fut = self.loop.create_future()
 
         if registered:
             self.loop.remove_writer(fd)
 
         if not data:
             return
 
         try:
-            bytes_sent = self._sock.sendto(data, addr)
+            bytes_sent = self._send_sock.sendto(data, addr)
         except (BlockingIOError, InterruptedError):
             self.loop.add_writer(fd, self._sock_send, data, addr, fut, True)
         except Exception as e:
             fut.set_exception(e)
             self._socket_error(e)
         else:
             fut.set_result(bytes_sent)
 
+        self._send_sock.close()
+
         return fut
 
     async def _throttle(self, data_len, speed=0):
         delay = (data_len / speed) if speed > 0 else 0
         await asyncio.sleep(delay)
 
     async def _send_periodically(self):
```

### Comparing `pychonet-2.3.8/pychonet.egg-info/PKG-INFO` & `pychonet-2.3.9/pychonet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychonet
-Version: 2.3.8
+Version: 2.3.9
 Summary: A library for interfacing via the ECHONETlite protocol.
 Home-page: http://pypi.python.org/pypi/pychonet/
 Author: Scott Phillips
 Author-email: scotty.phillips@hotmail.com
 License: LICENSE.txt
 Description: # Pychonet
         
@@ -141,14 +141,20 @@
         Thanks to Jeffro Carr who inspired me to write my own native Python ECHONET
         library for Home Assistant.
         
         Thanks to Futomi Hatano for open sourcing a well-documented ECHONET Lite
         library in Node JS.
         (https://github.com/futomi/node-echonet-lite)
         
+        ## References for ECHONET specifications
+        
+        - [ECHONET Lite Specification, Version 1.13](https://echonet.jp/spec_v113_lite_en/)
+          - [Part 2 ECHONET Lite Communications Middleware Specifications](https://echonet.jp/wp/wp-content/uploads/pdf/General/Standard/ECHONET_lite_V1_13_en/ECHONET-Lite_Ver.1.13(02)_E.pdf)
+        - [APPENDIX, Detailed Requirements for ECHONET Device objects, Release Q](https://echonet.jp/wp/wp-content/uploads/pdf/General/Standard/Release/Release_Q/Appendix_Release_Q_E.pdf)
+        
         ## License
         
         This application is licensed under an MIT license, refer to LICENSE-MIT for details.
         
         Portions of 'ECHONET Lite Device Emulator' (Copyright 2020 Kanagawa Institute of Technology)
         have been used in this application. This code was licensed under the MIT licence.
```

### Comparing `pychonet-2.3.8/setup.py` & `pychonet-2.3.9/setup.py`

 * *Files identical despite different names*

