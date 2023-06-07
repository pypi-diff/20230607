# Comparing `tmp/idbadapter-1.4.tar.gz` & `tmp/idbadapter-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.4.tar", last modified: Mon May 29 08:37:34 2023, max compression
+gzip compressed data, was "idbadapter-1.5.tar", last modified: Wed Jun  7 15:10:51 2023, max compression
```

## Comparing `idbadapter-1.4.tar` & `idbadapter-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 08:37:34.591438 idbadapter-1.4/
--rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.4/LICENSE
--rw-rw-rw-   0        0        0      695 2023-05-29 08:37:34.592438 idbadapter-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 08:37:34.574439 idbadapter-1.4/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.4/idbadapter/__init__.py
--rw-rw-rw-   0        0        0     7838 2023-05-29 08:29:56.000000 idbadapter-1.4/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-29 08:37:34.591438 idbadapter-1.4/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 08:37:34.593438 idbadapter-1.4/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-05-29 08:37:15.000000 idbadapter-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:10:51.049651 idbadapter-1.5/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.5/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-06-07 15:10:51.049651 idbadapter-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 15:10:51.025650 idbadapter-1.5/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.5/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0     7801 2023-06-07 14:57:59.000000 idbadapter-1.5/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:10:51.047680 idbadapter-1.5/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 15:10:50.000000 idbadapter-1.5/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 15:10:51.051647 idbadapter-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-07 15:08:05.000000 idbadapter-1.5/setup.py
```

### Comparing `idbadapter-1.4/LICENSE` & `idbadapter-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.4/PKG-INFO` & `idbadapter-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.4
+Version: 1.5
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.4/idbadapter/schedule_loader.py` & `idbadapter-1.5/idbadapter/schedule_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,9 +190,9 @@
 
         df = self.convert_df(df)
 
         return df
 
     @staticmethod
     def convert_df(df: pd.DataFrame):
-        result = df.pivot_table("fraction", ["is_work", "basic_name", "name", "object_id", "object_name", "full_fraction", ], "date")
+        result = df.pivot_table("fraction", set(df.columns) - set(["fraction", "date"]), "date")
         return result.reset_index()
```

### Comparing `idbadapter-1.4/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.5/idbadapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.4
+Version: 1.5
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.4/setup.py` & `idbadapter-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 
 version = '1.3'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.4',
+      version='1.5',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

