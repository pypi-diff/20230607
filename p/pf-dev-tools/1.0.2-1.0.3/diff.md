# Comparing `tmp/pf_dev_tools-1.0.2.tar.gz` & `tmp/pf_dev_tools-1.0.3.tar.gz`

## Comparing `pf_dev_tools-1.0.2.tar` & `pf_dev_tools-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.flake8
--rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.nova/Artwork
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.nova/Configuration.json
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/Exceptions.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/__about__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/__init__.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfBuildCore.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfConfig.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfSconsEnvironment.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfUtils.py
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/__main__.py
--rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfBuild.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClean.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClone.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfCommand.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfConvert.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDelete.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDryRun.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfEject.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfInstall.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfMake.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfQfs.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfReverse.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/LICENSE
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/README.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.flake8
+-rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.nova/Artwork
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.nova/Configuration.json
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/Exceptions.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/__about__.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/__init__.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfBuildCore.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfConfig.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfSconsEnvironment.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfUtils.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClean.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClone.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfCommand.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfConvert.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDelete.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDryRun.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfEject.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfInstall.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfMake.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfPackage.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfQfs.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfReverse.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/LICENSE
+-rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/README.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/PKG-INFO
```

### Comparing `pf_dev_tools-1.0.2/.nova/Artwork` & `pf_dev_tools-1.0.3/.nova/Artwork`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/__init__.py` & `pf_dev_tools-1.0.3/pfDevTools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 
-from .pfCommand.pfBuild import pfBuild
 from .pfCommand.pfClone import pfClone
 from .pfCommand.pfConvert import pfConvert
 from .pfCommand.pfDelete import pfDelete
 from .pfCommand.pfEject import pfEject
 from .pfCommand.pfInstall import pfInstall
 from .pfCommand.pfMake import pfMake
+from .pfCommand.pfPackage import pfPackage
 from .pfCommand.pfQfs import pfQfs
 from .pfCommand.pfReverse import pfReverse
 
 from .pfConfig import pfConfig
 from .pfSconsEnvironment import Environment
 from .pfUtils import pfUtils
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfBuildCore.py` & `pf_dev_tools-1.0.3/pfDevTools/pfBuildCore.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
     @classmethod
     def _cloneRepo(cls, target, source, env):
         command_line: List[str] = []
 
         url = env.get('PF_CORE_TEMPLATE_REPO_URL', None)
         if url is not None:
-            command_line += [url]
+            command_line.append(url)
 
         tag = env.get('PF_CORE_TEMPLATE_REPO_TAG', None)
         if tag is not None:
-            command_line += ['tag', tag]
+            command_line.append(f'tag={tag}')
 
         command_line.append(env['PF_BUILD_FOLDER'])
 
         pfDevTools.pfClone(command_line).run()
 
     @classmethod
     def _updateQsfFile(cls, target, source, env):
@@ -42,19 +42,16 @@
         except RuntimeError:
             raise RuntimeError("Cannot start docker container. Are you sure the docker engine is running?")
 
         pfDevTools.pfQfs([str(source[0]), str(target[0]), f'cpus={"max" if len(result) != 1 else result[0]}'] + core_verilog_files[1:]).run()
 
     @classmethod
     def _installCore(cls, target, source, env):
-        # -- If PF_CORE_INSTALL_VOLUME is not defined, we default to POCKET
-        core_install_volume = os.environ.get('PF_CORE_INSTALL_VOLUME', 'POCKET')
-
-        pfDevTools.pfInstall([str(source[0]), core_install_volume]).run()
-        pfDevTools.pfEject([core_install_volume]).run()
+        pfDevTools.pfInstall([str(source[0])]).run()
+        pfDevTools.pfEject([]).run()
 
     @classmethod
     def _copyFile(cls, target, source, env):
         source_file = str(source[0])
         target_file = str(target[0])
         parent_dest_dir = Path(target_file).parent
         os.makedirs(parent_dest_dir, exist_ok=True)
@@ -89,15 +86,15 @@
 
     @classmethod
     def _compileBitStream(cls, target, source, env):
         pfDevTools.pfUtils.shellCommand(f'docker run --platform linux/amd64 -t --rm -v {os.path.realpath(env["PF_CORE_FPGA_FOLDER"])}:/build {env["PF_DOCKER_IMAGE"]} quartus_sh --flow compile pf_core')
 
     @classmethod
     def _packageCore(cls, target, source, env):
-        build_process: pfDevTools.pfBuild = pfDevTools.pfBuild([env['PF_CORE_CONFIG_FILE'], env['PF_BUILD_FOLDER'], env['PF_CORE_BITSTREAM_FILE']])
+        build_process: pfDevTools.pfPackage = pfDevTools.pfPackage([env['PF_CORE_CONFIG_FILE'], env['PF_CORE_BITSTREAM_FILE'], env['PF_BUILD_FOLDER']])
         print('Building core...')
         build_process.run()
 
     @classmethod
     def build(cls, env, config_file: str, extra_files: List[str] = []):
         pfDevTools.pfUtils.requireCommand('docker')
 
@@ -131,15 +128,15 @@
         dest_verilog_files: List[str] = pfBuildCore._searchSourceFiles(env, src_folder, dest_verilog_folder)
         extra_dest_files: List[str] = pfBuildCore._addExtraFiles(env, src_folder, dest_verilog_folder, extra_files)
 
         env.Command(core_output_qsf_file, [core_input_qsf_file] + dest_verilog_files, pfBuildCore._updateQsfFile)
 
         env.Command(core_output_bitstream_file, [core_output_qsf_file] + extra_dest_files, pfBuildCore._compileBitStream)
 
-        build_process: pfDevTools.pfBuild = pfDevTools.pfBuild([config_file, build_folder, core_output_bitstream_file])
+        build_process: pfDevTools.pfPackage = pfDevTools.pfPackage([config_file, core_output_bitstream_file, build_folder])
         packaged_core = os.path.join(build_folder, build_process.packagedFilename())
         p = env.Command(packaged_core, build_process.dependencies(), pfBuildCore._packageCore)
 
         env.Default(packaged_core)
         env.Clean(packaged_core, build_folder)
 
         install_command = env.Command(None, packaged_core, pfBuildCore._installCore)
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfConfig.py` & `pf_dev_tools-1.0.3/pfDevTools/pfConfig.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 
 from typing import Dict
+from sys import platform
+
 from .Exceptions import ArgumentError
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
@@ -107,7 +109,19 @@
         return self._getConfigParam('Video', 'rotation')
 
     def videoMirror(self) -> str:
         return self._getConfigParam('Video', 'mirror')
 
     def fullPlatformName(self) -> str:
         return f'{self.authorName()}.{self.platformShortName()}'
+
+    @classmethod
+    def coreInstallVolumePath(cls) -> str:
+        volume_path: str = os.environ.get('PF_CORE_INSTALL_VOLUME', None)
+        if volume_path is None:
+            if platform == "darwin":
+                # -- On macOS, if PF_CORE_INSTALL_VOLUME is not defined, we default to POCKET
+                volume_path = os.path.join('/Volumes', 'POCKET')
+            else:
+                raise RuntimeError('PF_CORE_INSTALL_VOLUME is not defined in the environment.')
+
+        return volume_path
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfUtils.py` & `pf_dev_tools-1.0.3/pfDevTools/pfUtils.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/__main__.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfBuild.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfPackage.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 from pfDevTools.pfConfig import pfConfig
 
 from .pfConvert import pfConvert
 from .pfReverse import pfReverse
 
 
 # -- Classes
-class pfBuild:
-    """A tool to build an analog pocket core"""
+class pfPackage:
+    """A tool to package an analog pocket core"""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 3:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
         self._config = pfConfig(arguments[0])
-        self._destination_folder: str = arguments[1]
-        self._bitstream_file: str = arguments[2]
+        self._bitstream_file: str = arguments[1]
+        self._destination_folder: str = arguments[2]
         self._core_folder = os.path.join(self._destination_folder, '_core')
         self._today = str(date.today())
 
     def _generateDefinitionFiles(self, cores_folder, platforms_folder) -> None:
         output_filename = os.path.join(cores_folder, 'audio.json')
         with open(output_filename, 'w') as out_file:
             out_file.write('{\n')
@@ -217,9 +217,9 @@
 
     @classmethod
     def name(cls) -> str:
         return 'build'
 
     @classmethod
     def usage(cls) -> None:
-        print('   build config_file dest_folder bistream_file')
+        print('   build config_file bistream_file dest_folder')
         print('                                         - Build core according to a config_file.')
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClean.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClean.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClone.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClone.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 # -- Classes
 class pfClone:
     """A tool to clone the Github core template."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
-        nb_of_arguments = len(arguments)
-
-        self._branch_name: str = None
         self._tag_name: str = None
         self._url: str = 'https://github.com/DidierMalenfant/pfCoreTemplate.git'
 
-        if nb_of_arguments == 2 or nb_of_arguments == 4:
+        nb_of_arguments = len(arguments)
+        if nb_of_arguments == 1 or nb_of_arguments == 3:
             self._url: str = arguments[0]
             nb_of_arguments -= 1
             arguments = arguments[1:]
 
-        if nb_of_arguments == 1:
+        if nb_of_arguments == 0:
             self._destination_folder: str = arguments[0]
-        elif nb_of_arguments == 3:
-            if arguments[0] == 'tag':
-                self._tag_name = arguments[1]
+        elif nb_of_arguments == 2:
+            if arguments[0].startswith('tag='):
+                self._tag_name = arguments[0][4:]
             else:
                 raise ArgumentError('Invalid cloning arguments. Maybe start with `pf --help?')
 
