# Comparing `tmp/tcare_sbvalidator-0.0.5.tar.gz` & `tmp/tcare_sbvalidator-0.0.6.tar.gz`

## Comparing `tcare_sbvalidator-0.0.5.tar` & `tcare_sbvalidator-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/reqs.txt
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/test.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/test2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/sb_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/models/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/models/cloudevents.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/reqs.txt
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/test.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/test2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/src/tcare_sbvalidator/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/src/tcare_sbvalidator/sb_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/src/tcare_sbvalidator/models/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/src/tcare_sbvalidator/models/cloudevents.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.6/PKG-INFO
```

### Comparing `tcare_sbvalidator-0.0.5/requirements.txt` & `tcare_sbvalidator-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.5/src/tcare_sbvalidator/sb_validator.py` & `tcare_sbvalidator-0.0.6/src/tcare_sbvalidator/sb_validator.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.5/.gitignore` & `tcare_sbvalidator-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.5/LICENSE.txt` & `tcare_sbvalidator-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.5/pyproject.toml` & `tcare_sbvalidator-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcare_sbvalidator"
-version = "0.0.5"
+version = "0.0.6"
+dependencies = [ "pydantic" ]
 authors = [
   { name="TCARE", email="elijah.kennedy@tcare.ai" },
 ]
 description = "Validate that servicebus messages are in the correct format"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcare_sbvalidator-0.0.5/PKG-INFO` & `tcare_sbvalidator-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tcare_sbvalidator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Validate that servicebus messages are in the correct format
 Project-URL: Homepage, https://github.com/TCARE1/tcare_sbvalidator
 Project-URL: Bug Tracker, https://github.com/TCARE1/tcare_sbvalidator/issues
 Author-email: TCARE <elijah.kennedy@tcare.ai>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # Tcare Servicebus Validotor (tcare-sbv)
 
 This package was developed to validate all messages passed to and received from azure service bus. This is achieved by a series of common schemas declared with Pydantic's class-based validation.
 
 # Publishing
```

