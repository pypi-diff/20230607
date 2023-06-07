# Comparing `tmp/gaitmap_mad-2.1.1a0.tar.gz` & `tmp/gaitmap_mad-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap_mad-2.1.1a0.tar", max compression
+gzip compressed data, was "gaitmap_mad-2.2.0.tar", max compression
```

## Comparing `gaitmap_mad-2.1.1a0.tar` & `gaitmap_mad-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      734 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/LICENSE
--rw-r--r--   0        0        0      597 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/README.md
--rw-r--r--   0        0        0      483 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/__init__.py
--rw-r--r--   0        0        0      441 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/event_detection/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
--rw-r--r--   0        0        0    14317 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/event_detection/_rampp_event_detection.py
--rw-r--r--   0        0        0      340 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/gait_detection/__init__.py
--rw-r--r--   0        0        0    24779 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
--rw-r--r--   0        0        0      117 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/preprocessing/__init__.py
--rw-r--r--   0        0        0      234 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0    12666 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
--rw-r--r--   0        0        0     1114 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/__init__.py
--rw-r--r--   0        0        0      813 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/__init__.py
--rw-r--r--   0        0        0    15170 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
--rw-r--r--   0        0        0    36773 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
--rw-r--r--   0        0        0     8568 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
--rw-r--r--   0        0        0      436 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
--rw-r--r--   0        0        0     7513 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
--rw-r--r--   0        0        0    15956 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
--rw-r--r--   0        0        0     3589 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
--rw-r--r--   0        0        0     1182 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/__init__.py
--rw-r--r--   0        0        0    10922 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
--rw-r--r--   0        0        0    12026 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
--rw-r--r--   0        0        0        0 2023-06-07 09:47:01.393997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
--rw-r--r--   0        0        0   397824 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
--rw-r--r--   0        0        0    27197 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
--rw-r--r--   0        0        0    19087 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
--rw-r--r--   0        0        0    26902 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_utils.py
--rw-r--r--   0        0        0      265 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0      263 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     9877 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
--rw-r--r--   0        0        0      591 2023-06-07 09:47:01.397997 gaitmap_mad-2.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 gaitmap_mad-2.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/LICENSE
+-rw-r--r--   0        0        0      597 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/README.md
+-rw-r--r--   0        0        0      481 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/__init__.py
+-rw-r--r--   0        0        0      441 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/event_detection/__init__.py
+-rw-r--r--   0        0        0     6013 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
+-rw-r--r--   0        0        0    14317 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_rampp_event_detection.py
+-rw-r--r--   0        0        0      340 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/gait_detection/__init__.py
+-rw-r--r--   0        0        0    24779 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
+-rw-r--r--   0        0        0      117 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0    12666 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
+-rw-r--r--   0        0        0     1114 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/__init__.py
+-rw-r--r--   0        0        0    15170 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
+-rw-r--r--   0        0        0    36773 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
+-rw-r--r--   0        0        0     8568 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
+-rw-r--r--   0        0        0      436 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
+-rw-r--r--   0        0        0     7513 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
+-rw-r--r--   0        0        0    15956 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
+-rw-r--r--   0        0        0     3589 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
+-rw-r--r--   0        0        0     1182 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/__init__.py
+-rw-r--r--   0        0        0    10922 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
+-rw-r--r--   0        0        0    12026 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
+-rw-r--r--   0        0        0   397824 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
+-rw-r--r--   0        0        0    27197 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
+-rw-r--r--   0        0        0    19087 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
+-rw-r--r--   0        0        0    26902 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_utils.py
+-rw-r--r--   0        0        0      265 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     9877 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
+-rw-r--r--   0        0        0      589 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 gaitmap_mad-2.2.0/PKG-INFO
```

### Comparing `gaitmap_mad-2.1.1a0/LICENSE` & `gaitmap_mad-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/README.md` & `gaitmap_mad-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py` & `gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/event_detection/_rampp_event_detection.py` & `gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py` & `gaitmap_mad-2.2.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py` & `gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/__init__.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/__init__.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/__init__.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/stride_segmentation/hmm/_utils.py` & `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py` & `gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.1.1a0/pyproject.toml` & `gaitmap_mad-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap_mad"
-version = "2.1.1a0"
+version = "2.2.0"
 description = "Specific algorithm implementaions by the mad_lab"
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap_mad-2.1.1a0/PKG-INFO` & `gaitmap_mad-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap-mad
-Version: 2.1.1a0
+Version: 2.2.0
 Summary: Specific algorithm implementaions by the mad_lab
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: AGPL-3.0
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