-            self._destination_folder: str = arguments[2]
+            self._destination_folder: str = arguments[1]
         else:
             raise ArgumentError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
         if pfUtils.commandExists('git') is False:
             raise RuntimeError('You must have git installed on your machine to continue.')
 
@@ -46,17 +44,15 @@
         if os.path.exists(repo_folder):
             pfUtils.deleteFolder(repo_folder, force_delete=True)
 
         print('Cloning core template in \'' + repo_folder + '\'.')
 
         command_line = 'git clone --depth 1 '
 
-        if self._branch_name is not None:
-            command_line += f'--branch {self._branch_name} '
-        elif self._tag_name is not None:
+        if self._tag_name is not None:
             command_line += f'--branch {self._tag_name} '
 
         command_line += self._url
 
         pfUtils.shellCommand(command_line, from_dir=self._destination_folder, silent_mode=True)
 
         git_folder = os.path.join(repo_folder, '.git')
@@ -65,9 +61,9 @@
 
     @classmethod
     def name(cls) -> str:
         return 'clone'
 
     @classmethod
     def usage(cls) -> None:
-        print('   clone <url> <tag name> dest_folder    - Clone repo at url, optionally at a given tag.')
+        print('   clone <url> <tag=name> dest_folder    - Clone repo at url, optionally at a given tag/branch.')
         print('                                           (url defaults to pfCoreTemplate\'s repo if missing).')
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfCommand.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfCommand.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 # import os
 import sys
 import getopt
 
 from pfDevTools.__about__ import __version__
 from pfDevTools.Exceptions import ArgumentError
 
