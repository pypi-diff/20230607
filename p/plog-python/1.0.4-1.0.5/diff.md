# Comparing `tmp/plog-python-1.0.4.tar.gz` & `tmp/plog-python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plog-python-1.0.4.tar", last modified: Wed Jun  7 02:05:45 2023, max compression
+gzip compressed data, was "plog-python-1.0.5.tar", last modified: Wed Jun  7 02:12:52 2023, max compression
```

## Comparing `plog-python-1.0.4.tar` & `plog-python-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:05:45.641391 plog-python-1.0.4/
--rw-rw-r--   0 ali       (1000) ali       (1000)      289 2023-06-07 02:05:45.641391 plog-python-1.0.4/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     1476 2023-06-07 01:35:59.000000 plog-python-1.0.4/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:05:45.641391 plog-python-1.0.4/plog/
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-02 22:52:59.000000 plog-python-1.0.4/plog/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:05:45.641391 plog-python-1.0.4/plog/components/
--rw-rw-r--   0 ali       (1000) ali       (1000)       93 2023-06-02 22:51:09.000000 plog-python-1.0.4/plog/components/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-06-02 12:37:24.000000 plog-python-1.0.4/plog/components/checkpoint.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      882 2023-06-07 00:40:09.000000 plog-python-1.0.4/plog/components/objectframe.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1366 2023-06-02 22:50:37.000000 plog-python-1.0.4/plog/components/task.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      231 2023-06-07 02:01:03.000000 plog-python-1.0.4/plog/db.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:05:45.641391 plog-python-1.0.4/plog/handlers/
--rw-rw-r--   0 ali       (1000) ali       (1000)      103 2023-06-02 13:01:06.000000 plog-python-1.0.4/plog/handlers/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1711 2023-06-07 01:56:12.000000 plog-python-1.0.4/plog/handlers/log_handler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1517 2023-06-07 01:56:09.000000 plog-python-1.0.4/plog/handlers/object_handler.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:05:45.641391 plog-python-1.0.4/plog/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       55 2023-06-02 12:47:53.000000 plog-python-1.0.4/plog/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      104 2023-05-30 12:14:34.000000 plog-python-1.0.4/plog/models/file_model.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1057 2023-06-02 23:06:56.000000 plog-python-1.0.4/plog/models/log_model.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:05:45.641391 plog-python-1.0.4/plog_python.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)      289 2023-06-07 02:05:45.000000 plog-python-1.0.4/plog_python.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      495 2023-06-07 02:05:45.000000 plog-python-1.0.4/plog_python.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-07 02:05:45.000000 plog-python-1.0.4/plog_python.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       49 2023-06-07 02:05:45.000000 plog-python-1.0.4/plog_python.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        5 2023-06-07 02:05:45.000000 plog-python-1.0.4/plog_python.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       38 2023-06-07 02:05:45.641391 plog-python-1.0.4/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)      539 2023-06-07 02:04:55.000000 plog-python-1.0.4/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:12:52.434083 plog-python-1.0.5/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      289 2023-06-07 02:12:52.434083 plog-python-1.0.5/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1476 2023-06-07 01:35:59.000000 plog-python-1.0.5/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:12:52.434083 plog-python-1.0.5/plog/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-02 22:52:59.000000 plog-python-1.0.5/plog/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:12:52.434083 plog-python-1.0.5/plog/components/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       93 2023-06-02 22:51:09.000000 plog-python-1.0.5/plog/components/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-06-02 12:37:24.000000 plog-python-1.0.5/plog/components/checkpoint.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      882 2023-06-07 00:40:09.000000 plog-python-1.0.5/plog/components/objectframe.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1366 2023-06-02 22:50:37.000000 plog-python-1.0.5/plog/components/task.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      281 2023-06-07 02:12:16.000000 plog-python-1.0.5/plog/db.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:12:52.434083 plog-python-1.0.5/plog/handlers/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      103 2023-06-02 13:01:06.000000 plog-python-1.0.5/plog/handlers/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1711 2023-06-07 01:56:12.000000 plog-python-1.0.5/plog/handlers/log_handler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1517 2023-06-07 01:56:09.000000 plog-python-1.0.5/plog/handlers/object_handler.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:12:52.434083 plog-python-1.0.5/plog/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       55 2023-06-02 12:47:53.000000 plog-python-1.0.5/plog/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      104 2023-05-30 12:14:34.000000 plog-python-1.0.5/plog/models/file_model.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1057 2023-06-02 23:06:56.000000 plog-python-1.0.5/plog/models/log_model.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-07 02:12:52.434083 plog-python-1.0.5/plog_python.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      289 2023-06-07 02:12:52.000000 plog-python-1.0.5/plog_python.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      495 2023-06-07 02:12:52.000000 plog-python-1.0.5/plog_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-07 02:12:52.000000 plog-python-1.0.5/plog_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       49 2023-06-07 02:12:52.000000 plog-python-1.0.5/plog_python.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        5 2023-06-07 02:12:52.000000 plog-python-1.0.5/plog_python.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       38 2023-06-07 02:12:52.438083 plog-python-1.0.5/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)      539 2023-06-07 02:12:50.000000 plog-python-1.0.5/setup.py
```

### Comparing `plog-python-1.0.4/README.md` & `plog-python-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `plog-python-1.0.4/plog/components/objectframe.py` & `plog-python-1.0.5/plog/components/objectframe.py`

 * *Files identical despite different names*

### Comparing `plog-python-1.0.4/plog/components/task.py` & `plog-python-1.0.5/plog/components/task.py`

 * *Files identical despite different names*

### Comparing `plog-python-1.0.4/plog/handlers/log_handler.py` & `plog-python-1.0.5/plog/handlers/log_handler.py`

 * *Files identical despite different names*

### Comparing `plog-python-1.0.4/plog/handlers/object_handler.py` & `plog-python-1.0.5/plog/handlers/object_handler.py`

 * *Files identical despite different names*

### Comparing `plog-python-1.0.4/plog/models/log_model.py` & `plog-python-1.0.5/plog/models/log_model.py`

 * *Files identical despite different names*

### Comparing `plog-python-1.0.4/setup.py` & `plog-python-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='plog-python',
-    version='1.0.4',
+    version='1.0.5',
     description='A service for logging data and objects in different steps of applications',
     long_description='A service for logging data and objects in different steps of applications',
     author='Ali Khodadoost',
     author_email='ali1.khodadoost@gmail.com',
     license='MIT',
     packages=find_packages("."),
     install_requires=[
```

