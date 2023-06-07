# Comparing `tmp/fileformats_testing-0.2.tar.gz` & `tmp/fileformats_testing-0.3.tar.gz`

## Comparing `fileformats_testing-0.2.tar` & `fileformats_testing-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.codespell-ignorewords
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.2/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.2/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/_version.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/basic.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/converters.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/headers.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 fileformats_testing-0.2/fileformats/testing/qualifers.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fileformats_testing-0.2/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_testing-0.2/LICENSE
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fileformats_testing-0.2/README.rst
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fileformats_testing-0.2/pyproject.toml
--rw-r--r--   0        0        0    17301 2020-02-02 00:00:00.000000 fileformats_testing-0.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_testing-0.3/.codespell-ignorewords
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.3/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_testing-0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.3/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_testing-0.3/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_testing-0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fileformats_testing-0.3/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fileformats_testing-0.3/fileformats/testing/_version.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats_testing-0.3/fileformats/testing/basic.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fileformats_testing-0.3/fileformats/testing/converters.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_testing-0.3/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 fileformats_testing-0.3/fileformats/testing/qualifers.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fileformats_testing-0.3/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_testing-0.3/LICENSE
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fileformats_testing-0.3/README.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fileformats_testing-0.3/pyproject.toml
+-rw-r--r--   0        0        0    17301 2020-02-02 00:00:00.000000 fileformats_testing-0.3/PKG-INFO
```

### Comparing `fileformats_testing-0.2/.pre-commit-config.yaml` & `fileformats_testing-0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/conftest.py` & `fileformats_testing-0.3/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/.github/workflows/publish.yml` & `fileformats_testing-0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/fileformats/testing/converters.py` & `fileformats_testing-0.3/fileformats/testing/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/fileformats/testing/headers.py` & `fileformats_testing-0.3/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/fileformats/testing/qualifers.py` & `fileformats_testing-0.3/fileformats/testing/qualifers.py`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/LICENSE` & `fileformats_testing-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/README.rst` & `fileformats_testing-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/pyproject.toml` & `fileformats_testing-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_testing-0.2/PKG-INFO` & `fileformats_testing-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-testing
-Version: 0.2
+Version: 0.3
 Summary: Dummy classes for testing the 'fileformats' package
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-testing
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

