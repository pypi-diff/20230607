# Comparing `tmp/zensvi-0.5.0.tar.gz` & `tmp/zensvi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.5.0.tar", max compression
+gzip compressed data, was "zensvi-0.5.1.tar", max compression
```

## Comparing `zensvi-0.5.0.tar` & `zensvi-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.5.0/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.5.0/README.md
--rwxr-xr-x   0        0        0      713 2023-06-05 08:56:03.272061 zensvi-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.5.0/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.5.0/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.5.0/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39841 2023-06-05 07:31:29.453652 zensvi-0.5.0/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.5.0/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.344850 zensvi-0.5.0/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.5.0/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.5.0/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.345206 zensvi-0.5.0/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.345880 zensvi-0.5.0/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.5.0/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.346254 zensvi-0.5.0/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.5.0/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.5.0/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.5.0/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.5.0/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 zensvi-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.5.1/README.md
+-rwxr-xr-x   0        0        0      712 2023-06-07 07:54:52.881620 zensvi-0.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.5.1/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.5.1/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.5.1/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39841 2023-06-05 07:31:29.453652 zensvi-0.5.1/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.5.1/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.5.1/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.5.1/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.5.1/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.5.1/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.5.1/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.5.1/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.5.1/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 zensvi-0.5.1/PKG-INFO
```

### Comparing `zensvi-0.5.0/LICENSE` & `zensvi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/README.md` & `zensvi-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/pyproject.toml` & `zensvi-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.5.0"
+version = "0.5.1"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -17,15 +17,15 @@
 pandas = "^1.3.3"
 requests = "^2.25.1"
 setuptools = "^64.0.3"
 Shapely=">=1.8.1"
 torch = "^2.0.0"
 tqdm = "^4.0.0"
 transformers = "^4.10.2"
-scipy = "^1.7.1"
+scipy = "1.7.3"
 networkx="^3.1"
 mapillary="^1.0.11"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `zensvi-0.5.0/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.5.1/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/streetview_downloader.py` & `zensvi-0.5.1/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.5.1/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.5.1/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/utils/get_pids.py` & `zensvi-0.5.1/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/utils/helpers.py` & `zensvi-0.5.1/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/utils/imtool.py` & `zensvi-0.5.1/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/download/utils/proxies.csv` & `zensvi-0.5.1/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/src/zensvi/transform/transform_image.py` & `zensvi-0.5.1/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.0/PKG-INFO` & `zensvi-0.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.5.0
+Version: 0.5.1
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Requires-Dist: mapillary (>=1.0.11,<2.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.21.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: scipy (>=1.7.1,<2.0.0)
+Requires-Dist: scipy (==1.7.3)
 Requires-Dist: setuptools (>=64.0.3,<65.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Requires-Dist: transformers (>=4.10.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # ZenSVI
```

