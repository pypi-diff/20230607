# Comparing `tmp/BatteryRateCap-0.1.0.tar.gz` & `tmp/BatteryRateCap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/user/Downloads/BatteryRateCap/dist/.tmp-3386q4i_/BatteryRateCap-0.1.0.tar", last modified: Tue May 30 23:07:26 2023, max compression
+gzip compressed data, was "/home/user/Downloads/BatteryRateCap/dist/.tmp-jl8lpx5f/BatteryRateCap-0.1.1.tar", last modified: Wed Jun  7 19:05:41 2023, max compression
```

## Comparing `BatteryRateCap-0.1.0.tar` & `BatteryRateCap-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/BatteryRateCap.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     8162 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/BatteryRateCap.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      300 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/BatteryRateCap.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/BatteryRateCap.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       15 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/BatteryRateCap.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1059 2023-05-30 18:15:22.000000 BatteryRateCap-0.1.0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8162 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     6150 2023-05-30 18:15:22.000000 BatteryRateCap-0.1.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-05-30 23:05:50.000000 BatteryRateCap-0.1.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:07:26.000000 BatteryRateCap-0.1.0/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     2157 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.0/tests/test_correlationtest.py
--rw-rw-r--   0 user      (1000) user      (1000)     4128 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.0/tests/test_data_converter.py
--rw-rw-r--   0 user      (1000) user      (1000)     3821 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.0/tests/test_fitcaprate.py
--rw-rw-r--   0 user      (1000) user      (1000)     1445 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.0/tests/test_visualization.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     8166 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      300 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       15 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1059 2023-05-30 18:15:22.000000 BatteryRateCap-0.1.1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8166 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     6154 2023-05-31 17:45:04.000000 BatteryRateCap-0.1.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-06-07 19:04:49.000000 BatteryRateCap-0.1.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     2157 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_correlationtest.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4128 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_data_converter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3821 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_fitcaprate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1445 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_visualization.py
```

### Comparing `BatteryRateCap-0.1.0/BatteryRateCap.egg-info/PKG-INFO` & `BatteryRateCap-0.1.1/BatteryRateCap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BatteryRateCap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for battery rate capability analysis.
 Author-email: Chih-Hsuan Hung <dhung@uw.edu>, Praise Anyanwu <anyanc@uw.edu>, "Kevin G. Lee" <gskl92@uw.edu>, "Matthew J. Canin" <matthewcanin@gmail.com>, Kevin Martinez-Chavez <martikev@protonmail.com>
 Maintainer-email: Chih-Hsuan Hung <dhung@uw.edu>
 License: MIT License
         
         Copyright (c) 2021 c.
         
@@ -115,21 +115,21 @@
 and highlights potential outliers (in red) to the linear relationship.
 ![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/correlation_test_example.png)
 
  
 ## How to Install
 *BatteryRateCap* can be installed by cloning the entire repoitory or via pip:</br>
 ```
-pip install batteryratecap
+pip install BatteryRateCap
 ```
 
 ## Software Dependency
 - Python >=3.6
 - See environment.yml for all Python package dependencies
 
 
 ## Community Guidelines
-If you encounter any issue using *BatRateCap* or would like to request an additional feature, please report using a [Github 
+If you encounter any issue using *BatteryRateCap* or would like to request an additional feature, please report using a [Github 
 issue](https://github.com/BatteryDesign/BatteryRateCap/issues). If you would like to directly contribute to this project, please email the 
 reporsitory maintainer Doris Hung at dhung@uw.edu.
```

### Comparing `BatteryRateCap-0.1.0/LICENSE.txt` & `BatteryRateCap-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.0/PKG-INFO` & `BatteryRateCap-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BatteryRateCap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for battery rate capability analysis.
 Author-email: Chih-Hsuan Hung <dhung@uw.edu>, Praise Anyanwu <anyanc@uw.edu>, "Kevin G. Lee" <gskl92@uw.edu>, "Matthew J. Canin" <matthewcanin@gmail.com>, Kevin Martinez-Chavez <martikev@protonmail.com>
 Maintainer-email: Chih-Hsuan Hung <dhung@uw.edu>
 License: MIT License
         
         Copyright (c) 2021 c.
         
@@ -115,21 +115,21 @@
 and highlights potential outliers (in red) to the linear relationship.
 ![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/correlation_test_example.png)
 
  
 ## How to Install
 *BatteryRateCap* can be installed by cloning the entire repoitory or via pip:</br>
 ```
-pip install batteryratecap
+pip install BatteryRateCap
 ```
 
 ## Software Dependency
 - Python >=3.6
 - See environment.yml for all Python package dependencies
 
 
 ## Community Guidelines
-If you encounter any issue using *BatRateCap* or would like to request an additional feature, please report using a [Github 
+If you encounter any issue using *BatteryRateCap* or would like to request an additional feature, please report using a [Github 
 issue](https://github.com/BatteryDesign/BatteryRateCap/issues). If you would like to directly contribute to this project, please email the 
 reporsitory maintainer Doris Hung at dhung@uw.edu.
```

### Comparing `BatteryRateCap-0.1.0/README.md` & `BatteryRateCap-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,21 +77,21 @@
 and highlights potential outliers (in red) to the linear relationship.
 ![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/correlation_test_example.png)
 
  
 ## How to Install
 *BatteryRateCap* can be installed by cloning the entire repoitory or via pip:</br>
 ```
-pip install batteryratecap
+pip install BatteryRateCap
 ```
 
 ## Software Dependency
 - Python >=3.6
 - See environment.yml for all Python package dependencies
 
 
 ## Community Guidelines
-If you encounter any issue using *BatRateCap* or would like to request an additional feature, please report using a [Github 
+If you encounter any issue using *BatteryRateCap* or would like to request an additional feature, please report using a [Github 
 issue](https://github.com/BatteryDesign/BatteryRateCap/issues). If you would like to directly contribute to this project, please email the 
 reporsitory maintainer Doris Hung at dhung@uw.edu.
```

### Comparing `BatteryRateCap-0.1.0/pyproject.toml` & `BatteryRateCap-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "BatteryRateCap"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package for battery rate capability analysis."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 keywords = ["battery", "rate analysis", "rate capability"]
 authors = [
     {name = "Chih-Hsuan Hung", email = "dhung@uw.edu"},
```

### Comparing `BatteryRateCap-0.1.0/tests/test_correlationtest.py` & `BatteryRateCap-0.1.1/tests/test_correlationtest.py`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.0/tests/test_data_converter.py` & `BatteryRateCap-0.1.1/tests/test_data_converter.py`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.0/tests/test_fitcaprate.py` & `BatteryRateCap-0.1.1/tests/test_fitcaprate.py`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.0/tests/test_visualization.py` & `BatteryRateCap-0.1.1/tests/test_visualization.py`

 * *Files identical despite different names*

