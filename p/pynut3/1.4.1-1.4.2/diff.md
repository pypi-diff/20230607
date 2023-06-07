# Comparing `tmp/pynut3-1.4.1.tar.gz` & `tmp/pynut3-1.4.2.tar.gz`

## Comparing `pynut3-1.4.1.tar` & `pynut3-1.4.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pynut3-1.4.1/.editorconfig
--rw-r--r--   0        0        0    20692 2020-02-02 00:00:00.000000 pynut3-1.4.1/.pylintrc
--rwxr-xr-x   0        0        0     2217 2020-02-02 00:00:00.000000 pynut3-1.4.1/build
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pynut3-1.4.1/tox.ini
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pynut3-1.4.1/.github/dependabot.yml
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 pynut3-1.4.1/demo/upsdemo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynut3-1.4.1/src/pynut3/__init__.py
--rw-r--r--   0        0        0    20270 2020-02-02 00:00:00.000000 pynut3-1.4.1/src/pynut3/nut3.py
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pynut3-1.4.1/.gitignore
--rw-r--r--   0        0        0    35068 2020-02-02 00:00:00.000000 pynut3-1.4.1/LICENSE
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pynut3-1.4.1/README.md
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pynut3-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pynut3-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pynut3-1.4.2/.editorconfig
+-rw-r--r--   0        0        0    20692 2020-02-02 00:00:00.000000 pynut3-1.4.2/.pylintrc
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pynut3-1.4.2/BUILDING.md
+-rwxr-xr-x   0        0        0     2334 2020-02-02 00:00:00.000000 pynut3-1.4.2/mkbld
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pynut3-1.4.2/tox.ini
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pynut3-1.4.2/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 pynut3-1.4.2/demo/upsdemo.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pynut3-1.4.2/src/pynut3/__init__.py
+-rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 pynut3-1.4.2/src/pynut3/nut3.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 pynut3-1.4.2/.gitignore
+-rw-r--r--   0        0        0    35068 2020-02-02 00:00:00.000000 pynut3-1.4.2/LICENSE
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pynut3-1.4.2/README.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pynut3-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pynut3-1.4.2/PKG-INFO
```

### Comparing `pynut3-1.4.1/.pylintrc` & `pynut3-1.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `pynut3-1.4.1/build` & `pynut3-1.4.2/mkbld`

 * *Files 6% similar despite different names*

```diff
@@ -24,40 +24,39 @@
     rm dist/*
     python3 -m build
 }
 
 test_app() {
     LOCATION=$1
     echo "Upload package to TestPyPi from $LOCATION"
+    ping -c 1 upload.pypi.org >/dev/null || { echo " The remote server is unavailable" ; exit 3; }
     python3 -m twine upload --repository testpypi dist/*
     echo ""
     echo "To test installing this package use:"
     echo "python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps ${PACKAGE_NAME}"
 }
 
 dist_app() {
     LOCATION=$1
     echo "Upload distribution package to PyPi from $LOCATION"
-    # throw away files if upload was succesful
-    python3 -m twine upload --repository pypi dist/*   # && rm dist/*
+    ping -c 1 upload.pypi.org >/dev/null || { echo " The remote server is unavailable" ; exit 2; }
+    python3 -m twine upload --repository pypi dist/*
     echo ""
     echo "To install this package use:"
     echo "python3 -m pip install ${PACKAGE_NAME}"
 }
 
 update_local_repo() {
     branch_name=$1
     git fetch origin "${branch_name}" || { sleep 60; git fetch origin "${branch_name}" || exit 1; }
     git reset --hard "origin/${branch_name}" || exit 1
     git clean -f -d || exit 1
     git pull || exit 1
 }
 
-"${HERE}"/check
-
 # check commandline parameters
 case $CMD in
     -b | --build)
         # build
         build_app "${HERE}" || exit 1
         ;;
     -d | --dist)
```

### Comparing `pynut3-1.4.1/tox.ini` & `pynut3-1.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pynut3-1.4.1/.github/dependabot.yml` & `pynut3-1.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pynut3-1.4.1/demo/upsdemo.py` & `pynut3-1.4.2/demo/upsdemo.py`

 * *Files identical despite different names*

### Comparing `pynut3-1.4.1/src/pynut3/nut3.py` & `pynut3-1.4.2/src/pynut3/nut3.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import logging
 import socket
 
