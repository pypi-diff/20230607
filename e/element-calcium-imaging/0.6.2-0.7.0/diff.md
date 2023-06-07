# Comparing `tmp/element-calcium-imaging-0.6.2.tar.gz` & `tmp/element-calcium-imaging-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.6.2.tar", last modified: Tue May 23 14:13:08 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.7.0.tar", last modified: Wed Jun  7 21:19:40 2023, max compression
```

## Comparing `element-calcium-imaging-0.6.2.tar` & `element-calcium-imaging-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:08.502443 element-calcium-imaging-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-23 14:13:08.502443 element-calcium-imaging-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:08.502443 element-calcium-imaging-0.6.2/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66658 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74194 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:08.502443 element-calcium-imaging-0.6.2/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    26752 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:08.502443 element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-23 14:13:08.000000 element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 14:13:08.000000 element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:13:08.000000 element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 14:13:08.000000 element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 14:13:08.000000 element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:13:08.502443 element-calcium-imaging-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-23 14:13:01.000000 element-calcium-imaging-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:19:40.122112 element-calcium-imaging-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-07 21:19:40.122112 element-calcium-imaging-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:19:40.122112 element-calcium-imaging-0.7.0/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66523 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63721 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:19:40.122112 element-calcium-imaging-0.7.0/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:19:40.122112 element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-07 21:19:40.000000 element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-07 21:19:40.000000 element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:19:40.000000 element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-07 21:19:40.000000 element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 21:19:40.000000 element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:19:40.122112 element-calcium-imaging-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 21:19:37.000000 element-calcium-imaging-0.7.0/setup.py
```

### Comparing `element-calcium-imaging-0.6.2/LICENSE` & `element-calcium-imaging-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/imaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 
 import datajoint as dj
 import numpy as np
 from element_interface.utils import dict_to_uuid, find_full_path, find_root_directory
 
 from . import imaging_report, scan
 from .scan import (
+    get_image_files,
     get_imaging_root_data_dir,
-    get_nd2_files,
-    get_prairieview_files,
     get_processed_root_data_dir,
-    get_scan_box_files,
-    get_scan_image_files,
 )
 
 schema = dj.Schema()
 
 _linking_module = None
 
 
@@ -76,23 +73,22 @@
 
 
 # -------------- Table declarations --------------
 
 
 @schema
 class ProcessingMethod(dj.Lookup):
