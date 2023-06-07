# Comparing `tmp/neon_speech-3.3.2a9-py3-none-any.whl.zip` & `tmp/neon_speech-4.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17818 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-Jun-01 22:13 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2784 b- defN 23-Jun-01 22:13 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5171 b- defN 23-Jun-01 22:13 neon_speech/cli.py
--rw-r--r--  2.0 unx    20934 b- defN 23-Jun-01 22:13 neon_speech/service.py
--rw-r--r--  2.0 unx     4459 b- defN 23-Jun-01 22:13 neon_speech/stt.py
--rw-r--r--  2.0 unx     4395 b- defN 23-Jun-01 22:13 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 22:13 neon_speech-3.3.2a9.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2451 b- defN 23-Jun-01 22:13 neon_speech-3.3.2a9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 22:13 neon_speech-3.3.2a9.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-Jun-01 22:13 neon_speech-3.3.2a9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-01 22:13 neon_speech-3.3.2a9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      988 b- defN 23-Jun-01 22:13 neon_speech-3.3.2a9.dist-info/RECORD
-12 files, 44862 bytes uncompressed, 16160 bytes compressed:  64.0%
+Zip file size: 17764 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jun-07 17:01 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2784 b- defN 23-Jun-07 17:01 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5167 b- defN 23-Jun-07 17:01 neon_speech/cli.py
+-rw-r--r--  2.0 unx    20934 b- defN 23-Jun-07 17:01 neon_speech/service.py
+-rw-r--r--  2.0 unx     4459 b- defN 23-Jun-07 17:01 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4395 b- defN 23-Jun-07 17:01 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-07 17:01 neon_speech-4.0.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jun-07 17:01 neon_speech-4.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 17:01 neon_speech-4.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-07 17:01 neon_speech-4.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-07 17:01 neon_speech-4.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-07 17:01 neon_speech-4.0.0.dist-info/RECORD
+12 files, 44807 bytes uncompressed, 16130 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.2a9.dist-info/LICENSE.md
+Filename: neon_speech-4.0.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.2a9.dist-info/METADATA
+Filename: neon_speech-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.2a9.dist-info/WHEEL
+Filename: neon_speech-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.2a9.dist-info/entry_points.txt
+Filename: neon_speech-4.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a9.dist-info/top_level.txt
+Filename: neon_speech-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a9.dist-info/RECORD
+Filename: neon_speech-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/cli.py

```diff
@@ -26,14 +26,15 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import click
 
 from click_default_group import DefaultGroup
 from neon_utils.packaging_utils import get_package_version_spec
+from neon_utils.configuration_utils import init_config_dir
 
 
 @click.group("neon-speech", cls=DefaultGroup,
              no_args_is_help=True, invoke_without_command=True,
              help="Neon Core Commands\n\n"
                   "See also: neon COMMAND --help")
 @click.option("--version", "-v", is_flag=True, required=False,
@@ -48,15 +49,14 @@
 @click.option("--module", "-m", default=None,
               help="STT Plugin to configure")
 @click.option("--package", "-p", default=None,
               help="STT package spec to install")
 @click.option("--force-install", "-f", default=False, is_flag=True,
               help="Force pip installation of configured module")
 def run(module, package, force_install):
-    from neon_utils.configuration_utils import init_config_dir
     init_config_dir()
 
     from neon_speech.__main__ import main
     from ovos_config.config import Configuration
     speech_config = Configuration()
     if force_install or module or package:
         install_plugin(module, package, force_install)
```

## Comparing `neon_speech-3.3.2a9.dist-info/LICENSE.md` & `neon_speech-4.0.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.2a9.dist-info/METADATA` & `neon_speech-4.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.2a9
+Version: 4.0.0
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: ovos-dinkum-listener (>=0.0.2a33,~=0.0.1)
+Requires-Dist: ovos-dinkum-listener (~=0.0.2)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-utils (~=0.0.30)
-Requires-Dist: ovos-plugin-manager (>=0.0.23a17,~=0.0.19)
+Requires-Dist: ovos-plugin-manager (~=0.0.23)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
-Requires-Dist: neon-utils[audio,network] (>=1.5.0a5,~=1.3)
+Requires-Dist: neon-utils[audio,network] (~=1.5)
 Requires-Dist: ovos-config (~=0.0.7)
 Requires-Dist: ovos-vad-plugin-webrtcvad (~=0.0.1)
 Requires-Dist: ovos-ww-plugin-vosk (~=0.1)
 Provides-Extra: docker
 Requires-Dist: ovos-stt-plugin-vosk (~=0.1) ; extra == 'docker'
 Requires-Dist: neon-stt-plugin-nemo (~=0.0.2) ; extra == 'docker'
 Requires-Dist: ovos-ww-plugin-pocketsphinx (~=0.1) ; extra == 'docker'
@@ -53,7 +53,9 @@
 -v ~/.config/pulse/cookie:/tmp/pulse_cookie:ro \
 -v ${XDG_RUNTIME_DIR}/pulse:${XDG_RUNTIME_DIR}/pulse:ro \
 --device=/dev/snd:/dev/snd \
 -e PULSE_SERVER=unix:${XDG_RUNTIME_DIR}/pulse/native \
 -e PULSE_COOKIE=/tmp/pulse_cookie \
 neon_speech
 ```
+
+
```

