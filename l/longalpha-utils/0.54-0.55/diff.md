# Comparing `tmp/longalpha_utils-0.54.tar.gz` & `tmp/longalpha_utils-0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.54.tar", last modified: Thu May 25 02:35:43 2023, max compression
+gzip compressed data, was "longalpha_utils-0.55.tar", last modified: Wed Jun  7 01:54:42 2023, max compression
```

## Comparing `longalpha_utils-0.54.tar` & `longalpha_utils-0.55.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:35:43.592790 longalpha_utils-0.54/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 02:35:43.592790 longalpha_utils-0.54/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:35:43.592790 longalpha_utils-0.54/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-25 02:35:30.000000 longalpha_utils-0.54/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:35:43.592790 longalpha_utils-0.54/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 02:35:43.000000 longalpha_utils-0.54/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 02:35:43.592790 longalpha_utils-0.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 02:35:30.000000 longalpha_utils-0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:54:42.054169 longalpha_utils-0.55/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 01:54:42.054169 longalpha_utils-0.55/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:54:42.054169 longalpha_utils-0.55/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:54:42.054169 longalpha_utils-0.55/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 01:54:42.054169 longalpha_utils-0.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 01:54:31.000000 longalpha_utils-0.55/setup.py
```

### Comparing `longalpha_utils-0.54/longalpha_utils/messenger.py` & `longalpha_utils-0.55/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.54/longalpha_utils/transfers.py` & `longalpha_utils-0.55/longalpha_utils/transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     ]
     # default spark conf
     spark_conf = (
         SparkConf()
         .set("spark.executor.memory", spark_executor_memory)
         .set("spark.driver.memory", spark_driver_memory)
         .set("spark.sql.execution.arrow.pyspark.enabled", "true")
-        .set("spark.ui.port", "4043")
         .set(
             "spark.jars.packages", ",".join(jars)
         )  # if you set park.jars.packages more than once, only the last one will be used.
         .set("spark.hadoop.fs.s3a.impl", "org.apache.hadoop.fs.s3a.S3AFileSystem")
         .set("spark.hadoop.fs.s3a.path.style.access", "true")
     )
     builder =SparkSession.builder.config(conf=spark_conf)
@@ -118,59 +117,78 @@
             object_name: object name in the minio bucket
 
         Returns:
 
         """
         self.minio_client.fput_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
-    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, index=False) -> None:
+    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, index=False, to_pickle=False) -> None:
         """
         put a pandas frame to parquet in s3
 
         Args:
             dataframe: a pandas dataframe
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
             index: whether to save the index of the dataframe, only used for parquet
+            to_pickle: whether to save the dataframe as pickle
 
 
         Returns:
 
         """
         with tempfile.TemporaryDirectory() as temp_dir:
-            path = os.path.join(temp_dir, "file.parquet")
-            dataframe.to_parquet(path, index=index)
+            if to_pickle:
+                path = os.path.join(temp_dir, "file.pkl")
+                dataframe.to_pickle(path)
+            else:
+                path = os.path.join(temp_dir, "file.parquet")
+                dataframe.to_parquet(path, index=index)
 
             self.fput(file_path=path, bucket_name=bucket_name, object_name=object_name)
 
     def fget(self, file_path: str, bucket_name: str, object_name: str):
         self.minio_client.fget_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
     def get(
         self,
         bucket_name: str,
         object_name: str,
+        from_pickle: bool = False,
     ) -> pd.DataFrame:
         """
         get a parquet from s3 and read it into pandas dataframe
         Args:
             bucket_name: Minio bucket_name
             object_name: path + file_name
+            from_pickle: whether to read the file from pickle
 
         Returns: A pandas dataframe
 
         """
-        file = self.minio_client.get_object(
-            bucket_name,
-            object_name,
-        )
-        res = pd.read_parquet(BytesIO(file.data))
-        file.close()
-        file.release_conn()
-        return res
+        # file = self.minio_client.get_object(
+        #     bucket_name,
+        #     object_name,
+        # )
+        # if to_pickle:
+        #     res = pd.read_pickle(BytesIO(file.data))
+        # else:
+        #     res = pd.read_parquet(BytesIO(file.data))
+        # file.close()
+        # file.release_conn()
+        # return res
+        with tempfile.TemporaryDirectory() as temp_dir:
+            if from_pickle:
+                path = os.path.join(temp_dir, "file.pkl")
+                self.fget(file_path=path, bucket_name=bucket_name, object_name=object_name)
+                return pd.read_pickle(path)
+            else:
+                path = os.path.join(temp_dir, "file.parquet")
+                self.fget(file_path=path, bucket_name=bucket_name, object_name=object_name)
+                return pd.read_parquet(path)
 
     def get_latest(self, bucket_name: str) -> pd.DataFrame:
         """
         get the latest parquet file and read it into pandas. Note that this does not include files in the
         sub-folders of the bucket. To do this, we need to recursively list all the files in the bucket.
         Args:
             bucket_name: bucket_name: Minio bucket_name
```

### Comparing `longalpha_utils-0.54/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.55/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.54/longalpha_utils/utils.py` & `longalpha_utils-0.55/longalpha_utils/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 
     Returns: s3 path
 
     """
     if day:
         return f"s3a://" + os.path.join(bucket, prefix, day.strftime("%Y"), day.strftime("%m"), day.strftime("%d"))
     else:
-        return f"s3a://" + os.path.join(bucket, prefix)
+        return f"s3a://" + os.path.join(bucket, prefix)
```

### Comparing `longalpha_utils-0.54/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.55/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.54/setup.py` & `longalpha_utils-0.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.54",
+    version="0.55",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