-# TODO: implement telnetlib3 to replace deprecated telnetlib (PEP-594)
+# TODO: implement pexpect to replace deprecated telnetlib (PEP-594)
+# ref:
+#   https://stackoverflow.com/questions/75778543/python-telnetlib3-examples
+#   https://pexpect.readthedocs.io/en/stable/index.html
+
 from telnetlib import Telnet
 from typing import Any, Dict, List, Optional
 
-__version__ = "1.4.1"
-__all__ = ["PyNUT3Error", "PyNUT3Client"]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PyNUT3Error(Exception):
     """Base class for custom exceptions."""
 
@@ -380,15 +382,19 @@
         offset: int = len(f"ENUM {ups} {var}")
         end_offset: int = 0 - (len(f"END LIST ENUM {ups} {var}\n") + 1)
 
         if not self._persistent:
             self._disconnect()
 
         try:
-            return [c[offset:].split('"')[1].strip() for c in result[:end_offset].split("\n") if '"' in c[offset:]]
+            return [
+                c[offset:].split('"')[1].strip()
+                for c in result[:end_offset].split("\n")
+                if '"' in c[offset:]
+            ]
         except IndexError as exc:
             raise PyNUT3Error(result.replace("\n", "")) from exc
 
     def list_range(self, ups: str, var: str) -> List[str]:
         """Get a list of valid values for an range variable.
 
         The result is presented as a list.
@@ -407,15 +413,19 @@
         offset: int = len(f"RANGE {ups} {var}")
         end_offset: int = 0 - (len(f"END LIST RANGE {ups} {var}\n") + 1)
 
         if not self._persistent:
             self._disconnect()
 
         try:
-            return [c[offset:].split('"')[1].strip() for c in result[:end_offset].split("\n") if '"' in c[offset:]]
+            return [
+                c[offset:].split('"')[1].strip()
+                for c in result[:end_offset].split("\n")
+                if '"' in c[offset:]
+            ]
         except IndexError as exc:
             raise PyNUT3Error(result.replace("\n", "")) from exc
 
     def set_var(self, ups: str, var: str, value: str) -> None:
         """Set a variable to the specified value on selected UPS.
 
         The variable must be a writable value (cf list_rw_vars) and you
```

### Comparing `pynut3-1.4.1/.gitignore` & `pynut3-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pynut3-1.4.1/LICENSE` & `pynut3-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynut3-1.4.1/README.md` & `pynut3-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ```python3
 from pynut3 import nut3
 client = nut3.PyNUT3Client(host='192.168.2.17')
 print(client.help())
 ups_dict = client.list_ups()
 for k1, v1 in ups_dict.items():
     print(f"{v1} is called with id {k1}")
-    vars_dict = client.list_vars(k)
+    vars_dict = client.list_vars(k1)
     for k2, v2 in vars_dict.items():
         print(f"{k2}\t:\t{v2}")
 ```
 
 Please note that this module has completely and intentionally broken backwards compatibility with (previous) versions of PyNUT.
 
 ## Acknowledgements
```

### Comparing `pynut3-1.4.1/pyproject.toml` & `pynut3-1.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pynut3"
 description = "A Python3 abstraction class to access NUT servers for uninterruptible power supplies (UPS)."
-version = "1.4.1"
+version = "1.4.2" # latest production version
+# version = "1.5.1" # latest testing version
 dependencies = []
 license = "GPL-3.0-only"
 authors = [
   { name="Mausy5043" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `pynut3-1.4.1/PKG-INFO` & `pynut3-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynut3
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python3 abstraction class to access NUT servers for uninterruptible power supplies (UPS).
 Project-URL: Homepage, https://github.com/Mausy5043/python-nut3
 Project-URL: Bug Tracker, https://github.com/Mausy5043/python-nut3/issues
 Author: Mausy5043
 License-Expression: GPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 ```python3
 from pynut3 import nut3
 client = nut3.PyNUT3Client(host='192.168.2.17')
 print(client.help())
 ups_dict = client.list_ups()
 for k1, v1 in ups_dict.items():
     print(f"{v1} is called with id {k1}")
-    vars_dict = client.list_vars(k)
+    vars_dict = client.list_vars(k1)
     for k2, v2 in vars_dict.items():
         print(f"{k2}\t:\t{v2}")
 ```
 
 Please note that this module has completely and intentionally broken backwards compatibility with (previous) versions of PyNUT.
 
 ## Acknowledgements
```

