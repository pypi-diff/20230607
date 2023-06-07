# Comparing `tmp/mock_data_generator-1.2.7.tar.gz` & `tmp/mock_data_generator-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.7.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.8.tar", max compression
```

## Comparing `mock_data_generator-1.2.7.tar` & `mock_data_generator-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.7/LICENSE
--rw-r--r--   0        0        0     3015 2023-06-07 11:10:02.591876 mock_data_generator-1.2.7/README.md
--rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.7/mock_data_generator/driver.py
--rw-r--r--   0        0        0     1030 2023-06-07 06:55:46.532920 mock_data_generator-1.2.7/mock_data_generator/generator/generate.py
--rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.7/mock_data_generator/generator/mappings.py
--rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.7/mock_data_generator/generator/misc.py
--rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.7/mock_data_generator/generator/output.py
--rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.7/mock_data_generator/generator/predefined.py
--rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.7/mock_data_generator/resources/config.ini
--rw-r--r--   0        0        0     1954 2023-06-07 06:55:45.873670 mock_data_generator-1.2.7/mock_data_generator/resources/schema.json
--rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.7/mock_data_generator/schema_handler/schema_validator.py
--rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.7/mock_data_generator/tests/fileutils_test.py
--rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.7/mock_data_generator/tests/schema_validator_test.py
--rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.7/mock_data_generator/tests/test.json
--rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.7/mock_data_generator/utils/constants.py
--rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.7/mock_data_generator/utils/fileutils.py
--rw-r--r--   0        0        0      947 2023-06-07 11:10:49.900882 mock_data_generator-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     3806 1970-01-01 00:00:00.000000 mock_data_generator-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.8/LICENSE
+-rw-r--r--   0        0        0     3021 2023-06-07 11:12:55.484556 mock_data_generator-1.2.8/README.md
+-rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.8/mock_data_generator/driver.py
+-rw-r--r--   0        0        0     1030 2023-06-07 06:55:46.532920 mock_data_generator-1.2.8/mock_data_generator/generator/generate.py
+-rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.8/mock_data_generator/generator/mappings.py
+-rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.8/mock_data_generator/generator/misc.py
+-rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.8/mock_data_generator/generator/output.py
+-rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.8/mock_data_generator/generator/predefined.py
+-rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.8/mock_data_generator/resources/config.ini
+-rw-r--r--   0        0        0     1954 2023-06-07 06:55:45.873670 mock_data_generator-1.2.8/mock_data_generator/resources/schema.json
+-rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.8/mock_data_generator/schema_handler/schema_validator.py
+-rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.8/mock_data_generator/tests/fileutils_test.py
+-rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.8/mock_data_generator/tests/schema_validator_test.py
+-rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.8/mock_data_generator/tests/test.json
+-rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.8/mock_data_generator/utils/constants.py
+-rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.8/mock_data_generator/utils/fileutils.py
+-rw-r--r--   0        0        0      947 2023-06-07 11:15:45.168252 mock_data_generator-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 mock_data_generator-1.2.8/PKG-INFO
```

### Comparing `mock_data_generator-1.2.7/LICENSE` & `mock_data_generator-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/README.md` & `mock_data_generator-1.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Data Generator - WIP
 
 ## Overview
 During every data project I came across a very basic common problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those have certain limitations on the number of columns and rows.
 To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
-Step by step on [medium](https://medium.com/@rahulsmtauti/mock-data-generation-for-data-projects-3999865cb82c).
+Step by step guide on [medium](https://medium.com/@rahulsmtauti/mock-data-generation-for-data-projects-3999865cb82c).
 
 ## How to use
 Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
 ### Inputs
 It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP","ADDRESS","CITY","COUNTRY","COUNTRY_CODE","POSTCODE","LICENSE_PLATE","SWIFT","COMPANY","COMPANY_SUFFIX","CREDIT_CARD","CREDIT_CARD_PROVIDER","CREDIT_CARD_NUMBER","CURRENCY","DAY_NUM","DAY_NAME","MONTH_NUM","MONTH_NAME","YEAR","COORDINATE","LATITUDE","LONGITUDE","EMAIL","HOSTNAME","IPV4","IPV6","URI","URL","JOB","TEXT","PASSWORD","SHA1","SHA256","UUID","PASSPORT_NUMBER","NAME","LANGUAGE_NAME","LAST_NAME","FIRST_NAME","PHONE_NUMBER","SSN"`
 #### Supported Input Parameters
```

### Comparing `mock_data_generator-1.2.7/mock_data_generator/driver.py` & `mock_data_generator-1.2.8/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/generator/generate.py` & `mock_data_generator-1.2.8/mock_data_generator/generator/generate.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/generator/mappings.py` & `mock_data_generator-1.2.8/mock_data_generator/generator/mappings.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/generator/misc.py` & `mock_data_generator-1.2.8/mock_data_generator/generator/misc.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/generator/output.py` & `mock_data_generator-1.2.8/mock_data_generator/generator/output.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/resources/schema.json` & `mock_data_generator-1.2.8/mock_data_generator/resources/schema.json`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/schema_handler/schema_validator.py` & `mock_data_generator-1.2.8/mock_data_generator/schema_handler/schema_validator.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/tests/fileutils_test.py` & `mock_data_generator-1.2.8/mock_data_generator/tests/fileutils_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/tests/schema_validator_test.py` & `mock_data_generator-1.2.8/mock_data_generator/tests/schema_validator_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/utils/constants.py` & `mock_data_generator-1.2.8/mock_data_generator/utils/constants.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/mock_data_generator/utils/fileutils.py` & `mock_data_generator-1.2.8/mock_data_generator/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.7/pyproject.toml` & `mock_data_generator-1.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.7"
+version = "1.2.8"
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
-current_version = "1.2.7"
+current_version = "1.2.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.2.7/PKG-INFO` & `mock_data_generator-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.7
+Version: 1.2.8
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 
 # Data Generator - WIP
 
 ## Overview
 During every data project I came across a very basic common problem where we have to wait for the test data. For fewer columns it's quite easy to generate the data using online utilities but those have certain limitations on the number of columns and rows.
 To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
-Step by step on [medium](https://medium.com/@rahulsmtauti/mock-data-generation-for-data-projects-3999865cb82c).
+Step by step guide on [medium](https://medium.com/@rahulsmtauti/mock-data-generation-for-data-projects-3999865cb82c).
 
 ## How to use
 Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
 ### Inputs
 It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP","ADDRESS","CITY","COUNTRY","COUNTRY_CODE","POSTCODE","LICENSE_PLATE","SWIFT","COMPANY","COMPANY_SUFFIX","CREDIT_CARD","CREDIT_CARD_PROVIDER","CREDIT_CARD_NUMBER","CURRENCY","DAY_NUM","DAY_NAME","MONTH_NUM","MONTH_NAME","YEAR","COORDINATE","LATITUDE","LONGITUDE","EMAIL","HOSTNAME","IPV4","IPV6","URI","URL","JOB","TEXT","PASSWORD","SHA1","SHA256","UUID","PASSPORT_NUMBER","NAME","LANGUAGE_NAME","LAST_NAME","FIRST_NAME","PHONE_NUMBER","SSN"`
 #### Supported Input Parameters
```

