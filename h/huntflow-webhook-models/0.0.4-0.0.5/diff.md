# Comparing `tmp/huntflow_webhook_models-0.0.4.tar.gz` & `tmp/huntflow_webhook_models-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_webhook_models-0.0.4.tar", last modified: Tue Jun  6 12:39:14 2023, max compression
+gzip compressed data, was "huntflow_webhook_models-0.0.5.tar", last modified: Wed Jun  7 07:34:31 2023, max compression
```

## Comparing `huntflow_webhook_models-0.0.4.tar` & `huntflow_webhook_models-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/LICENSE
--rw-r--r--   0        0        0       69 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/README.md
--rw-r--r--   0        0        0      122 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/__init__.py
--rw-r--r--   0        0        0      666 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/applicant.py
--rw-r--r--   0        0        0     1331 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/base.py
--rw-r--r--   0        0        0        0 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/__init__.py
--rw-r--r--   0        0        0     6585 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/applicant.py
--rw-r--r--   0        0        0     5459 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/calendar_event.py
--rw-r--r--   0        0        0      669 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/hf_base.py
--rw-r--r--   0        0        0     2950 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/survey_questionary.py
--rw-r--r--   0        0        0     3261 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/vacancy.py
--rw-r--r--   0        0        0     1638 2023-06-06 12:38:59.351184 huntflow_webhook_models-0.0.4/huntflow_webhook_models/consts.py
--rw-r--r--   0        0        0     1403 2023-06-06 12:39:14.467260 huntflow_webhook_models-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/README.md
+-rw-r--r--   0        0        0      122 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/applicant.py
+-rw-r--r--   0        0        0     1331 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/base.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/__init__.py
+-rw-r--r--   0        0        0     6585 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/applicant.py
+-rw-r--r--   0        0        0     5459 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/calendar_event.py
+-rw-r--r--   0        0        0      669 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/hf_base.py
+-rw-r--r--   0        0        0     2950 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/survey_questionary.py
+-rw-r--r--   0        0        0     3252 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/vacancy.py
+-rw-r--r--   0        0        0     1638 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/consts.py
+-rw-r--r--   0        0        0     1403 2023-06-07 07:34:31.064895 huntflow_webhook_models-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.5/PKG-INFO
```

### Comparing `huntflow_webhook_models-0.0.4/LICENSE` & `huntflow_webhook_models-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/applicant.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/applicant.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/base.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/applicant.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/applicant.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/calendar_event.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/calendar_event.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/hf_base.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/hf_base.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/survey_questionary.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/survey_questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/common_models/vacancy.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/vacancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     )
     company: Optional[str] = Field(None, description="Vacancy company", example="Huntflow")
     conditions: Optional[str] = Field(
         None,
         description="Vacancy conditions(HTML)",
         example="<p>Big salary</p>",
     )
-    created: datetime = Field(
+    created: date = Field(
         ...,
-        description="Date time the vacancy was created",
+        description="Date the vacancy was created",
         example=datetime(1970, 1, 1, 1, 1, 1),
     )
     deadline: Optional[date] = Field(..., description="Vacancy deadline", example=date(1970, 1, 1))
     fill_quotas: List[FillQuota] = Field([], description="Vacancy fill quota")
     frame_id: int = Field(..., description="Vacancy frame ID", example=1)
     hidden: bool = Field(..., description="Hidden vacnacy flag", example=True)
     money: Optional[str] = Field(None, description="Salary for vacacny", example="100000")
```

### Comparing `huntflow_webhook_models-0.0.4/huntflow_webhook_models/consts.py` & `huntflow_webhook_models-0.0.5/huntflow_webhook_models/consts.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.4/pyproject.toml` & `huntflow_webhook_models-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-webhook-models"
-version = "0.0.4"
+version = "0.0.5"
 description = "Huntflow webhooks requests data models"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "pydantic>=1.7.2",
     "openapi-schema-pydantic>=1.2.4",
```

### Comparing `huntflow_webhook_models-0.0.4/PKG-INFO` & `huntflow_webhook_models-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-webhook-models
-Version: 0.0.4
+Version: 0.0.5
 Summary: Huntflow webhooks requests data models
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

