# Comparing `tmp/histoprep-2.0.3.tar.gz` & `tmp/histoprep-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histoprep-2.0.3.tar", max compression
+gzip compressed data, was "histoprep-2.0.4.tar", max compression
```

## Comparing `histoprep-2.0.3.tar` & `histoprep-2.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-04-13 12:39:17.917382 histoprep-2.0.3/LICENSE
--rw-r--r--   0        0        0     4498 2023-04-13 12:39:17.917382 histoprep-2.0.3/README.md
--rw-r--r--   0        0        0      208 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/__init__.py
--rw-r--r--   0        0        0    12824 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/_backend.py
--rw-r--r--   0        0        0    13109 2023-05-03 06:56:36.411842 histoprep-2.0.3/histoprep/_cli.py
--rw-r--r--   0        0        0     2632 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/_data.py
--rw-r--r--   0        0        0    27500 2023-05-03 07:09:28.294664 histoprep-2.0.3/histoprep/_reader.py
--rw-r--r--   0        0        0      907 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_check.py
--rw-r--r--   0        0        0     1297 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_concurrent.py
--rw-r--r--   0        0        0     5400 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_dearray.py
--rw-r--r--   0        0        0     4305 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_draw.py
--rw-r--r--   0        0        0     2641 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_images.py
--rw-r--r--   0        0        0      410 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_level.py
--rw-r--r--   0        0        0     1881 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_mean_std.py
--rw-r--r--   0        0        0     5490 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_metrics.py
--rw-r--r--   0        0        0     5476 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_normalize.py
--rw-r--r--   0        0        0     8211 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_tiles.py
--rw-r--r--   0        0        0     4766 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_tissue.py
--rw-r--r--   0        0        0      421 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/utils/__init__.py
--rw-r--r--   0        0        0     5870 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/utils/_normalize.py
--rw-r--r--   0        0        0    12291 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/utils/_process.py
--rw-r--r--   0        0        0     5436 2023-05-03 07:09:58.615718 histoprep-2.0.3/histoprep/utils/_torch.py
--rw-r--r--   0        0        0      724 2023-04-20 09:43:03.036936 histoprep-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 12:39:17.917382 histoprep-2.0.4/LICENSE
+-rw-r--r--   0        0        0     4498 2023-04-13 12:39:17.917382 histoprep-2.0.4/README.md
+-rw-r--r--   0        0        0      208 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/__init__.py
+-rw-r--r--   0        0        0    12826 2023-06-07 07:19:02.277991 histoprep-2.0.4/histoprep/_backend.py
+-rw-r--r--   0        0        0    13109 2023-05-03 07:35:52.585670 histoprep-2.0.4/histoprep/_cli.py
+-rw-r--r--   0        0        0     2632 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/_data.py
+-rw-r--r--   0        0        0    27500 2023-05-03 07:36:53.711787 histoprep-2.0.4/histoprep/_reader.py
+-rw-r--r--   0        0        0      907 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/functional/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/functional/_check.py
+-rw-r--r--   0        0        0     1297 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/functional/_concurrent.py
+-rw-r--r--   0        0        0     5400 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/functional/_dearray.py
+-rw-r--r--   0        0        0     4305 2023-04-13 12:39:17.921382 histoprep-2.0.4/histoprep/functional/_draw.py
+-rw-r--r--   0        0        0     2641 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_images.py
+-rw-r--r--   0        0        0      410 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_level.py
+-rw-r--r--   0        0        0     1881 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_mean_std.py
+-rw-r--r--   0        0        0     5490 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_metrics.py
+-rw-r--r--   0        0        0     5476 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_normalize.py
+-rw-r--r--   0        0        0     8211 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_tiles.py
+-rw-r--r--   0        0        0     4766 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/functional/_tissue.py
+-rw-r--r--   0        0        0      421 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/utils/__init__.py
+-rw-r--r--   0        0        0     5870 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/utils/_normalize.py
+-rw-r--r--   0        0        0    12291 2023-04-13 12:39:17.925382 histoprep-2.0.4/histoprep/utils/_process.py
+-rw-r--r--   0        0        0     5436 2023-05-03 07:19:44.032056 histoprep-2.0.4/histoprep/utils/_torch.py
+-rw-r--r--   0        0        0      724 2023-06-07 07:20:22.104750 histoprep-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.4/PKG-INFO
```

### Comparing `histoprep-2.0.3/LICENSE` & `histoprep-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/README.md` & `histoprep-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/_backend.py` & `histoprep-2.0.4/histoprep/_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         # Calculate actual downsamples.
         slide_h, slide_w = self.dimensions
         self.__level_downsamples = {}
         for lvl, (level_h, level_w) in self.__level_dimensions.items():
             self.__level_downsamples[lvl] = (slide_h / level_h, slide_w / level_w)
 
     @property
