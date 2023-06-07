# Comparing `tmp/neon_phal_plugin_reset-0.2.0-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_reset-0.2.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11271 bytes, number of entries: 10
--rw-r--r--  2.0 unx    12157 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset/__init__.py
--rw-r--r--  2.0 unx     2687 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset/config.py
--rw-r--r--  2.0 unx     3873 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset/create_media.py
--rw-r--r--  2.0 unx     1854 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset/version.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset-0.2.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1189 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       84 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      940 b- defN 23-Jun-02 01:49 neon_phal_plugin_reset-0.2.0.dist-info/RECORD
-10 files, 24533 bytes uncompressed, 9631 bytes compressed:  60.7%
+Zip file size: 11307 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    12154 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset/__init__.py
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset/config.py
+-rw-r--r--  2.0 unx     3873 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset/create_media.py
+-rw-r--r--  2.0 unx     1856 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset/version.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset-0.2.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1234 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset-0.2.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset-0.2.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset-0.2.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset-0.2.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      952 b- defN 23-Jun-07 21:43 neon_phal_plugin_reset-0.2.1a1.dist-info/RECORD
+10 files, 24590 bytes uncompressed, 9643 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: neon_phal_plugin_reset/create_media.py
 Comment: 
 
 Filename: neon_phal_plugin_reset/version.py
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.2.0.dist-info/LICENSE.md
+Filename: neon_phal_plugin_reset-0.2.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.2.0.dist-info/METADATA
+Filename: neon_phal_plugin_reset-0.2.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.2.0.dist-info/WHEEL
+Filename: neon_phal_plugin_reset-0.2.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.2.0.dist-info/entry_points.txt
+Filename: neon_phal_plugin_reset-0.2.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.2.0.dist-info/top_level.txt
+Filename: neon_phal_plugin_reset-0.2.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.2.0.dist-info/RECORD
+Filename: neon_phal_plugin_reset-0.2.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_reset/__init__.py

```diff
@@ -29,15 +29,15 @@
 from shutil import move, rmtree
 from subprocess import Popen
 from os import remove
 from os.path import isfile, join, isdir
 from threading import RLock
 from zipfile import BadZipFile
 
-from mycroft_bus_client import Message
+from ovos_bus_client import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_skill_installer import download_extract_zip
 
 
 class DeviceReset(PHALPlugin):
     def __init__(self, bus=None, name="neon-phal-plugin-reset",
```

## neon_phal_plugin_reset/version.py

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.2.0"
+__version__ = "0.2.1a1"
```

## Comparing `neon_phal_plugin_reset-0.2.0.dist-info/LICENSE.md` & `neon_phal_plugin_reset-0.2.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_reset-0.2.0.dist-info/METADATA` & `neon_phal_plugin_reset-0.2.1a1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: ovos-utils (~=0.0.26)
-Requires-Dist: mycroft-messagebus-client (~=0.10)
 Requires-Dist: ovos-plugin-manager (~=0.0.20)
 Requires-Dist: requests
+Requires-Dist: ovos-bus-client (~=0.0.3)
+Requires-Dist: ovos-skill-installer (~=0.0.5)
 
 # Neon Reset Plugin
 Plugin to handle factory reset requests. Note that this plugin will install system
 services and modify system config as part of its installation. Installation may
 fail if not completed as `root`.
 
 ## Default Reset Behavior
 By default, the reset plugin will reset your Python environment to the state it
 was in when this plugin was installed. It will also restore the user `.local`, 
 `.cache`, and `.config` directories to the state their original state.
 `/etc/neon/neon.yaml` will be updated to the latest default if an internet connection
 is available. The reset script comes from the 
 [neon-image-recipe repository](https://github.com/NeonGeckoCom/neon-image-recipe/blob/master/11_factory_reset/overlay/opt/neon/reset).
-
```

