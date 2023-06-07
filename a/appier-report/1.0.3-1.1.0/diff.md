# Comparing `tmp/appier_report-1.0.3.tar.gz` & `tmp/appier_report-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appier_report-1.0.3.tar", max compression
+gzip compressed data, was "appier_report-1.1.0.tar", max compression
```

## Comparing `appier_report-1.0.3.tar` & `appier_report-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-07 07:11:11.655702 appier_report-1.0.3/LICENSE
--rw-r--r--   0        0        0      712 2023-06-07 07:11:11.655702 appier_report-1.0.3/README.md
--rw-r--r--   0        0        0       67 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/__init__.py
--rw-r--r--   0        0        0     4430 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/cost_api.py
--rw-r--r--   0        0        0        0 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/utils/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-07 07:11:11.655702 appier_report-1.0.3/appier_report/utils/date_utils.py
--rw-r--r--   0        0        0     2560 2023-06-07 07:11:11.659702 appier_report-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-07 07:11:11.659702 appier_report-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-07 07:11:11.659702 appier_report-1.0.3/tests/test_app.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-07 08:33:28.645925 appier_report-1.1.0/LICENSE
+-rw-r--r--   0        0        0      712 2023-06-07 08:33:28.645925 appier_report-1.1.0/README.md
+-rw-r--r--   0        0        0       67 2023-06-07 08:33:28.645925 appier_report-1.1.0/appier_report/__init__.py
+-rw-r--r--   0        0        0     3785 2023-06-07 08:33:28.645925 appier_report-1.1.0/appier_report/cost_api.py
+-rw-r--r--   0        0        0        0 2023-06-07 08:33:28.645925 appier_report-1.1.0/appier_report/utils/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-07 08:33:28.645925 appier_report-1.1.0/appier_report/utils/date_utils.py
+-rw-r--r--   0        0        0     2560 2023-06-07 08:33:28.649925 appier_report-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-07 08:33:28.649925 appier_report-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-07 08:33:28.649925 appier_report-1.1.0/tests/test_app.py
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.1.0/PKG-INFO
```

### Comparing `appier_report-1.0.3/LICENSE` & `appier_report-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.3/README.md` & `appier_report-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.3/appier_report/cost_api.py` & `appier_report-1.1.0/appier_report/cost_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import time
-import traceback
-from datetime import datetime, timedelta
-
 import requests
-
+from requests.adapters import HTTPAdapter
+from datetime import datetime, timedelta
 from appier_report.utils.date_utils import DateUtils
 
 
 class Report:
     """
     This class is used to interact with the Appier Campaign Report API.
     """
@@ -36,15 +33,14 @@
 
     def _get_report(
         self,
         start_date: str = None,
         end_date: str = None,
         timezone: int = 0,
         max_retries: int = 3,
-        retry_interval: int = 30,
         **kwargs,
     ) -> list[dict]:
         """
         Get campaign report data from Appier Cost API.
 
         Args:
             start_date: Format YYYY-MM-DD
@@ -66,49 +62,41 @@
         params = {
             "access_token": self.access_token,
             "start_date": start_date,
             "end_date": end_date,
             "timezone": timezone,
             **kwargs,
         }
-
-        for i in range(max_retries + 1):
-            try:
-                response = requests.get(url=self.endpoint, params=params)
-                if response.status_code == 200:
-                    return response.json()
-            except Exception as e:
-                print(f"Error: {e}")
-                print('---------------------------------')
-                print(traceback.format_exc())
-                print('---------------------------------')
-                print(f"Retrying in {retry_interval} seconds...")
-                time.sleep(retry_interval)
-        raise Exception(f"Error: {response.status_code}")
+        adapter = HTTPAdapter(max_retries=max_retries)
+        with requests.Session() as session:
+            session.mount(self.endpoint, adapter)
+            response = session.get(url=self.endpoint, params=params)
+            if response.status_code == 200:
+                return response.json()
+            else:
+                raise Exception(f"Error: {response.status_code}")
 
     def get_report(
         self,
         start_date: str = None,
         end_date: str = None,
         date_interval: int = 5,
         timezone: int = 0,
         max_retries: int = 3,
-        retry_interval: int = 30,
         **kwargs,
     ) -> list[dict]:
         """
         Wrapper for _get_report() to get report data from Appier Cost API.
 
         Args:
             start_date: Format YYYY-MM-DD
             end_date: Format YYYY-MM-DD
             date_interval: Number of days between each request.
             timezone: Timezone offset in hours.
             max_retries: Number of retries before giving up.
-            retry_interval: Time to wait between retries.
             **kwargs: Other parameters
 
         Returns:
             Report data in JSON format.
         Doc Author:
             minhpc@ikameglobal.com
         """
@@ -122,19 +110,12 @@
         for start, end in date_ranges:
             result.extend(
                 self._get_report(
                     start_date=start,
                     end_date=end,
                     timezone=timezone,
                     max_retries=max_retries,
-                    retry_interval=retry_interval,
                     **kwargs,
                 )
             )
 
         return result
-
-
-if __name__ == '__main__':
-    inventory_report = Report(access_token="52da5d8cd6a84a9dbef1fd7c55159193", api_type='inventory')
-    report = inventory_report.get_report(start_date='2023-06-04', end_date='2023-06-04')
-    print(report)
```

### Comparing `appier_report-1.0.3/appier_report/utils/date_utils.py` & `appier_report-1.1.0/appier_report/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.3/pyproject.toml` & `appier_report-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "appier-report"
-version = "1.0.3"
+version = "1.1.0"
 homepage = "https://github.com/ikamedawn/appier-report"
 description = "Report APIs wrapper"
 authors = ["ikamedawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `appier_report-1.0.3/tests/test_app.py` & `appier_report-1.1.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.3/PKG-INFO` & `appier_report-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appier-report
-Version: 1.0.3
+Version: 1.1.0
 Summary: Report APIs wrapper
 Home-page: https://github.com/ikamedawn/appier-report
 License: MIT
 Author: ikamedawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

