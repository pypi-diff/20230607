# Comparing `tmp/sun-1.5.1.tar.gz` & `tmp/sun-1.5.2.tar.gz`

## Comparing `sun-1.5.1.tar` & `sun-1.5.2.tar`

### file list

```diff
@@ -1,57 +1,54 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:31:46.000000 sun-1.5.1/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/extra/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/extra/xdg/
--rw-r--r--   0 dslackw   (1000) users      (100)      275 2023-05-24 10:30:28.000000 sun-1.5.1/extra/xdg/sun_daemon.desktop.sample
--rw-r--r--   0 dslackw   (1000) users      (100)      321 2023-05-24 10:30:28.000000 sun-1.5.1/extra/xdg/sun.desktop
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/extra/icon/
--rw-r--r--   0 dslackw   (1000) users      (100)     6188 2023-05-24 10:30:28.000000 sun-1.5.1/extra/icon/sun.png
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/extra/desktop/
--rw-r--r--   0 dslackw   (1000) users      (100)      231 2023-05-24 10:30:28.000000 sun-1.5.1/extra/desktop/sun.desktop
--rw-r--r--   0 dslackw   (1000) users      (100)    32402 2023-05-24 10:30:28.000000 sun-1.5.1/LICENSE.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     5314 2023-05-24 10:30:28.000000 sun-1.5.1/CHANGES.md
--rw-r--r--   0 dslackw   (1000) users      (100)       58 2023-05-24 10:30:28.000000 sun-1.5.1/MANIFEST.in
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:31:43.000000 sun-1.5.1/sun/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/sun/gtk/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/sun/gtk/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7619 2023-05-24 10:30:28.000000 sun-1.5.1/sun/gtk/status_icon.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6622 2023-05-24 10:30:28.000000 sun-1.5.1/sun/utils.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2246 2023-05-24 10:30:28.000000 sun-1.5.1/sun/daemon.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1853 2023-05-24 10:30:28.000000 sun-1.5.1/sun/__metadata__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2145 2023-05-24 10:30:28.000000 sun-1.5.1/sun/licenses.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:31:43.000000 sun-1.5.1/sun/__pycache__/
--rw-r--r--   0 dslackw   (1000) users      (100)      140 2023-05-24 10:31:43.000000 sun-1.5.1/sun/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)     1155 2023-05-24 10:31:43.000000 sun-1.5.1/sun/__pycache__/__metadata__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/sun/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3260 2023-05-24 10:30:28.000000 sun-1.5.1/sun/configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/sun/cli/
--rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-05-24 10:30:28.000000 sun-1.5.1/sun/cli/tool.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/sun/cli/__init__.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      900 2023-05-24 10:30:28.000000 sun-1.5.1/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      543 2023-05-24 10:30:28.000000 sun-1.5.1/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      457 2023-05-24 10:30:28.000000 sun-1.5.1/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     3628 2023-05-24 10:30:28.000000 sun-1.5.1/slackbuild/sun.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)     2791 2023-05-24 10:30:28.000000 sun-1.5.1/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3463 2023-05-24 10:30:28.000000 sun-1.5.1/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       39 2023-05-24 10:30:28.000000 sun-1.5.1/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/sbin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     2730 2023-05-24 10:30:28.000000 sun-1.5.1/sbin/sun_daemon
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)      596 2023-05-24 10:30:28.000000 sun-1.5.1/tests/test_tools.py
--rw-r--r--   0 dslackw   (1000) users      (100)      853 2023-05-24 10:30:28.000000 sun-1.5.1/tests/test_utils.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:31:43.000000 sun-1.5.1/sun.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-24 10:31:43.000000 sun-1.5.1/sun.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      499 2023-05-24 10:31:43.000000 sun-1.5.1/sun.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-05-24 10:31:43.000000 sun-1.5.1/sun.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       29 2023-05-24 10:31:43.000000 sun-1.5.1/sun.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     4411 2023-05-24 10:31:43.000000 sun-1.5.1/sun.egg-info/PKG-INFO
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1787 2023-05-24 10:30:28.000000 sun-1.5.1/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)       78 2023-05-24 10:30:28.000000 sun-1.5.1/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/conf/
--rw-r--r--   0 dslackw   (1000) users      (100)     1391 2023-05-24 10:30:28.000000 sun-1.5.1/conf/sun.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     1684 2023-05-24 10:30:28.000000 sun-1.5.1/conf/repositories.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1196 2023-05-24 10:30:28.000000 sun-1.5.1/bin/sun_daemon
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1130 2023-05-24 10:30:28.000000 sun-1.5.1/bin/sun
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1207 2023-05-24 10:30:28.000000 sun-1.5.1/bin/sun_gtk
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-24 10:30:28.000000 sun-1.5.1/bin/__init__.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:58:55.000000 sun-1.5.2/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/extra/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/extra/xdg/
+-rw-r--r--   0 dslackw   (1000) users      (100)      275 2023-06-07 09:54:56.000000 sun-1.5.2/extra/xdg/sun_daemon.desktop.sample
+-rw-r--r--   0 dslackw   (1000) users      (100)      321 2023-06-07 09:54:56.000000 sun-1.5.2/extra/xdg/sun.desktop
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/extra/icon/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6188 2023-06-07 09:54:56.000000 sun-1.5.2/extra/icon/sun.png
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/extra/desktop/
+-rw-r--r--   0 dslackw   (1000) users      (100)      231 2023-06-07 09:54:56.000000 sun-1.5.2/extra/desktop/sun.desktop
+-rw-r--r--   0 dslackw   (1000) users      (100)    32402 2023-06-07 09:54:56.000000 sun-1.5.2/LICENSE.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     5389 2023-06-07 09:54:56.000000 sun-1.5.2/CHANGES.md
+-rw-r--r--   0 dslackw   (1000) users      (100)       58 2023-06-07 09:54:56.000000 sun-1.5.2/MANIFEST.in
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:59:21.000000 sun-1.5.2/sun/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/sun/gtk/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/sun/gtk/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7619 2023-06-07 09:54:56.000000 sun-1.5.2/sun/gtk/status_icon.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6591 2023-06-07 09:54:56.000000 sun-1.5.2/sun/utils.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2254 2023-06-07 09:54:56.000000 sun-1.5.2/sun/daemon.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1853 2023-06-07 09:54:56.000000 sun-1.5.2/sun/__metadata__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2145 2023-06-07 09:54:56.000000 sun-1.5.2/sun/licenses.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/sun/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3260 2023-06-07 09:54:56.000000 sun-1.5.2/sun/configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/sun/cli/
+-rw-r--r--   0 dslackw   (1000) users      (100)     5730 2023-06-07 09:54:56.000000 sun-1.5.2/sun/cli/tool.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/sun/cli/__init__.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:58:39.000000 sun-1.5.2/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      900 2023-06-07 09:54:56.000000 sun-1.5.2/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      543 2023-06-07 09:54:56.000000 sun-1.5.2/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      457 2023-06-07 09:54:56.000000 sun-1.5.2/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     3628 2023-06-07 09:54:56.000000 sun-1.5.2/slackbuild/sun.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     2791 2023-06-07 09:54:56.000000 sun-1.5.2/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3463 2023-06-07 09:54:56.000000 sun-1.5.2/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       39 2023-06-07 09:54:56.000000 sun-1.5.2/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/sbin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     2730 2023-06-07 09:54:56.000000 sun-1.5.2/sbin/sun_daemon
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)      596 2023-06-07 09:54:56.000000 sun-1.5.2/tests/test_tools.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      853 2023-06-07 09:54:56.000000 sun-1.5.2/tests/test_utils.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:58:51.000000 sun-1.5.2/sun.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-07 09:58:51.000000 sun-1.5.2/sun.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)      499 2023-06-07 09:58:51.000000 sun-1.5.2/sun.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-07 09:58:51.000000 sun-1.5.2/sun.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       29 2023-06-07 09:58:51.000000 sun-1.5.2/sun.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     4411 2023-06-07 09:58:51.000000 sun-1.5.2/sun.egg-info/PKG-INFO
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1787 2023-06-07 09:54:56.000000 sun-1.5.2/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)       78 2023-06-07 09:54:56.000000 sun-1.5.2/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/conf/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1391 2023-06-07 09:54:56.000000 sun-1.5.2/conf/sun.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     1684 2023-06-07 09:54:56.000000 sun-1.5.2/conf/repositories.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1196 2023-06-07 09:54:56.000000 sun-1.5.2/bin/sun_daemon
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1130 2023-06-07 09:54:56.000000 sun-1.5.2/bin/sun
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1207 2023-06-07 09:54:56.000000 sun-1.5.2/bin/sun_gtk
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-07 09:54:56.000000 sun-1.5.2/bin/__init__.py
```