-from .pfBuild import pfBuild
 from .pfClean import pfClean
 from .pfClone import pfClone
 from .pfConvert import pfConvert
 from .pfDelete import pfDelete
 from .pfDryRun import pfDryRun
 from .pfEject import pfEject
 from .pfInstall import pfInstall
 from .pfMake import pfMake
+from .pfPackage import pfPackage
 from .pfQfs import pfQfs
 from .pfReverse import pfReverse
 
 
 # -- Classes
 class pfCommand:
     """The pf command line tool for Project Freedom."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
-            self._commands = [pfBuild, pfClean, pfClone, pfConvert, pfDelete, pfDryRun, pfEject, pfInstall, pfMake, pfQfs, pfReverse]
+            self._commands = [pfClean, pfClone, pfConvert, pfDelete, pfDryRun, pfEject, pfInstall, pfMake, pfPackage, pfQfs, pfReverse]
 
             # -- Gather the arguments
             opts, arguments = getopt.getopt(args, 'dhv', ['debug', 'help', 'version'])
 
             for o, a in opts:
                 if o in ('-d', '--debug'):
                     # -- We ignore this argument because it was already dealt with in the calling main() code.
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfConvert.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfConvert.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDelete.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDelete.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import shutil
 import contextlib
+import pfDevTools
 
 from pathlib import Path
 
 
 # -- Classes
 class pfDelete:
     """A tool to delete a core from a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
-        if len(arguments) != 2:
+        nb_of_arguments = len(arguments)
+        if nb_of_arguments == 2:
+            self._volume_path = arguments[1]
+            arguments = arguments[:0]
+            nb_of_arguments -= 1
+        else:
+            self._volume_path = pfDevTools.pfConfig.coreInstallVolumePath()
+
+        if len(arguments) != 1:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
         self._name_of_core_to_delete: str = arguments[0]
-        self._volume_name: str = arguments[1]
 
     def _destCoresFolder(self) -> str:
-        return os.path.join('/Volumes', self._volume_name, 'Cores')
+        return os.path.join(self._volume_path, 'Cores')
 
     def _destPlatformsFolder(self) -> str:
-        return os.path.join('/Volumes', self._volume_name, 'Platforms')
+        return os.path.join(self._volume_path, 'Platforms')
 
     def _deleteFile(self, filepath) -> None:
         with contextlib.suppress(FileNotFoundError):
             os.remove(filepath)
 
     def run(self) -> None:
         cores_folder = self._destCoresFolder()
@@ -87,8 +95,8 @@
 
     @classmethod
     def name(cls) -> str:
         return 'delete'
 
     @classmethod
     def usage(cls) -> None:
