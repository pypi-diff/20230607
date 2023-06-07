# Comparing `tmp/xcodex-0.0.5.tar.gz` & `tmp/xcodex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcodex-0.0.5.tar", last modified: Mon May 29 19:54:47 2023, max compression
+gzip compressed data, was "xcodex-0.0.6.tar", last modified: Wed Jun  7 12:34:33 2023, max compression
```

## Comparing `xcodex-0.0.5.tar` & `xcodex-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-29 19:54:14.000000 xcodex-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-29 19:54:47.786617 xcodex-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-29 19:54:14.000000 xcodex-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 19:54:14.000000 xcodex-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:54:47.786617 xcodex-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-29 19:54:14.000000 xcodex-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.782617 xcodex-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/src/Util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/create_dodsrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/create_netrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/download_file_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/generate_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/make_Dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/Util/var_imp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/src/xcodex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/xcodex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-05-29 19:54:14.000000 xcodex-0.0.5/src/xcodex/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 19:54:14.000000 xcodex-0.0.5/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:54:47.786617 xcodex-0.0.5/xcodex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 19:54:47.000000 xcodex-0.0.5/xcodex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:34:33.189962 xcodex-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-07 12:33:58.000000 xcodex-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-07 12:34:33.189962 xcodex-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-07 12:33:58.000000 xcodex-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-07 12:33:58.000000 xcodex-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:34:33.189962 xcodex-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-07 12:33:58.000000 xcodex-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:34:33.185963 xcodex-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:34:33.189962 xcodex-0.0.6/src/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/create_dodsrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/create_netrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/download_file_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/generate_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/make_Dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/Util/var_imp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:34:33.189962 xcodex-0.0.6/src/xcodex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/xcodex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-07 12:33:58.000000 xcodex-0.0.6/src/xcodex/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:34:33.189962 xcodex-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 12:33:58.000000 xcodex-0.0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:34:33.189962 xcodex-0.0.6/xcodex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-07 12:34:33.000000 xcodex-0.0.6/xcodex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 12:34:33.000000 xcodex-0.0.6/xcodex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:34:33.000000 xcodex-0.0.6/xcodex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 12:34:33.000000 xcodex-0.0.6/xcodex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 12:34:33.000000 xcodex-0.0.6/xcodex.egg-info/top_level.txt
```

### Comparing `xcodex-0.0.5/LICENSE` & `xcodex-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/PKG-INFO` & `xcodex-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcodex
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES)
 Author: henriquefl24@git
 Author-email: Henrique Fontellas Laurito <henrique.f.laurito@unesp.br>
 Project-URL: Homepage, https://github.com/henriquefl24/xcodex
 Project-URL: Bug Tracker, https://github.com/henriquefl24/xcodex/issues
 Keywords: python,NASA,GES DISC,XCO2,daily,OCO-2,jupyter notebook,xcodex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xcodex-0.0.5/README.md` & `xcodex-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/pyproject.toml` & `xcodex-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 	"requests~=2.31.0",
 	"setuptools==67.8.0",
 	"jupyter==1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xcodex"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   {name="Henrique Fontellas Laurito", email="henrique.f.laurito@unesp.br" }
 ]
 description = """This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES)
                  Data and Information Services Center (DISC)"
 
               Source citation: Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
```

### Comparing `xcodex-0.0.5/setup.py` & `xcodex-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = """This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES) 
                  Data and Information Services Center (DISC)"
               Source citation: Brad Weir, Lesley Ott and OCO-2 Science Team (2022), OCO-2 GEOS Level 3 daily,
               0.5x0.625 assimilated CO2 V10r, Greenbelt, MD, USA, Goddard Earth Sciences Data
               and Information Services Center (GES DISC), Accessed: 10/31/2022,
               doi: 10.5067/Y9M4NM9MPCGH"""
```

### Comparing `xcodex-0.0.5/src/Util/check.py` & `xcodex-0.0.6/src/Util/check.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/date.py` & `xcodex-0.0.6/src/Util/date.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/download.py` & `xcodex-0.0.6/src/Util/download.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/download_file_progress.py` & `xcodex-0.0.6/src/Util/download_file_progress.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/generate_links.py` & `xcodex-0.0.6/src/Util/generate_links.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/make_Dataframe.py` & `xcodex-0.0.6/src/Util/make_Dataframe.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/missing.py` & `xcodex-0.0.6/src/Util/missing.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/Util/var_imp.py` & `xcodex-0.0.6/src/Util/var_imp.py`

 * *Files identical despite different names*

### Comparing `xcodex-0.0.5/src/xcodex/main.py` & `xcodex-0.0.6/src/xcodex/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         new_subset(dataframe)
 
     # Padronizing values to float
 
     dataframe.set_index('location', inplace=True, drop=True)
     dataframe = dataframe.astype(float)
     dataframe.reset_index(inplace=True, drop=False)
+    dataframe.to_csv("output_xco2_data.csv", sep=";")
 
     return dataframe
 
 
 def download_file(start: str, end: str) -> None:
     """
     This method will effectively download .nc4 files from NASA
```

### Comparing `xcodex-0.0.5/xcodex.egg-info/PKG-INFO` & `xcodex-0.0.6/xcodex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcodex
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package will download and extract daily data of XCO2 from the NASA Goddard Earth Sciences (GES)
 Author: henriquefl24@git
 Author-email: Henrique Fontellas Laurito <henrique.f.laurito@unesp.br>
 Project-URL: Homepage, https://github.com/henriquefl24/xcodex
 Project-URL: Bug Tracker, https://github.com/henriquefl24/xcodex/issues
 Keywords: python,NASA,GES DISC,XCO2,daily,OCO-2,jupyter notebook,xcodex
 Classifier: Development Status :: 4 - Beta
```

