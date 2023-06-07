# Comparing `tmp/persian-gender-detection-1.0.2.tar.gz` & `tmp/persian-gender-detection-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-gender-detection-1.0.2.tar", last modified: Wed Jun  7 16:21:01 2023, max compression
+gzip compressed data, was "persian-gender-detection-1.0.4.tar", last modified: Wed Jun  7 16:42:10 2023, max compression
```

## Comparing `persian-gender-detection-1.0.2.tar` & `persian-gender-detection-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:21:01.852138 persian-gender-detection-1.0.2/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.0.2/LICENSE
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2255 2023-06-07 16:21:01.852138 persian-gender-detection-1.0.2/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      937 2023-06-07 16:20:16.000000 persian-gender-detection-1.0.2/README.md
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:21:01.844138 persian-gender-detection-1.0.2/persian_gender_detection/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.0.2/persian_gender_detection/__init__.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:21:01.848138 persian-gender-detection-1.0.2/persian_gender_detection/gender/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   135092 2023-06-05 10:24:08.000000 persian-gender-detection-1.0.2/persian_gender_detection/gender/female.json
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   125412 2023-06-07 15:15:48.000000 persian-gender-detection-1.0.2/persian_gender_detection/gender/male.json
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   116646 2023-06-05 10:24:08.000000 persian-gender-detection-1.0.2/persian_gender_detection/gender/names.csv
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      922 2023-06-07 16:04:24.000000 persian-gender-detection-1.0.2/persian_gender_detection/persian_gender_detection.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:21:01.848138 persian-gender-detection-1.0.2/persian_gender_detection.egg-info/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2255 2023-06-07 16:21:01.000000 persian-gender-detection-1.0.2/persian_gender_detection.egg-info/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      484 2023-06-07 16:21:01.000000 persian-gender-detection-1.0.2/persian_gender_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-07 16:21:01.000000 persian-gender-detection-1.0.2/persian_gender_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-07 16:21:01.000000 persian-gender-detection-1.0.2/persian_gender_detection.egg-info/top_level.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-07 16:21:01.852138 persian-gender-detection-1.0.2/setup.cfg
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1759 2023-06-07 16:20:04.000000 persian-gender-detection-1.0.2/setup.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:21:01.852138 persian-gender-detection-1.0.2/test/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.0.2/test/test_clean_name.py
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1874 2023-06-07 16:03:13.000000 persian-gender-detection-1.0.2/test/test_get_gender.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:42:10.558711 persian-gender-detection-1.0.4/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.0.4/LICENSE
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2249 2023-06-07 16:42:10.558711 persian-gender-detection-1.0.4/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      931 2023-06-07 16:31:09.000000 persian-gender-detection-1.0.4/README.md
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:42:10.550711 persian-gender-detection-1.0.4/persian_gender_detection/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.0.4/persian_gender_detection/__init__.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:42:10.554711 persian-gender-detection-1.0.4/persian_gender_detection/gender/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   135092 2023-06-05 10:24:08.000000 persian-gender-detection-1.0.4/persian_gender_detection/gender/female.json
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   125412 2023-06-07 15:15:48.000000 persian-gender-detection-1.0.4/persian_gender_detection/gender/male.json
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   116646 2023-06-05 10:24:08.000000 persian-gender-detection-1.0.4/persian_gender_detection/gender/names.csv
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      922 2023-06-07 16:04:24.000000 persian-gender-detection-1.0.4/persian_gender_detection/persian_gender_detection.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:42:10.550711 persian-gender-detection-1.0.4/persian_gender_detection.egg-info/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2249 2023-06-07 16:42:10.000000 persian-gender-detection-1.0.4/persian_gender_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      484 2023-06-07 16:42:10.000000 persian-gender-detection-1.0.4/persian_gender_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-07 16:42:10.000000 persian-gender-detection-1.0.4/persian_gender_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-07 16:42:10.000000 persian-gender-detection-1.0.4/persian_gender_detection.egg-info/top_level.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-07 16:42:10.558711 persian-gender-detection-1.0.4/setup.cfg
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1759 2023-06-07 16:41:48.000000 persian-gender-detection-1.0.4/setup.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:42:10.554711 persian-gender-detection-1.0.4/test/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.0.4/test/test_clean_name.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1874 2023-06-07 16:03:13.000000 persian-gender-detection-1.0.4/test/test_get_gender.py
```

### Comparing `persian-gender-detection-1.0.2/LICENSE` & `persian-gender-detection-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.2/PKG-INFO` & `persian-gender-detection-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-gender-detection
-Version: 1.0.2
+Version: 1.0.4
 Summary: A simple python package to detect gender by Persian first name. (With more than 6K names).
 Home-page: https://github.com/zeoses/persian-gender-detection
 Author: Mehraban
 License: MIT License
 Project-URL: Source, https://github.com/zeoses/persian-gender-detection
 Project-URL: Documentation, https://github.com/zeoses/persian-gender-detection
 Keywords: persian-gender-detection,farsi gender,iranian gender,name gender,persian gender detection,gender detection
