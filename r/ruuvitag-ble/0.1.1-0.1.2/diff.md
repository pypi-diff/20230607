# Comparing `tmp/ruuvitag_ble-0.1.1.tar.gz` & `tmp/ruuvitag_ble-0.1.2.tar.gz`

## Comparing `ruuvitag_ble-0.1.1.tar` & `ruuvitag_ble-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,17 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.flake8
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/setup.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/aws.xml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/govee-ble.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/ruuvitag-ble.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/watcherTasks.xml
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/src/ruuvitag_ble/__init__.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/src/ruuvitag_ble/df5_decoder.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/src/ruuvitag_ble/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/src/ruuvitag_ble/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/tests/test_parser.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/LICENSE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/README.md
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/.flake8
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/setup.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/src/ruuvitag_ble/__init__.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/src/ruuvitag_ble/df5_decoder.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/src/ruuvitag_ble/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/src/ruuvitag_ble/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/tests/test_parser.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/LICENSE
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/README.md
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 ruuvitag_ble-0.1.2/PKG-INFO
```

### Comparing `ruuvitag_ble-0.1.1/.pre-commit-config.yaml` & `ruuvitag_ble-0.1.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,14 @@
       - id: debug-statements
   - repo: https://github.com/asottile/pyupgrade
     rev: v2.37.1
     hooks:
       - id: pyupgrade
         args: [--py39-plus]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
```

### Comparing `ruuvitag_ble-0.1.1/src/ruuvitag_ble/df5_decoder.py` & `ruuvitag_ble-0.1.2/src/ruuvitag_ble/df5_decoder.py`

 * *Files identical despite different names*

### Comparing `ruuvitag_ble-0.1.1/src/ruuvitag_ble/parser.py` & `ruuvitag_ble-0.1.2/src/ruuvitag_ble/parser.py`

 * *Files identical despite different names*

### Comparing `ruuvitag_ble-0.1.1/tests/test_parser.py` & `ruuvitag_ble-0.1.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `ruuvitag_ble-0.1.1/LICENSE` & `ruuvitag_ble-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ruuvitag_ble-0.1.1/pyproject.toml` & `ruuvitag_ble-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ruuvitag-ble"
-version = "0.1.1"
+version = "0.1.2"
 description = "Manage Ruuvitag BLE devices"
 authors = [
     { name = "Aarni Koskela", email = "akx@iki.fi" },
 ]
 requires-python = ">=3.9"
 license = "MIT"
 readme = "README.md"
@@ -17,18 +17,18 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "ruuvitag_ble", from = "src" },
 ]
 dependencies = [
-    "bluetooth-data-tools~=0.1",
-    "bluetooth-sensor-state-data~=1.6",
-    "home-assistant-bluetooth~=1.6",
-    "sensor-state-data~=2.9",
+    "bluetooth-data-tools>=0.1",
+    "bluetooth-sensor-state-data>=1.6",
+    "home-assistant-bluetooth>=1.6",
+    "sensor-state-data>=2.9",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/bluetooth-devices/ruuvitag-ble/issues"
 "Changelog" = "https://github.com/bluetooth-devices/ruuvitag-ble/blob/main/CHANGELOG.md"
 
 [tool.semantic_release]
```

### Comparing `ruuvitag_ble-0.1.1/PKG-INFO` & `ruuvitag_ble-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ruuvitag-ble
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manage Ruuvitag BLE devices
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/ruuvitag-ble/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/ruuvitag-ble/blob/main/CHANGELOG.md
 Author-email: Aarni Koskela <akx@iki.fi>
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
-Requires-Dist: bluetooth-data-tools~=0.1
-Requires-Dist: bluetooth-sensor-state-data~=1.6
-Requires-Dist: home-assistant-bluetooth~=1.6
-Requires-Dist: sensor-state-data~=2.9
+Requires-Dist: bluetooth-data-tools>=0.1
+Requires-Dist: bluetooth-sensor-state-data>=1.6
+Requires-Dist: home-assistant-bluetooth>=1.6
+Requires-Dist: sensor-state-data>=2.9
 Description-Content-Type: text/markdown
 
 # ruuvitag-ble
 Parser for Ruuvitag BLE devices
```

