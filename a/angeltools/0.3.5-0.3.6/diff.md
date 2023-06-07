# Comparing `tmp/angeltools-0.3.5.tar.gz` & `tmp/angeltools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angeltools-0.3.5.tar", last modified: Wed May 24 08:47:25 2023, max compression
+gzip compressed data, was "angeltools-0.3.6.tar", last modified: Wed Jun  7 09:15:05 2023, max compression
```

## Comparing `angeltools-0.3.5.tar` & `angeltools-0.3.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-24 08:47:25.962235 angeltools-0.3.5/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.3.5/LICENSE
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-24 08:47:25.962235 angeltools-0.3.5/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.3.5/README.md
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-24 08:47:25.958235 angeltools-0.3.5/angeltools/
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-24 08:47:25.958235 angeltools-0.3.5/angeltools/Db/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.3.5/angeltools/Db/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3297 2023-05-19 07:03:17.000000 angeltools-0.3.5/angeltools/Db/redis_connector.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.3.5/angeltools/ImageTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.3.5/angeltools/MathTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.3.5/angeltools/Slavers.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    18214 2023-05-24 08:46:21.000000 angeltools-0.3.5/angeltools/StrTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.3.5/angeltools/TimeTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.3.5/angeltools/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.3.5/angeltools/commands.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-24 08:47:25.958235 angeltools-0.3.5/angeltools/fdfs/
--rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.3.5/angeltools/fdfs/__init__.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-24 08:47:25.962235 angeltools-0.3.5/angeltools/fdfs/fdfs_client/
--rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/connection.py
--rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/exceptions.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/fdfs_protol.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/fdfs_test.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/storage_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/tracker_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_client/utils.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.3.5/angeltools/fdfs/fdfs_operator.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-24 08:47:25.958235 angeltools-0.3.5/angeltools.egg-info/
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-24 08:47:25.000000 angeltools-0.3.5/angeltools.egg-info/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-24 08:47:25.000000 angeltools-0.3.5/angeltools.egg-info/SOURCES.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-24 08:47:25.000000 angeltools-0.3.5/angeltools.egg-info/dependency_links.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-24 08:47:25.000000 angeltools-0.3.5/angeltools.egg-info/entry_points.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.3.5/angeltools.egg-info/not-zip-safe
--rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-24 08:47:25.000000 angeltools-0.3.5/angeltools.egg-info/requires.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-24 08:47:25.000000 angeltools-0.3.5/angeltools.egg-info/top_level.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-24 08:47:25.962235 angeltools-0.3.5/setup.cfg
--rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-24 08:47:19.000000 angeltools-0.3.5/setup.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-06-07 09:15:05.943639 angeltools-0.3.6/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.3.6/LICENSE
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-06-07 09:15:05.943639 angeltools-0.3.6/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.3.6/README.md
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-06-07 09:15:05.939639 angeltools-0.3.6/angeltools/
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-06-07 09:15:05.943639 angeltools-0.3.6/angeltools/Db/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.3.6/angeltools/Db/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3297 2023-05-19 07:03:17.000000 angeltools-0.3.6/angeltools/Db/redis_connector.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.3.6/angeltools/ImageTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.3.6/angeltools/MathTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.3.6/angeltools/Slavers.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    18242 2023-06-07 09:08:21.000000 angeltools-0.3.6/angeltools/StrTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.3.6/angeltools/TimeTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.3.6/angeltools/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.3.6/angeltools/commands.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-06-07 09:15:05.943639 angeltools-0.3.6/angeltools/fdfs/
+-rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.3.6/angeltools/fdfs/__init__.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-06-07 09:15:05.943639 angeltools-0.3.6/angeltools/fdfs/fdfs_client/
+-rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/connection.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/exceptions.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/fdfs_protol.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/fdfs_test.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/storage_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/tracker_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_client/utils.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.3.6/angeltools/fdfs/fdfs_operator.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-06-07 09:15:05.943639 angeltools-0.3.6/angeltools.egg-info/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-06-07 09:15:05.000000 angeltools-0.3.6/angeltools.egg-info/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-06-07 09:15:05.000000 angeltools-0.3.6/angeltools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-06-07 09:15:05.000000 angeltools-0.3.6/angeltools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-06-07 09:15:05.000000 angeltools-0.3.6/angeltools.egg-info/entry_points.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.3.6/angeltools.egg-info/not-zip-safe
+-rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-06-07 09:15:05.000000 angeltools-0.3.6/angeltools.egg-info/requires.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-06-07 09:15:05.000000 angeltools-0.3.6/angeltools.egg-info/top_level.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-06-07 09:15:05.943639 angeltools-0.3.6/setup.cfg
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-06-07 09:14:42.000000 angeltools-0.3.6/setup.py
```

### Comparing `angeltools-0.3.5/LICENSE` & `angeltools-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/PKG-INFO` & `angeltools-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.3.5
+Version: 0.3.6
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.3.5/README.md` & `angeltools-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/Db/__init__.py` & `angeltools-0.3.6/angeltools/Db/__init__.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/Db/redis_connector.py` & `angeltools-0.3.6/angeltools/Db/redis_connector.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/ImageTool.py` & `angeltools-0.3.6/angeltools/ImageTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/MathTool.py` & `angeltools-0.3.6/angeltools/MathTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/Slavers.py` & `angeltools-0.3.6/angeltools/Slavers.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/StrTool.py` & `angeltools-0.3.6/angeltools/StrTool.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
                 if file.startswith(file_lock_prefix):
                     try:
                         os.remove(self.lock_dir / file)
                     except:
                         pass
 
     def __lock_dir(self):
-        if sys.platform == 'linux':
+        if sys.platform == 'linux' or sys.platform == 'darwin':
             self.lock_dir = Path(f'/tmp/')
         else:
             self.lock_dir = Path(__file__).parent / 'FileLock'
 
     def __get_lock_prefix(self):
         self.fp_prefix = self.lock_dir / file_lock_prefix
```

### Comparing `angeltools-0.3.5/angeltools/TimeTool.py` & `angeltools-0.3.6/angeltools/TimeTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/commands.py` & `angeltools-0.3.6/angeltools/commands.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/client.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/connection.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/connection.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/fdfs_protol.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/fdfs_protol.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/fdfs_test.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/fdfs_test.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/storage_client.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/storage_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/tracker_client.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/tracker_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_client/utils.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_client/utils.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools/fdfs/fdfs_operator.py` & `angeltools-0.3.6/angeltools/fdfs/fdfs_operator.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/angeltools.egg-info/PKG-INFO` & `angeltools-0.3.6/angeltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.3.5
+Version: 0.3.6
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.3.5/angeltools.egg-info/SOURCES.txt` & `angeltools-0.3.6/angeltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angeltools-0.3.5/setup.py` & `angeltools-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 using_setuptools = True
 
 setup_args = {
     "name": "angeltools",
-    "version": "0.3.5",
+    "version": "0.3.6",
     "url": "https://github.com/ga1008/angeltools",
     "description": "personal python small tools collection",
     "long_description": long_description,
     "author": "Guardian",
     "author_email": "zhling2012@live.com",
     "maintainer": "Guardian",
     "maintainer_email": "zhling2012@live.com",
```

