# Comparing `tmp/mock_data_generator-1.2.5.tar.gz` & `tmp/mock_data_generator-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.5.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.6.tar", max compression
```

## Comparing `mock_data_generator-1.2.5.tar` & `mock_data_generator-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.5/LICENSE
--rw-r--r--   0        0        0     2903 2023-06-07 06:54:20.675614 mock_data_generator-1.2.5/README.md
--rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.5/mock_data_generator/driver.py
--rw-r--r--   0        0        0     1030 2023-06-07 06:55:46.532920 mock_data_generator-1.2.5/mock_data_generator/generator/generate.py
--rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.5/mock_data_generator/generator/mappings.py
--rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.5/mock_data_generator/generator/misc.py
--rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.5/mock_data_generator/generator/output.py
--rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.5/mock_data_generator/generator/predefined.py
--rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.5/mock_data_generator/resources/config.ini
--rw-r--r--   0        0        0     1954 2023-06-07 06:55:45.873670 mock_data_generator-1.2.5/mock_data_generator/resources/schema.json
--rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.5/mock_data_generator/schema_handler/schema_validator.py
--rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.5/mock_data_generator/tests/fileutils_test.py
--rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.5/mock_data_generator/tests/schema_validator_test.py
--rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.5/mock_data_generator/tests/test.json
--rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.5/mock_data_generator/utils/constants.py
--rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.5/mock_data_generator/utils/fileutils.py
--rw-r--r--   0        0        0      947 2023-06-07 06:56:18.477609 mock_data_generator-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 mock_data_generator-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.6/LICENSE
+-rw-r--r--   0        0        0     2903 2023-06-07 06:54:20.675614 mock_data_generator-1.2.6/README.md
+-rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.6/mock_data_generator/driver.py
+-rw-r--r--   0        0        0     1030 2023-06-07 06:55:46.532920 mock_data_generator-1.2.6/mock_data_generator/generator/generate.py
+-rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.6/mock_data_generator/generator/mappings.py
+-rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.6/mock_data_generator/generator/misc.py
+-rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.6/mock_data_generator/generator/output.py
+-rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.6/mock_data_generator/generator/predefined.py
+-rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.6/mock_data_generator/resources/config.ini
+-rw-r--r--   0        0        0     1954 2023-06-07 06:55:45.873670 mock_data_generator-1.2.6/mock_data_generator/resources/schema.json
+-rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.6/mock_data_generator/schema_handler/schema_validator.py
+-rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.6/mock_data_generator/tests/fileutils_test.py
+-rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.6/mock_data_generator/tests/schema_validator_test.py
+-rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.6/mock_data_generator/tests/test.json
+-rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.6/mock_data_generator/utils/constants.py
+-rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.6/mock_data_generator/utils/fileutils.py
+-rw-r--r--   0        0        0      947 2023-06-07 07:07:53.366996 mock_data_generator-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 mock_data_generator-1.2.6/PKG-INFO
```

### Comparing `mock_data_generator-1.2.5/LICENSE` & `mock_data_generator-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/README.md` & `mock_data_generator-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/driver.py` & `mock_data_generator-1.2.6/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/generator/generate.py` & `mock_data_generator-1.2.6/mock_data_generator/generator/generate.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/generator/mappings.py` & `mock_data_generator-1.2.6/mock_data_generator/generator/mappings.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/generator/misc.py` & `mock_data_generator-1.2.6/mock_data_generator/generator/misc.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/generator/output.py` & `mock_data_generator-1.2.6/mock_data_generator/generator/output.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/resources/schema.json` & `mock_data_generator-1.2.6/mock_data_generator/resources/schema.json`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/schema_handler/schema_validator.py` & `mock_data_generator-1.2.6/mock_data_generator/schema_handler/schema_validator.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/tests/fileutils_test.py` & `mock_data_generator-1.2.6/mock_data_generator/tests/fileutils_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/tests/schema_validator_test.py` & `mock_data_generator-1.2.6/mock_data_generator/tests/schema_validator_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/utils/constants.py` & `mock_data_generator-1.2.6/mock_data_generator/utils/constants.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/mock_data_generator/utils/fileutils.py` & `mock_data_generator-1.2.6/mock_data_generator/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.5/pyproject.toml` & `mock_data_generator-1.2.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.5"
+version = "1.2.6"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
@@ -32,13 +32,13 @@
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "1.2.4"
+current_version = "1.2.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.2.5/PKG-INFO` & `mock_data_generator-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.5
+Version: 1.2.6
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

