# Comparing `tmp/cobra_db-0.4.2.tar.gz` & `tmp/cobra_db-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobra_db-0.4.2.tar", max compression
+gzip compressed data, was "cobra_db-0.4.3.tar", max compression
```

## Comparing `cobra_db-0.4.2.tar` & `cobra_db-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0      609 2022-08-25 09:24:06.242378 cobra_db-0.4.2/LICENSE
--rw-r--r--   0        0        0     3540 2023-05-23 08:22:03.656463 cobra_db-0.4.2/README.md
--rw-r--r--   0        0        0     1846 2023-06-05 12:07:47.703589 cobra_db-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      332 2022-08-26 14:33:49.499529 cobra_db-0.4.2/src/cobra_db/__init__.py
--rw-r--r--   0        0        0     2160 2022-08-25 10:25:47.249683 cobra_db-0.4.2/src/cobra_db/dataset_mod.py
--rw-r--r--   0        0        0     4899 2023-06-05 12:04:44.309815 cobra_db-0.4.2/src/cobra_db/deid.py
--rw-r--r--   0        0        0    19064 2023-05-27 06:45:18.858208 cobra_db-0.4.2/src/cobra_db/deid_recipe.txt
--rw-r--r--   0        0        0     2382 2023-02-09 15:28:28.969845 cobra_db-0.4.2/src/cobra_db/deid_recipe_mr.txt
--rw-r--r--   0        0        0     4423 2023-05-23 08:22:03.657525 cobra_db-0.4.2/src/cobra_db/encrypt.py
--rw-r--r--   0        0        0     4603 2022-09-22 19:04:29.847121 cobra_db-0.4.2/src/cobra_db/enums.py
--rw-r--r--   0        0        0     2266 2023-02-16 16:28:15.413447 cobra_db-0.4.2/src/cobra_db/filesystem.py
--rw-r--r--   0        0        0    18282 2023-06-05 12:04:44.310223 cobra_db-0.4.2/src/cobra_db/model.py
--rw-r--r--   0        0        0    19451 2023-05-23 08:22:03.658390 cobra_db-0.4.2/src/cobra_db/mongo_dao.py
--rw-r--r--   0        0        0        0 2022-09-20 13:32:34.744297 cobra_db-0.4.2/src/cobra_db/scripts/__init__.py
--rw-r--r--   0        0        0    10338 2023-06-05 12:04:44.310757 cobra_db-0.4.2/src/cobra_db/scripts/pseudonymize_image_metadata.py
--rw-r--r--   0        0        0    13064 2022-11-15 12:38:50.520888 cobra_db-0.4.2/src/cobra_db/scripts/stage_1_ingest_images.py
--rw-r--r--   0        0        0     2508 2022-09-22 11:58:01.231405 cobra_db-0.4.2/src/cobra_db/scripts/stage_2.py
--rw-r--r--   0        0        0     2397 2022-09-22 11:38:28.493491 cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_patients.py
--rw-r--r--   0        0        0     4709 2022-09-21 16:52:48.434815 cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_series.py
--rw-r--r--   0        0        0     5058 2023-05-23 08:22:03.658713 cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_studies.py
--rw-r--r--   0        0        0     1042 2022-09-20 13:32:34.746137 cobra_db-0.4.2/src/cobra_db/scripts/utils.py
--rw-r--r--   0        0        0      535 2022-08-25 10:25:47.234583 cobra_db-0.4.2/src/cobra_db/types.py
--rw-r--r--   0        0        0     4635 2022-10-20 08:57:54.475224 cobra_db-0.4.2/src/cobra_db/utils.py
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0      609 2023-06-07 16:03:05.471212 cobra_db-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3540 2023-06-07 16:03:05.471212 cobra_db-0.4.3/README.md
+-rw-r--r--   0        0        0     1846 2023-06-07 16:03:41.451392 cobra_db-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      332 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/__init__.py
+-rw-r--r--   0        0        0     2160 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/dataset_mod.py
+-rw-r--r--   0        0        0     4899 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/deid.py
+-rw-r--r--   0        0        0    19064 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/deid_recipe.txt
+-rw-r--r--   0        0        0     2382 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/deid_recipe_mr.txt
+-rw-r--r--   0        0        0     4423 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/encrypt.py
+-rw-r--r--   0        0        0     4603 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/enums.py
+-rw-r--r--   0        0        0     2266 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/filesystem.py
+-rw-r--r--   0        0        0    18248 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/model.py
+-rw-r--r--   0        0        0    19451 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/mongo_dao.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/__init__.py
+-rw-r--r--   0        0        0    10338 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/pseudonymize_image_metadata.py
+-rw-r--r--   0        0        0    13064 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/stage_1_ingest_images.py
+-rw-r--r--   0        0        0     2508 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/stage_2.py
+-rw-r--r--   0        0        0     2397 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/stage_2_group_patients.py
+-rw-r--r--   0        0        0     4709 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/stage_2_group_series.py
+-rw-r--r--   0        0        0     5058 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/stage_2_group_studies.py
+-rw-r--r--   0        0        0     1042 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/scripts/utils.py
+-rw-r--r--   0        0        0      535 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/types.py
+-rw-r--r--   0        0        0     4635 2023-06-07 16:03:05.491212 cobra_db-0.4.3/src/cobra_db/utils.py
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.4.3/PKG-INFO
```

### Comparing `cobra_db-0.4.2/LICENSE` & `cobra_db-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/README.md` & `cobra_db-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/pyproject.toml` & `cobra_db-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cobra_db"
-version = "0.4.2"
+version = "0.4.3"
 description = "COnsolidated BReast cancer Analysis DataBase"
 authors = ["Fernando Cossio", "Apostolia Tsirikoglou", "Haiko Schurz", "Hui Li", "Fredrik Strand"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["src/cobra_db/deid_recipe.txt"]
 
 [tool.poetry.dependencies]
```

### Comparing `cobra_db-0.4.2/src/cobra_db/dataset_mod.py` & `cobra_db-0.4.3/src/cobra_db/dataset_mod.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/deid.py` & `cobra_db-0.4.3/src/cobra_db/deid.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/deid_recipe.txt` & `cobra_db-0.4.3/src/cobra_db/deid_recipe.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/deid_recipe_mr.txt` & `cobra_db-0.4.3/src/cobra_db/deid_recipe_mr.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/encrypt.py` & `cobra_db-0.4.3/src/cobra_db/encrypt.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/enums.py` & `cobra_db-0.4.3/src/cobra_db/enums.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/filesystem.py` & `cobra_db-0.4.3/src/cobra_db/filesystem.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/model.py` & `cobra_db-0.4.3/src/cobra_db/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from copy import copy
 from dataclasses import dataclass, fields, is_dataclass
 from datetime import datetime, timezone
 from typing import Callable, List, Literal, Tuple, Type, Union
-
+from pathlib import Path
 import numpy as np
 import pydicom
 from bson import ObjectId
 from pydicom.dataset import Dataset
 
 from cobra_db import __version__
 from cobra_db.dataset_mod import DatasetMod
@@ -215,18 +215,18 @@
     def from_mount_paths(cls, filepath: str, mount_paths: dict):
         """create an instance from the filepath and the mount_paths.
 
         :param filepath: _description_
         :param mount_paths: _description_
         """
         for drive_name, mount_path in mount_paths.items():
-            rel_path = os.path.relpath(filepath, mount_path)
-            # TODO: this method will raise ValueError in Windows
-            if not rel_path.startswith(".."):  # file in the mount_path
-                return cls(drive_name=drive_name, rel_path=rel_path)
+            path = Path(filepath)
+            mount_path = Path(mount_path)
+            rel_path = str(path.relative_to(mount_path).as_posix())
+            return cls(drive_name=drive_name, rel_path=rel_path)
         raise ValueError(f"{filepath} is not in any of the mount paths: {mount_paths}")
 
 
 @dataclass
 class Patient(Entity):
     """Represents a unique person that has gone through at least one study.
     https://dicom.nema.org/medical/dicom/current/output/chtml/part03/sect_C.2.2.html
```

### Comparing `cobra_db-0.4.2/src/cobra_db/mongo_dao.py` & `cobra_db-0.4.3/src/cobra_db/mongo_dao.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/pseudonymize_image_metadata.py` & `cobra_db-0.4.3/src/cobra_db/scripts/pseudonymize_image_metadata.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/stage_1_ingest_images.py` & `cobra_db-0.4.3/src/cobra_db/scripts/stage_1_ingest_images.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/stage_2.py` & `cobra_db-0.4.3/src/cobra_db/scripts/stage_2.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_patients.py` & `cobra_db-0.4.3/src/cobra_db/scripts/stage_2_group_patients.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_series.py` & `cobra_db-0.4.3/src/cobra_db/scripts/stage_2_group_series.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/stage_2_group_studies.py` & `cobra_db-0.4.3/src/cobra_db/scripts/stage_2_group_studies.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/scripts/utils.py` & `cobra_db-0.4.3/src/cobra_db/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/types.py` & `cobra_db-0.4.3/src/cobra_db/types.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/src/cobra_db/utils.py` & `cobra_db-0.4.3/src/cobra_db/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.4.2/PKG-INFO` & `cobra_db-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-db
-Version: 0.4.2
+Version: 0.4.3
 Summary: COnsolidated BReast cancer Analysis DataBase
 License: Apache-2.0
 Author: Fernando Cossio
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

