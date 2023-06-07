# Comparing `tmp/watchmen_inquiry_surface-16.5.6.tar.gz` & `tmp/watchmen_inquiry_surface-16.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_surface-16.5.6.tar", max compression
+gzip compressed data, was "watchmen_inquiry_surface-16.5.7.tar", max compression
```

## Comparing `watchmen_inquiry_surface-16.5.6.tar` & `watchmen_inquiry_surface-16.5.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/LICENSE
--rw-r--r--   0        0        0     1304 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/pyproject.toml
--rw-r--r--   0        0        0       46 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/src/watchmen_inquiry_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/src/watchmen_inquiry_surface/data/__init__.py
--rw-r--r--   0        0        0    12415 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/src/watchmen_inquiry_surface/data/data_router.py
--rw-r--r--   0        0        0      176 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/src/watchmen_inquiry_surface/main.py
--rw-r--r--   0        0        0      476 2023-06-06 17:50:48.791399 watchmen_inquiry_surface-16.5.6/src/watchmen_inquiry_surface/settings.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/LICENSE
+-rw-r--r--   0        0        0     1304 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/src/watchmen_inquiry_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/src/watchmen_inquiry_surface/data/__init__.py
+-rw-r--r--   0        0        0    12810 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/src/watchmen_inquiry_surface/data/data_router.py
+-rw-r--r--   0        0        0      176 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/src/watchmen_inquiry_surface/main.py
+-rw-r--r--   0        0        0      476 2023-06-07 11:34:15.619986 watchmen_inquiry_surface-16.5.7/src/watchmen_inquiry_surface/settings.py
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.7/PKG-INFO
```

### Comparing `watchmen_inquiry_surface-16.5.6/LICENSE` & `watchmen_inquiry_surface-16.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.5.6/pyproject.toml` & `watchmen_inquiry_surface-16.5.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-surface"
-version = "16.5.6"
+version = "16.5.7"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.6"
-watchmen-rest = "16.5.6"
-watchmen-inquiry-trino = { version = "16.5.6", optional = true }
-watchmen-storage-mysql = { version = "16.5.6", optional = true }
-watchmen-storage-oracle = { version = "16.5.6", optional = true }
-watchmen-storage-mongodb = { version = "16.5.6", optional = true }
-watchmen-storage-mssql = { version = "16.5.6", optional = true }
-watchmen-storage-postgresql = { version = "16.5.6", optional = true }
-watchmen-storage-oss = { version = "16.5.6", optional = true }
-watchmen-storage-s3 = { version = "16.5.6", optional = true }
+watchmen-inquiry-kernel = "16.5.7"
+watchmen-rest = "16.5.7"
+watchmen-inquiry-trino = { version = "16.5.7", optional = true }
+watchmen-storage-mysql = { version = "16.5.7", optional = true }
+watchmen-storage-oracle = { version = "16.5.7", optional = true }
+watchmen-storage-mongodb = { version = "16.5.7", optional = true }
+watchmen-storage-mssql = { version = "16.5.7", optional = true }
+watchmen-storage-postgresql = { version = "16.5.7", optional = true }
+watchmen-storage-oss = { version = "16.5.7", optional = true }
+watchmen-storage-s3 = { version = "16.5.7", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 trino = ["watchmen-inquiry-trino"]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_surface-16.5.6/src/watchmen_inquiry_surface/data/data_router.py` & `watchmen_inquiry_surface-16.5.7/src/watchmen_inquiry_surface/data/data_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,18 +157,18 @@
 	if subject is None:
 		raise_400(f'Subject not found by given criteria[id={subject_id}, name={subject_name}].')
 
 	subject_column_map: Dict[str, SubjectDatasetColumn] = ArrayHelper(subject.dataset.columns) \
 		.to_map(lambda x: x.columnId, lambda x: x)
 
 	def to_report_indicator(indicator: SubjectDatasetCriteriaIndicator) -> ReportIndicator:
-		columnId = indicator.columnId
-		dataset_column = subject_column_map.get(columnId)
+		column_id = indicator.columnId
+		dataset_column = subject_column_map.get(column_id)
 		if dataset_column is None:
-			raise_400(f'Cannot find column[columnId={columnId}] from subject.')
+			raise_400(f'Cannot find column[columnId={column_id}] from subject.')
 
 		arithmetic = ReportIndicatorArithmetic.NONE
 		if indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.COUNT:
 			arithmetic = ReportIndicatorArithmetic.COUNT
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.DISTINCT_COUNT:
 			arithmetic = ReportIndicatorArithmetic.DISTINCT_COUNT
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.SUMMARY:
@@ -286,8 +286,16 @@
 
 
 @router.post('/subject/data/criteria/sql', tags=[UserRole.ADMIN], response_model=str)
 async def query_dataset(
 		criteria: SubjectDatasetCriteria,
 		principal_service: PrincipalService = Depends(get_console_principal)) -> str:
 	subject, report, pageable = ask_subject_criteria(criteria, principal_service)
+	return get_report_data_service(subject, report, principal_service).find_sql()
+
+
+@router.post('/subject/data/criteria/page-sql', tags=[UserRole.ADMIN], response_model=str)
+async def query_dataset(
+		criteria: SubjectDatasetCriteria,
+		principal_service: PrincipalService = Depends(get_console_principal)) -> str:
+	subject, report, pageable = ask_subject_criteria(criteria, principal_service)
 	return get_report_data_service(subject, report, principal_service).page_sql(pageable)
```

### Comparing `watchmen_inquiry_surface-16.5.6/PKG-INFO` & `watchmen_inquiry_surface-16.5.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-surface
-Version: 16.5.6
+Version: 16.5.7
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.6)
-Requires-Dist: watchmen-inquiry-trino (==16.5.6) ; extra == "trino"
-Requires-Dist: watchmen-rest (==16.5.6)
-Requires-Dist: watchmen-storage-mongodb (==16.5.6) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.6) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.6) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.6) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.6) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.6) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.6) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.7)
+Requires-Dist: watchmen-inquiry-trino (==16.5.7) ; extra == "trino"
+Requires-Dist: watchmen-rest (==16.5.7)
+Requires-Dist: watchmen-storage-mongodb (==16.5.7) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.7) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.7) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.7) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.7) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.7) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.7) ; extra == "s3"
```

