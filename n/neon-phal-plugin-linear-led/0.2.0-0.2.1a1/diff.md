# Comparing `tmp/neon_phal_plugin_linear_led-0.2.0-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_linear_led-0.2.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11261 bytes, number of entries: 9
--rw-r--r--  2.0 unx    17185 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led/__init__.py
--rw-r--r--  2.0 unx     2662 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led/neopixel_led.py
--rw-r--r--  2.0 unx     2455 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led/smbus_led.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led-0.2.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3639 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      229 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      899 b- defN 23-Apr-20 23:12 neon_phal_plugin_linear_led-0.2.0.dist-info/RECORD
-9 files, 28823 bytes uncompressed, 9667 bytes compressed:  66.5%
+Zip file size: 11284 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    17182 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led/__init__.py
+-rw-r--r--  2.0 unx     2662 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led/neopixel_led.py
+-rw-r--r--  2.0 unx     2455 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led/smbus_led.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led-0.2.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3638 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led-0.2.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led-0.2.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led-0.2.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led-0.2.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jun-07 21:44 neon_phal_plugin_linear_led-0.2.1a1.dist-info/RECORD
+9 files, 28834 bytes uncompressed, 9666 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: neon_phal_plugin_linear_led/neopixel_led.py
 Comment: 
 
 Filename: neon_phal_plugin_linear_led/smbus_led.py
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.2.0.dist-info/LICENSE.md
+Filename: neon_phal_plugin_linear_led-0.2.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.2.0.dist-info/METADATA
+Filename: neon_phal_plugin_linear_led-0.2.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.2.0.dist-info/WHEEL
+Filename: neon_phal_plugin_linear_led-0.2.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.2.0.dist-info/entry_points.txt
+Filename: neon_phal_plugin_linear_led-0.2.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.2.0.dist-info/top_level.txt
+Filename: neon_phal_plugin_linear_led-0.2.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.2.0.dist-info/RECORD
+Filename: neon_phal_plugin_linear_led-0.2.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_linear_led/__init__.py

```diff
@@ -24,15 +24,15 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from threading import RLock
 
-from mycroft_bus_client import Message
+from ovos_bus_client import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.templates.phal import PHALPlugin
 from ovos_plugin_manager.hardware.led import Color, AbstractLed
 from ovos_plugin_manager.hardware.led.animations import BreatheLedAnimation, \
     FillLedAnimation, BlinkLedAnimation, AlternatingLedAnimation,\
     animations, LedAnimation
 from ovos_utils.network_utils import is_connected
```

## Comparing `neon_phal_plugin_linear_led-0.2.0.dist-info/LICENSE.md` & `neon_phal_plugin_linear_led-0.2.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_linear_led-0.2.0.dist-info/METADATA` & `neon_phal_plugin_linear_led-0.2.1a1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear-led
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: sj201-interface (~=0.0.1)
 Requires-Dist: ovos-plugin-manager (~=0.0.21)
 Requires-Dist: ovos-utils (~=0.0.26)
-Requires-Dist: mycroft-messagebus-client (~=0.10)
+Requires-Dist: ovos-bus-client (~=0.0.3)
 
 # PHAL Linear LED Plugin
 Enables interaction with LEDs in a one-dimensional physical arrangement.
 
 ## Standard LED Events
 There are default LED animations that are shown when certain things happen. Note
 that some of these behaviors are configurable while others are hard-coded so
@@ -101,8 +101,7 @@
         {'animation': 'chase',
          'color': 'green',
          'timeout': 10})
 ```
 
 Note that the plugin may enforce a limit to how long the animation is displayed
 and also may replace the animation with a different one that is triggered.
-
```

