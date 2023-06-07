# Comparing `tmp/iosense_connect-3.0.0.tar.gz` & `tmp/iosense_connect-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-3.0.0.tar", last modified: Tue May 23 12:11:14 2023, max compression
+gzip compressed data, was "dist\iosense_connect-3.0.1.tar", last modified: Wed Jun  7 06:39:44 2023, max compression
```

## Comparing `iosense_connect-3.0.0.tar` & `iosense_connect-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 12:11:13.990509 iosense_connect-3.0.0/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-3.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-23 12:11:13.988193 iosense_connect-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:11:13.904440 iosense_connect-3.0.0/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-3.0.0/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    23854 2023-05-23 12:11:09.000000 iosense_connect-3.0.0/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:11:13.985191 iosense_connect-3.0.0/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-23 12:11:13.000000 iosense_connect-3.0.0/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-23 12:11:13.000000 iosense_connect-3.0.0/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 12:11:13.000000 iosense_connect-3.0.0/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 12:11:13.000000 iosense_connect-3.0.0/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 12:11:13.991319 iosense_connect-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-23 12:11:09.000000 iosense_connect-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:39:44.235623 iosense_connect-3.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-3.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-07 06:39:44.233624 iosense_connect-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:39:44.101382 iosense_connect-3.0.1/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-3.0.1/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    23915 2023-06-07 06:39:14.000000 iosense_connect-3.0.1/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:39:44.126379 iosense_connect-3.0.1/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-06-07 06:39:43.000000 iosense_connect-3.0.1/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-07 06:39:43.000000 iosense_connect-3.0.1/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:39:43.000000 iosense_connect-3.0.1/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-07 06:39:43.000000 iosense_connect-3.0.1/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 06:39:43.000000 iosense_connect-3.0.1/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:39:44.235623 iosense_connect-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-06-07 06:36:07.000000 iosense_connect-3.0.1/setup.py
```

### Comparing `iosense_connect-3.0.0/LICENSE.txt` & `iosense_connect-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-3.0.0/PKG-INFO` & `iosense_connect-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 3.0.0
+Version: 3.0.1
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-3.0.0/README.md` & `iosense_connect-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-3.0.0/iosense_connect/data_access.py` & `iosense_connect-3.0.1/iosense_connect/data_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,23 +484,25 @@
                         if sensors != None and len(sensors_filtered) != 0:
                             sensors_filtered.insert(0,'time')
                             df =  df[sensors_filtered]
                         if len(sensors_filtered) == 0:
                             df = pd.DataFrame()
                         df.sort_values(['time'], inplace=True)
                         df.reset_index(drop=True, inplace=True)
-                        last_date = df['time'].iloc[len(df) - 1]
-                        start_date = last_date.date() + timedelta(days=1)
-                        end_time = pd.to_datetime(end_time)
-                        if last_date.date() != end_time.date():
-                            df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
-                            df = pd.concat([df, df1])
-                            df.reset_index(drop=True, inplace=True)
-                        else:
-                            df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                        last_date = str(df['time'].iloc[-1])
+                        start_date = df['time'].iloc[-1].date() + timedelta(days=1)
+                        end_time = str(end_time)
+
+                        last_date = datetime.strptime(last_date, "%Y-%m-%d %H:%M:%S.%f")
+                        end_time = datetime.strptime(end_time, "%Y-%m-%d %H:%M:%S")
+
+                        if last_date.year != end_time.year and last_date.month != end_time.month and last_date.day != end_time.day and last_date.hour != end_time.hour:
+                            df1 = DataAccess.fetch_data(self, device_id, start_time=str(start_date), alias=False,
+                                                        end_time=end_time, sensors=sensors, echo=True,
+                                                        onpremise=onpremise, IST=IST)
                             df = pd.concat([df, df1])
                             df.reset_index(drop=True, inplace=True)
             else:
                 df_devices = DataAccess.get_device_details(self,onpremise=onpremise)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
                     df = DataAccess.fetch_data(self, device_id, start_time,end_time, alias,sensors=sensors,echo=True,onpremise=onpremise,IST=IST)
```

### Comparing `iosense_connect-3.0.0/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-3.0.1/iosense_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 3.0.0
+Version: 3.0.1
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-3.0.0/setup.py` & `iosense_connect-3.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "3.0.0",
+    version = "3.0.1",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
+    install_requires=[
+        'numpy',
+        'pandas',
+        'pyarrow',
+        'requests',
+        'azure-storage-blob',
+        'azure-core',
+        'pytz'
+    ],
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
```

