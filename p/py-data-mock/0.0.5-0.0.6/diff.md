# Comparing `tmp/py-data-mock-0.0.5.tar.gz` & `tmp/py-data-mock-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.5.tar", last modified: Fri Jun  2 03:59:15 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.6.tar", last modified: Tue Jun  6 23:19:32 2023, max compression
```

## Comparing `py-data-mock-0.0.5.tar` & `py-data-mock-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/
--rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-20 20:50:55.000000 py-data-mock-0.0.5/LICENSE
--rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)     4391 2023-05-24 05:45:14.000000 py-data-mock-0.0.5/README.md
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/
--rw-rw-r--   0 henry     (1000) henry     (1000)       53 2023-05-26 05:01:26.000000 py-data-mock-0.0.5/data_mock/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       43 2023-05-23 07:44:51.000000 py-data-mock-0.0.5/data_mock/exceptions.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.925548 py-data-mock-0.0.5/data_mock/google/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/
--rw-rw-r--   0 henry     (1000) henry     (1000)      827 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     6323 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/client.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      301 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/dataset.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1427 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/enums.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       85 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/exceptions.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/
--rw-rw-r--   0 henry     (1000) henry     (1000)      329 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      350 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/load.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       80 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/job/query.py
--rw-rw-r--   0 henry     (1000) henry     (1000)       22 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/retry.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      865 2023-05-26 05:01:26.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/schema.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     3013 2023-05-26 04:55:53.000000 py-data-mock-0.0.5/data_mock/google/cloud/bigquery/table.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/google/cloud/storage/
--rw-rw-r--   0 henry     (1000) henry     (1000)      110 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1228 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/blob.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      522 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/bucket.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      445 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/google/cloud/storage/client.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.929548 py-data-mock-0.0.5/data_mock/mock_helpers/
--rw-rw-r--   0 henry     (1000) henry     (1000)     8025 2023-06-02 02:05:27.000000 py-data-mock-0.0.5/data_mock/mock_helpers/generate_data.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2238 2023-05-25 03:01:07.000000 py-data-mock-0.0.5/data_mock/mock_helpers/provider.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      116 2023-05-23 16:41:34.000000 py-data-mock-0.0.5/data_mock/mock_helpers/writer.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/data_mock/scripts/
--rw-rw-r--   0 henry     (1000) henry     (1000)     2245 2023-05-20 20:51:44.000000 py-data-mock-0.0.5/data_mock/scripts/mkmock.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/py_data_mock.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      363 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)     1008 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      132 2023-06-02 03:59:15.000000 py-data-mock-0.0.5/py_data_mock.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)      649 2023-05-26 05:01:26.000000 py-data-mock-0.0.5/setup.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-02 03:59:15.933548 py-data-mock-0.0.5/tests/
--rw-rw-r--   0 henry     (1000) henry     (1000)     1167 2023-05-20 20:54:11.000000 py-data-mock-0.0.5/tests/test1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.688691 py-data-mock-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.680691 py-data-mock-0.0.6/data_mock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.680691 py-data-mock-0.0.6/data_mock/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.680691 py-data-mock-0.0.6/data_mock/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6323 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/client.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/enums.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/load.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/query.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/retry.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/google/cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/blob.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/mock_helpers/
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/mock_helpers/generate_data.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/mock_helpers/provider.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/mock_helpers/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/psycopg2/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4979 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/connect.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/cursor.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/extras.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/py_data_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 23:19:32.688691 py-data-mock-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/setup.py
```

### Comparing `py-data-mock-0.0.5/LICENSE` & `py-data-mock-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/README.md` & `py-data-mock-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/client.py` & `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/enums.py` & `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/enums.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/schema.py` & `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/schema.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/storage/blob.py` & `py-data-mock-0.0.6/data_mock/google/cloud/storage/blob.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/google/cloud/storage/bucket.py` & `py-data-mock-0.0.6/data_mock/google/cloud/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/mock_helpers/generate_data.py` & `py-data-mock-0.0.6/data_mock/mock_helpers/generate_data.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/data_mock/mock_helpers/provider.py` & `py-data-mock-0.0.6/data_mock/mock_helpers/provider.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.5/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.6/py_data_mock.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,13 +17,16 @@
 data_mock/google/cloud/storage/__init__.py
 data_mock/google/cloud/storage/blob.py
 data_mock/google/cloud/storage/bucket.py
 data_mock/google/cloud/storage/client.py
 data_mock/mock_helpers/generate_data.py
 data_mock/mock_helpers/provider.py
 data_mock/mock_helpers/writer.py
-data_mock/scripts/mkmock.py
+data_mock/psycopg2/__init__.py
+data_mock/psycopg2/connect.py
+data_mock/psycopg2/cursor.py
+data_mock/psycopg2/exceptions.py
+data_mock/psycopg2/extras.py
 py_data_mock.egg-info/PKG-INFO
 py_data_mock.egg-info/SOURCES.txt
 py_data_mock.egg-info/dependency_links.txt
-py_data_mock.egg-info/top_level.txt
-tests/test1.py
+py_data_mock.egg-info/top_level.txt
```

### Comparing `py-data-mock-0.0.5/setup.py` & `py-data-mock-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='py-data-mock',
-    version='0.0.5',    
-    scripts=['data_mock/scripts/mkmock.py'],
+    version='0.0.6',    
     description='Mock Data',
     url='https://github.com/paulhtremblay/py-data-mock',
     author='Henry Tremblay',
     author_email='paulhtremblay@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['data_mock/google/cloud/bigquery/job', 'data_mock/google/cloud/bigquery',
         'data_mock/google/cloud/storage','data_mock/mock_helpers', 'data_mock',
+        'data_mock/psycopg2/',
         ],
      classifiers=[
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Testing :: Mocking'
     ],
 )
```

