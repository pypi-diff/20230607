# Comparing `tmp/mcap-etl-0.1.3.tar.gz` & `tmp/mcap-etl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-etl-0.1.3.tar", last modified: Wed Jun  7 18:13:27 2023, max compression
+gzip compressed data, was "mcap-etl-0.1.4.tar", last modified: Wed Jun  7 20:40:56 2023, max compression
```

## Comparing `mcap-etl-0.1.3.tar` & `mcap-etl-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.671272 mcap-etl-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/convert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/convert/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/convert/mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/parser/rosbag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl/timescale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/timescale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/timescale/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/mcap_etl/timescale/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:13:27.667271 mcap-etl-0.1.3/mcap_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 18:13:27.000000 mcap-etl-0.1.3/mcap_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:13:27.671272 mcap-etl-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-07 18:13:11.000000 mcap-etl-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/mcap_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/mcap_etl/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/convert/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/convert/mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/mcap_etl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/parser/rosbag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/mcap_etl/timescale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/timescale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/timescale/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/mcap_etl/timescale/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/mcap_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 20:40:55.000000 mcap-etl-0.1.4/mcap_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 20:40:56.000000 mcap-etl-0.1.4/mcap_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:40:55.000000 mcap-etl-0.1.4/mcap_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 20:40:55.000000 mcap-etl-0.1.4/mcap_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 20:40:55.000000 mcap-etl-0.1.4/mcap_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 20:40:55.000000 mcap-etl-0.1.4/mcap_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:40:56.057113 mcap-etl-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-07 20:40:39.000000 mcap-etl-0.1.4/setup.py
```

### Comparing `mcap-etl-0.1.3/.github/workflows/release.yml` & `mcap-etl-0.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/PKG-INFO` & `mcap-etl-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-etl
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transform mcap (or rosbag) files into databases or other files
 Home-page: https://github.com/SensorSurf/mcap-etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap-etl/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap-etl
 Keywords: ros,ros2,rosbag,mcap,timescale,etl,timeseries,database,etl
```

### Comparing `mcap-etl-0.1.3/README.md` & `mcap-etl-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/mcap_etl/convert/mcap.py` & `mcap-etl-0.1.4/mcap_etl/convert/mcap.py`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/mcap_etl/main.py` & `mcap-etl-0.1.4/mcap_etl/main.py`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/mcap_etl/timescale/executor.py` & `mcap-etl-0.1.4/mcap_etl/timescale/executor.py`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/mcap_etl/timescale/postgres.py` & `mcap-etl-0.1.4/mcap_etl/timescale/postgres.py`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/mcap_etl.egg-info/PKG-INFO` & `mcap-etl-0.1.4/mcap_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-etl
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transform mcap (or rosbag) files into databases or other files
 Home-page: https://github.com/SensorSurf/mcap-etl
 Author: SensorSurf
 Author-email: support@sensorsurf.com
 Project-URL: Bug Reports, https://github.com/SensorSurf/mcap-etl/issues
 Project-URL: Source, https://github.com/SensorSurf/mcap-etl
 Keywords: ros,ros2,rosbag,mcap,timescale,etl,timeseries,database,etl
```

### Comparing `mcap-etl-0.1.3/mcap_etl.egg-info/SOURCES.txt` & `mcap-etl-0.1.4/mcap_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcap-etl-0.1.3/setup.py` & `mcap-etl-0.1.4/setup.py`

 * *Files identical despite different names*