-    def reader(self) -> openslide.OpenSlide:
+    def reader(self) -> "openslide.OpenSlide":
         """OpenSlide instance."""
         return self.__reader
 
     @property
     def data_bounds(self) -> tuple[int, int, int, int]:
         properties = dict(self.__reader.properties)
         x_bound = int(properties.get("openslide.bounds-x", 0))
```

### Comparing `histoprep-2.0.3/histoprep/_cli.py` & `histoprep-2.0.4/histoprep/_cli.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/_data.py` & `histoprep-2.0.4/histoprep/_data.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/_reader.py` & `histoprep-2.0.4/histoprep/_reader.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/__init__.py` & `histoprep-2.0.4/histoprep/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_check.py` & `histoprep-2.0.4/histoprep/functional/_check.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_concurrent.py` & `histoprep-2.0.4/histoprep/functional/_concurrent.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_dearray.py` & `histoprep-2.0.4/histoprep/functional/_dearray.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_draw.py` & `histoprep-2.0.4/histoprep/functional/_draw.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_images.py` & `histoprep-2.0.4/histoprep/functional/_images.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_mean_std.py` & `histoprep-2.0.4/histoprep/functional/_mean_std.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_metrics.py` & `histoprep-2.0.4/histoprep/functional/_metrics.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_normalize.py` & `histoprep-2.0.4/histoprep/functional/_normalize.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_tiles.py` & `histoprep-2.0.4/histoprep/functional/_tiles.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/functional/_tissue.py` & `histoprep-2.0.4/histoprep/functional/_tissue.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/utils/_normalize.py` & `histoprep-2.0.4/histoprep/utils/_normalize.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/utils/_process.py` & `histoprep-2.0.4/histoprep/utils/_process.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/histoprep/utils/_torch.py` & `histoprep-2.0.4/histoprep/utils/_torch.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.3/pyproject.toml` & `histoprep-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "histoprep"
-version = "2.0.3"
+version = "2.0.4"
 description = "Read and process histological slide images with python!"
 authors = ["jopo666 <jopo@birdlover.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 HistoPrep = 'histoprep._cli:cut_slides'
```

### Comparing `histoprep-2.0.3/PKG-INFO` & `histoprep-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histoprep
-Version: 2.0.3
+Version: 2.0.4
 Summary: Read and process histological slide images with python!
 Author: jopo666
 Author-email: jopo@birdlover.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: histoprep Version: 2.0.3 Summary: Read and process
+Metadata-Version: 2.1 Name: histoprep Version: 2.0.4 Summary: Read and process
 histological slide images with python! Author: jopo666 Author-email:
 jopo@birdlover.com Requires-Python: >=3.9,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aicspylibczi (>=3,<4) Requires-Dist: matplotlib
 Requires-Dist: mpire (>=2.6,<3.0) Requires-Dist: numpy Requires-Dist: opencv-
 python-headless (>=4,<5) Requires-Dist: openslide-python (>=1.2,<2.0) Requires-
```

