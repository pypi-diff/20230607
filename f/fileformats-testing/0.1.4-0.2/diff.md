# Comparing `tmp/fileformats_testing-0.1.4.tar.gz` & `tmp/fileformats_testing-0.2.tar.gz`

## Comparing `fileformats_testing-0.1.4.tar` & `fileformats_testing-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/.codespell-ignorewords
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/fileformats/testing/_version.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/fileformats/testing/basic.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/fileformats/testing/converters.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/fileformats/testing/headers.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/fileformats/testing/qualifers.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/LICENSE
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/README.rst
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    17343 2020-02-02 00:00:00.000000 fileformats_testing-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.codespell-ignorewords
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.2/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.2/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/_version.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/basic.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/converters.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/qualifers.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_testing-0.2/LICENSE
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fileformats_testing-0.2/README.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fileformats_testing-0.2/pyproject.toml
+-rw-r--r--   0        0        0    17301 2020-02-02 00:00:00.000000 fileformats_testing-0.2/PKG-INFO
```

### Comparing `fileformats_testing-0.1.4/.pre-commit-config.yaml` & `fileformats_testing-0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/conftest.py` & `fileformats_testing-0.2/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/.github/workflows/publish.yml` & `fileformats_testing-0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/fileformats/testing/converters.py` & `fileformats_testing-0.2/fileformats/testing/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/fileformats/testing/headers.py` & `fileformats_testing-0.2/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/fileformats/testing/qualifers.py` & `fileformats_testing-0.2/fileformats/testing/qualifers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as ty
 import attrs
 from fileformats.core import DataType
 from fileformats.generic import File
-from fileformats.field import Singluar
+from fileformats.field import Singular
 from fileformats.core.mixin import WithQualifiers
 
 
 class FileClassifier(DataType):
     pass
 
 
@@ -78,15 +78,15 @@
 class N(WithQualifiers, File):
     qualifiers_attr_name = "content_types"
     content_types = ()
     ext = ".n"
 
 
 @attrs.define
-class TestField(Singluar):
+class TestField(Singular):
 
     value: ty.Any
 
 
 class P(WithQualifiers, File):
     ext = ".p"
     qualifiers_attr_name = "content_types"
```

### Comparing `fileformats_testing-0.1.4/LICENSE` & `fileformats_testing-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/README.rst` & `fileformats_testing-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.1.4/pyproject.toml` & `fileformats_testing-0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "flake8",
     "flake8-pyproject",
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
-    "codecov",
 ]
 
 converters = [
     "pydra >= 0.20.0"
 ]
 
 [project.urls]
```

### Comparing `fileformats_testing-0.1.4/PKG-INFO` & `fileformats_testing-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-testing
-Version: 0.1.4
+Version: 0.2
 Summary: Dummy classes for testing the 'fileformats' package
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-testing
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -118,15 +118,14 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats Extension - Testing
 ===============================
```

