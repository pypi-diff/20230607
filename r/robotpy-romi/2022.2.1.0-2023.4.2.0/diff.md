# Comparing `tmp/robotpy-romi-2022.2.1.0.tar.gz` & `tmp/robotpy-romi-2023.4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotpy-romi-2022.2.1.0.tar", last modified: Mon Feb 14 05:20:24 2022, max compression
+gzip compressed data, was "robotpy-romi-2023.4.2.0.tar", last modified: Tue Jun  6 22:07:00 2023, max compression
```

## Comparing `robotpy-romi-2022.2.1.0.tar` & `robotpy-romi-2023.4.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.279083 robotpy-romi-2022.2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.279083 robotpy-romi-2022.2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     6875 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4169 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/docs/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/gen/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/gen/OnBoardIO.yml
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/gen/RomiGyro.yml
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/gen/RomiMotor.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/romi/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/romi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/romi/src/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/romi/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-02-14 05:20:24.000000 robotpy-romi-2022.2.1.0/romi/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 05:20:24.283084 robotpy-romi-2022.2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/tests/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      248 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-14 05:20:17.000000 robotpy-romi-2022.2.1.0/tests/test_romi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.050071 robotpy-romi-2023.4.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.050071 robotpy-romi-2023.4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/docs/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/gen/OnBoardIO.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/gen/RomiGyro.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/gen/RomiMotor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 22:07:00.000000 robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/romi/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/romi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/romi/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/romi/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-06 22:06:59.000000 robotpy-romi-2023.4.2.0/romi/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:07:00.054071 robotpy-romi-2023.4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      246 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 22:06:51.000000 robotpy-romi-2023.4.2.0/tests/test_romi.py
```

### Comparing `robotpy-romi-2022.2.1.0/.github/workflows/dist.yml` & `robotpy-romi-2023.4.2.0/.github/workflows/dist.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   pull_request:
   push:
     tags:
     - '*'
 
 jobs:
   ci:
-    uses: robotpy/build-actions/.github/workflows/package-ci.yml@v2022
+    uses: robotpy/build-actions/.github/workflows/package-ci.yml@v2023
     with:
       enable_roborio: false
     secrets:
       SSH_USER: ${{ secrets.SSH_USER }}
       SSH_KEY: ${{ secrets.SSH_KEY }}
       SSH_PASSPHRASE: ${{ secrets.SSH_PASSPHRASE }}
       META_REPO_ACCESS_TOKEN: ${{ secrets.REPO_ACCESS_TOKEN }}
```

### Comparing `robotpy-romi-2022.2.1.0/PKG-INFO` & `robotpy-romi-2023.4.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotpy-romi
-Version: 2022.2.1.0
+Version: 2023.4.2.0
 Summary: Binary wrapper for WPILib Romi Vendor library
 Home-page: https://github.com/robotpy/robotpy-romi
 Author: RobotPy Development Team
 Author-email: robotpy@googlegroups.com
 License: BSD-3-Clause
 Description: robotpy-romi
         ============
```

### Comparing `robotpy-romi-2022.2.1.0/docs/Makefile` & `robotpy-romi-2023.4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `robotpy-romi-2022.2.1.0/docs/conf.py` & `robotpy-romi-2023.4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `robotpy-romi-2022.2.1.0/docs/setup.py` & `robotpy-romi-2023.4.2.0/docs/setup.py`

 * *Files identical despite different names*

### Comparing `robotpy-romi-2022.2.1.0/pyproject.toml` & `robotpy-romi-2023.4.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,23 @@
+[tool.robotpy-build.metadata]
+name = "robotpy-romi"
+description = "Binary wrapper for WPILib Romi Vendor library"
+author = "RobotPy Development Team"
+author_email = "robotpy@googlegroups.com"
+url = "https://github.com/robotpy/robotpy-romi"
+license = "BSD-3-Clause"
+install_requires = [
+    "wpilib~=2023.4.3"
+]
+
+
 [build-system]
 requires = [
-    "robotpy-build<2023.0.0,>=2022.2.0",
-    "wpilib<2023.0.0,>=2022.2.1.3"
+    "robotpy-build<2024.0.0,>=2023.1.1",
+    "wpilib~=2023.4.3"
 ]
 
 [tool.robotpy-build]
 base_package = "romi"
 
 [tool.robotpy-build.wrappers."romi"]
 name = "romi"
@@ -22,22 +34,12 @@
 OnBoardIO = "frc/romi/OnBoardIO.h"
 RomiGyro = "frc/romi/RomiGyro.h"
 RomiMotor = "frc/romi/RomiMotor.h"
 
 [tool.robotpy-build.wrappers."romi".maven_lib_download]
 artifact_id = "romi-vendordep-cpp"
 group_id = "edu.wpi.first.romi"
-repo_url = "https://frcmaven.wpi.edu/artifactory/release"
-version = "2022.2.1"
+repo_url = "https://frcmaven.wpi.edu/artifactory/development"
+version = "2023.4.2"
 libs = ["Romi"]
 
 
-[tool.robotpy-build.metadata]
-name = "robotpy-romi"
-description = "Binary wrapper for WPILib Romi Vendor library"
-author = "RobotPy Development Team"
-author_email = "robotpy@googlegroups.com"
-url = "https://github.com/robotpy/robotpy-romi"
-license = "BSD-3-Clause"
-install_requires = [
-    "wpilib<2023.0.0,>=2022.2.1.3"
-]
```

### Comparing `robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/PKG-INFO` & `robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotpy-romi
-Version: 2022.2.1.0
+Version: 2023.4.2.0
 Summary: Binary wrapper for WPILib Romi Vendor library
 Home-page: https://github.com/robotpy/robotpy-romi
 Author: RobotPy Development Team
 Author-email: robotpy@googlegroups.com
 License: BSD-3-Clause
 Description: robotpy-romi
         ============
```

### Comparing `robotpy-romi-2022.2.1.0/robotpy_romi.egg-info/SOURCES.txt` & `robotpy-romi-2023.4.2.0/robotpy_romi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

