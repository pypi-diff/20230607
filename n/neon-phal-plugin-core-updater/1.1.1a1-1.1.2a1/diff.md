# Comparing `tmp/neon_phal_plugin_core_updater-1.1.1a1-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.1.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6654 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8281 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2333 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/RECORD
-7 files, 13195 bytes uncompressed, 5326 bytes compressed:  59.6%
+Zip file size: 6671 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8286 b- defN 23-Jun-07 21:43 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      726 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/RECORD
+7 files, 13278 bytes uncompressed, 5343 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_core_updater/__init__.py

```diff
@@ -30,15 +30,15 @@
 
 from os.path import isfile
 from typing import List
 from datetime import datetime
 from os import close
 from subprocess import Popen
 from tempfile import mkstemp
-from mycroft_bus_client import Message
+from ovos_bus_client.message import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.phal import PHALPlugin
 
 
 class CoreUpdater(PHALPlugin):
     def __init__(self, bus=None, name="neon-phal-plugin-core-updater",
                  config=None):
```

## Comparing `neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.1.1a1
+Version: 1.1.2a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: neon-utils (~=1.1)
 Requires-Dist: ovos-plugin-manager (~=0.0.20)
+Requires-Dist: ovos-bus-client (~=0.0.3)
+Requires-Dist: ovos-utils (~=0.0.30)
 
 # Core Updater Plugin
 Exposes a messagebus API to check for and initiate core module updates. Update
 checks use GitHub releases or PyPI indices, depending on plugin configuration.
 The update command is configurable and is started in a new session. Note that
 the calling module might be killed during updates and in many cases, systemD 
 will kill the update process if the parent service stops.
```

