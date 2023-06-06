# Comparing `tmp/mlplatformutils-0.9.0.1.tar.gz` & `tmp/mlplatformutils-0.9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.0.1.tar", last modified: Tue Jun  6 22:52:45 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.0.2.tar", last modified: Tue Jun  6 23:08:36 2023, max compression
```

## Comparing `mlplatformutils-0.9.0.1.tar` & `mlplatformutils-0.9.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:52:45.637331 mlplatformutils-0.9.0.1/
--rw-rw-rw-   0        0        0     3410 2023-06-06 22:52:45.638330 mlplatformutils-0.9.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.0.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-06 22:52:45.648330 mlplatformutils-0.9.0.1/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-06-06 22:52:31.000000 mlplatformutils-0.9.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:52:45.570809 mlplatformutils-0.9.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 22:52:45.582806 mlplatformutils-0.9.0.1/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:52:45.635338 mlplatformutils-0.9.0.1/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-06 20:44:51.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     5970 2023-06-06 22:45:20.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-06 22:52:19.000000 mlplatformutils-0.9.0.1/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:52:45.611812 mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3410 2023-06-06 22:52:45.000000 mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-06 22:52:45.000000 mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:52:45.000000 mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-06 22:52:45.000000 mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 22:52:45.000000 mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 23:08:36.589771 mlplatformutils-0.9.0.2/
+-rw-rw-rw-   0        0        0     3410 2023-06-06 23:08:36.589771 mlplatformutils-0.9.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.0.2/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-06 23:08:36.591776 mlplatformutils-0.9.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      780 2023-06-06 23:07:53.000000 mlplatformutils-0.9.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:08:36.430198 mlplatformutils-0.9.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 23:08:36.457194 mlplatformutils-0.9.0.2/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:08:36.587817 mlplatformutils-0.9.0.2/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-06 20:44:51.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     5996 2023-06-06 23:08:33.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-06 23:07:46.000000 mlplatformutils-0.9.0.2/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:08:36.493195 mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3410 2023-06-06 23:08:36.000000 mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-06 23:08:36.000000 mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 23:08:36.000000 mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-06 23:08:36.000000 mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 23:08:36.000000 mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.0.1/PKG-INFO` & `mlplatformutils-0.9.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.0.1
+Version: 0.9.0.2
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.0.1/setup.py` & `mlplatformutils-0.9.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.0.1',
+    version='0.9.0.2',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.0.2/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.0.2/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.0.2/src/mlplatformutils/core/pandasutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     tenant_id=tenant_id,
     client_id=SOURCE_READ_SPN_VALUE,
     client_secret=SOURCE_READ_SPNKEY_VALUE)
     
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     #pandas_df = pd.read_parquet(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs , engine="pyarrow")
-    pandas_df = pq.read_table(source=AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs).to_pandas()
+    pandas_df = pq.read_table(source=AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs, use_legacy_dataset= True).to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
```

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.0.2/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.0.2/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.0.1
+Version: 0.9.0.2
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.0.1/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.0.2/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

