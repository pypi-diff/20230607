# Comparing `tmp/isikukood-1.0.0.tar.gz` & `tmp/isikukood-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isikukood-1.0.0.tar", last modified: Wed Jun  7 20:34:18 2023, max compression
+gzip compressed data, was "dist/isikukood-1.0.1.tar", last modified: Wed Jun  7 21:12:37 2023, max compression
```

## Comparing `isikukood-1.0.0.tar` & `isikukood-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 20:34:18.000000 isikukood-1.0.0/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2023-05-30 11:16:14.000000 isikukood-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11397 2023-06-07 20:34:18.000000 isikukood-1.0.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    10701 2023-06-07 19:58:20.000000 isikukood-1.0.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood/
--rw-r--r--   0 user      (1000) user      (1000)      482 2023-06-03 15:39:16.000000 isikukood-1.0.0/isikukood/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5606 2023-06-07 08:19:34.000000 isikukood-1.0.0/isikukood/assertions.py
--rw-r--r--   0 user      (1000) user      (1000)      149 2023-05-30 13:24:27.000000 isikukood-1.0.0/isikukood/errors.py
--rw-r--r--   0 user      (1000) user      (1000)     6854 2023-06-07 19:57:01.000000 isikukood-1.0.0/isikukood/functions.py
--rw-r--r--   0 user      (1000) user      (1000)     4102 2023-06-07 18:59:17.000000 isikukood-1.0.0/isikukood/isikukood.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11397 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      302 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       12 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-07 20:34:18.000000 isikukood-1.0.0/isikukood.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-07 20:34:18.000000 isikukood-1.0.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1077 2023-06-07 14:55:53.000000 isikukood-1.0.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:12:37.000000 isikukood-1.0.1/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2023-05-30 11:16:14.000000 isikukood-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11479 2023-06-07 21:12:37.000000 isikukood-1.0.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    10783 2023-06-07 20:58:43.000000 isikukood-1.0.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood/
+-rw-r--r--   0 user      (1000) user      (1000)      482 2023-06-03 15:39:16.000000 isikukood-1.0.1/isikukood/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5606 2023-06-07 08:19:34.000000 isikukood-1.0.1/isikukood/assertions.py
+-rw-r--r--   0 user      (1000) user      (1000)      149 2023-05-30 13:24:27.000000 isikukood-1.0.1/isikukood/errors.py
+-rw-r--r--   0 user      (1000) user      (1000)     6854 2023-06-07 19:57:01.000000 isikukood-1.0.1/isikukood/functions.py
+-rw-r--r--   0 user      (1000) user      (1000)     4107 2023-06-07 20:47:46.000000 isikukood-1.0.1/isikukood/isikukood.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11479 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      302 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       12 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-07 21:12:37.000000 isikukood-1.0.1/isikukood.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-07 21:12:37.000000 isikukood-1.0.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1077 2023-06-07 21:12:01.000000 isikukood-1.0.1/setup.py
```

### Comparing `isikukood-1.0.0/LICENSE` & `isikukood-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.0/PKG-INFO` & `isikukood-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isikukood
-Version: 1.0.0
+Version: 1.0.1
 Summary: Estonian SSN library
 Home-page: https://github.com/ui-1/isikukood
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Isikukood
 
 Small Estonian social security number library (I know they're not really SSNs but I don't have a better English name for them)
 
+# Installation
+
+Simply run the following:
+```bash
+pip install isikukood
+```
+
 # Table of Contents
 
 * [functions](#functions)
   * [ordernumber\_from\_ssn](#functions.ordernumber_from_ssn)
   * [gender\_from\_ssn](#functions.gender_from_ssn)
   * [gender\_marker](#functions.gender_marker)
   * [birthdate\_from\_ssn](#functions.birthdate_from_ssn)
@@ -289,15 +296,15 @@
 ```
 
 Instantiate the class from an already existing SSN.
 
 **Examples**:
 
 ```python
-    >>>isikukood.Isikukood('m', '2000-01-01')
+    >>>isikukood.Isikukood.from_ssn('50001010006')
 ```
   
 
 **Raises**:
 
 - `ValueError` - When the given SSN is invalid.
```

### Comparing `isikukood-1.0.0/README.md` & `isikukood-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Isikukood
 
 Small Estonian social security number library (I know they're not really SSNs but I don't have a better English name for them)
 
+# Installation
+
+Simply run the following:
+```bash
+pip install isikukood
+```
+
 # Table of Contents
 
 * [functions](#functions)
   * [ordernumber\_from\_ssn](#functions.ordernumber_from_ssn)
   * [gender\_from\_ssn](#functions.gender_from_ssn)
   * [gender\_marker](#functions.gender_marker)
   * [birthdate\_from\_ssn](#functions.birthdate_from_ssn)
@@ -269,15 +276,15 @@
 ```
 
 Instantiate the class from an already existing SSN.
 
 **Examples**:
 
 ```python
-    >>>isikukood.Isikukood('m', '2000-01-01')
+    >>>isikukood.Isikukood.from_ssn('50001010006')
 ```
   
 
 **Raises**:
 
 - `ValueError` - When the given SSN is invalid.
```

### Comparing `isikukood-1.0.0/isikukood/assertions.py` & `isikukood-1.0.1/isikukood/assertions.py`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.0/isikukood/functions.py` & `isikukood-1.0.1/isikukood/functions.py`

 * *Files identical despite different names*

### Comparing `isikukood-1.0.0/isikukood/isikukood.py` & `isikukood-1.0.1/isikukood/isikukood.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     @classmethod
     def from_ssn(cls, ssn: str):
         """Instantiate the class from an already existing SSN.
 
         Examples:
         ```python
-            >>>isikukood.Isikukood('m', '2000-01-01')
+            >>>isikukood.Isikukood.from_ssn('50001010006')
         ```
 
         Raises:
             ValueError: When the given SSN is invalid.
         """
 
         try: isikukood.assertions.assert_valid_ssn(ssn)
```

### Comparing `isikukood-1.0.0/isikukood.egg-info/PKG-INFO` & `isikukood-1.0.1/isikukood.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isikukood
-Version: 1.0.0
+Version: 1.0.1
 Summary: Estonian SSN library
 Home-page: https://github.com/ui-1/isikukood
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Isikukood
 
 Small Estonian social security number library (I know they're not really SSNs but I don't have a better English name for them)
 
+# Installation
+
+Simply run the following:
+```bash
+pip install isikukood
+```
+
 # Table of Contents
 
 * [functions](#functions)
   * [ordernumber\_from\_ssn](#functions.ordernumber_from_ssn)
   * [gender\_from\_ssn](#functions.gender_from_ssn)
   * [gender\_marker](#functions.gender_marker)
   * [birthdate\_from\_ssn](#functions.birthdate_from_ssn)
@@ -289,15 +296,15 @@
 ```
 
 Instantiate the class from an already existing SSN.
 
 **Examples**:
 
 ```python
-    >>>isikukood.Isikukood('m', '2000-01-01')
+    >>>isikukood.Isikukood.from_ssn('50001010006')
 ```
   
 
 **Raises**:
 
 - `ValueError` - When the given SSN is invalid.
```

### Comparing `isikukood-1.0.0/setup.py` & `isikukood-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="isikukood",
-    version="1.0.0",
+    version="1.0.1",
     description="Estonian SSN library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ui-1/isikukood",
     author="ui-1",
     author_email="ui-1@posteo.org",
     license="GPLv3",
```

