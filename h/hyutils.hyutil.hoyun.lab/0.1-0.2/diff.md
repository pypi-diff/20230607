# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.1.tar.gz` & `tmp/hyutils.hyutil.hoyun.lab-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.1.tar", last modified: Wed Jun  7 08:04:33 2023, max compression
+gzip compressed data, was "hyutils.hyutil.hoyun.lab-0.2.tar", last modified: Wed Jun  7 08:44:59 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.1.tar` & `hyutils.hyutil.hoyun.lab-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 08:04:33.421329 hyutils-hyutil-hoyun-lab-0.1/
--rw-rw-rw-   0        0        0       40 2023-06-07 07:35:20.000000 hyutils-hyutil-hoyun-lab-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      596 2023-06-07 08:04:33.420833 hyutils-hyutil-hoyun-lab-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.1/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 08:04:33.421476 hyutils-hyutil-hoyun-lab-0.1/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-06-07 08:04:18.000000 hyutils-hyutil-hoyun-lab-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:04:33.403948 hyutils-hyutil-hoyun-lab-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 08:04:33.414376 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      205 2023-06-07 01:36:26.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0      860 2023-06-07 07:24:26.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0      529 2023-06-01 07:38:08.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/xmlutil.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:04:33.419352 hyutils-hyutil-hoyun-lab-0.1/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      596 2023-06-07 08:04:33.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-07 08:04:33.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:04:33.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-07 08:04:33.000000 hyutils-hyutil-hoyun-lab-0.1/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:59.456934 hyutils.hyutil.hoyun.lab-0.2/
+-rw-rw-rw-   0        0        0       40 2023-06-07 07:35:20.000000 hyutils.hyutil.hoyun.lab-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      596 2023-06-07 08:44:59.456436 hyutils.hyutil.hoyun.lab-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils.hyutil.hoyun.lab-0.2/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils.hyutil.hoyun.lab-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 08:44:59.457080 hyutils.hyutil.hoyun.lab-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      848 2023-06-07 08:44:34.000000 hyutils.hyutil.hoyun.lab-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:59.438558 hyutils.hyutil.hoyun.lab-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:59.450973 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      205 2023-06-07 01:36:26.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0      860 2023-06-07 07:24:26.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0      529 2023-06-01 07:38:08.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/xmlutil.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:59.454947 hyutils.hyutil.hoyun.lab-0.2/src/hyutils.hyutil.hoyun.lab.egg-info/
+-rw-rw-rw-   0        0        0      596 2023-06-07 08:44:59.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutils.hyutil.hoyun.lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-07 08:44:59.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutils.hyutil.hoyun.lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:44:59.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutils.hyutil.hoyun.lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-07 08:44:59.000000 hyutils.hyutil.hoyun.lab-0.2/src/hyutils.hyutil.hoyun.lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.1/PKG-INFO` & `hyutils.hyutil.hoyun.lab-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyutils-hyutil-hoyun-lab
-Version: 0.1
+Name: hyutils.hyutil.hoyun.lab
+Version: 0.2
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.1/setup.py` & `hyutils.hyutil.hoyun.lab-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
-    name="hyutils-hyutil-hoyun-lab",
-    version="0.1",
+    name="hyutils.hyutil.hoyun.lab",
+    version="0.2",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/date_time.py` & `hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/dirjob.py` & `hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/hashing.py` & `hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.1/src/hyutil_hoyun_lab/xmlutil.py` & `hyutils.hyutil.hoyun.lab-0.2/src/hyutil_hoyun_lab/xmlutil.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils.hyutil.hoyun.lab-0.2/src/hyutils.hyutil.hoyun.lab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyutils-hyutil-hoyun-lab
-Version: 0.1
+Name: hyutils.hyutil.hoyun.lab
+Version: 0.2
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