### Comparing `sun-1.5.1/extra/icon/sun.png` & `sun-1.5.2/extra/icon/sun.png`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/LICENSE.txt` & `sun-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/CHANGES.md` & `sun-1.5.2/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 SUN (Slackware Update Notifier)
 ===============================
+Version 1.5.2 - (07/06/2023)
+Updated:
+- For urllib3.exceptions.HTTPError
+
+
 Version 1.5.1 - (24/05/2023)
 ### Fixed
 - SlackBuild script for repositories.toml file
 
 Version 1.5.0 - (19/05/2023)
 ### Fixed
 - Daemon notification message
```

### Comparing `sun-1.5.1/sun/gtk/status_icon.py` & `sun-1.5.2/sun/gtk/status_icon.py`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/sun/utils.py` & `sun-1.5.2/sun/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 import re
 import getpass
 import urllib3
-import requests
-from typing import Generator
 from pathlib import Path
+from typing import Generator
+from urllib3.exceptions import HTTPError
 from sun.configs import Configs
 from sun.__metadata__ import data_configs
 
 
 class Utilities(Configs):
     """ General utilities. """
 
@@ -41,34 +41,33 @@
         self.data_configs: dict = data_configs
 
     @staticmethod
     def read_repo_text_file(mirror: str) -> str:
         """ Reads and returns the mirror log text files. """
         log_txt: str = str()
         try:
-            requests.get(mirror, timeout=2)
             http = urllib3.PoolManager()
             con = http.request('GET', mirror)
             log_txt = con.data.decode()
         except KeyError:
-            print('SUN: error: ftp mirror not supported')
-        except requests.exceptions.RequestException:
-            print(f'Error: Failed to connect to {mirror}')
+            print('SUN: Error: Ftp mirror not supported')
+        except HTTPError:
+            print(f'SUN: Error: Failed to connect to {mirror}')
 
         return log_txt
 
     @staticmethod
     def read_local_text_file(registry: Path) -> str:
         """ Reads and returns the local log text files. """
         log_txt: str = str()
         if registry.is_file():
             with open(registry, 'r', encoding='utf-8', errors='ignore') as file_txt:
                 log_txt = file_txt.read()
         else:
-            print(f"\nError: Failed to find '{registry}' file.\n")
+            print(f"\nSUN: Error: Failed to find '{registry}' file.\n")
 
         return log_txt
 
     def slack_version(self) -> tuple:
         """ Returns the distribution name and version. """
         version_file: str = self.read_local_text_file(Path('/etc/slackware-version'))
         slackware_version: list = re.findall(r'\d+\.\d+', version_file)
@@ -137,15 +136,15 @@
             self.repo_name: str = repository['REPOSITORY_NAME']
             self.repo_mirror: str = repository['HTTP_MIRROR']
             self.repo_log_path: str = repository['LOG_PATH']
             self.repo_log_file: str = repository['LOG_FILE']
             self.repo_pattern: str = repository['PACKAGE_PATTERN']
             self.repo_compare: str = repository['COMPARE_PATTERN']
         except KeyError as error:
-            print(f"KeyError: {error}: in the config file '{self.config_path}{self.config_file}'.")
+            print(f"SUN: KeyError: {error}: in the config file '{self.config_path}{self.config_file}'.")
 
     def patch_line_for_slackware(self, line: str) -> str:
         """ Patches the line for linux updates. """
         slack_name: tuple = ('Slackware', 'slackware', 'Slack', 'slack')
         if line.startswith('patches/packages/linux') and self.repo_name in slack_name:
             line = line.split("/")[-2]
         return line
```

