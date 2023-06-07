# Comparing `tmp/mock_data_generator-1.2.4.tar.gz` & `tmp/mock_data_generator-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.4.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.5.tar", max compression
```

## Comparing `mock_data_generator-1.2.4.tar` & `mock_data_generator-1.2.5.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.4/LICENSE
--rw-r--r--   0        0        0     2440 2023-06-06 05:50:20.846447 mock_data_generator-1.2.4/README.md
--rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.4/mock_data_generator/driver.py
--rw-r--r--   0        0        0     2519 2023-06-06 05:48:30.284997 mock_data_generator-1.2.4/mock_data_generator/generator/generate.py
--rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.4/mock_data_generator/resources/config.ini
--rw-r--r--   0        0        0      348 2023-06-06 05:48:30.286577 mock_data_generator-1.2.4/mock_data_generator/resources/schema.json
--rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.4/mock_data_generator/schema_handler/schema_validator.py
--rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.4/mock_data_generator/tests/fileutils_test.py
--rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.4/mock_data_generator/tests/schema_validator_test.py
--rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.4/mock_data_generator/tests/test.json
--rw-r--r--   0        0        0      152 2023-06-06 05:48:30.289575 mock_data_generator-1.2.4/mock_data_generator/utils/constants.py
--rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.4/mock_data_generator/utils/fileutils.py
--rw-r--r--   0        0        0      947 2023-06-06 05:56:11.033730 mock_data_generator-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 mock_data_generator-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.5/LICENSE
+-rw-r--r--   0        0        0     2903 2023-06-07 06:54:20.675614 mock_data_generator-1.2.5/README.md
+-rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.5/mock_data_generator/driver.py
+-rw-r--r--   0        0        0     1030 2023-06-07 06:55:46.532920 mock_data_generator-1.2.5/mock_data_generator/generator/generate.py
+-rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.5/mock_data_generator/generator/mappings.py
+-rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.5/mock_data_generator/generator/misc.py
+-rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.5/mock_data_generator/generator/output.py
+-rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.5/mock_data_generator/generator/predefined.py
+-rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.5/mock_data_generator/resources/config.ini
+-rw-r--r--   0        0        0     1954 2023-06-07 06:55:45.873670 mock_data_generator-1.2.5/mock_data_generator/resources/schema.json
+-rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.5/mock_data_generator/schema_handler/schema_validator.py
+-rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.5/mock_data_generator/tests/fileutils_test.py
+-rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.5/mock_data_generator/tests/schema_validator_test.py
+-rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.5/mock_data_generator/tests/test.json
+-rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.5/mock_data_generator/utils/constants.py
+-rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.5/mock_data_generator/utils/fileutils.py
+-rw-r--r--   0        0        0      947 2023-06-07 06:56:18.477609 mock_data_generator-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 mock_data_generator-1.2.5/PKG-INFO
```

### Comparing `mock_data_generator-1.2.4/LICENSE` & `mock_data_generator-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.4/README.md` & `mock_data_generator-1.2.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
 Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
 ### Inputs
-It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
+It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP","ADDRESS","CITY","COUNTRY","COUNTRY_CODE","POSTCODE","LICENSE_PLATE","SWIFT","COMPANY","COMPANY_SUFFIX","CREDIT_CARD","CREDIT_CARD_PROVIDER","CREDIT_CARD_NUMBER","CURRENCY","DAY_NUM","DAY_NAME","MONTH_NUM","MONTH_NAME","YEAR","COORDINATE","LATITUDE","LONGITUDE","EMAIL","HOSTNAME","IPV4","IPV6","URI","URL","JOB","TEXT","PASSWORD","SHA1","SHA256","UUID","PASSPORT_NUMBER","NAME","LANGUAGE_NAME","LAST_NAME","FIRST_NAME","PHONE_NUMBER","SSN"`
 #### Supported Input Parameters
 
 - --input_json_schema_path: Provide absolute path of the json schema file/folder. It accepts folders(that contains valid json schema files) or absolute path of a json schema file.
 
 > Json schema file format.
 ```json
 {
@@ -27,21 +27,21 @@
 ```
 > The sample json schema file would look like below.
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
-    "name": { "type": "string" },
-    "a": { "type": "integer" },
-    "b": { "type": "float" },
-    "c": { "type": "boolean" },
+    "name": { "type": "name" },
+    "location": { "type": "COORDINATE" },
+    "flt": { "type": "float" },
+    "email_id": { "type": "EMAIL" },
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
-    "e": { "type": "boolean" }
+    "is_valid": { "type": "boolean" }
   }
 }
 ```
 The generator will skip the current json schema file if an error occurred. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
```

### Comparing `mock_data_generator-1.2.4/mock_data_generator/driver.py` & `mock_data_generator-1.2.5/mock_data_generator/driver.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.4/mock_data_generator/schema_handler/schema_validator.py` & `mock_data_generator-1.2.5/mock_data_generator/schema_handler/schema_validator.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.4/mock_data_generator/tests/fileutils_test.py` & `mock_data_generator-1.2.5/mock_data_generator/tests/fileutils_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.4/mock_data_generator/tests/schema_validator_test.py` & `mock_data_generator-1.2.5/mock_data_generator/tests/schema_validator_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.4/mock_data_generator/utils/fileutils.py` & `mock_data_generator-1.2.5/mock_data_generator/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.4/pyproject.toml` & `mock_data_generator-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.4"
+version = "1.2.5"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
```

### Comparing `mock_data_generator-1.2.4/PKG-INFO` & `mock_data_generator-1.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.4
+Version: 1.2.5
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
 
 ## How to use
 Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
 ### Inputs
-It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP"`
+It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP","ADDRESS","CITY","COUNTRY","COUNTRY_CODE","POSTCODE","LICENSE_PLATE","SWIFT","COMPANY","COMPANY_SUFFIX","CREDIT_CARD","CREDIT_CARD_PROVIDER","CREDIT_CARD_NUMBER","CURRENCY","DAY_NUM","DAY_NAME","MONTH_NUM","MONTH_NAME","YEAR","COORDINATE","LATITUDE","LONGITUDE","EMAIL","HOSTNAME","IPV4","IPV6","URI","URL","JOB","TEXT","PASSWORD","SHA1","SHA256","UUID","PASSPORT_NUMBER","NAME","LANGUAGE_NAME","LAST_NAME","FIRST_NAME","PHONE_NUMBER","SSN"`
 #### Supported Input Parameters
 
 - --input_json_schema_path: Provide absolute path of the json schema file/folder. It accepts folders(that contains valid json schema files) or absolute path of a json schema file.
 
 > Json schema file format.
 ```json
 {
@@ -49,21 +49,21 @@
 ```
 > The sample json schema file would look like below.
 ```json
 {
   "type": "object",
   "properties": {
     "price": { "type": "number" },
-    "name": { "type": "string" },
-    "a": { "type": "integer" },
-    "b": { "type": "float" },
-    "c": { "type": "boolean" },
+    "name": { "type": "name" },
+    "location": { "type": "COORDINATE" },
+    "flt": { "type": "float" },
+    "email_id": { "type": "EMAIL" },
     "dt": { "type": "date" },
     "ts": { "type": "timestamp" },
-    "e": { "type": "boolean" }
+    "is_valid": { "type": "boolean" }
   }
 }
 ```
 The generator will skip the current json schema file if an error occurred. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
```

