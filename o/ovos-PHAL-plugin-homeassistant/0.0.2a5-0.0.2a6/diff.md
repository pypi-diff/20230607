# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a5.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a5.tar", last modified: Wed May 31 20:14:30 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a6.tar", last modified: Tue Jun  6 23:07:20 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5.tar` & `ovos-PHAL-plugin-homeassistant-0.0.2a6.tar`

### file list

```diff
@@ -1,22 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 20:14:22.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.835793 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.220246 ovos-PHAL-plugin-homeassistant-0.0.2a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.204246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.212246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.212246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.212246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.204246 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:07:20.220246 ovos-PHAL-plugin-homeassistant-0.0.2a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a5/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a6/setup.py`

 * *Files identical despite different names*

