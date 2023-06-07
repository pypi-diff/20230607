# Comparing `tmp/dwclib-2022.9.14.tar.gz` & `tmp/dwclib-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwclib-2022.9.14.tar", max compression
+gzip compressed data, was "dwclib-2023.6.7.tar", max compression
```

## Comparing `dwclib-2022.9.14.tar` & `dwclib-2023.6.7.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2022.9.14/LICENSE
--rw-r--r--   0        0        0     1263 2022-09-14 11:01:06.119049 dwclib-2022.9.14/README.md
--rw-r--r--   0        0        0      348 2022-08-03 21:04:16.883345 dwclib-2022.9.14/dwclib/__init__.py
--rw-r--r--   0        0        0     1138 2022-08-29 09:33:47.147038 dwclib-2022.9.14/dwclib/common/db.py
--rw-r--r--   0        0        0     1178 2022-08-29 09:43:53.277965 dwclib-2022.9.14/dwclib/common/meta.py
--rw-r--r--   0        0        0     2398 2022-09-14 10:49:41.882996 dwclib-2022.9.14/dwclib/common/numerics.py
--rw-r--r--   0        0        0     1397 2022-06-23 11:17:59.203893 dwclib-2022.9.14/dwclib/common/wave_unfold.py
--rw-r--r--   0        0        0     2178 2022-05-29 17:17:10.168724 dwclib-2022.9.14/dwclib/common/waves.py
--rw-r--r--   0        0        0      153 2022-06-23 12:44:07.658211 dwclib-2022.9.14/dwclib/dask/__init__.py
--rw-r--r--   0        0        0      917 2022-06-23 12:57:09.740836 dwclib-2022.9.14/dwclib/dask/generic.py
--rw-r--r--   0        0        0      820 2022-09-14 09:58:08.358141 dwclib-2022.9.14/dwclib/dask/numerics.py
--rw-r--r--   0        0        0      817 2022-08-03 21:01:26.270600 dwclib-2022.9.14/dwclib/dask/waves.py
--rw-r--r--   0        0        0     1419 2022-05-29 14:30:25.929650 dwclib-2022.9.14/dwclib/dask/waves_convert.py
--rw-r--r--   0        0        0       65 2022-05-16 14:58:12.304397 dwclib-2022.9.14/dwclib/numerics/__init__.py
--rw-r--r--   0        0        0     1551 2022-09-14 10:50:22.442995 dwclib-2022.9.14/dwclib/numerics/numerics.py
--rw-r--r--   0        0        0       95 2022-05-16 14:58:12.304397 dwclib-2022.9.14/dwclib/patients/__init__.py
--rw-r--r--   0        0        0     4141 2022-09-14 10:01:45.119302 dwclib-2022.9.14/dwclib/patients/patients.py
--rw-r--r--   0        0        0       56 2022-05-16 14:58:12.304397 dwclib-2022.9.14/dwclib/waves/__init__.py
--rw-r--r--   0        0        0     1334 2022-05-16 14:58:12.304397 dwclib-2022.9.14/dwclib/waves/waves.py
--rw-r--r--   0        0        0      801 2022-09-14 11:11:52.235164 dwclib-2022.9.14/pyproject.toml
--rw-r--r--   0        0        0     2127 2022-09-14 11:15:35.910340 dwclib-2022.9.14/setup.py
--rw-r--r--   0        0        0     2027 2022-09-14 11:15:35.910612 dwclib-2022.9.14/PKG-INFO
+-rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2023.6.7/LICENSE
+-rw-r--r--   0        0        0     1263 2022-09-14 11:01:06.119049 dwclib-2023.6.7/README.md
+-rw-r--r--   0        0        0      823 2023-06-07 10:28:17.376535 dwclib-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/__init__.py
+-rw-r--r--   0        0        0       59 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/alerts/__init__.py
+-rw-r--r--   0        0        0     2672 2023-03-03 15:13:00.467651 dwclib-2023.6.7/src/dwclib/alerts/alerts.py
+-rw-r--r--   0        0        0        0 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/assets/__init__.py
+-rw-r--r--   0        0        0   173360 2023-03-03 14:48:35.668082 dwclib-2023.6.7/src/dwclib/assets/alert_ref.csv
+-rw-r--r--   0        0        0     1451 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/db.py
+-rw-r--r--   0        0        0     1178 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/meta.py
+-rw-r--r--   0        0        0     2398 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/numerics.py
+-rw-r--r--   0        0        0     1397 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/wave_unfold.py
+-rw-r--r--   0        0        0     2178 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/common/waves.py
+-rw-r--r--   0        0        0      153 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/__init__.py
+-rw-r--r--   0        0        0      917 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/generic.py
+-rw-r--r--   0        0        0      820 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/numerics.py
+-rw-r--r--   0        0        0      817 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/waves.py
+-rw-r--r--   0        0        0     1419 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/waves_convert.py
+-rw-r--r--   0        0        0       65 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/numerics/__init__.py
+-rw-r--r--   0        0        0     1551 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/numerics/numerics.py
+-rw-r--r--   0        0        0       95 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/patients/__init__.py
+-rw-r--r--   0        0        0     4141 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/patients/patients.py
+-rw-r--r--   0        0        0       56 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/waves/__init__.py
+-rw-r--r--   0        0        0     1334 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/waves/waves.py
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 dwclib-2023.6.7/PKG-INFO
```

### Comparing `dwclib-2022.9.14/LICENSE` & `dwclib-2023.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/README.md` & `dwclib-2023.6.7/README.md`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/common/meta.py` & `dwclib-2023.6.7/src/dwclib/common/meta.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/common/numerics.py` & `dwclib-2023.6.7/src/dwclib/common/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/common/wave_unfold.py` & `dwclib-2023.6.7/src/dwclib/common/wave_unfold.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/common/waves.py` & `dwclib-2023.6.7/src/dwclib/common/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/dask/generic.py` & `dwclib-2023.6.7/src/dwclib/dask/generic.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/dask/numerics.py` & `dwclib-2023.6.7/src/dwclib/dask/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/dask/waves.py` & `dwclib-2023.6.7/src/dwclib/dask/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/dask/waves_convert.py` & `dwclib-2023.6.7/src/dwclib/dask/waves_convert.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/numerics/numerics.py` & `dwclib-2023.6.7/src/dwclib/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/patients/patients.py` & `dwclib-2023.6.7/src/dwclib/patients/patients.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/dwclib/waves/waves.py` & `dwclib-2023.6.7/src/dwclib/waves/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2022.9.14/pyproject.toml` & `dwclib-2023.6.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dwclib"
-version = "2022.9.14"
+version = "2023.6.7"
 description = "Python wrapper to DataWarehouse Connect"
 authors = ["Jona Joachim <jona@joachim.cc>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/larib-data/dwclib"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-numpy = "~1.22"
-pandas = "~1.4"
-numba = "~0.55"
-dask = "^2022"
+python = ">=3.8,<4"
+numpy = "^1"
+pandas = ">=1.4,<3"
+numba = "~0.57"
+dask = ">=2022"
 SQLAlchemy = "~1.4"
+platformdirs = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 flake8-bandit = "^3.0.0"
 safety = "^1.10.3"
 flake8-bugbear = "^22.4.25"
 Sphinx = "^5.0.1"
```

