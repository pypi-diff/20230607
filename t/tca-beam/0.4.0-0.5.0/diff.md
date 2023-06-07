# Comparing `tmp/tca_beam-0.4.0.tar.gz` & `tmp/tca_beam-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.4.0.tar", max compression
+gzip compressed data, was "tca_beam-0.5.0.tar", max compression
```

## Comparing `tca_beam-0.4.0.tar` & `tca_beam-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.4.0/README.md
--rw-r--r--   0        0        0      425 2023-06-06 10:04:56.526747 tca_beam-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.4.0/tca_beam/__init__.py
--rw-r--r--   0        0        0      459 2023-06-06 09:39:44.292506 tca_beam-0.4.0/tca_beam/click_sample.py
--rw-r--r--   0        0        0     1325 2023-06-06 08:44:16.962819 tca_beam-0.4.0/tca_beam/nogroup_demo.py
--rw-r--r--   0        0        0     6703 2023-06-06 09:44:49.698473 tca_beam-0.4.0/tca_beam/tca_beam.py
--rw-r--r--   0        0        0      526 2023-06-05 10:09:21.285125 tca_beam-0.4.0/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-04 16:14:37.894614 tca_beam-0.4.0/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.4.0/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.4.0/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      633 2023-06-05 09:48:58.421080 tca_beam-0.4.0/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.4.0/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.4.0/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.5.0/README.md
+-rw-r--r--   0        0        0      425 2023-06-07 20:39:31.828225 tca_beam-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.5.0/tca_beam/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-07 20:35:05.908095 tca_beam-0.5.0/tca_beam/config.py
+-rw-r--r--   0        0        0     6778 2023-06-07 20:38:27.028889 tca_beam-0.5.0/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0      628 2023-06-07 19:24:52.000000 tca_beam-0.5.0/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-07 17:31:44.668724 tca_beam-0.5.0/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.5.0/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.5.0/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0      723 2023-06-07 19:20:58.432700 tca_beam-0.5.0/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.5.0/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.5.0/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.5.0/PKG-INFO
```

### Comparing `tca_beam-0.4.0/setup.py` & `tca_beam-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Feature stub generation for The Composable Architecture',
     'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tca_beam-0.4.0/PKG-INFO` & `tca_beam-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.4.0
+Version: 0.5.0
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

