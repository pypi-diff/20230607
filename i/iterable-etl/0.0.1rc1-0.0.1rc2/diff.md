# Comparing `tmp/iterable_etl-0.0.1rc1.tar.gz` & `tmp/iterable_etl-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.0.1rc1.tar", last modified: Wed Jun  7 18:54:12 2023, max compression
+gzip compressed data, was "iterable_etl-0.0.1rc2.tar", last modified: Wed Jun  7 19:28:42 2023, max compression
```

## Comparing `iterable_etl-0.0.1rc1.tar` & `iterable_etl-0.0.1rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.0.1rc1/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1287 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      776 2023-06-07 17:53:35.000000 iterable_etl-0.0.1rc1/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/iterable_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 iterable_etl-0.0.1rc1/iterable_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-07 15:07:58.000000 iterable_etl-0.0.1rc1/iterable_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      833 2023-06-07 17:20:53.000000 iterable_etl-0.0.1rc1/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/iterable_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.0.1rc1/iterable_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      516 2023-06-07 15:37:52.000000 iterable_etl-0.0.1rc1/iterable_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1433 2023-06-07 17:23:24.000000 iterable_etl-0.0.1rc1/iterable_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      343 2023-06-07 15:39:49.000000 iterable_etl-0.0.1rc1/iterable_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      634 2023-06-07 15:37:19.000000 iterable_etl-0.0.1rc1/iterable_etl/libs/spark.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      462 2023-06-07 15:37:30.000000 iterable_etl-0.0.1rc1/iterable_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/iterable_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.0.1rc1/iterable_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      778 2023-06-07 17:19:26.000000 iterable_etl-0.0.1rc1/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1254 2023-06-07 17:22:03.000000 iterable_etl-0.0.1rc1/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1613 2023-06-07 17:48:15.000000 iterable_etl-0.0.1rc1/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      704 2023-06-07 17:20:13.000000 iterable_etl-0.0.1rc1/iterable_etl/tables/list.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/iterable_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1287 2023-06-07 18:54:12.000000 iterable_etl-0.0.1rc1/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      666 2023-06-07 18:54:12.000000 iterable_etl-0.0.1rc1/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-07 18:54:12.000000 iterable_etl-0.0.1rc1/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       48 2023-06-07 18:54:12.000000 iterable_etl-0.0.1rc1/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-07 18:54:12.000000 iterable_etl-0.0.1rc1/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      957 2023-06-07 18:53:30.000000 iterable_etl-0.0.1rc1/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 18:54:12.909731 iterable_etl-0.0.1rc1/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.0.1rc1/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.0.1rc2/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1654 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1143 2023-06-07 19:27:23.000000 iterable_etl-0.0.1rc2/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 iterable_etl-0.0.1rc2/iterable_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-07 15:07:58.000000 iterable_etl-0.0.1rc2/iterable_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      833 2023-06-07 17:20:53.000000 iterable_etl-0.0.1rc2/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      516 2023-06-07 15:37:52.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      524 2023-06-07 19:21:02.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      636 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/spark.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      463 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      779 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1310 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1615 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      705 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/list.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1654 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      666 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       48 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      957 2023-06-07 19:27:52.000000 iterable_etl-0.0.1rc2/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.0.1rc2/tests/__init__.py
```

### Comparing `iterable_etl-0.0.1rc1/PKG-INFO` & `iterable_etl-0.0.1rc2/iterable_etl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iterable_etl
-Version: 0.0.1rc1
+Name: iterable-etl
+Version: 0.0.1rc2
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,22 +14,36 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # `iterable_etl`
 
 > Replicate data from iterable in databricks
 
-## Usage
+### CLI
 
 ```bash
 python -m iterable_etl --table <table-name>
 ```
 
 where <table-name> is one of the following: `campaign_history`, `campaign_metrics`, `campaign_list_history`, `list`, or `ALL`.
 
+### API
+
+```python
+from iterable_etl.tables.campaign_history import campaign_history_df
+from iterable_etl.tables.campaign_metrics import campaign_metrics_df
+from iterable_etl.tables.list import list_df
+from iterable_etl.tables.campaign_list_history import campaign_list_history_df
+
+campaign_history_df()
+campaign_metrics_df()
+list_df()
+campaign_list_history_df()
+```
+
 Further configs are set via environment variables:
 
 - `ITERABLE_KEY`: API access
 - `APP_ENV`: <development/production> - debug mode
 - `SAMPLE_OUTPUT`: <True/False> - Save dataframes to csv
 
 ## DEV
