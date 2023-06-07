# Comparing `tmp/mlplatformutils-0.9.0.3.tar.gz` & `tmp/mlplatformutils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.0.3.tar", last modified: Tue Jun  6 23:24:57 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.1.tar", last modified: Wed Jun  7 03:19:40 2023, max compression
```

## Comparing `mlplatformutils-0.9.0.3.tar` & `mlplatformutils-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 23:24:57.460150 mlplatformutils-0.9.0.3/
--rw-rw-rw-   0        0        0     3410 2023-06-06 23:24:57.461140 mlplatformutils-0.9.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.0.3/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-06 23:24:57.470141 mlplatformutils-0.9.0.3/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-06-06 23:24:30.000000 mlplatformutils-0.9.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:24:57.383392 mlplatformutils-0.9.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 23:24:57.394389 mlplatformutils-0.9.0.3/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:24:57.458139 mlplatformutils-0.9.0.3/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-06 20:44:51.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6106 2023-06-06 23:24:21.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-06 23:24:25.000000 mlplatformutils-0.9.0.3/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:24:57.428619 mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3410 2023-06-06 23:24:57.000000 mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-06 23:24:57.000000 mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 23:24:57.000000 mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-06 23:24:57.000000 mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 23:24:57.000000 mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 03:19:40.662640 mlplatformutils-0.9.1/
+-rw-rw-rw-   0        0        0     3468 2023-06-07 03:19:40.662640 mlplatformutils-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.1/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-07 03:19:40.665640 mlplatformutils-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-06-07 03:17:29.000000 mlplatformutils-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:19:40.510421 mlplatformutils-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 03:19:40.536033 mlplatformutils-0.9.1/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.1/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:19:40.660647 mlplatformutils-0.9.1/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     9559 2023-06-07 03:19:29.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-06 22:09:17.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-07 03:17:18.000000 mlplatformutils-0.9.1/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:19:40.574211 mlplatformutils-0.9.1/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3468 2023-06-07 03:19:40.000000 mlplatformutils-0.9.1/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-07 03:19:40.000000 mlplatformutils-0.9.1/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:19:40.000000 mlplatformutils-0.9.1/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-07 03:19:40.000000 mlplatformutils-0.9.1/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 03:19:40.000000 mlplatformutils-0.9.1/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.0.3/PKG-INFO` & `mlplatformutils-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.0.3
+Version: 0.9.1
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -83,16 +83,17 @@
 * write_to_adls_gen2
 * read_from_kusto
 * read_from_azsql
 
 **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
-* read_from_adlsgen2_parquet_as_pandas
-* write_pandas_as_parquet_to_adlsgen2
+* read_parquet_file_from_adlsgen2_as_pandas
+* read_parquet_directory_from_adlsgen2_as_pandas
+* write_pandas_as_parquet_file_to_adlsgen2
 
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
 **print(is_package_installed("pandas"))** <br />
```

### Comparing `mlplatformutils-0.9.0.3/setup.py` & `mlplatformutils-0.9.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.0.3',
+    version='0.9.1',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     keywords='mlplatformutils',
     install_requires=[
-          'applicationinsights','gremlinpython','azureml-core','azure-identity'
+          'applicationinsights','gremlinpython','azureml-core','azure-identity','azure-storage-file-datalake'
       ],
 
 )
```

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.1/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.1/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.1/src/mlplatformutils/core/pandasutils.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("delta"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
     return pandas_df
 
-def read_from_adlsgen2_parquet_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
+def read_parquet_file_from_adlsgen2_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
                                 RUN_ID,\
                                 PIPELINE_STEP_NAME,\
                                 LineageLogger):
-    
+    #AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH "<your_container>/<directory>/<file_name>.parquet"
     from azure.identity import ClientSecretCredential
     import pyarrow.fs
     import pyarrowfs_adlgen2
     import pandas as pd
     import pyarrow.parquet as pq
 
     credential = ClientSecretCredential(
@@ -70,16 +70,78 @@
     sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
 
     return pandas_df
 
+def list_directory_contents(storage_account_name,\
+                            tenant_id,client_id,\
+                            client_secret,\
+                            directory_path):
+    from azure.storage.filedatalake import DataLakeServiceClient
+    from azure.identity import ClientSecretCredential
+    try:
+        container = directory_path.split("/")[0]
+        directory_path ="/".join(directory_path.split("/")[1:])
+        credential = ClientSecretCredential(tenant_id=tenant_id,
+                                            client_id=client_id,
+                                            client_secret=client_secret)
+        
+        service_client = DataLakeServiceClient(account_url="{}://{}.dfs.core.windows.net".format("https", storage_account_name),\
+                                               credential=credential)
+        file_system_client = service_client.get_file_system_client(file_system=container)
+
+        paths = file_system_client.get_paths(path=directory_path)
+        filenames=[]
+        for path in paths:
+            if (path.name).endswith(".parquet"):
+                filenames.append(container+"/"+path.name)
+        return filenames
+    except Exception as e:
+     print(e)
+
+def read_parquet_directory_from_adlsgen2_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
+                                SOURCE_READ_SPN_VALUE,\
+                                SOURCE_READ_SPNKEY_VALUE,\
+                                tenant_id,\
+                                AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
+                                RUN_ID,\
+                                PIPELINE_STEP_NAME,\
+                                LineageLogger):
+    #AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH "<your_container>/<directory>"
+    parquet_files_from_path_list = list_directory_contents(SOURCE_STORAGE_ACCOUNT_VALUE,\
+                                                 tenant_id,\
+                                                 SOURCE_READ_SPN_VALUE,\
+                                                 SOURCE_READ_SPNKEY_VALUE,\
+                                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH)
+
+    from azure.identity import ClientSecretCredential
+    import pyarrow.fs
+    import pyarrowfs_adlgen2
+    import pandas as pd
+    import pyarrow.parquet as pq
+
+    credential = ClientSecretCredential(
+    tenant_id=tenant_id,
+    client_id=SOURCE_READ_SPN_VALUE,
+    client_secret=SOURCE_READ_SPNKEY_VALUE)
+
+    handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
+    fs = pyarrow.fs.PyFileSystem(handler)
+    pandas_df = pq.ParquetDataset(parquet_files_from_path_list,filesystem=fs).read().to_pandas()
+
+    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns",LineageLogger)
+    LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
+                                             "FileFormat_"+sourcePostfix:str("parquet"),\
+                                             "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+    return pandas_df
 
-def write_pandas_as_parquet_to_adlsgen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
+def write_pandas_as_parquet_file_to_adlsgen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
                                 pandas_df,\
                                 RUN_ID,\
                                 PIPELINE_STEP_NAME,\
```

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.1/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.1/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.1/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.0.3
+Version: 0.9.1
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -83,16 +83,17 @@
 * write_to_adls_gen2
 * read_from_kusto
 * read_from_azsql
 
 **pandasutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark while ensuring integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
-* read_from_adlsgen2_parquet_as_pandas
-* write_pandas_as_parquet_to_adlsgen2
+* read_parquet_file_from_adlsgen2_as_pandas
+* read_parquet_directory_from_adlsgen2_as_pandas
+* write_pandas_as_parquet_file_to_adlsgen2
 
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
 **print(is_package_installed("pandas"))** <br />
```

### Comparing `mlplatformutils-0.9.0.3/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.1/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