@@ -40,20 +40,20 @@
 ```
 
 Example
 ------
 ```python
 from persian_gender_detection import get_gender
 
-// Detect gender
-get_gender('  عــــلی  ');         // MALE
-get_gender('نرگـــ😉ــس');         // FEMALE
-get_gender('حســ😎ــن');          // MALE
-get_gender('۱۲۳۹۹۳محمدعلی123');  // MALE
-get_gender('۱۲۳مهناز۱۲۳');       // FEMALE
+# Detect gender
+get_gender('  عــــلی  ')         # MALE
+get_gender('نرگـــ😉ــس')         # FEMALE
+get_gender('حســ😎ــن')           # MALE
+get_gender('۱۲۳۹۹۳محمدعلی123')    # MALE
+get_gender('۱۲۳مهناز۱۲۳')         # FEMALE
 ```
 
 Issues
 ------
 
 Feel free to submit issues and enhancement requests.
```

### Comparing `persian-gender-detection-1.0.2/README.md` & `persian-gender-detection-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 ```
 
 Example
 ------
 ```python
 from persian_gender_detection import get_gender
 
-// Detect gender
-get_gender('  عــــلی  ');         // MALE
-get_gender('نرگـــ😉ــس');         // FEMALE
-get_gender('حســ😎ــن');          // MALE
-get_gender('۱۲۳۹۹۳محمدعلی123');  // MALE
-get_gender('۱۲۳مهناز۱۲۳');       // FEMALE
+# Detect gender
+get_gender('  عــــلی  ')         # MALE
+get_gender('نرگـــ😉ــس')         # FEMALE
+get_gender('حســ😎ــن')           # MALE
+get_gender('۱۲۳۹۹۳محمدعلی123')    # MALE
+get_gender('۱۲۳مهناز۱۲۳')         # FEMALE
 ```
 
 Issues
 ------
 
 Feel free to submit issues and enhancement requests.
```

### Comparing `persian-gender-detection-1.0.2/persian_gender_detection/gender/female.json` & `persian-gender-detection-1.0.4/persian_gender_detection/gender/female.json`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.2/persian_gender_detection/gender/male.json` & `persian-gender-detection-1.0.4/persian_gender_detection/gender/male.json`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.2/persian_gender_detection/gender/names.csv` & `persian-gender-detection-1.0.4/persian_gender_detection/gender/names.csv`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.2/persian_gender_detection/persian_gender_detection.py` & `persian-gender-detection-1.0.4/persian_gender_detection/persian_gender_detection.py`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.2/persian_gender_detection.egg-info/PKG-INFO` & `persian-gender-detection-1.0.4/persian_gender_detection.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-gender-detection
-Version: 1.0.2
+Version: 1.0.4
 Summary: A simple python package to detect gender by Persian first name. (With more than 6K names).
 Home-page: https://github.com/zeoses/persian-gender-detection
 Author: Mehraban
 License: MIT License
 Project-URL: Source, https://github.com/zeoses/persian-gender-detection
 Project-URL: Documentation, https://github.com/zeoses/persian-gender-detection
 Keywords: persian-gender-detection,farsi gender,iranian gender,name gender,persian gender detection,gender detection
@@ -40,20 +40,20 @@
 ```
 
 Example
 ------
 ```python
 from persian_gender_detection import get_gender
 
-// Detect gender
-get_gender('  عــــلی  ');         // MALE
-get_gender('نرگـــ😉ــس');         // FEMALE
-get_gender('حســ😎ــن');          // MALE
-get_gender('۱۲۳۹۹۳محمدعلی123');  // MALE
-get_gender('۱۲۳مهناز۱۲۳');       // FEMALE
+# Detect gender
+get_gender('  عــــلی  ')         # MALE
+get_gender('نرگـــ😉ــس')         # FEMALE
+get_gender('حســ😎ــن')           # MALE
+get_gender('۱۲۳۹۹۳محمدعلی123')    # MALE
+get_gender('۱۲۳مهناز۱۲۳')         # FEMALE
 ```
 
 Issues
 ------
 
 Feel free to submit issues and enhancement requests.
```

### Comparing `persian-gender-detection-1.0.2/setup.py` & `persian-gender-detection-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('./README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='persian-gender-detection',
-    version='1.0.2',
+    version='1.0.4',
     packages=['persian_gender_detection'],
     include_package_data=True,
     data_files=[('', [
         'persian_gender_detection/gender/female.json',
         'persian_gender_detection/gender/male.json',
         'persian_gender_detection/gender/names.csv',
     ])],
```

### Comparing `persian-gender-detection-1.0.2/test/test_clean_name.py` & `persian-gender-detection-1.0.4/test/test_clean_name.py`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.2/test/test_get_gender.py` & `persian-gender-detection-1.0.4/test/test_get_gender.py`

 * *Files identical despite different names*

