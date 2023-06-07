# Comparing `tmp/piksi_tools-3.1.4-py2.py3-none-any.whl.zip` & `tmp/piksi_tools-4.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,87 +1,28 @@
-Zip file size: 197391 bytes, number of entries: 85
--rw-r--r--  2.0 unx      599 b- defN 21-Mar-03 20:19 piksi_tools/__init__.py
--rw-r--r--  2.0 unx      117 b- defN 21-Oct-13 23:13 piksi_tools/_version.py
--rw-r--r--  2.0 unx     1008 b- defN 21-Mar-03 20:19 piksi_tools/acq_plot.py
--rw-r--r--  2.0 unx     4285 b- defN 21-Mar-03 20:19 piksi_tools/acq_results.py
--rw-r--r--  2.0 unx    10428 b- defN 21-Mar-03 20:19 piksi_tools/action_logger.py
--rw-r--r--  2.0 unx     6577 b- defN 21-Mar-03 20:19 piksi_tools/almanac.py
--rw-r--r--  2.0 unx     3528 b- defN 21-Mar-03 20:19 piksi_tools/bootload_v3.py
--rw-r--r--  2.0 unx     8090 b- defN 21-Mar-03 20:19 piksi_tools/diagnostics.py
--rw-r--r--  2.0 unx    27969 b- defN 21-Oct-13 23:11 piksi_tools/fileio.py
--rw-r--r--  2.0 unx     1070 b- defN 21-Mar-03 20:19 piksi_tools/heartbeat.py
--rw-r--r--  2.0 unx    14588 b- defN 21-Aug-25 00:02 piksi_tools/interpolate_event_positions.py
--rw-r--r--  2.0 unx     1238 b- defN 21-Mar-03 20:19 piksi_tools/log_wrapper.py
--rw-r--r--  2.0 unx     2765 b- defN 21-Mar-03 20:19 piksi_tools/recover_ftdi.py
--rw-r--r--  2.0 unx     4859 b- defN 21-Aug-25 00:02 piksi_tools/sbp_msg_2_csv.py
--rw-r--r--  2.0 unx     1578 b- defN 21-Mar-03 20:19 piksi_tools/sbpjson_expand.py
--rw-r--r--  2.0 unx    12345 b- defN 21-Mar-03 20:19 piksi_tools/serial_link.py
--rw-r--r--  2.0 unx    16300 b- defN 21-Sep-10 00:59 piksi_tools/settings.py
--rw-r--r--  2.0 unx     2406 b- defN 21-Mar-03 20:19 piksi_tools/simulator_almanac_generator.py
--rw-r--r--  2.0 unx     3902 b- defN 21-Mar-03 20:19 piksi_tools/stm_unique_id.py
--rw-r--r--  2.0 unx     1774 b- defN 21-Mar-03 20:19 piksi_tools/timeout.py
--rw-r--r--  2.0 unx     4489 b- defN 21-Mar-03 20:19 piksi_tools/utils.py
--rw-r--r--  2.0 unx      496 b- defN 21-Mar-03 20:19 piksi_tools/ardupilot/__init__.py
--rw-r--r--  2.0 unx     2546 b- defN 21-Sep-10 00:59 piksi_tools/ardupilot/mavlink2pandas.py
--rw-r--r--  2.0 unx    13304 b- defN 21-Mar-03 20:19 piksi_tools/ardupilot/mavlink_decode.py
--rw-r--r--  2.0 unx     3185 b- defN 21-Mar-03 20:19 piksi_tools/ardupilot/mavlink_split.py
--rw-r--r--  2.0 unx     2860 b- defN 21-Mar-03 20:19 piksi_tools/ardupilot/udp_bridge.py
--rw-r--r--  2.0 unx     1675 b- defN 21-Sep-10 00:59 piksi_tools/ardupilot/udp_receive.py
--rw-r--r--  2.0 unx     4649 b- defN 21-Mar-03 20:19 piksi_tools/console/GitVersion.py
--rw-r--r--  2.0 unx     2273 b- defN 21-Mar-03 20:19 piksi_tools/console/README.txt
--rw-r--r--  2.0 unx      496 b- defN 21-Mar-03 20:19 piksi_tools/console/__init__.py
--rw-r--r--  2.0 unx       37 b- defN 21-Mar-03 20:19 piksi_tools/console/__main__.py
--rw-r--r--  2.0 unx    20898 b- defN 21-Sep-10 00:59 piksi_tools/console/baseline_view.py
--rw-r--r--  2.0 unx     3908 b- defN 21-Mar-03 20:19 piksi_tools/console/callback_prompt.py
--rw-r--r--  2.0 unx    42496 b- defN 21-Oct-13 23:13 piksi_tools/console/console.py
--rw-r--r--  2.0 unx     2861 b- defN 21-Mar-03 20:19 piksi_tools/console/deprecated.py
--rw-r--r--  2.0 unx     4826 b- defN 21-Mar-17 22:34 piksi_tools/console/fusion_engine_status.py
--rw-r--r--  2.0 unx     2568 b- defN 21-Mar-03 20:19 piksi_tools/console/generate_settings.py
--rw-r--r--  2.0 unx     6145 b- defN 21-Mar-03 20:19 piksi_tools/console/gui_utils.py
--rw-r--r--  2.0 unx     6560 b- defN 21-Sep-10 00:59 piksi_tools/console/ins_view.py
--rw-r--r--  2.0 unx     3910 b- defN 21-Sep-10 00:59 piksi_tools/console/mag_view.py
--rw-r--r--  2.0 unx    12741 b- defN 21-Mar-03 20:19 piksi_tools/console/observation_view.py
--rw-r--r--  2.0 unx    10281 b- defN 21-Mar-03 20:19 piksi_tools/console/output_list.py
--rw-r--r--  2.0 unx     4486 b- defN 21-Mar-03 20:19 piksi_tools/console/output_stream.py
--rw-r--r--  2.0 unx     6405 b- defN 21-Mar-03 20:19 piksi_tools/console/port_chooser.py
--rw-r--r--  2.0 unx     8548 b- defN 21-Sep-10 00:59 piksi_tools/console/sbp_relay_view.py
--rw-r--r--  2.0 unx   100142 b- defN 21-Sep-10 00:59 piksi_tools/console/settings.yaml
--rw-r--r--  2.0 unx     2686 b- defN 21-Mar-03 20:19 piksi_tools/console/settings_list.py
--rw-r--r--  2.0 unx     2784 b- defN 21-Mar-03 20:19 piksi_tools/console/settings_template.tex
--rw-r--r--  2.0 unx    34769 b- defN 21-Sep-10 21:04 piksi_tools/console/settings_view.py
--rw-r--r--  2.0 unx    15816 b- defN 21-Mar-03 20:19 piksi_tools/console/skyplot_view.py
--rw-r--r--  2.0 unx    39398 b- defN 21-Sep-10 00:59 piksi_tools/console/solution_view.py
--rw-r--r--  2.0 unx     6818 b- defN 21-Mar-03 20:19 piksi_tools/console/spectrum_analyzer_view.py
--rw-r--r--  2.0 unx     8988 b- defN 21-Mar-03 20:19 piksi_tools/console/system_monitor_view.py
--rw-r--r--  2.0 unx    12546 b- defN 21-Mar-03 20:19 piksi_tools/console/tracking_view.py
--rw-r--r--  2.0 unx     2792 b- defN 21-Sep-10 00:59 piksi_tools/console/update_downloader.py
--rw-r--r--  2.0 unx    34693 b- defN 21-Sep-10 00:59 piksi_tools/console/update_view.py
--rw-r--r--  2.0 unx    15976 b- defN 21-Sep-10 00:59 piksi_tools/console/utils.py
--rw-r--r--  2.0 unx     5051 b- defN 21-Sep-10 00:59 piksi_tools/console/velocity_view.py
--rw-r--r--  2.0 unx     7525 b- defN 21-Mar-03 20:19 piksi_tools/console/images/icon.png
--rw-r--r--  2.0 unx     1081 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/LICENSE.txt
--rw-r--r--  2.0 unx     1420 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/README.md
--rw-r--r--  2.0 unx      634 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/download.svg
--rw-r--r--  2.0 unx      488 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/exclamation-triangle.svg
--rw-r--r--  2.0 unx      661 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/floppy-o.svg
--rwxr-xr-x  2.0 unx     2043 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/power27.svg
--rw-r--r--  2.0 unx      737 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/refresh.svg
--rw-r--r--  2.0 unx      740 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/refresh_blue.svg
--rw-r--r--  2.0 unx      290 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/stop.svg
--rw-r--r--  2.0 unx      580 b- defN 21-Mar-03 20:19 piksi_tools/console/images/fontawesome/upload.svg
--rw-r--r--  2.0 unx      591 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/AUTHORS
--rw-r--r--  2.0 unx    17262 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/LICENSE
--rw-r--r--  2.0 unx     1341 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/arrows_blue.png
--rw-r--r--  2.0 unx      533 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/arrows_grey.png
--rw-r--r--  2.0 unx      992 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/fullscreen.svg
--rw-r--r--  2.0 unx      884 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/move.svg
--rw-r--r--  2.0 unx      652 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/pause.svg
--rw-r--r--  2.0 unx      582 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/play.svg
--rw-r--r--  2.0 unx      576 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/stop.svg
--rw-r--r--  2.0 unx     1602 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/target.svg
--rw-r--r--  2.0 unx      694 b- defN 21-Mar-03 20:19 piksi_tools/console/images/iconic/x.svg
--rw-r--r--  2.0 unx     7651 b- defN 21-Oct-13 23:13 piksi_tools-3.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     5149 b- defN 21-Oct-13 23:13 piksi_tools-3.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Oct-13 23:13 piksi_tools-3.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 21-Oct-13 23:13 piksi_tools-3.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7867 b- defN 21-Oct-13 23:13 piksi_tools-3.1.4.dist-info/RECORD
-85 files, 643225 bytes uncompressed, 184747 bytes compressed:  71.3%
+Zip file size: 50848 bytes, number of entries: 26
+-rw-rw-r--  2.0 unx      599 b- defN 22-Feb-17 21:17 piksi_tools/__init__.py
+-rw-rw-r--  2.0 unx      142 b- defN 23-May-10 18:29 piksi_tools/_version.py
+-rw-rw-r--  2.0 unx     1008 b- defN 22-Feb-17 21:17 piksi_tools/acq_plot.py
+-rw-rw-r--  2.0 unx     4285 b- defN 22-Feb-17 21:17 piksi_tools/acq_results.py
+-rw-rw-r--  2.0 unx    10428 b- defN 22-Feb-17 21:17 piksi_tools/action_logger.py
+-rw-rw-r--  2.0 unx     6577 b- defN 22-Feb-17 21:17 piksi_tools/almanac.py
+-rw-rw-r--  2.0 unx     3528 b- defN 22-Feb-17 21:17 piksi_tools/bootload_v3.py
+-rw-rw-r--  2.0 unx     8083 b- defN 23-Jun-07 16:35 piksi_tools/diagnostics.py
+-rw-rw-r--  2.0 unx    27969 b- defN 22-Feb-17 21:17 piksi_tools/fileio.py
+-rw-rw-r--  2.0 unx     1070 b- defN 22-Feb-17 21:17 piksi_tools/heartbeat.py
+-rw-rw-r--  2.0 unx    14588 b- defN 22-Feb-17 21:17 piksi_tools/interpolate_event_positions.py
+-rw-rw-r--  2.0 unx     1238 b- defN 22-Feb-17 21:17 piksi_tools/log_wrapper.py
+-rw-rw-r--  2.0 unx     2765 b- defN 22-Feb-17 21:17 piksi_tools/recover_ftdi.py
+-rw-rw-r--  2.0 unx     4859 b- defN 22-Feb-17 21:17 piksi_tools/sbp_msg_2_csv.py
+-rw-rw-r--  2.0 unx     1578 b- defN 22-Feb-17 21:17 piksi_tools/sbpjson_expand.py
+-rw-rw-r--  2.0 unx    12345 b- defN 22-Feb-17 21:17 piksi_tools/serial_link.py
+-rw-rw-r--  2.0 unx    16401 b- defN 23-May-10 07:39 piksi_tools/settings.py
+-rw-rw-r--  2.0 unx     2406 b- defN 22-Feb-17 21:17 piksi_tools/simulator_almanac_generator.py
+-rw-rw-r--  2.0 unx     3902 b- defN 22-Feb-17 21:17 piksi_tools/stm_unique_id.py
+-rw-rw-r--  2.0 unx     1774 b- defN 22-Feb-17 21:17 piksi_tools/timeout.py
+-rw-rw-r--  2.0 unx     4489 b- defN 22-Feb-17 21:17 piksi_tools/utils.py
+-rw-rw-r--  2.0 unx     7651 b- defN 23-Jun-07 16:42 piksi_tools-4.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3271 b- defN 23-Jun-07 16:42 piksi_tools-4.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-07 16:42 piksi_tools-4.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-07 16:42 piksi_tools-4.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-07 16:42 piksi_tools-4.0.0.dist-info/RECORD
+26 files, 143240 bytes uncompressed, 47382 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -57,200 +57,23 @@
 
 Filename: piksi_tools/timeout.py
 Comment: 
 
 Filename: piksi_tools/utils.py
 Comment: 
 