### Comparing `dwclib-2022.9.14/setup.py` & `dwclib-2023.6.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,59 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dwclib
+Version: 2023.6.7
+Summary: Python wrapper to DataWarehouse Connect
+Home-page: https://github.com/larib-data/dwclib
+License: ISC
+Author: Jona Joachim
+Author-email: jona@joachim.cc
+Requires-Python: >=3.8,<4
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: SQLAlchemy (>=1.4,<1.5)
+Requires-Dist: dask (>=2022)
+Requires-Dist: numba (>=0.57,<0.58)
+Requires-Dist: numpy (>=1,<2)
+Requires-Dist: pandas (>=1.4,<3)
+Requires-Dist: platformdirs (>=3.0.0,<4.0.0)
+Project-URL: Repository, https://github.com/larib-data/dwclib
+Description-Content-Type: text/markdown
+
+# Overview
+Python wrapper to DataWarehouse Connect.
+-   Free software: ISC license
+
+## Installation
+`conda install -c conda-forge dwclib`
+
+`pip install dwclib`
+
+Installation through conda greatly simplifies dependency management.
+
+Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
+See here for more information: https://github.com/mkleehammer/pyodbc/wiki
+
+
+## Changelog
+- 2022.9.14
+    - Support numeric labels and sublabels in read_patients and read_numerics
+    - Support to query for multiple patients at once in read_numerics
+
+- 2022.6.23
+    - Convert packaging from flit to poetry
+    - Add linting and testing with nox, flake8 and safety
+    - Create scaffolding for future Sphinx documentation
+    - Fix a number of bugs in corner cases (division by zero, ...)
+    - Add a generic Dask wrapper to run custom DWC queries with Dask
+
+- 2022.3.22
+    - Convert packaging from old-style setup.py to flit
+    - Refactor: extract common code between dask and pandas version
+    - No longer relies on user defined function in the database
+    - Patients: add read_patient function to fetch a single patient
+    - Numerics: read_numerics patientids can be a list or a str. When it is a list, a MultiIndex is returned
 
-packages = \
-['dwclib',
- 'dwclib.common',
- 'dwclib.dask',
- 'dwclib.numerics',
- 'dwclib.patients',
- 'dwclib.waves']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['SQLAlchemy>=1.4,<1.5',
- 'dask>=2022,<2023',
- 'numba>=0.55,<0.56',
- 'numpy>=1.22,<1.23',
- 'pandas>=1.4,<1.5']
-
-setup_kwargs = {
-    'name': 'dwclib',
-    'version': '2022.9.14',
-    'description': 'Python wrapper to DataWarehouse Connect',
-    'long_description': '# Overview\nPython wrapper to DataWarehouse Connect.\n-   Free software: ISC license\n\n## Installation\n`conda install -c conda-forge dwclib`\n\n`pip install dwclib`\n\nInstallation through conda greatly simplifies dependency management.\n\nAdditionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.\nSee here for more information: https://github.com/mkleehammer/pyodbc/wiki\n\n\n## Changelog\n- 2022.9.14\n    - Support numeric labels and sublabels in read_patients and read_numerics\n    - Support to query for multiple patients at once in read_numerics\n\n- 2022.6.23\n    - Convert packaging from flit to poetry\n    - Add linting and testing with nox, flake8 and safety\n    - Create scaffolding for future Sphinx documentation\n    - Fix a number of bugs in corner cases (division by zero, ...)\n    - Add a generic Dask wrapper to run custom DWC queries with Dask\n\n- 2022.3.22\n    - Convert packaging from old-style setup.py to flit\n    - Refactor: extract common code between dask and pandas version\n    - No longer relies on user defined function in the database\n    - Patients: add read_patient function to fetch a single patient\n    - Numerics: read_numerics patientids can be a list or a str. When it is a list, a MultiIndex is returned\n\n',
-    'author': 'Jona Joachim',
-    'author_email': 'jona@joachim.cc',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/larib-data/dwclib',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
 
-
-setup(**setup_kwargs)
```