```

### Comparing `iterable_etl-0.0.1rc1/README_PUBLIC.md` & `iterable_etl-0.0.1rc2/README_PUBLIC.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 # `iterable_etl`
 
 > Replicate data from iterable in databricks
 
-## Usage
+### CLI
 
 ```bash
 python -m iterable_etl --table <table-name>
 ```
 
 where <table-name> is one of the following: `campaign_history`, `campaign_metrics`, `campaign_list_history`, `list`, or `ALL`.
 
+### API
+
+```python
+from iterable_etl.tables.campaign_history import campaign_history_df
+from iterable_etl.tables.campaign_metrics import campaign_metrics_df
+from iterable_etl.tables.list import list_df
+from iterable_etl.tables.campaign_list_history import campaign_list_history_df
+
+campaign_history_df()
+campaign_metrics_df()
+list_df()
+campaign_list_history_df()
+```
+
 Further configs are set via environment variables:
 
 - `ITERABLE_KEY`: API access
 - `APP_ENV`: <development/production> - debug mode
 - `SAMPLE_OUTPUT`: <True/False> - Save dataframes to csv
 
 ## DEV
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/iterable_etl.py` & `iterable_etl-0.0.1rc2/iterable_etl/iterable_etl.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/libs/cnst.py` & `iterable_etl-0.0.1rc2/iterable_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/libs/dbg.py` & `iterable_etl-0.0.1rc2/iterable_etl/libs/dbg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 """dbg"""
 
 import os
 from typing import Any, Callable, TypeVar
 
+from loguru import logger
 import pandas as pd
 
-T = TypeVar('T')
+T = TypeVar("T")
+
+
+def dbg(__message: str, *args: Any, **kwargs: Any) -> None:
+    """dbg"""
+    if os.environ.get("APP_ENV") == "development":
+        logger.debug(__message, *args, **kwargs)
+
 
 def print_dataframe_head(func: Callable[..., T]) -> Callable[..., T]:
     def wrapper(*args: Any, **kwargs: Any) -> T:
         result = func(*args, **kwargs)
         if os.environ.get("APP_ENV") == "development":
             if isinstance(result, pd.DataFrame):
-                print(func.__name__)
-                print(result.head(10))
-                print("")
+                dbg(func.__name__)
+                dbg(result.head(10))
+                dbg("")
             else:
-                print("Returned object is not a DataFrame.")
+                dbg("Returned object is not a DataFrame.")
         return result
+
     return wrapper
 
-def write_dataframe_to_csv(file_name:str):
+
+def write_dataframe_to_csv(file_name: str):
     def _write_dataframe_to_csv(func: Callable[..., T]) -> Callable[..., T]:
         def wrapper(*args: Any, **kwargs: Any) -> T:
             result = func(*args, **kwargs)
             if os.environ.get("SAMPLE_OUTPUT") == "True":
                 if isinstance(result, pd.DataFrame):
                     directory = "sample_output"
                     os.makedirs(directory, exist_ok=True)
                     csv_filename = f"{file_name}.csv"
                     csv_path = os.path.join(directory, csv_filename)
                     result.to_csv(csv_path, index=False)
-                    print(f"DataFrame saved to: {csv_path}")
+                    dbg(f"DataFrame saved to: {csv_path}")
                 else:
-                    print("Returned object is not a DataFrame.")
+                    dbg("Returned object is not a DataFrame.")
             return result
+
         return wrapper
+
     return _write_dataframe_to_csv
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/libs/spark.py` & `iterable_etl-0.0.1rc2/iterable_etl/libs/spark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """spark"""
 
 from pandas import DataFrame as PandasDF
 from pyspark.sql import DataFrame as SparkDF
 from pyspark.sql import SparkSession
 
 
-def dataframe_to_spark(df: PandasDF, spark:SparkSession) -> SparkDF:
+def dataframe_to_spark(df: PandasDF, spark: SparkSession) -> SparkDF:
     """
     Convert the Pandas DataFrame to a Spark DataFrame.
 
     from pyspark.sql import SparkSession
     spark = SparkSession.builder.getOrCreate()
     """
     spark_df = spark.createDataFrame(df)
     return spark_df
 
+
 def write_to_databricks_table(spark_df: SparkDF, table_name: str) -> None:
     """
     Write the Spark DataFrame to a Databricks table.
     """
     spark_df.write.mode("overwrite").saveAsTable(table_name)
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_history.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 def get_campaign_data(api_url: str, headers: Dict[str, str]) -> Dict[str, Any]:
     """Make a GET request to the Iterable API and return a dictionary of campaigns data."""
     data = get_data(api_url, headers)
     return data["campaigns"]
 