-Filename: piksi_tools/ardupilot/__init__.py
+Filename: piksi_tools-4.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: piksi_tools/ardupilot/mavlink2pandas.py
+Filename: piksi_tools-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: piksi_tools/ardupilot/mavlink_decode.py
+Filename: piksi_tools-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: piksi_tools/ardupilot/mavlink_split.py
+Filename: piksi_tools-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: piksi_tools/ardupilot/udp_bridge.py
-Comment: 
-
-Filename: piksi_tools/ardupilot/udp_receive.py
-Comment: 
-
-Filename: piksi_tools/console/GitVersion.py
-Comment: 
-
-Filename: piksi_tools/console/README.txt
-Comment: 
-
-Filename: piksi_tools/console/__init__.py
-Comment: 
-
-Filename: piksi_tools/console/__main__.py
-Comment: 
-
-Filename: piksi_tools/console/baseline_view.py
-Comment: 
-
-Filename: piksi_tools/console/callback_prompt.py
-Comment: 
-
-Filename: piksi_tools/console/console.py
-Comment: 
-
-Filename: piksi_tools/console/deprecated.py
-Comment: 
-
-Filename: piksi_tools/console/fusion_engine_status.py
-Comment: 
-
-Filename: piksi_tools/console/generate_settings.py
-Comment: 
-
-Filename: piksi_tools/console/gui_utils.py
-Comment: 
-
-Filename: piksi_tools/console/ins_view.py
-Comment: 
-
-Filename: piksi_tools/console/mag_view.py
-Comment: 
-
-Filename: piksi_tools/console/observation_view.py
-Comment: 
-
-Filename: piksi_tools/console/output_list.py
-Comment: 
-
-Filename: piksi_tools/console/output_stream.py
-Comment: 
-
-Filename: piksi_tools/console/port_chooser.py
-Comment: 
-
-Filename: piksi_tools/console/sbp_relay_view.py
-Comment: 
-
-Filename: piksi_tools/console/settings.yaml
-Comment: 
-
-Filename: piksi_tools/console/settings_list.py
-Comment: 
-
-Filename: piksi_tools/console/settings_template.tex
-Comment: 
-
-Filename: piksi_tools/console/settings_view.py
-Comment: 
-
-Filename: piksi_tools/console/skyplot_view.py
-Comment: 
-
-Filename: piksi_tools/console/solution_view.py
-Comment: 
-
-Filename: piksi_tools/console/spectrum_analyzer_view.py
-Comment: 
-
-Filename: piksi_tools/console/system_monitor_view.py
-Comment: 
-
-Filename: piksi_tools/console/tracking_view.py
-Comment: 
-
-Filename: piksi_tools/console/update_downloader.py
-Comment: 
-
-Filename: piksi_tools/console/update_view.py
-Comment: 
-
-Filename: piksi_tools/console/utils.py
-Comment: 
-
-Filename: piksi_tools/console/velocity_view.py
-Comment: 
-
-Filename: piksi_tools/console/images/icon.png
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/LICENSE.txt
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/README.md
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/download.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/exclamation-triangle.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/floppy-o.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/power27.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/refresh.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/refresh_blue.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/stop.svg
-Comment: 
-
-Filename: piksi_tools/console/images/fontawesome/upload.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/AUTHORS
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/LICENSE
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/arrows_blue.png
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/arrows_grey.png
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/fullscreen.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/move.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/pause.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/play.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/stop.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/target.svg
-Comment: 
-
-Filename: piksi_tools/console/images/iconic/x.svg
-Comment: 
-
-Filename: piksi_tools-3.1.4.dist-info/LICENSE
-Comment: 
-
-Filename: piksi_tools-3.1.4.dist-info/METADATA
-Comment: 
-
-Filename: piksi_tools-3.1.4.dist-info/WHEEL
-Comment: 
-
-Filename: piksi_tools-3.1.4.dist-info/top_level.txt
-Comment: 
-
-Filename: piksi_tools-3.1.4.dist-info/RECORD
+Filename: piksi_tools-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## piksi_tools/_version.py

