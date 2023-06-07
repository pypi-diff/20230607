# Comparing `tmp/tcare_sbvalidator-0.0.7.tar.gz` & `tmp/tcare_sbvalidator-0.0.8.tar.gz`

## Comparing `tcare_sbvalidator-0.0.7.tar` & `tcare_sbvalidator-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/Makefile
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/reqs.txt
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/requirements.txt
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/test.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/test2.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/uploadkey
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/sb_validator.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/sms_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/models/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/models/cloudevents.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/Makefile
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/reqs.txt
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/test.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/test2.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/uploadkey
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sb_validator.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sms_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/models/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/models/cloudevents.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/PKG-INFO
```

### Comparing `tcare_sbvalidator-0.0.7/requirements.txt` & `tcare_sbvalidator-0.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.7/test.py` & `tcare_sbvalidator-0.0.8/test.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/sb_validator.py` & `tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sb_validator.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.7/src/tcare_sbvalidator/sms_handler.py` & `tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sms_handler.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.7/.gitignore` & `tcare_sbvalidator-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.7/LICENSE.txt` & `tcare_sbvalidator-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.7/pyproject.toml` & `tcare_sbvalidator-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcare_sbvalidator"
-version = "0.0.7"
-dependencies = [ "pydantic", "azure-identity", "azure-servicebus", "azure"]
+version = "0.0.8"
+dependencies = [ "pydantic", "azure-identity", "azure-servicebus"]
 authors = [
   { name="TCARE", email="elijah.kennedy@tcare.ai" },
 ]
 description = "Validate that servicebus messages are in the correct format"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcare_sbvalidator-0.0.7/PKG-INFO` & `tcare_sbvalidator-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: tcare_sbvalidator
-Version: 0.0.7
+Version: 0.0.8
 Summary: Validate that servicebus messages are in the correct format
 Project-URL: Homepage, https://github.com/TCARE1/tcare_sbvalidator
 Project-URL: Bug Tracker, https://github.com/TCARE1/tcare_sbvalidator/issues
 Author-email: TCARE <elijah.kennedy@tcare.ai>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: azure
 Requires-Dist: azure-identity
 Requires-Dist: azure-servicebus
 Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # Tcare Servicebus Validotor (tcare-sbv)
```