### Comparing `sun-1.5.1/sun/daemon.py` & `sun-1.5.2/sun/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.count_packages: int = 0
         self.title: str = f"{'':>10}Software Updates"
         self.icon: str = f'{data_configs["icon_path"]}/{__all__}.png'
 
         notify2.uninit()
         notify2.init('sun')
 
-    def set_notification_message(self):
+    def set_notification_message(self) -> None:
         self.count_packages: int = len(list(self.fetch.updates()))
         self.message: str = f"{'':>3}{self.count_packages} Software updates are available\n"
         self.notify = notify2.Notification(self.title, self.message, self.icon)
         self.notify.set_timeout(60000 * self.standby)
 
     def daemon(self) -> None:
         """ SUN daemon. """
```

### Comparing `sun-1.5.1/sun/__metadata__.py` & `sun-1.5.2/sun/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import subprocess
 from pathlib import Path
 
 
 __all__: str = 'sun'
 __author__: str = 'dslackw'
 __copyright__: str = '2015-2022'
-__version_info__: tuple = (1, 5, 1)
+__version_info__: tuple = (1, 5, 2)
 __version__: str = '{0}.{1}.{2}'.format(*__version_info__)
 __license__: str = 'GNU General Public License v3 (GPLv3)'
 __email__: str = 'dslackw@gmail.com'
 __website__: str = 'https://gitlab.com/dslackw/sun'
 
 
 data_configs: dict = {
```

### Comparing `sun-1.5.1/sun/licenses.py` & `sun-1.5.2/sun/licenses.py`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/sun/configs.py` & `sun-1.5.2/sun/configs.py`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/sun/cli/tool.py` & `sun-1.5.2/sun/cli/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,21 +146,21 @@
 
         elif len(self.args) == 2 and self.args[0] == 'start' and self.args[1] == '--gtk':
             subprocess.call('sun_gtk &', shell=True)
 
         else:
             raise SystemExit("try: 'sun help'")
 
-    def view_start(self):
+    def view_start(self) -> None:
         print(self.tools.daemon_process(self.args[0], 'Starting SUN daemon:  sun_daemon &'))
 
-    def view_stop(self):
+    def view_stop(self) -> None:
         print(self.tools.daemon_process(self.args[0], 'Stopping SUN daemon:  sun_daemon'))
 
-    def view_restart(self):
+    def view_restart(self) -> None:
         print(self.tools.daemon_process(self.args[0], 'Restarting SUN daemon:  sun_daemon'))
 
-    def view_status(self):
+    def view_status(self) -> None:
         print('SUN is running...' if self.tools.daemon_status() else 'SUN is not running')
 
-    def view_info(self):
+    def view_info(self) -> None:
         print(self.utils.os_info())
```

### Comparing `sun-1.5.1/slackbuild/slack-desc` & `sun-1.5.2/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/slackbuild/doinst.sh` & `sun-1.5.2/slackbuild/doinst.sh`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/slackbuild/sun.SlackBuild` & `sun-1.5.2/slackbuild/sun.SlackBuild`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/setup.py` & `sun-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/README.rst` & `sun-1.5.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 Installing
 ----------
 
 .. code-block:: bash
 
     Required root privileges
 
-    $ tar xvf sun-1.5.1.tar.gz
-    $ cd sun-1.5.1
+    $ tar xvf sun-1.5.2.tar.gz
+    $ cd sun-1.5.2
     $ ./install.sh
 
     Installed as Slackware package
 
 
 Usage
 -----
@@ -57,15 +57,15 @@
 
 CLI
 ---
 
 .. code-block:: bash
 
     $ sun help
-    SUN (Slackware Update Notifier) - Version: 1.5.1
+    SUN (Slackware Update Notifier) - Version: 1.5.2
 
     Usage: sun [OPTIONS]
 
     Optional arguments:
       help       Display this help and exit.
       start      Start sun daemon.
       stop       Stop sun daemon.
@@ -80,16 +80,16 @@
     $ sun start
     Starting SUN daemon:  /usr/bin/sun_daemon &
 
     $ sun check
     3 software updates are available from 1 repository
 
     Slack: samba-4.1.17-x86_64-1_slack14.1.txz
-    Slack: mozilla-firefox-31.5.1esr-x86_64-1_slack14.1.txz
-    Slack: mozilla-thunderbird-31.5.1-x86_64-1_slack14.1.txz
+    Slack: mozilla-firefox-31.5.2esr-x86_64-1_slack14.1.txz
+    Slack: mozilla-thunderbird-31.5.2-x86_64-1_slack14.1.txz
 
     $ sun stop
     Stopping SUN daemon:  /usr/bin/sun_daemon
 
     $ sun status
     SUN is not running
```

### Comparing `sun-1.5.1/sbin/sun_daemon` & `sun-1.5.2/sbin/sun_daemon`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/tests/test_tools.py` & `sun-1.5.2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/tests/test_utils.py` & `sun-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/sun.egg-info/PKG-INFO` & `sun-1.5.2/sun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sun
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tray notification applet for informing about package updates in Slackware
 Home-page: https://gitlab.com/dslackw/sun
 Author: dslackw
 Author-email: dslackw@gmail.com
 License: UNKNOWN
 Keywords: tray,notify,slackware,desktop
 Platform: UNKNOWN
@@ -51,16 +51,16 @@
 Installing
 ----------
 
 .. code-block:: bash
 
     Required root privileges
 
-    $ tar xvf sun-1.5.1.tar.gz
-    $ cd sun-1.5.1
+    $ tar xvf sun-1.5.2.tar.gz
+    $ cd sun-1.5.2
     $ ./install.sh
 
     Installed as Slackware package
 
 
 Usage
 -----
@@ -83,15 +83,15 @@
 
 CLI
 ---
 
 .. code-block:: bash
 
     $ sun help
-    SUN (Slackware Update Notifier) - Version: 1.5.1
+    SUN (Slackware Update Notifier) - Version: 1.5.2
 
     Usage: sun [OPTIONS]
 
     Optional arguments:
       help       Display this help and exit.
       start      Start sun daemon.
       stop       Stop sun daemon.
@@ -106,16 +106,16 @@
     $ sun start
     Starting SUN daemon:  /usr/bin/sun_daemon &
 
     $ sun check
     3 software updates are available from 1 repository
 
     Slack: samba-4.1.17-x86_64-1_slack14.1.txz
-    Slack: mozilla-firefox-31.5.1esr-x86_64-1_slack14.1.txz
-    Slack: mozilla-thunderbird-31.5.1-x86_64-1_slack14.1.txz
+    Slack: mozilla-firefox-31.5.2esr-x86_64-1_slack14.1.txz
+    Slack: mozilla-thunderbird-31.5.2-x86_64-1_slack14.1.txz
 
     $ sun stop
     Stopping SUN daemon:  /usr/bin/sun_daemon
 
     $ sun status
     SUN is not running
```

### Comparing `sun-1.5.1/install.sh` & `sun-1.5.2/install.sh`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/conf/sun.toml` & `sun-1.5.2/conf/sun.toml`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/conf/repositories.toml` & `sun-1.5.2/conf/repositories.toml`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/bin/sun_daemon` & `sun-1.5.2/bin/sun_daemon`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/bin/sun` & `sun-1.5.2/bin/sun`

 * *Files identical despite different names*

### Comparing `sun-1.5.1/bin/sun_gtk` & `sun-1.5.2/bin/sun_gtk`

 * *Files identical despite different names*