```diff
@@ -1,4 +1,4 @@
 # coding: utf-8
 # file generated by setuptools_scm
 # don't change, don't track in version control
-version = 'v3.1.4'
+version = 'v3.1.1.dev14+g27d57f0.d20230510'
```

## piksi_tools/diagnostics.py

```diff
@@ -10,15 +10,15 @@
 # WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A PARTICULAR PURPOSE.
 
 from __future__ import absolute_import, print_function
 
 import struct
 import time
 
-from ruamel.yaml import YAML
+import yaml
 
 
 from sbp.bootload import (SBP_MSG_BOOTLOADER_HANDSHAKE_DEP_A,
                           SBP_MSG_BOOTLOADER_HANDSHAKE_RESP,
                           MsgBootloaderJumpToApp, MsgBootloaderHandshakeResp)
 from sbp.client import Framer, Handler
 from sbp.logging import SBP_MSG_LOG, SBP_MSG_PRINT_DEP
@@ -26,15 +26,14 @@
 from sbp.settings import (
     SBP_MSG_SETTINGS_READ_BY_INDEX_DONE, SBP_MSG_SETTINGS_READ_BY_INDEX_REQ,
     SBP_MSG_SETTINGS_READ_BY_INDEX_RESP, MsgSettingsReadByIndexReq)
 from sbp.system import SBP_MSG_HEARTBEAT, MsgHeartbeat
 
 from . import serial_link
 
-yaml = YAML(typ='safe')
 
 DIAGNOSTICS_FILENAME = "diagnostics.yaml"
 
 
 class Diagnostics(object):
     """
     Diagnostics
@@ -138,28 +137,28 @@
         self.settings_received = True
 
 
 def parse_device_details_yaml(device_details):
     """Parse from yaml string the device settings.
 
     """
-    return yaml.load(device_details)['settings']['system_info']
+    return yaml.load(device_details, yaml.SafeLoader)['settings']['system_info']
 
 
 def check_diagnostics(diagnostics_filename, version):
     """Check that Piksi's firmware/nap settings are properly set.
 
     Given a diagnostics_filename output and an expected firmware/NAP
     versions (via a Yaml string), returns True if expected fw/nap are
     properly loaded.
 
     """
     if version is None:
         raise Exception("Empty version string!")
-    parsed = yaml.load(version)
+    parsed = yaml.load(version, yaml.SafeLoader)
     fw = parsed.get('fw', None)
     nap = parsed.get('hdl', None)
     with open(diagnostics_filename, 'r+') as f:
         details = parse_device_details_yaml(f.read())
         firmware_version = details.get('firmware_version', None)
         nap_version = details.get('nap_version', None)
         return (firmware_version and nap_version) \
```

