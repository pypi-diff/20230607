# Comparing `tmp/nrsdk-1.1.1.2.tar.gz` & `tmp/nrsdk-1.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrsdk-1.1.1.2.tar", last modified: Wed Jun  7 06:05:49 2023, max compression
+gzip compressed data, was "nrsdk-1.1.1.3.tar", last modified: Wed Jun  7 06:11:34 2023, max compression
```

## Comparing `nrsdk-1.1.1.2.tar` & `nrsdk-1.1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:05:49.111524 nrsdk-1.1.1.2/
--rw-rw-rw-   0        0        0      199 2023-06-07 06:05:49.111524 nrsdk-1.1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-06-01 05:33:10.000000 nrsdk-1.1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 06:05:49.093591 nrsdk-1.1.1.2/nrsdk.egg-info/
--rw-rw-rw-   0        0        0      199 2023-06-07 06:05:49.000000 nrsdk-1.1.1.2/nrsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-06-07 06:05:49.000000 nrsdk-1.1.1.2/nrsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:05:49.000000 nrsdk-1.1.1.2/nrsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 06:05:49.000000 nrsdk-1.1.1.2/nrsdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-06-07 06:05:49.000000 nrsdk-1.1.1.2/nrsdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 06:05:49.107535 nrsdk-1.1.1.2/qlapi_nrsdk/
--rw-rw-rw-   0        0        0      119 2023-06-01 03:56:43.000000 nrsdk-1.1.1.2/qlapi_nrsdk/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-16 09:18:13.000000 nrsdk-1.1.1.2/qlapi_nrsdk/base.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:05:49.107535 nrsdk-1.1.1.2/qlapi_nrsdk/lib/
--rw-rw-rw-   0        0        0  1810944 2023-06-05 08:20:03.000000 nrsdk-1.1.1.2/qlapi_nrsdk/lib/QLNRSdk.dll
--rw-rw-rw-   0        0        0     1975 2023-06-01 03:59:11.000000 nrsdk-1.1.1.2/qlapi_nrsdk/mcf_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:05:49.110527 nrsdk-1.1.1.2/qlapi_nrsdk/neuro_recorder/
--rw-rw-rw-   0        0        0     3808 2023-06-07 03:26:39.000000 nrsdk-1.1.1.2/qlapi_nrsdk/neuro_recorder/__init__.py
--rw-rw-rw-   0        0        0     5594 2023-06-07 05:25:29.000000 nrsdk-1.1.1.2/qlapi_nrsdk/nrsdk.py
--rw-rw-rw-   0        0        0     1995 2023-06-02 02:35:19.000000 nrsdk-1.1.1.2/qlapi_nrsdk/paradigm.py
--rw-rw-rw-   0        0        0      136 2023-06-01 03:57:57.000000 nrsdk-1.1.1.2/qlapi_nrsdk/rsa.py
--rw-rw-rw-   0        0        0       42 2023-06-07 06:05:49.111524 nrsdk-1.1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      579 2023-06-07 06:05:33.000000 nrsdk-1.1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.985592 nrsdk-1.1.1.3/
+-rw-rw-rw-   0        0        0      199 2023-06-07 06:11:34.985592 nrsdk-1.1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-06-01 05:33:10.000000 nrsdk-1.1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.967638 nrsdk-1.1.1.3/nrsdk/
+-rw-rw-rw-   0        0        0      119 2023-06-01 03:56:43.000000 nrsdk-1.1.1.3/nrsdk/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-16 09:18:13.000000 nrsdk-1.1.1.3/nrsdk/base.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.982601 nrsdk-1.1.1.3/nrsdk/lib/
+-rw-rw-rw-   0        0        0  1810944 2023-06-05 08:20:03.000000 nrsdk-1.1.1.3/nrsdk/lib/QLNRSdk.dll
+-rw-rw-rw-   0        0        0     1975 2023-06-01 03:59:11.000000 nrsdk-1.1.1.3/nrsdk/mcf_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.984596 nrsdk-1.1.1.3/nrsdk/neuro_recorder/
+-rw-rw-rw-   0        0        0     3808 2023-06-07 03:26:39.000000 nrsdk-1.1.1.3/nrsdk/neuro_recorder/__init__.py
+-rw-rw-rw-   0        0        0     5594 2023-06-07 05:25:29.000000 nrsdk-1.1.1.3/nrsdk/nrsdk.py
+-rw-rw-rw-   0        0        0     1995 2023-06-02 02:35:19.000000 nrsdk-1.1.1.3/nrsdk/paradigm.py
+-rw-rw-rw-   0        0        0      136 2023-06-01 03:57:57.000000 nrsdk-1.1.1.3/nrsdk/rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.981603 nrsdk-1.1.1.3/nrsdk.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-07 06:05:49.000000 nrsdk-1.1.1.3/nrsdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:11:34.985592 nrsdk-1.1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-06-07 06:11:20.000000 nrsdk-1.1.1.3/setup.py
```

### Comparing `nrsdk-1.1.1.2/README.md` & `nrsdk-1.1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/qlapi_nrsdk/base.py` & `nrsdk-1.1.1.3/nrsdk/base.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/qlapi_nrsdk/lib/QLNRSdk.dll` & `nrsdk-1.1.1.3/nrsdk/lib/QLNRSdk.dll`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/qlapi_nrsdk/mcf_reader.py` & `nrsdk-1.1.1.3/nrsdk/mcf_reader.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/qlapi_nrsdk/neuro_recorder/__init__.py` & `nrsdk-1.1.1.3/nrsdk/neuro_recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/qlapi_nrsdk/nrsdk.py` & `nrsdk-1.1.1.3/nrsdk/nrsdk.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/qlapi_nrsdk/paradigm.py` & `nrsdk-1.1.1.3/nrsdk/paradigm.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.2/setup.py` & `nrsdk-1.1.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '1.1.1.2'
+VERSION = '1.1.1.3'
 AUTHOR='eegion'
 EMAIL='hehuajun@eegion.com'
 REQUIRED = [
     'beautifulsoup',
     "lxml"
 ]
 
@@ -14,12 +14,12 @@
     version=VERSION,  # package version
     author=AUTHOR,
     author_email=EMAIL,
     requires=REQUIRED,
     description='Api for use quanlan device, since v1.1.1.2',  # package description
     packages=find_packages(),
     package_data={
-        "qlapi_nrsdk": ["lib/*.dll"],
+        "nrsdk": ["lib/*.dll"],
         "":["*.txt", "*.md"]
     },
     zip_safe=False,
 )
```

