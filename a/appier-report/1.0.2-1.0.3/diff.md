# Comparing `tmp/appier_report-1.0.2.tar.gz` & `tmp/appier_report-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appier_report-1.0.2.tar", max compression
+gzip compressed data, was "appier_report-1.0.3.tar", max compression
```

## Comparing `appier_report-1.0.2.tar` & `appier_report-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-06 11:27:55.672820 appier_report-1.0.2/LICENSE
--rw-r--r--   0        0        0      712 2023-06-06 11:27:55.672820 appier_report-1.0.2/README.md
--rw-r--r--   0        0        0       67 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/__init__.py
--rw-r--r--   0        0        0     4190 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/cost_api.py
--rw-r--r--   0        0        0        0 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/utils/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/utils/date_utils.py
--rw-r--r--   0        0        0     2560 2023-06-06 11:27:55.672820 appier_report-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-06 11:27:55.672820 appier_report-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-06 11:27:55.672820 appier_report-1.0.2/tests/test_app.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-07 07:11:11.655702 appier_report-1.0.3/LICENSE
+-rw-r--r--   0        0        0      712 2023-06-07 07:11:11.655702 appier_report-1.0.3/README.md
+-rw-r--r--   0        0        0       67 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/__init__.py
+-rw-r--r--   0        0        0     4430 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/cost_api.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/utils/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/utils/date_utils.py
+-rw-r--r--   0        0        0     2560 2023-06-07 07:11:11.659702 appier_report-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-07 07:11:11.659702 appier_report-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-07 07:11:11.659702 appier_report-1.0.3/tests/test_app.py
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.0.3/PKG-INFO
```

### Comparing `appier_report-1.0.2/LICENSE` & `appier_report-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.2/README.md` & `appier_report-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.2/appier_report/utils/date_utils.py` & `appier_report-1.0.3/appier_report/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.2/pyproject.toml` & `appier_report-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "appier-report"
-version = "1.0.2"
+version = "1.0.3"
 homepage = "https://github.com/ikamedawn/appier-report"
 description = "Report APIs wrapper"
 authors = ["ikamedawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `appier_report-1.0.2/tests/test_app.py` & `appier_report-1.0.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.2/PKG-INFO` & `appier_report-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appier-report
-Version: 1.0.2
+Version: 1.0.3
 Summary: Report APIs wrapper
 Home-page: https://github.com/ikamedawn/appier-report
 License: MIT
 Author: ikamedawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

