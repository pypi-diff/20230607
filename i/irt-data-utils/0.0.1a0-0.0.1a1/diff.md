# Comparing `tmp/irt-data-utils-0.0.1a0.tar.gz` & `tmp/irt-data-utils-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irt-data-utils-0.0.1a0.tar", last modified: Wed Dec 14 14:52:08 2022, max compression
+gzip compressed data, was "irt-data-utils-0.0.1a1.tar", last modified: Wed Jun  7 02:42:47 2023, max compression
```

## Comparing `irt-data-utils-0.0.1a0.tar` & `irt-data-utils-0.0.1a1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 14:52:08.380907 irt-data-utils-0.0.1a0/
--rw-rw-rw-   0        0        0     1086 2022-12-14 14:51:58.000000 irt-data-utils-0.0.1a0/LICENSE
--rw-rw-rw-   0        0        0      270 2022-12-14 14:51:58.000000 irt-data-utils-0.0.1a0/MANIFEST.in
--rw-rw-rw-   0        0        0     1453 2022-12-14 14:52:08.381904 irt-data-utils-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0      265 2022-12-14 14:51:58.000000 irt-data-utils-0.0.1a0/README.md
--rw-rw-rw-   0        0        0       81 2022-12-14 14:52:08.381904 irt-data-utils-0.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0     8668 2022-12-14 14:51:58.000000 irt-data-utils-0.0.1a0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-14 14:52:08.366651 irt-data-utils-0.0.1a0/src/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:52:08.378884 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/
--rw-rw-rw-   0        0        0     1453 2022-12-14 14:52:08.000000 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2022-12-14 14:52:08.000000 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 14:52:08.000000 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-12-14 14:52:08.000000 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2022-12-14 14:52:08.000000 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-14 14:52:08.000000 irt-data-utils-0.0.1a0/src/irt_data_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-14 14:52:08.379910 irt-data-utils-0.0.1a0/src/irtdata/
--rw-rw-rw-   0        0        0     2400 2022-12-14 14:46:32.000000 irt-data-utils-0.0.1a0/src/irtdata/DDTFile.py
--rw-rw-rw-   0        0        0        0 2022-12-14 14:30:20.000000 irt-data-utils-0.0.1a0/src/irtdata/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-14 14:52:08.380907 irt-data-utils-0.0.1a0/src/irtdata/__pycache__/
--rw-rw-rw-   0        0        0     2373 2022-12-14 14:35:40.000000 irt-data-utils-0.0.1a0/src/irtdata/__pycache__/DDTFile.cpython-39.pyc
--rw-rw-rw-   0        0        0      169 2022-12-14 14:35:40.000000 irt-data-utils-0.0.1a0/src/irtdata/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-07 02:42:47.359806 irt-data-utils-0.0.1a1/
+-rw-rw-rw-   0        0        0     1106 2023-06-07 02:42:06.000000 irt-data-utils-0.0.1a1/LICENSE
+-rw-rw-rw-   0        0        0      270 2023-06-07 02:42:06.000000 irt-data-utils-0.0.1a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1616 2023-06-07 02:42:47.359806 irt-data-utils-0.0.1a1/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-06-07 02:42:06.000000 irt-data-utils-0.0.1a1/README.md
+-rw-rw-rw-   0        0        0       81 2023-06-07 02:42:47.362813 irt-data-utils-0.0.1a1/setup.cfg
+-rw-rw-rw-   0        0        0     8668 2023-06-07 02:42:06.000000 irt-data-utils-0.0.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 02:42:46.679080 irt-data-utils-0.0.1a1/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 02:42:46.970672 irt-data-utils-0.0.1a1/src/irt_data_utils.egg-info/
+-rw-rw-rw-   0        0        0     1616 2023-06-07 02:42:46.000000 irt-data-utils-0.0.1a1/src/irt_data_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-07 02:42:46.000000 irt-data-utils-0.0.1a1/src/irt_data_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 02:42:46.000000 irt-data-utils-0.0.1a1/src/irt_data_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-07 02:42:46.000000 irt-data-utils-0.0.1a1/src/irt_data_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 02:42:46.000000 irt-data-utils-0.0.1a1/src/irt_data_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 02:42:47.160757 irt-data-utils-0.0.1a1/src/irtdata/
+-rw-rw-rw-   0        0        0     2400 2022-12-14 14:46:32.000000 irt-data-utils-0.0.1a1/src/irtdata/DDTFile.py
+-rw-rw-rw-   0        0        0     5430 2023-06-07 02:37:36.000000 irt-data-utils-0.0.1a1/src/irtdata/FLIR.py
+-rw-rw-rw-   0        0        0        0 2022-12-14 14:30:20.000000 irt-data-utils-0.0.1a1/src/irtdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 02:42:47.358299 irt-data-utils-0.0.1a1/src/irtdata/__pycache__/
+-rw-rw-rw-   0        0        0     2373 2022-12-14 14:35:40.000000 irt-data-utils-0.0.1a1/src/irtdata/__pycache__/DDTFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4526 2023-06-07 02:36:10.000000 irt-data-utils-0.0.1a1/src/irtdata/__pycache__/FLIR.cpython-39.pyc
+-rw-rw-rw-   0        0        0      169 2022-12-14 14:35:40.000000 irt-data-utils-0.0.1a1/src/irtdata/__pycache__/__init__.cpython-39.pyc
```

### Comparing `irt-data-utils-0.0.1a0/LICENSE` & `irt-data-utils-0.0.1a1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `irt-data-utils-0.0.1a0/setup.py` & `irt-data-utils-0.0.1a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1a0',  # Required
+    version='0.0.1a1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Infrared Thermal Data Utils',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `irt-data-utils-0.0.1a0/src/irtdata/DDTFile.py` & `irt-data-utils-0.0.1a1/src/irtdata/DDTFile.py`

 * *Files identical despite different names*

### Comparing `irt-data-utils-0.0.1a0/src/irtdata/__pycache__/DDTFile.cpython-39.pyc` & `irt-data-utils-0.0.1a1/src/irtdata/__pycache__/DDTFile.cpython-39.pyc`

 * *Files identical despite different names*

