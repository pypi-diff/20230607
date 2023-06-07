# Comparing `tmp/mcap_etl-0.1.2.tar.gz` & `tmp/mcap-etl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap_etl-0.1.2.tar", last modified: Tue Jun  6 23:19:15 2023, max compression
+gzip compressed data, was "mcap-etl-0.1.3.tar", last modified: Wed Jun  7 18:13:27 2023, max compression
```

## Comparing `mcap_etl-0.1.2.tar` & `mcap-etl-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/mcap_etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/mcap_etl/convert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/convert/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/convert/mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/mcap_etl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/parser/rosbag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/mcap_etl/timescale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/timescale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/timescale/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/mcap_etl/timescale/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:19:15.877798 mcap_etl-0.1.2/mcap_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 23:19:15.000000 mcap_etl-0.1.2/mcap_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:19:15.881799 mcap_etl-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-06 23:19:02.000000 mcap_etl-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.671272 mcap-etl-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/convert/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/convert/mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/parser/rosbag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/timescale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/timescale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/timescale/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/timescale/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:13:27.671272 mcap-etl-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/setup.py
```

### Comparing `mcap_etl-0.1.2/.github/workflows/release.yml` & `mcap-etl-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/PKG-INFO` & `mcap-etl-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: mcap_etl
-Version: 0.1.2
+Name: mcap-etl
+Version: 0.1.3
 Summary: Transform mcap (or rosbag) files into databases or other files
-Home-page: https://github.com/SensorSurf/mcap_etl
+Home-page: https://github.com/SensorSurf/mcap-etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
-Project-URL: Bug Reports, https://github.com/SensorSurf/mcap_etl/issues
-Project-URL: Source, https://github.com/SensorSurf/mcap_etl
+Project-URL: Bug Reports, https://github.com/SensorSurf/mcap-etl/issues
+Project-URL: Source, https://github.com/SensorSurf/mcap-etl
 Keywords: ros,ros2,rosbag,mcap,timescale,etl,timeseries,database,etl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mcap_etl-0.1.2/README.md` & `mcap-etl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/mcap_etl/convert/mcap.py` & `mcap-etl-0.1.3/mcap_etl/convert/mcap.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/mcap_etl/main.py` & `mcap-etl-0.1.3/mcap_etl/main.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/mcap_etl/parser/rosbag.py` & `mcap-etl-0.1.3/mcap_etl/parser/rosbag.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/mcap_etl/timescale/executor.py` & `mcap-etl-0.1.3/mcap_etl/timescale/executor.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/mcap_etl/timescale/postgres.py` & `mcap-etl-0.1.3/mcap_etl/timescale/postgres.py`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/mcap_etl.egg-info/PKG-INFO` & `mcap-etl-0.1.3/mcap_etl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mcap-etl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transform mcap (or rosbag) files into databases or other files
-Home-page: https://github.com/SensorSurf/mcap_etl
+Home-page: https://github.com/SensorSurf/mcap-etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
-Project-URL: Bug Reports, https://github.com/SensorSurf/mcap_etl/issues
-Project-URL: Source, https://github.com/SensorSurf/mcap_etl
+Project-URL: Bug Reports, https://github.com/SensorSurf/mcap-etl/issues
+Project-URL: Source, https://github.com/SensorSurf/mcap-etl
 Keywords: ros,ros2,rosbag,mcap,timescale,etl,timeseries,database,etl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mcap_etl-0.1.2/mcap_etl.egg-info/SOURCES.txt` & `mcap-etl-0.1.3/mcap_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcap_etl-0.1.2/setup.py` & `mcap-etl-0.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,56 +2,43 @@
 
 from setuptools import setup, find_packages
 
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
+with open('requirements.txt') as file:
+    requirements = file.read().splitlines()
+
 setup(
-    name='mcap_etl',
+    name='mcap-etl',
     author='SensorSurf',
     author_email='support@sensorsurf.com',
     description='Transform mcap (or rosbag) files into databases or other files',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/SensorSurf/mcap_etl',
+    url='https://github.com/SensorSurf/mcap-etl',
     packages=find_packages(),
     use_scm_version=True,
     setup_requires=['setuptools_scm'],
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
     keywords='ros, ros2, rosbag, mcap, timescale, etl, timeseries, database, etl',
-    install_requires=[
-        'jmespath==1.0.1',
-        'lz4==4.3.2',
-        'mcap==1.0.2',
-        'numpy==1.23.1',
-        'pandas==2.0.1',
-        'psycopg2-binary==2.9.6',
-        'python-dateutil==2.8.2',
-        'pytz==2023.3',
-        'rosbags==0.9.15',
-        'ruamel.yaml==0.17.26',
-        'ruamel.yaml.clib==0.2.7',
-        'six==1.16.0',
-        'tzdata==2023.3',
-        'urllib3==1.26.15',
-        'zstandard==0.21.0',
-    ],
+    install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'mcap_etl=mcap_etl.main:main',
+            'mcap-etl=mcap_etl.main:main',
         ],
     },
     project_urls={
-        'Bug Reports': 'https://github.com/SensorSurf/mcap_etl/issues',
-        'Source': 'https://github.com/SensorSurf/mcap_etl',
+        'Bug Reports': 'https://github.com/SensorSurf/mcap-etl/issues',
+        'Source': 'https://github.com/SensorSurf/mcap-etl',
     },
 )
```

