# Comparing `tmp/mcap_etl-0.1.1.tar.gz` & `tmp/mcap_etl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap_etl-0.1.1.tar", last modified: Tue Jun  6 21:12:00 2023, max compression
+gzip compressed data, was "mcap_etl-0.1.2.tar", last modified: Tue Jun  6 23:19:15 2023, max compression
```

## Comparing `mcap_etl-0.1.1.tar` & `mcap_etl-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/
--rw-rw-r--   0 alec      (1000) alec      (1000)     3639 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)     2743 2023-06-06 21:10:38.000000 mcap_etl-0.1.1/README.md
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/__init__.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/convert/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/convert/__init__.py
--rw-rw-r--   0 alec      (1000) alec      (1000)      432 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/convert/executor.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     1597 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/convert/mcap.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     1529 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/main.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/parser/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/parser/__init__.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     4023 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/parser/rosbag.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl/timescale/
--rw-rw-r--   0 alec      (1000) alec      (1000)        0 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/timescale/__init__.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     1657 2023-06-06 21:08:24.000000 mcap_etl-0.1.1/mcap_etl/timescale/executor.py
--rw-rw-r--   0 alec      (1000) alec      (1000)     3297 2023-06-06 21:11:45.000000 mcap_etl-0.1.1/mcap_etl/timescale/postgres.py
-drwxrwxr-x   0 alec      (1000) alec      (1000)        0 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/mcap_etl.egg-info/
--rw-rw-r--   0 alec      (1000) alec      (1000)     3639 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/PKG-INFO
--rw-rw-r--   0 alec      (1000) alec      (1000)      480 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        1 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       49 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/entry_points.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)      249 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/requires.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)        9 2023-06-06 21:12:00.000000 mcap_etl-0.1.1/mcap_etl.egg-info/top_level.txt
--rw-rw-r--   0 alec      (1000) alec      (1000)       38 2023-06-06 21:12:00.836145 mcap_etl-0.1.1/setup.cfg
--rw-rw-r--   0 alec      (1000) alec      (1000)     1764 2023-06-06 21:11:53.000000 mcap_etl-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/mcap_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/mcap_etl/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/convert/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/convert/mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/mcap_etl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/parser/rosbag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/mcap_etl/timescale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/timescale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/timescale/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/timescale/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/mcap_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/setup.py
```

### Comparing `mcap_etl-0.1.1/PKG-INFO` & `mcap_etl-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: mcap_etl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transform mcap (or rosbag) files into databases or other files
 Home-page: https://github.com/SensorSurf/mcap_etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap_etl/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap_etl
-Keywords: ros,ros1,rosbag,mcap,timescale,etl,timeseries,database,etl
-Platform: UNKNOWN
+Keywords: ros,ros2,rosbag,mcap,timescale,etl,timeseries,database,etl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -68,8 +66,7 @@
 ## Key Design Considerations
 
 mcap_etl has been designed with the following key principles:
 
 * __Timescale Hypertables__: Due to the large number of messages, we use Timescale's hypertables and take advantage of their compression features.
 * __No ROS Dependency__: mcap_etl operates without any ROS dependencies, avoiding the complexity of ROS installations for simple data extraction from `.bag` or `.mcap` files. Instead, we utilize the `rosbags` project, which allows for dynamic loading of message schemas at runtime.
 * __MCAP to ROS bag Transformation__: mcap_etl first converts MCAP files into ROS bags before performing data transformations. This approach avoids the need to rewrite the ingestion flow.
-
```

### Comparing `mcap_etl-0.1.1/README.md` & `mcap_etl-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.1/mcap_etl/convert/mcap.py` & `mcap_etl-0.1.2/mcap_etl/convert/mcap.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.1/mcap_etl/main.py` & `mcap_etl-0.1.2/mcap_etl/main.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.1/mcap_etl/parser/rosbag.py` & `mcap_etl-0.1.2/mcap_etl/parser/rosbag.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.1/mcap_etl/timescale/executor.py` & `mcap_etl-0.1.2/mcap_etl/timescale/executor.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.1/mcap_etl/timescale/postgres.py` & `mcap_etl-0.1.2/mcap_etl/timescale/postgres.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.1/mcap_etl.egg-info/PKG-INFO` & `mcap_etl-0.1.2/mcap_etl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: mcap-etl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transform mcap (or rosbag) files into databases or other files
 Home-page: https://github.com/SensorSurf/mcap_etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap_etl/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap_etl
-Keywords: ros,ros1,rosbag,mcap,timescale,etl,timeseries,database,etl
-Platform: UNKNOWN
+Keywords: ros,ros2,rosbag,mcap,timescale,etl,timeseries,database,etl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -68,8 +66,7 @@
 ## Key Design Considerations
 
 mcap_etl has been designed with the following key principles:
 
 * __Timescale Hypertables__: Due to the large number of messages, we use Timescale's hypertables and take advantage of their compression features.
 * __No ROS Dependency__: mcap_etl operates without any ROS dependencies, avoiding the complexity of ROS installations for simple data extraction from `.bag` or `.mcap` files. Instead, we utilize the `rosbags` project, which allows for dynamic loading of message schemas at runtime.
 * __MCAP to ROS bag Transformation__: mcap_etl first converts MCAP files into ROS bags before performing data transformations. This approach avoids the need to rewrite the ingestion flow.
-
```

### Comparing `mcap_etl-0.1.1/setup.py` & `mcap_etl-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mcap_etl',
-    version='0.1.1',
     author='SensorSurf',
     author_email='support@sensorsurf.com',
     description='Transform mcap (or rosbag) files into databases or other files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/SensorSurf/mcap_etl',
     packages=find_packages(),
+    use_scm_version=True,
+    setup_requires=['setuptools_scm'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    keywords='ros, ros1, rosbag, mcap, timescale, etl, timeseries, database, etl',
+    keywords='ros, ros2, rosbag, mcap, timescale, etl, timeseries, database, etl',
     install_requires=[
         'jmespath==1.0.1',
         'lz4==4.3.2',
         'mcap==1.0.2',
         'numpy==1.23.1',
         'pandas==2.0.1',
         'psycopg2-binary==2.9.6',
```

