# Comparing `tmp/pysimflow-0.0.42.tar.gz` & `tmp/pysimflow-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimflow-0.0.42.tar", last modified: Wed Jun  7 02:41:30 2023, max compression
+gzip compressed data, was "pysimflow-0.0.43.tar", last modified: Wed Jun  7 02:49:15 2023, max compression
```

## Comparing `pysimflow-0.0.42.tar` & `pysimflow-0.0.43.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.293341 pysimflow-0.0.42/
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 02:41:30.293341 pysimflow-0.0.42/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26999 2023-06-07 02:03:31.000000 pysimflow-0.0.42/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.292342 pysimflow-0.0.42/digitaltwin/
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-05 06:58:11.000000 pysimflow-0.0.42/digitaltwin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2231 2023-05-29 08:58:34.000000 pysimflow-0.0.42/digitaltwin/active_obj.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-06-05 08:48:15.000000 pysimflow-0.0.42/digitaltwin/box.py
--rw-r--r--   0 root         (0) root         (0)    16516 2023-05-30 11:24:25.000000 pysimflow-0.0.42/digitaltwin/camera.py
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-05 06:50:25.000000 pysimflow-0.0.42/digitaltwin/cube.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 06:56:29.000000 pysimflow-0.0.42/digitaltwin/cylinder.py
--rw-r--r--   0 root         (0) root         (0)     4392 2023-06-05 09:24:58.000000 pysimflow-0.0.42/digitaltwin/editor.py
--rw-r--r--   0 root         (0) root         (0)     2685 2023-05-25 09:07:12.000000 pysimflow-0.0.42/digitaltwin/placer.py
--rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.42/digitaltwin/printer.py
--rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.42/digitaltwin/render.py
--rw-r--r--   0 root         (0) root         (0)    22619 2023-06-05 09:46:39.000000 pysimflow-0.0.42/digitaltwin/robot.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-05-30 11:28:51.000000 pysimflow-0.0.42/digitaltwin/scene.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-06-02 01:48:36.000000 pysimflow-0.0.42/digitaltwin/stacker.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-06-05 04:04:34.000000 pysimflow-0.0.42/digitaltwin/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.292342 pysimflow-0.0.42/digitaltwin_data/
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 02:54:55.000000 pysimflow-0.0.42/digitaltwin_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.293341 pysimflow-0.0.42/pysimflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-07 02:41:30.293341 pysimflow-0.0.42/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      368 2023-06-07 02:37:57.000000 pysimflow-0.0.42/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:49:15.519626 pysimflow-0.0.43/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 02:49:15.519626 pysimflow-0.0.43/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26999 2023-06-07 02:03:31.000000 pysimflow-0.0.43/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:49:15.519626 pysimflow-0.0.43/digitaltwin/
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-05 06:58:11.000000 pysimflow-0.0.43/digitaltwin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2023-05-29 08:58:34.000000 pysimflow-0.0.43/digitaltwin/active_obj.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-06-05 08:48:15.000000 pysimflow-0.0.43/digitaltwin/box.py
+-rw-r--r--   0 root         (0) root         (0)    16516 2023-05-30 11:24:25.000000 pysimflow-0.0.43/digitaltwin/camera.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-05 06:50:25.000000 pysimflow-0.0.43/digitaltwin/cube.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 06:56:29.000000 pysimflow-0.0.43/digitaltwin/cylinder.py
+-rw-r--r--   0 root         (0) root         (0)     4392 2023-06-05 09:24:58.000000 pysimflow-0.0.43/digitaltwin/editor.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-05-25 09:07:12.000000 pysimflow-0.0.43/digitaltwin/placer.py
+-rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.43/digitaltwin/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.43/digitaltwin/render.py
+-rw-r--r--   0 root         (0) root         (0)    22619 2023-06-05 09:46:39.000000 pysimflow-0.0.43/digitaltwin/robot.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-30 11:28:51.000000 pysimflow-0.0.43/digitaltwin/scene.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-02 01:48:36.000000 pysimflow-0.0.43/digitaltwin/stacker.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-06-05 04:04:34.000000 pysimflow-0.0.43/digitaltwin/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:49:15.519626 pysimflow-0.0.43/digitaltwin_data/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 02:54:55.000000 pysimflow-0.0.43/digitaltwin_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:49:15.519626 pysimflow-0.0.43/pysimflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 02:49:15.000000 pysimflow-0.0.43/pysimflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-07 02:49:15.000000 pysimflow-0.0.43/pysimflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 02:49:15.000000 pysimflow-0.0.43/pysimflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 02:49:15.000000 pysimflow-0.0.43/pysimflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 02:49:15.000000 pysimflow-0.0.43/pysimflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-07 02:49:15.520626 pysimflow-0.0.43/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-07 02:49:08.000000 pysimflow-0.0.43/setup.py
```

### Comparing `pysimflow-0.0.42/README.md` & `pysimflow-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/active_obj.py` & `pysimflow-0.0.43/digitaltwin/active_obj.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/box.py` & `pysimflow-0.0.43/digitaltwin/box.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/camera.py` & `pysimflow-0.0.43/digitaltwin/camera.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/cube.py` & `pysimflow-0.0.43/digitaltwin/cube.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/cylinder.py` & `pysimflow-0.0.43/digitaltwin/cylinder.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/editor.py` & `pysimflow-0.0.43/digitaltwin/editor.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/placer.py` & `pysimflow-0.0.43/digitaltwin/placer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/printer.py` & `pysimflow-0.0.43/digitaltwin/printer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/render.py` & `pysimflow-0.0.43/digitaltwin/render.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/robot.py` & `pysimflow-0.0.43/digitaltwin/robot.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/scene.py` & `pysimflow-0.0.43/digitaltwin/scene.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/stacker.py` & `pysimflow-0.0.43/digitaltwin/stacker.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/digitaltwin/workflow.py` & `pysimflow-0.0.43/digitaltwin/workflow.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.42/pysimflow.egg-info/SOURCES.txt` & `pysimflow-0.0.43/pysimflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