-    """Method, package, or analysis suite used for processing of calcium imaging data
-        (e.g. Suite2p, CaImAn, etc.).
+    """Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
 
     Attributes:
         processing_method (str): Processing method.
         processing_method_desc (str): Processing method description.
     """
 
-    definition = """# Method for calcium imaging processing
+    definition = """# Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
     processing_method: char(8)
     ---
     processing_method_desc: varchar(1000)  # Processing method description
     """
 
     contents = [
         ("suite2p", "suite2p analysis suite"),
@@ -217,16 +213,16 @@
 @schema
 class ProcessingTask(dj.Manual):
     """A pairing of processing params and scans to be loaded or triggered
 
     This table defines a calcium imaging processing task for a combination of a
     `Scan` and a `ProcessingParamSet` entries, including all the inputs (scan, method,
     method's parameters). The task defined here is then run in the downstream table
-    Processing. This table supports definitions of both loading of pre-generated results
-    and the triggering of new analysis for all supported analysis methods
+    `Processing`. This table supports definitions of both loading of pre-generated results
+    and the triggering of new analysis for all supported analysis methods.
 
     Attributes:
         scan.Scan (foreign key): Primary key from scan.Scan.
         ProcessingParamSet (foreign key): Primary key from ProcessingParamSet.
         processing_output_dir (str): Output directory of the processed scan relative to the root data directory.
         task_mode (str): One of 'load' (load computed analysis results) or 'trigger'
             (trigger computation).
@@ -253,24 +249,22 @@
 
         Returns:
             dir (str): A default output directory for the processed results (processed_output_dir
                 in ProcessingTask) based on the following convention:
                 processed_dir / scan_dir / {processing_method}_{paramset_idx}
                 e.g.: sub4/sess1/scan0/suite2p_0
         """
-        image_locators = {
-            "NIS": get_nd2_files,
-            "ScanImage": get_scan_image_files,
-            "Scanbox": get_scan_box_files,
-            "PrairieView": get_prairieview_files,
-        }
-        image_locator = image_locators[(scan.Scan & key).fetch1("acq_software")]
+        acq_software = (scan.Scan & key).fetch1("acq_software")
+        filetypes = dict(
+            ScanImage="*.tif", Scanbox="*.sbx", NIS="*.nd2", PrairieView="*.tif"
+        )
 
         scan_dir = find_full_path(
-            get_imaging_root_data_dir(), image_locator(key)[0]
+            get_imaging_root_data_dir(),
+            get_image_files(key, filetypes[acq_software])[0],
         ).parent
         root_dir = find_root_directory(get_imaging_root_data_dir(), scan_dir)
 
         method = (
             (ProcessingParamSet & key).fetch1("processing_method").replace(".", "-")
         )
 
@@ -400,15 +394,14 @@
             elif method == "extract":
                 raise NotImplementedError(
                     "To use EXTRACT with this DataJoint Element please set `task_mode=trigger`"
                 )
             else:
                 raise NotImplementedError("Unknown method: {}".format(method))
         elif task_mode == "trigger":
-
             method = (ProcessingParamSet * ProcessingTask & key).fetch1(
                 "processing_method"
             )
 
             image_files = (scan.ScanInfo.ScanFile & key).fetch("file_path")
             image_files = [
                 find_full_path(get_imaging_root_data_dir(), image_file)
```

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/imaging_no_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 
 import datajoint as dj
 import numpy as np
 from element_interface.utils import dict_to_uuid, find_full_path, find_root_directory
 
 from . import imaging_report, scan
 from .scan import (
+    get_image_files,
     get_imaging_root_data_dir,
-    get_nd2_files,
-    get_prairieview_files,
     get_processed_root_data_dir,
-    get_scan_box_files,
-    get_scan_image_files,
 )
 
 schema = dj.Schema()
 
 _linking_module = None
 
 
@@ -76,23 +73,22 @@
 
 
 # -------------- Table declarations --------------
 
 
 @schema
 class ProcessingMethod(dj.Lookup):
-    """Method, package, or analysis suite used for processing of calcium imaging data
-        (e.g. Suite2p, CaImAn, etc.).
+    """Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
 
     Attributes:
         processing_method (str): Processing method.
         processing_method_desc (str): Processing method description.
     """
 
-    definition = """# Method for calcium imaging processing
+    definition = """# Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
     processing_method: char(8)
     ---
     processing_method_desc: varchar(1000)  # Processing method description
     """
 
     contents = [
         ("suite2p", "suite2p analysis suite"),
@@ -253,24 +249,22 @@
 
         Returns:
             dir (str): A default output directory for the processed results (processed_output_dir
                 in ProcessingTask) based on the following convention:
                 processed_dir / scan_dir / {processing_method}_{paramset_idx}
                 e.g.: sub4/sess1/scan0/suite2p_0
         """
-        image_locators = {
-            "NIS": get_nd2_files,
-            "ScanImage": get_scan_image_files,
-            "Scanbox": get_scan_box_files,
-            "PrairieView": get_prairieview_files,
-        }
-        image_locator = image_locators[(scan.Scan & key).fetch1("acq_software")]
+        acq_software = (scan.Scan & key).fetch1("acq_software")
+        filetypes = dict(
+            ScanImage="*.tif", Scanbox="*.sbx", NIS="*.nd2", PrairieView="*.tif"
+        )
 
         scan_dir = find_full_path(
-            get_imaging_root_data_dir(), image_locator(key)[0]
+            get_imaging_root_data_dir(),
+            get_image_files(key, filetypes[acq_software])[0],
         ).parent
         root_dir = find_root_directory(get_imaging_root_data_dir(), scan_dir)
 
         method = (
             (ProcessingParamSet & key).fetch1("processing_method").replace(".", "-")
         )
 
@@ -400,15 +394,14 @@
             elif method == "extract":
                 raise NotImplementedError(
                     "To use EXTRACT with this DataJoint Element please set `task_mode=trigger`"
                 )
             else:
                 raise NotImplementedError("Unknown method: {}".format(method))
         elif task_mode == "trigger":
-
             method = (ProcessingParamSet * ProcessingTask & key).fetch1(
                 "processing_method"
             )
 
             image_files = (scan.ScanInfo.ScanFile & key).fetch("file_path")
             image_files = [
                 find_full_path(get_imaging_root_data_dir(), image_file)
@@ -676,15 +669,15 @@
 
         method, imaging_dataset = get_loader_result(key, ProcessingTask)
 
         field_keys, _ = (scan.ScanInfo.Field & key).fetch(
             "KEY", "field_z", order_by="field_z"
         )
 
-        if method == "suite2p":
+        if method in ["suite2p", "extract"]:
             suite2p_dataset = imaging_dataset
 
             motion_correct_channel = suite2p_dataset.planes[0].alignment_channel
 
             # ---- iterate through all s2p plane outputs ----
             rigid_correction, nonrigid_correction, nonrigid_blocks = {}, {}, {}
             summary_images = []
```

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/imaging_preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 
 import datajoint as dj
 import numpy as np
 from element_interface.utils import dict_to_uuid, find_full_path, find_root_directory
 
 from . import imaging_report, scan
 from .scan import (
+    get_image_files,
     get_imaging_root_data_dir,
-    get_nd2_files,
-    get_prairieview_files,
     get_processed_root_data_dir,
-    get_scan_box_files,
-    get_scan_image_files,
 )
 
 schema = dj.Schema()
 
 _linking_module = None
 
 
@@ -266,17 +263,22 @@
             raise ValueError(f"Unknown task mode: {task_mode}")
 
         self.insert1(key)
 
 
 @schema
 class ProcessingMethod(dj.Lookup):
-    definition = """
-    # Method, package, analysis suite used for processing of calcium imaging
-    # data (e.g. Suite2p, CaImAn, etc.)
+    """Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
+
+    Attributes:
+        processing_method (str): Processing method.
+        processing_method_desc (str): Processing method description.
+    """
+
+    definition = """# Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
     processing_method: char(8)
     ---
     processing_method_desc: varchar(1000)  # Processing method description
     """
 
     contents = [
         ("suite2p", "suite2p analysis suite"),
@@ -401,16 +403,16 @@
 @schema
 class ProcessingTask(dj.Manual):
     """A pairing of processing params and scans to be loaded or triggered
 
     This table defines a calcium imaging processing task for a combination of a
     `Scan` and a `ProcessingParamSet` entries, including all the inputs (scan, method,
     method's parameters). The task defined here is then run in the downstream table
-    Processing. This table supports definitions of both loading of pre-generated results
-    and the triggering of new analysis for all supported analysis methods
+    `Processing`. This table supports definitions of both loading of pre-generated results
+    and the triggering of new analysis for all supported analysis methods.
 
     Attributes:
         Preprocess (foreign key): Primary key from Preprocess.
         ProcessingParamSet (foreign key): Primary key from ProcessingParamSet.
         processing_output_dir (str): Output directory of the processed scan relative to the root data directory.
         task_mode (str): One of 'load' (load computed analysis results) or 'trigger'
             (trigger computation).
@@ -437,24 +439,22 @@
 
         Returns:
             dir (str): A default output directory for the processed results (processed_output_dir
                 in ProcessingTask) based on the following convention:
                 processed_dir / scan_dir / {processing_method}_{paramset_idx}
                 e.g.: sub4/sess1/scan0/suite2p_0
         """
-        image_locators = {
-            "NIS": get_nd2_files,
-            "ScanImage": get_scan_image_files,
-            "Scanbox": get_scan_box_files,
-            "PrairieView": get_prairieview_files,
-        }
-        image_locator = image_locators[(scan.Scan & key).fetch1("acq_software")]
+        acq_software = (scan.Scan & key).fetch1("acq_software")
+        filetypes = dict(
+            ScanImage="*.tif", Scanbox="*.sbx", NIS="*.nd2", PrairieView="*.tif"
+        )
 
         scan_dir = find_full_path(
-            get_imaging_root_data_dir(), image_locator(key)[0]
+            get_imaging_root_data_dir(),
+            get_image_files(key, filetypes[acq_software])[0],
         ).parent
         root_dir = find_root_directory(get_imaging_root_data_dir(), scan_dir)
 
         method = (
             (ProcessingParamSet & key).fetch1("processing_method").replace(".", "-")
         )
 
@@ -584,15 +584,14 @@
             elif method == "extract":
                 raise NotImplementedError(
                     "To use EXTRACT with this DataJoint Element please set `task_mode=trigger`"
                 )
             else:
                 raise NotImplementedError("Unknown method: {}".format(method))
         elif task_mode == "trigger":
-
             method = (ProcessingParamSet * ProcessingTask & key).fetch1(
                 "processing_method"
             )
 
             preprocess_paramsets = (
                 PreprocessParamSteps.Step()
                 & dict(preprocess_param_steps_id=key["preprocess_param_steps_id"])
```

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/imaging_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def activate(
     schema_name: str,
     imaging_schema_name: str,
     *,
     create_schema: bool = True,
-    create_tables: bool = True
+    create_tables: bool = True,
 ):
     """Activate this schema.
 
     Args:
         schema_name (str): Schema name on the database server to activate the
             `imaging_report` schema
         imaging_schema_name (str): Schema name of the activated imaging element for
```

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.7.0/element_calcium_imaging/scan.py`

 * *Files 12% similar despite different names*

```diff
@@ -100,60 +100,24 @@
 
     if hasattr(_linking_module, "get_processed_root_data_dir"):
         return _linking_module.get_processed_root_data_dir()
     else:
         return get_imaging_root_data_dir()[0]
 
 
-def get_scan_image_files(scan_key: dict) -> list:
-    """Retrieve the list of ScanImage files associated with a given Scan.
+def get_image_files(scan_key: dict, file_type: str) -> list:
+    """Retrieve the list of image files associated with a given Scan.
 
     Args:
         scan_key: Primary key of a Scan entry.
 
     Returns:
-        A list of ScanImage files' full file-paths.
+        A list of full file paths.
     """
-    return _linking_module.get_scan_image_files(scan_key)
-
-
-def get_scan_box_files(scan_key: dict) -> list:
-    """Retrieve the list of Scanbox files (*.sbx) associated with a given Scan.
-
-    Args:
-        scan_key: Primary key of a Scan entry.
-
-    Returns:
-        A list of Scanbox files' full file-paths.
-    """
-    return _linking_module.get_scan_box_files(scan_key)
-
-
-def get_nd2_files(scan_key: dict) -> list:
-    """Retrieve the list of Nikon files (*.nd2) associated with a given Scan.
-
-    Args:
-        scan_key: Primary key of a Scan entry.
-
-    Returns:
-        A list of Nikon files' full file-paths.
-    """
-    return _linking_module.get_nd2_files(scan_key)
-
-
-def get_prairieview_files(scan_key: dict) -> list:
-    """Retrieve the list of Bruker PrairieView tif files (*.tif) with a given Scan.
-
-    Args:
-        scan_key: Primary key of a Scan entry.
-
-    Returns:
-        A list of Bruker PrairieView files' full file-paths.
-    """
-    return _linking_module.get_prairieview_files(scan_key)
+    return _linking_module.get_image_files(scan_key, file_type)
 
 
 # ----------------------------- Table declarations ----------------------
 
 
 @schema
 class AcquisitionSoftware(dj.Lookup):
@@ -326,15 +290,15 @@
 
         acq_software = (Scan & key).fetch1("acq_software")
 
         if acq_software == "ScanImage":
             import scanreader
 
             # Read the scan
-            scan_filepaths = get_scan_image_files(key)
+            scan_filepaths = get_image_files(key, "*.tif")
             scan = scanreader.read_scan(scan_filepaths)
 
             # Insert in ScanInfo
             x_zero, y_zero, z_zero = scan.motor_position_at_zero or (None, None, None)
 
             self.insert1(
                 dict(
@@ -402,15 +366,15 @@
                         for plane_idx in range(scan.num_scanning_depths)
                     ]
                 )
         elif acq_software == "Scanbox":
             import sbxreader
 
             # Read the scan
-            scan_filepaths = get_scan_box_files(key)
+            scan_filepaths = get_image_files(key, "*.sbx")
             sbx_meta = sbxreader.sbx_get_metadata(scan_filepaths[0])
             sbx_matinfo = sbxreader.sbx_get_info(scan_filepaths[0])
             is_multiROI = bool(
                 sbx_matinfo.mesoscope.enabled
             )  # currently not handling "multiROI" ingestion
 
             if is_multiROI:
@@ -461,15 +425,15 @@
                         for plane_idx in range(sbx_meta["num_planes"])
                     ]
                 )
         elif acq_software == "NIS":
             import nd2
 
             # Read the scan
-            scan_filepaths = get_nd2_files(key)
+            scan_filepaths = get_image_files(key, "*.nd2")
             nd2_file = nd2.ND2File(scan_filepaths[0])
             is_multiROI = False  # MultiROI to be implemented later
 
             # Frame per second
             try:
                 fps = 1000 / nd2_file.experiment[0].parameters.periods[0].periodDiff.avg
             except:  # noqa: E722
@@ -551,15 +515,15 @@
                         )
                         for plane_idx in range(nd2_file.sizes.get("Z", 1))
                     ]
                 )
         elif acq_software == "PrairieView":
             from element_interface import prairieviewreader
 
-            scan_filepaths = get_prairieview_files(key)
+            scan_filepaths = get_image_files(key, "*.tif")
             PVScan_info = prairieviewreader.get_pv_metadata(scan_filepaths[0])
             self.insert1(
                 dict(
                     key,
                     nfields=PVScan_info["num_fields"],
                     nchannels=PVScan_info["num_channels"],
                     ndepths=PVScan_info["num_planes"],
@@ -647,33 +611,33 @@
             "acq_software", "nchannels"
         )
 
         if acq_software == "ScanImage":
             import scanreader
 
             # Switch from FYXCT to TCYX
-            data = scanreader.read_scan(get_scan_image_files(key))[
+            data = scanreader.read_scan(get_image_files(key, "*.tif"))[
                 key["field_idx"]
             ].transpose(3, 2, 0, 1)
         elif acq_software == "Scanbox":
             from sbxreader import sbx_memmap
 
             # Switch from TFCYX to TCYX
-            data = sbx_memmap(get_scan_box_files(key))[:, key["field_idx"]]
+            data = sbx_memmap(get_image_files(key, "*.sbx"))[:, key["field_idx"]]
         elif acq_software == "NIS":
             import nd2
 
-            nd2_file = nd2.ND2File(get_nd2_files(key)[0])
+            nd2_file = nd2.ND2File(get_image_files(key, "*.nd2")[0])
 
             nd2_dims = {k: i for i, k in enumerate(nd2_file.sizes)}
 
             valid_dimensions = "TZCYX"
             assert set(nd2_dims) <= set(
                 valid_dimensions
-            ), f"Unknown dimensions {set(nd2_dims)-set(valid_dimensions)} in file {get_nd2_files(key)[0]}."
+            ), f"Unknown dimensions {set(nd2_dims)-set(valid_dimensions)} in file {get_image_files(key, '*.nd2')[0]}."
 
             # Sort the dimensions in the order of TZCYX, skipping the missing ones.
             data = nd2_file.asarray().transpose(
                 [nd2_dims[x] for x in valid_dimensions if x in nd2_dims]
             )
 
             # Expand array to include the missing dimensions.
```

### Comparing `element-calcium-imaging-0.6.2/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.7.0/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 element_calcium_imaging/__init__.py
+element_calcium_imaging/analysis.py
 element_calcium_imaging/imaging.py
 element_calcium_imaging/imaging_no_curation.py
 element_calcium_imaging/imaging_preprocess.py
 element_calcium_imaging/imaging_report.py
 element_calcium_imaging/scan.py
 element_calcium_imaging/version.py
 element_calcium_imaging.egg-info/PKG-INFO
```

### Comparing `element-calcium-imaging-0.6.2/setup.py` & `element-calcium-imaging-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 #!/usr/bin/env python
 from os import path
 
 from setuptools import find_packages, setup
 
-pkg_name = next(p for p in find_packages() if "." not in p)
+pkg_name = "element_calcium_imaging"
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), "r") as f:
     long_description = f.read()
 
-with open(path.join(here, "requirements.txt")) as f:
-    requirements = f.read().splitlines()
-
 with open(path.join(here, pkg_name, "version.py")) as f:
     exec(f.read())
 
 setup(
     name=pkg_name.replace("_", "-"),
     version=__version__,  # noqa: F821
-    description="Calcium Imaging DataJoint element",
+    description="Calcium Imaging DataJoint Element",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataJoint",
     author_email="info@datajoint.com",
     license="MIT",
     url=f'https://github.com/datajoint/{pkg_name.replace("_", "-")}',
     keywords="neuroscience calcium-imaging science datajoint",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     scripts=[],
-    install_requires=requirements,
+    install_requires=[
+        "datajoint>=0.13.0",
+        "ipykernel>=6.0.1",
+        "ipywidgets",
+        "plotly",
+    ],
+    extras_require={
+        "elements": [
+            "element-animal>=0.1.5",
+            "element-event>=0.2.0",
+            "element-interface>=0.5.4",
+            "element-lab>=0.3.0",
+            "element-session>=0.1.2",
+        ],
+        "extract": ["matlabengine", "scipy"],
+        "nd2": ["nd2"],
+        "suite2p": ["suite2p[io]>=0.12.1"],
+        "tests": ["pytest", "pytest-cov", "shutils"],
+    },
 )
```