-        print('   delete core_name dest_volume          - Delete core on volume.')
+        print('   delete core_name <dest_volume>        - Delete core on volume.')
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDryRun.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDryRun.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfEject.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfEject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
+import pfDevTools
 
 from sys import platform
 
 from pfDevTools.pfUtils import pfUtils
 
 
 # -- Classes
 class pfEject:
     """A tool to eject given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
-        if len(arguments) != 1:
+        nb_of_arguments = len(arguments)
+        if nb_of_arguments == 0:
+            self._volume_path = pfDevTools.pfConfig.coreInstallVolumePath()
+        elif nb_of_arguments == 1:
+            self._volume_path = arguments[0]
+        else:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
-        self._volume_name = arguments[0]
-
     def run(self) -> None:
+        if not os.path.exists(self._volume_path):
+            raise RuntimeError(f'Volume {self._volume_path} is not mounted.')
+    
         if platform == "darwin":
-            if not os.path.exists(os.path.join('/Volumes', self._volume_name)):
-                raise RuntimeError(f'Volume {self._volume_name} is not mounted.')
-
-            print('Ejecting \'' + self._volume_name + '\'.')
-            pfUtils.shellCommand(f'diskutil eject {self._volume_name}')
+            print(f'Ejecting {self._volume_path}.')
+            pfUtils.shellCommand(f'diskutil eject {self._volume_path}')
         else:
             print('Ejecting volumes is only supported on macOS right now.')
 
     @classmethod
     def name(cls) -> str:
         return 'eject'
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfInstall.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfInstall.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,69 +2,67 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import zipfile
 import tempfile
 import contextlib
+import pfDevTools
 
 from sys import platform
-
 from distutils.dir_util import copy_tree
-from pfDevTools.pfUtils import pfUtils
 
 
 # -- Classes
 class pfInstall:
     """A tool to install a zipped up core file onto a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         self._zip_filename = None
-        self._volume_name = None
+        self._volume_path = None
+
+        nb_of_arguments = len(arguments)
+        if nb_of_arguments != 0:
+            if nb_of_arguments == 2:
+                self._volume_path = arguments[1]
+                arguments = arguments[:0]
+                nb_of_arguments -= 1
+            else:
+                self._volume_path = pfDevTools.pfConfig.coreInstallVolumePath()
 
-        if len(arguments) != 0:
-            if len(arguments) != 2:
+            if nb_of_arguments != 1:
                 raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
             self._zip_filename = arguments[0]
-            self._volume_name = arguments[1]
 
             components = os.path.splitext(self._zip_filename)
             if len(components) != 2 or components[1] != '.zip':
                 raise RuntimeError('Can only install zipped up core files.')
 
             if not os.path.exists(self._zip_filename):
                 raise RuntimeError('File \'' + self._zip_filename + '\' does not exist.')
 
-    def _destVolume(self) -> str:
-        if platform == "darwin":
-            volume_path = os.path.join('/Volumes', self._volume_name)
-        else:
-            print('Installing cores is only supported on macOS right now.')
-
-        if not os.path.exists(volume_path):
-            raise RuntimeError(f'Volume {self._volume_name} is not mounted.')
-
-        return volume_path
+            if not os.path.exists(self._volume_path):
+                raise RuntimeError(f'Volume {self._volume_path} is not mounted.')
 
     def _destCoresFolder(self) -> str:
-        return os.path.join(self._destVolume(), 'Cores')
+        return os.path.join(self._volume_path, 'Cores')
 
     def _destPlatformsFolder(self) -> str:
-        return os.path.join(self._destVolume(), 'Platforms')
+        return os.path.join(self._volume_path, 'Platforms')
 
     def _deleteFile(self, filepath) -> None:
         with contextlib.suppress(FileNotFoundError):
             os.remove(filepath)
 
     def run(self) -> None:
-        if self._volume_name is None:
-            pfUtils.shellCommand('scons -Q -s install')
+        if self._volume_path is None:
+            pfDevTools.pfUtils.shellCommand('scons -Q -s install')
             return
 
         # -- In a temporary folder.
         with tempfile.TemporaryDirectory() as tmp_dir:
             # -- Unzip the file.
             with zipfile.ZipFile(self._zip_filename, 'r') as zip_ref:
                 zip_ref.extractall(tmp_dir)
@@ -93,8 +91,8 @@
 
     @classmethod
     def name(cls) -> str:
         return 'install'
 
     @classmethod
     def usage(cls) -> None:
-        print('   install <zip_file> <dest_volume>        - Install core on volume.')
+        print(f'   install zip_file <{"dest_volume" if platform == "darwin" else "volume_path"}>        - Install core on volume.')
```

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfMake.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfMake.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfQfs.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfQfs.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfReverse.py` & `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfReverse.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/LICENSE` & `pf_dev_tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.2/pyproject.toml` & `pf_dev_tools-1.0.3/pyproject.toml`

 * *Files identical despite different names*