## piksi_tools/settings.py

```diff
@@ -243,20 +243,23 @@
                 self.write(section, setting, value, verbose=verbose)
         return
 
     def _print_callback(self, msg, **metadata):
         print(msg.text.decode('ascii'))
 
     def _settings_callback(self, sbp_msg, **metadata):
-        section, setting, value, format_type = sbp_msg.payload.split(b'\0')[:4]
+        section, setting, value, *format_type = sbp_msg.payload.split(b'\0')[:4]
+        section = section.decode(KEY_ENCODING)
+        setting = setting.decode(KEY_ENCODING)
+        value = value.decode(VALUE_ENCODING) if format_type else None
         self.read_response_wait_dict[(
-            section.decode(KEY_ENCODING), setting.decode(KEY_ENCODING))] = value.decode(VALUE_ENCODING)
+            section, setting)] = value
 
     def _settings_list_callback(self, sbp_msg, **metadata):
-        section_b, setting_b, value_b, format_type_b = sbp_msg.payload[2:].split(b'\0')[:4]
+        section_b, setting_b, value_b, *format_type_b = sbp_msg.payload[2:].split(b'\0')[:4]
         section = section_b.decode(KEY_ENCODING)
         setting = setting_b.decode(KEY_ENCODING)
         value = value_b.decode(VALUE_ENCODING)
         if section not in self.settings_list:
             self.settings_list[section] = {}
         self.settings_list[section][setting] = value
         index = struct.unpack('<H', sbp_msg.payload[:2])[0]
```

## Comparing `piksi_tools-3.1.4.dist-info/LICENSE` & `piksi_tools-4.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