+
 @write_dataframe_to_csv("campaign_history")
 @print_dataframe_head
 def campaign_history_df():
     """campaign_history_dataframe"""
     data = get_campaign_data(urls["campaigns"], get_headers())
     df = json_to_dataframe(data)
     return df
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_list_history.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 from typing import Dict, Any, List
 import pandas as pd
 
 from iterable_etl.libs.network import get_data
 from iterable_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from iterable_etl.libs.cnst import urls, get_headers
 
+
 def get_campaign_data(api_url: str, headers: Dict[str, str]) -> List[Dict[str, Any]]:
     """Make a GET request to the Iterable API and return a dictionary of campaigns data."""
     data = get_data(api_url, headers)
     return data["campaigns"]
 
 
 def explode_list_ids(data: List[Dict[str, Any]]) -> pd.DataFrame:
     """flatten listIds and associate with campaignId"""
     df_data = []
     for campaign in data:
         if "listIds" in campaign:
             for list_id in campaign["listIds"]:
-                df_data.append({
-                    "campaignId": campaign["id"],
-                    "listId": list_id,
-                    "updatedAt": campaign["updatedAt"],
-                })
+                df_data.append(
+                    {
+                        "campaignId": campaign["id"],
+                        "listId": list_id,
+                        "updatedAt": campaign["updatedAt"],
+                    }
+                )
 
     df = pd.DataFrame(df_data)
 
     return df
 
+
 @write_dataframe_to_csv("campaign_list_history")
 @print_dataframe_head
 def campaign_list_history_df():
     """campaign_history_dataframe"""
     data = get_campaign_data(urls["campaigns"], get_headers())
     df = explode_list_ids(data)
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,23 @@
 
 def get_metrics_data(api_url: str, headers: Dict[str, str], campaign_id: int) -> bytes:
     """Make a GET request to the Iterable API and return the response content."""
     response = requests.get(api_url.format(campaign_id), headers=headers, timeout=10)
     response.raise_for_status()
     return response.content
 
+
 @write_dataframe_to_csv("campaign_metrics")
 @print_dataframe_head
 def campaign_metrics_df():
     """campaign_metrics dataframe"""
     campaign_ids = get_campaign_ids(urls["campaigns"], get_headers())
     df_list = []
     for i, campaign_id in enumerate(campaign_ids):
         data = get_metrics_data(urls["metrics"], get_headers(), campaign_id)
         df = csv_to_dataframe(data)
         df_list.append(df)
-        time.sleep(11) # suboptimal
+        time.sleep(11)  # suboptimal
         if i == 5 and os.environ.get("APP_ENV") == "development":
             break
     combined_df = pd.concat(df_list)
     return combined_df
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl/tables/list.py` & `iterable_etl-0.0.1rc2/iterable_etl/tables/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 def get_list_data(api_url: str, headers: Dict[str, str]) -> Dict[str, Any]:
     """Make a GET request to the Iterable API and return a dictionary of list data."""
     data = get_data(api_url, headers)
     return data["lists"]
 
+
 @write_dataframe_to_csv("list")
 @print_dataframe_head
 def list_df():
     """list dataframe"""
     data = get_list_data(urls["lists"], get_headers())
     df = json_to_dataframe(data)
     return df
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.0.1rc2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iterable-etl
-Version: 0.0.1rc1
+Name: iterable_etl
+Version: 0.0.1rc2
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,22 +14,36 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # `iterable_etl`
 
 > Replicate data from iterable in databricks
 
-## Usage
+### CLI
 
 ```bash
 python -m iterable_etl --table <table-name>
 ```
 
 where <table-name> is one of the following: `campaign_history`, `campaign_metrics`, `campaign_list_history`, `list`, or `ALL`.
 
+### API
+
+```python
+from iterable_etl.tables.campaign_history import campaign_history_df
+from iterable_etl.tables.campaign_metrics import campaign_metrics_df
+from iterable_etl.tables.list import list_df
+from iterable_etl.tables.campaign_list_history import campaign_list_history_df
+
+campaign_history_df()
+campaign_metrics_df()
+list_df()
+campaign_list_history_df()
+```
+
 Further configs are set via environment variables:
 
 - `ITERABLE_KEY`: API access
 - `APP_ENV`: <development/production> - debug mode
 - `SAMPLE_OUTPUT`: <True/False> - Save dataframes to csv
 
 ## DEV
```

### Comparing `iterable_etl-0.0.1rc1/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.0.1rc2/iterable_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc1/setup.py` & `iterable_etl-0.0.1rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.0.1rc1",
+    version="0.0.1rc2",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

