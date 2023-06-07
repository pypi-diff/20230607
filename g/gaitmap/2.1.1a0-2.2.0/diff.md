# Comparing `tmp/gaitmap-2.1.1a0.tar.gz` & `tmp/gaitmap-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap-2.1.1a0.tar", max compression
+gzip compressed data, was "gaitmap-2.2.0.tar", max compression
```

## Comparing `gaitmap-2.1.1a0.tar` & `gaitmap-2.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2032 2023-06-07 09:44:53.550473 gaitmap-2.1.1a0/LICENSE
--rw-r--r--   0        0        0     8141 2023-06-07 09:44:53.550473 gaitmap-2.1.1a0/README.md
--rw-r--r--   0        0        0       71 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/_event_detection_common/__init__.py
--rw-r--r--   0        0        0     7213 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/_event_detection_common/_event_detection_mixin.py
--rw-r--r--   0        0        0    12216 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/base.py
--rw-r--r--   0        0        0     1316 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/data_transform/__init__.py
--rw-r--r--   0        0        0    15931 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/data_transform/_base.py
--rw-r--r--   0        0        0    12004 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/data_transform/_feature_transform.py
--rw-r--r--   0        0        0     3969 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/data_transform/_filter.py
--rw-r--r--   0        0        0    15524 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/data_transform/_scaler.py
--rw-r--r--   0        0        0      765 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/evaluation_utils/__init__.py
--rw-r--r--   0        0        0     6326 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/evaluation_utils/event_detection.py
--rw-r--r--   0        0        0    28925 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/evaluation_utils/parameter_errors.py
--rw-r--r--   0        0        0    11515 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/evaluation_utils/scores.py
--rw-r--r--   0        0        0    22255 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/evaluation_utils/stride_segmentation.py
--rw-r--r--   0        0        0      702 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/event_detection/__init__.py
--rw-r--r--   0        0        0    19385 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/event_detection/_herzer_event_detection.py
--rw-r--r--   0        0        0     6781 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/example_data.py
--rw-r--r--   0        0        0      542 2023-06-07 09:44:53.614473 gaitmap-2.1.1a0/gaitmap/gait_detection/__init__.py
--rw-r--r--   0        0        0      350 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/parameters/__init__.py
--rw-r--r--   0        0        0    21721 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/parameters/_spatial_parameters.py
--rw-r--r--   0        0        0     7432 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/parameters/_temporal_parameters.py
--rw-r--r--   0        0        0      287 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/preprocessing/__init__.py
--rw-r--r--   0        0        0      785 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0     5094 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
--rw-r--r--   0        0        0     3940 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
--rw-r--r--   0        0        0     6322 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
--rw-r--r--   0        0        0     1732 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/stride_segmentation/__init__.py
--rw-r--r--   0        0        0    14875 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
--rw-r--r--   0        0        0     2713 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/stride_segmentation/_utils.py
--rw-r--r--   0        0        0     1181 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/stride_segmentation/hmm.py
--rw-r--r--   0        0        0     1029 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0    21419 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
--rw-r--r--   0        0        0     9438 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
--rw-r--r--   0        0        0    10746 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
--rw-r--r--   0        0        0      317 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
--rw-r--r--   0        0        0     8096 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
--rw-r--r--   0        0        0     4858 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
--rw-r--r--   0        0        0      618 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     7458 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
--rw-r--r--   0        0        0      243 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
--rw-r--r--   0        0        0    13664 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
--rw-r--r--   0        0        0    16637 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
--rw-r--r--   0        0        0       41 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/__init__.py
--rw-r--r--   0        0        0     1857 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/_algo_helper.py
--rw-r--r--   0        0        0     4695 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0     1020 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/_gaitmap_mad.py
--rw-r--r--   0        0        0      381 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/_types.py
--rw-r--r--   0        0        0    17992 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/array_handling.py
--rw-r--r--   0        0        0     2555 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/consts.py
--rw-r--r--   0        0        0     6284 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/coordinate_conversion.py
--rw-r--r--   0        0        0    48845 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/datatype_helper.py
--rw-r--r--   0        0        0     1089 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/exceptions.py
--rw-r--r--   0        0        0     1865 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/fast_quaternion_math.py
--rw-r--r--   0        0        0    18908 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/rotations.py
--rw-r--r--   0        0        0     2372 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/signal_processing.py
--rw-r--r--   0        0        0    14377 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/static_moment_detection.py
--rw-r--r--   0        0        0     8512 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/stride_list_conversion.py
--rw-r--r--   0        0        0     4115 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/utils/vector_math.py
--rw-r--r--   0        0        0      670 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/zupt_detection/__init__.py
--rw-r--r--   0        0        0     1582 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/zupt_detection/_base.py
--rw-r--r--   0        0        0     3068 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/zupt_detection/_combo_zupt_detector.py
--rw-r--r--   0        0        0    21964 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
--rw-r--r--   0        0        0     4897 2023-06-07 09:44:53.618473 gaitmap-2.1.1a0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
--rw-r--r--   0        0        0     5177 2023-06-07 09:44:53.626474 gaitmap-2.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     9476 1970-01-01 00:00:00.000000 gaitmap-2.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2032 2023-06-07 10:17:53.763523 gaitmap-2.2.0/LICENSE
+-rw-r--r--   0        0        0     8913 2023-06-07 10:17:53.763523 gaitmap-2.2.0/README.md
+-rw-r--r--   0        0        0       69 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/_event_detection_common/__init__.py
+-rw-r--r--   0        0        0     7213 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/_event_detection_common/_event_detection_mixin.py
+-rw-r--r--   0        0        0    12216 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/base.py
+-rw-r--r--   0        0        0     1316 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/__init__.py
+-rw-r--r--   0        0        0    15931 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_base.py
+-rw-r--r--   0        0        0    12004 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_feature_transform.py
+-rw-r--r--   0        0        0     3969 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_filter.py
+-rw-r--r--   0        0        0    15524 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_scaler.py
+-rw-r--r--   0        0        0      765 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/__init__.py
+-rw-r--r--   0        0        0     6326 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/event_detection.py
+-rw-r--r--   0        0        0    28925 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/parameter_errors.py
+-rw-r--r--   0        0        0    11515 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/scores.py
+-rw-r--r--   0        0        0    22255 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/stride_segmentation.py
+-rw-r--r--   0        0        0      702 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/event_detection/__init__.py
+-rw-r--r--   0        0        0    19385 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/event_detection/_herzer_event_detection.py
+-rw-r--r--   0        0        0     6735 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/example_data.py
+-rw-r--r--   0        0        0      542 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/gait_detection/__init__.py
+-rw-r--r--   0        0        0      350 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/parameters/__init__.py
+-rw-r--r--   0        0        0    21721 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/parameters/_spatial_parameters.py
+-rw-r--r--   0        0        0     7432 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/parameters/_temporal_parameters.py
+-rw-r--r--   0        0        0      287 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/__init__.py
+-rw-r--r--   0        0        0      785 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0     5094 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
+-rw-r--r--   0        0        0     3940 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
+-rw-r--r--   0        0        0     6322 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
+-rw-r--r--   0        0        0     1732 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0    14875 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
+-rw-r--r--   0        0        0     2713 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/stride_segmentation/_utils.py
+-rw-r--r--   0        0        0     1181 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/stride_segmentation/hmm.py
+-rw-r--r--   0        0        0     1029 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0    21419 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
+-rw-r--r--   0        0        0     9438 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
+-rw-r--r--   0        0        0    10746 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
+-rw-r--r--   0        0        0      317 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
+-rw-r--r--   0        0        0     8096 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
+-rw-r--r--   0        0        0     4858 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
+-rw-r--r--   0        0        0      618 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     7458 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
+-rw-r--r--   0        0        0      243 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
+-rw-r--r--   0        0        0    13664 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
+-rw-r--r--   0        0        0    16637 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
+-rw-r--r--   0        0        0       41 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/__init__.py
+-rw-r--r--   0        0        0     1857 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_algo_helper.py
+-rw-r--r--   0        0        0     4695 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0     1020 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_gaitmap_mad.py
+-rw-r--r--   0        0        0      381 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_types.py
+-rw-r--r--   0        0        0    17992 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/array_handling.py
+-rw-r--r--   0        0        0     2555 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/consts.py
+-rw-r--r--   0        0        0     6284 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/coordinate_conversion.py
+-rw-r--r--   0        0        0    48845 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/datatype_helper.py
+-rw-r--r--   0        0        0     1089 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/exceptions.py
+-rw-r--r--   0        0        0     1865 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/fast_quaternion_math.py
+-rw-r--r--   0        0        0    18908 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/rotations.py
+-rw-r--r--   0        0        0     2372 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/signal_processing.py
+-rw-r--r--   0        0        0    14377 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/static_moment_detection.py
+-rw-r--r--   0        0        0     8512 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/stride_list_conversion.py
+-rw-r--r--   0        0        0     4115 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/vector_math.py
+-rw-r--r--   0        0        0      670 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/__init__.py
+-rw-r--r--   0        0        0     1582 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_base.py
+-rw-r--r--   0        0        0     3068 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_combo_zupt_detector.py
+-rw-r--r--   0        0        0    21964 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
+-rw-r--r--   0        0        0     4897 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
+-rw-r--r--   0        0        0     5175 2023-06-07 10:17:53.851529 gaitmap-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10246 1970-01-01 00:00:00.000000 gaitmap-2.2.0/PKG-INFO
```

### Comparing `gaitmap-2.1.1a0/LICENSE` & `gaitmap-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/README.md` & `gaitmap-2.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 <img src="./docs/_static/logo/gaitmap_logo_with_text.png" height="200">
 
+[![PyPI](https://img.shields.io/pypi/v/gaitmap)](https://pypi.org/project/gaitmap/)
 [![pipeline status](https://github.com/mad-lab-fau/gaitmap/workflows/Test%20and%20Lint/badge.svg)](https://github.com/mad-lab-fau/gaitmap/actions/workflows/test-and-lint.yml)
-[![codecov](https://codecov.io/gh/mad-lab-fau/gaitmap/branch/master/graph/badge.svg?token=5NP5ZZ3KGX)](https://codecov.io/gh/mad-lab-fau/gaitmap)[![docs](https://img.shields.io/badge/docs-online-green.svg)](http://MadLab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/README.html)
+[![codecov](https://codecov.io/gh/mad-lab-fau/gaitmap/branch/master/graph/badge.svg?token=5NP5ZZ3KGX)](https://codecov.io/gh/mad-lab-fau/gaitmap)
+[![Documentation Status](https://readthedocs.org/projects/gaitmap/badge/?version=latest)](https://gaitmap.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/gaitmap)
 
 # gaitmap - The Gait and Movement Analysis Package
 
 *gaitmap* provides a set of algorithms to analyze your IMU movement data (with a focus on foot-worn IMUs) without 
 getting into your way.
 
-- 💻 20+ Algorithms from 17+ publications
-- 📚 Extensive documentation
-- 📝 Build to be easily extensible
+- 💻 [20+ Algorithms](https://gaitmap.readthedocs.io/en/latest/modules/index.html) from 17+ publications
+- 📚 Extensive [documentation](https://gaitmap.readthedocs.io/en/latest/)
+- 📝 Build to be [easily extensible](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
 - ⚙️ Familiar API inspired by scikit-learn
 - 🤝 Interoperable with the other libraries from the gaitmap ecosystem ([gaitmap-dataset](https://github.com/mad-lab-fau/gaitmap-datasets), [tpcp](https://github.com/mad-lab-fau/tpcp), ...)
 
-**Documentation:** TODO: Website Link<br>
+**Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/)<br>
 **Learn More about the gaitmap ecosystem:** TODO: Website Link
 
 ## Installation
 
-Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](TODO: Link to gaitmap_mad docu page).
+Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html).
 To get access to all available algorithms, you need to install both packages.
 
 ```
 pip install gaitmap gaitmap_mad --upgrade
 ```
 
 Both packages are always released together and have the same version number.
@@ -40,15 +43,15 @@
 ### Enabling specific features
 
 #### Hidden Markov Models
 
 To use the HMM (anything imported from `gaitmap.stride_segmentation.hmm`) based algorithms make sure you install `gaitmap` with the `hmm` extra.
 
 ```
-pip install "gaitmap_mad gaitmap[hmm]" --upgrade
+pip install gaitmap_mad "gaitmap[hmm]" --upgrade
 ```
 This installs the `pomegranate` package, which is the basis for the HMM implementation.
 Note, that we only support the `pomegranate` version `>=0.14.2,<=0.14.6` and that `pomegrante` is not compatible with 
 Python 3.10.
 
 We are working on upgrading to a newer version of `pomegranate`, but this is not a priority at the moment.
 You can track the progress in the [pull request](https://github.com/mad-lab-fau/gaitmap/pull/20).
@@ -62,17 +65,17 @@
 ## Working with Algorithms
 
 *gaitmap* is designed to be a toolbox and not a single algorithm.
 This means, that you are expected to pick and use individual algorithms.
 
 To get started with *gaitmap* we recommend to follow these steps:
 
-1. Understand the common datatypes we use: [Common Datatypes](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/user_guide/datatypes.html)
-2. Understand how to prepare your data: [Coordinate Systems](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/user_guide/coordinate_systems.html)
-3. Check the API docs and examples for available algorithms: [API Docs](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/autoapi/gaitmap/index.html)
+1. Understand the common datatypes we use: [Common Datatypes](https://gaitmap.readthedocs.io/en/latest/source/user_guide/datatypes.html), [Coordinate Systems](https://gaitmap.readthedocs.io/en/latest/source/user_guide/coordinate_systems.html)
+2. Learn how to prepare your own data (or play around with example data): TODO 
+3. Check the API docs and examples for available algorithms: [API Docs](https://gaitmap.readthedocs.io/en/latest/modules/index.html), [Examples](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
 
 Each algorithm is implemented as a class, which is initialized with the required parameters.
 In many cases the default parameters are sufficient, but to get the best results on your data, you should adapt them.
 
 ```python
 from gaitmap.stride_segmentation import BarthDtw
 
@@ -94,17 +97,17 @@
 
 Most algorithms have additional results available to provide further information.
 
 ```python
 dtw_warping_path = stride_segmenter.paths_
 ```
 
-To build a full gait analysis pipeline you can combine multiple algorithms ([Example]()).
-You can even substitute your own algorithms ([Guide]()) or use the provided tooling to validate
-and optimize your algorithms ([Guide]()).
+To build a full gait analysis pipeline you can combine multiple algorithms ([Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/full_pipelines/mad_gait_pipeline.html#sphx-glr-auto-examples-full-pipelines-mad-gait-pipeline-py)).
+You can even substitute your own algorithms ([Guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)) or use the provided tooling to validate
+and optimize your algorithms using tpcp ([General Guide](https://tpcp.readthedocs.io/en/latest/guides/index.html#optimization-and-validation), [Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/datasets_and_pipelines/gridsearch.html#sphx-glr-auto-examples-datasets-and-pipelines-gridsearch-py)).
 
 ## Citation
 
 If you use *gaitmap* in your research we would appreciate a citation.
 This helps us to justify the time we invest in the development and maintenance of the library.
 
 We currently prepare a paper to describe the *gaitmap* library in detail.
@@ -130,18 +133,15 @@
 Please, check the [AGPL-3.0 license](https://www.gnu.org/licenses/agpl-3.0.en.html) for more details and make sure
 you understand the implications.
 
 If you need to use *gaitmap_mad* in a closed source project, please contact us for a potential commercial license.
 
 ## For Developers
 
-The [Development Guide](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/development/development_guide.html)
-and the
-[Project Structure Guide](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/development/project_structure.html)
-have detailed information for all new developers.
+The [Development Guides](https://gaitmap.readthedocs.io/en/latest/source/development/index.html#development) have detailed information for all new developers.
 
 Here some quick references
 Install Python >=3.8 and [poetry](https://python-poetry.org).
 Then run the commands below to get the latest source and install the dependencies:
 
 ```bash
 git clone https://github.com/mad-lab-fau/gaitmap.git
```

### Comparing `gaitmap-2.1.1a0/gaitmap/_event_detection_common/_event_detection_mixin.py` & `gaitmap-2.2.0/gaitmap/_event_detection_common/_event_detection_mixin.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/base.py` & `gaitmap-2.2.0/gaitmap/base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/data_transform/__init__.py` & `gaitmap-2.2.0/gaitmap/data_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/data_transform/_base.py` & `gaitmap-2.2.0/gaitmap/data_transform/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/data_transform/_feature_transform.py` & `gaitmap-2.2.0/gaitmap/data_transform/_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/data_transform/_filter.py` & `gaitmap-2.2.0/gaitmap/data_transform/_filter.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/data_transform/_scaler.py` & `gaitmap-2.2.0/gaitmap/data_transform/_scaler.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/evaluation_utils/__init__.py` & `gaitmap-2.2.0/gaitmap/evaluation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/evaluation_utils/event_detection.py` & `gaitmap-2.2.0/gaitmap/evaluation_utils/event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/evaluation_utils/parameter_errors.py` & `gaitmap-2.2.0/gaitmap/evaluation_utils/parameter_errors.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/evaluation_utils/scores.py` & `gaitmap-2.2.0/gaitmap/evaluation_utils/scores.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/evaluation_utils/stride_segmentation.py` & `gaitmap-2.2.0/gaitmap/evaluation_utils/stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/event_detection/__init__.py` & `gaitmap-2.2.0/gaitmap/event_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/event_detection/_herzer_event_detection.py` & `gaitmap-2.2.0/gaitmap/event_detection/_herzer_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/example_data.py` & `gaitmap-2.2.0/gaitmap/example_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 
 from pathlib import Path
 
 import pandas as pd
 
 LOCAL_EXAMPLE_PATH = Path(__file__).parent.parent / "example_data/"
 PC_EXAMPLE_PATH = Path.home() / ".gaitmap_data/"
-GITLAB_FOLDER_PATH = (
-    "https://mad-srv.informatik.uni-erlangen.de/MadLab/GaitAnalysis/gaitmap/-/raw/master/example_data/{}?inline=false"
+GITHUB_FOLDER_PATH = (
+    "https://github.com/mad-lab-fau/gaitmap/tree/master/example_data/{}"
 )
 
 
 def _is_manual_installed() -> bool:
     return (LOCAL_EXAMPLE_PATH / "__init__.py").is_file()
 
 
 def _get_data(filename: str) -> str:
     if _is_manual_installed():
         return str(LOCAL_EXAMPLE_PATH / filename)
     if (PC_EXAMPLE_PATH / filename).is_file():
         return str(PC_EXAMPLE_PATH / filename)
-    gitlab_path = GITLAB_FOLDER_PATH.format(filename)
+    github_path = GITHUB_FOLDER_PATH.format(filename)
     raise ValueError(
-        "The gaitlab Python package does not contain the example data to save space. "
+        "The gaitmap Python package does not contain the example data to save space. "
         'Please dowload the example folder manually from "{}" and place its content in the folder "{}". '
         'If the folder does not exist create it. Note the "." in front of the folder name.'.format(
-            gitlab_path, PC_EXAMPLE_PATH
+            github_path, PC_EXAMPLE_PATH
         )
     )
 
 
 def get_healthy_example_imu_data():
     """Get example IMU data from a healthy subject doing a 2x20m gait test.
```

### Comparing `gaitmap-2.1.1a0/gaitmap/gait_detection/__init__.py` & `gaitmap-2.2.0/gaitmap/gait_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/parameters/_spatial_parameters.py` & `gaitmap-2.2.0/gaitmap/parameters/_spatial_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/parameters/_temporal_parameters.py` & `gaitmap-2.2.0/gaitmap/parameters/_temporal_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/__init__.py` & `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py` & `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py` & `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py` & `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/stride_segmentation/__init__.py` & `gaitmap-2.2.0/gaitmap/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/stride_segmentation/_roi_stride_segmentation.py` & `gaitmap-2.2.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/stride_segmentation/_utils.py` & `gaitmap-2.2.0/gaitmap/stride_segmentation/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/stride_segmentation/hmm.py` & `gaitmap-2.2.0/gaitmap/stride_segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/__init__.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/position_methods/__init__.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py` & `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/_algo_helper.py` & `gaitmap-2.2.0/gaitmap/utils/_algo_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/_datatype_validation_helper.py` & `gaitmap-2.2.0/gaitmap/utils/_datatype_validation_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/_gaitmap_mad.py` & `gaitmap-2.2.0/gaitmap/utils/_gaitmap_mad.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/array_handling.py` & `gaitmap-2.2.0/gaitmap/utils/array_handling.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/consts.py` & `gaitmap-2.2.0/gaitmap/utils/consts.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/coordinate_conversion.py` & `gaitmap-2.2.0/gaitmap/utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/datatype_helper.py` & `gaitmap-2.2.0/gaitmap/utils/datatype_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/exceptions.py` & `gaitmap-2.2.0/gaitmap/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/fast_quaternion_math.py` & `gaitmap-2.2.0/gaitmap/utils/fast_quaternion_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/rotations.py` & `gaitmap-2.2.0/gaitmap/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/signal_processing.py` & `gaitmap-2.2.0/gaitmap/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/static_moment_detection.py` & `gaitmap-2.2.0/gaitmap/utils/static_moment_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/stride_list_conversion.py` & `gaitmap-2.2.0/gaitmap/utils/stride_list_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/utils/vector_math.py` & `gaitmap-2.2.0/gaitmap/utils/vector_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/zupt_detection/__init__.py` & `gaitmap-2.2.0/gaitmap/zupt_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/zupt_detection/_base.py` & `gaitmap-2.2.0/gaitmap/zupt_detection/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/zupt_detection/_combo_zupt_detector.py` & `gaitmap-2.2.0/gaitmap/zupt_detection/_combo_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/zupt_detection/_moving_window_zupt_detector.py` & `gaitmap-2.2.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/gaitmap/zupt_detection/_stride_event_zupt_detector.py` & `gaitmap-2.2.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.1.1a0/pyproject.toml` & `gaitmap-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap"
-version = "2.1.1a0"
+version = "2.2.0"
 description = "The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis."
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap-2.1.1a0/PKG-INFO` & `gaitmap-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap
-Version: 2.1.1a0
+Version: 2.2.0
 Summary: The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis.
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,35 +28,38 @@
 Requires-Dist: tpcp (>=0.15.0)
 Requires-Dist: typing_extensions (>=4.1.1)
 Project-URL: Repository, https://github.com/mad-lab-fau/gaitmap
 Description-Content-Type: text/markdown
 
 <img src="./docs/_static/logo/gaitmap_logo_with_text.png" height="200">
 
+[![PyPI](https://img.shields.io/pypi/v/gaitmap)](https://pypi.org/project/gaitmap/)
 [![pipeline status](https://github.com/mad-lab-fau/gaitmap/workflows/Test%20and%20Lint/badge.svg)](https://github.com/mad-lab-fau/gaitmap/actions/workflows/test-and-lint.yml)
-[![codecov](https://codecov.io/gh/mad-lab-fau/gaitmap/branch/master/graph/badge.svg?token=5NP5ZZ3KGX)](https://codecov.io/gh/mad-lab-fau/gaitmap)[![docs](https://img.shields.io/badge/docs-online-green.svg)](http://MadLab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/README.html)
+[![codecov](https://codecov.io/gh/mad-lab-fau/gaitmap/branch/master/graph/badge.svg?token=5NP5ZZ3KGX)](https://codecov.io/gh/mad-lab-fau/gaitmap)
+[![Documentation Status](https://readthedocs.org/projects/gaitmap/badge/?version=latest)](https://gaitmap.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/gaitmap)
 
 # gaitmap - The Gait and Movement Analysis Package
 
 *gaitmap* provides a set of algorithms to analyze your IMU movement data (with a focus on foot-worn IMUs) without 
 getting into your way.
 
-- 💻 20+ Algorithms from 17+ publications
-- 📚 Extensive documentation
-- 📝 Build to be easily extensible
+- 💻 [20+ Algorithms](https://gaitmap.readthedocs.io/en/latest/modules/index.html) from 17+ publications
+- 📚 Extensive [documentation](https://gaitmap.readthedocs.io/en/latest/)
+- 📝 Build to be [easily extensible](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
 - ⚙️ Familiar API inspired by scikit-learn
 - 🤝 Interoperable with the other libraries from the gaitmap ecosystem ([gaitmap-dataset](https://github.com/mad-lab-fau/gaitmap-datasets), [tpcp](https://github.com/mad-lab-fau/tpcp), ...)
 
-**Documentation:** TODO: Website Link<br>
+**Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/)<br>
 **Learn More about the gaitmap ecosystem:** TODO: Website Link
 
 ## Installation
 
-Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](TODO: Link to gaitmap_mad docu page).
+Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html).
 To get access to all available algorithms, you need to install both packages.
 
 ```
 pip install gaitmap gaitmap_mad --upgrade
 ```
 
 Both packages are always released together and have the same version number.
@@ -72,15 +75,15 @@
 ### Enabling specific features
 
 #### Hidden Markov Models
 
 To use the HMM (anything imported from `gaitmap.stride_segmentation.hmm`) based algorithms make sure you install `gaitmap` with the `hmm` extra.
 
 ```
-pip install "gaitmap_mad gaitmap[hmm]" --upgrade
+pip install gaitmap_mad "gaitmap[hmm]" --upgrade
 ```
 This installs the `pomegranate` package, which is the basis for the HMM implementation.
 Note, that we only support the `pomegranate` version `>=0.14.2,<=0.14.6` and that `pomegrante` is not compatible with 
 Python 3.10.
 
 We are working on upgrading to a newer version of `pomegranate`, but this is not a priority at the moment.
 You can track the progress in the [pull request](https://github.com/mad-lab-fau/gaitmap/pull/20).
@@ -94,17 +97,17 @@
 ## Working with Algorithms
 
 *gaitmap* is designed to be a toolbox and not a single algorithm.
 This means, that you are expected to pick and use individual algorithms.
 
 To get started with *gaitmap* we recommend to follow these steps:
 
-1. Understand the common datatypes we use: [Common Datatypes](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/user_guide/datatypes.html)
-2. Understand how to prepare your data: [Coordinate Systems](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/user_guide/coordinate_systems.html)
-3. Check the API docs and examples for available algorithms: [API Docs](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/autoapi/gaitmap/index.html)
+1. Understand the common datatypes we use: [Common Datatypes](https://gaitmap.readthedocs.io/en/latest/source/user_guide/datatypes.html), [Coordinate Systems](https://gaitmap.readthedocs.io/en/latest/source/user_guide/coordinate_systems.html)
+2. Learn how to prepare your own data (or play around with example data): TODO 
+3. Check the API docs and examples for available algorithms: [API Docs](https://gaitmap.readthedocs.io/en/latest/modules/index.html), [Examples](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
 
 Each algorithm is implemented as a class, which is initialized with the required parameters.
 In many cases the default parameters are sufficient, but to get the best results on your data, you should adapt them.
 
 ```python
 from gaitmap.stride_segmentation import BarthDtw
 
@@ -126,17 +129,17 @@
 
 Most algorithms have additional results available to provide further information.
 
 ```python
 dtw_warping_path = stride_segmenter.paths_
 ```
 
-To build a full gait analysis pipeline you can combine multiple algorithms ([Example]()).
-You can even substitute your own algorithms ([Guide]()) or use the provided tooling to validate
-and optimize your algorithms ([Guide]()).
+To build a full gait analysis pipeline you can combine multiple algorithms ([Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/full_pipelines/mad_gait_pipeline.html#sphx-glr-auto-examples-full-pipelines-mad-gait-pipeline-py)).
+You can even substitute your own algorithms ([Guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)) or use the provided tooling to validate
+and optimize your algorithms using tpcp ([General Guide](https://tpcp.readthedocs.io/en/latest/guides/index.html#optimization-and-validation), [Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/datasets_and_pipelines/gridsearch.html#sphx-glr-auto-examples-datasets-and-pipelines-gridsearch-py)).
 
 ## Citation
 
 If you use *gaitmap* in your research we would appreciate a citation.
 This helps us to justify the time we invest in the development and maintenance of the library.
 
 We currently prepare a paper to describe the *gaitmap* library in detail.
@@ -162,18 +165,15 @@
 Please, check the [AGPL-3.0 license](https://www.gnu.org/licenses/agpl-3.0.en.html) for more details and make sure
 you understand the implications.
 
 If you need to use *gaitmap_mad* in a closed source project, please contact us for a potential commercial license.
 
 ## For Developers
 
-The [Development Guide](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/development/development_guide.html)
-and the
-[Project Structure Guide](http://madlab.mad-pages.informatik.uni-erlangen.de/GaitAnalysis/gaitmap/source/development/project_structure.html)
-have detailed information for all new developers.
+The [Development Guides](https://gaitmap.readthedocs.io/en/latest/source/development/index.html#development) have detailed information for all new developers.
 
 Here some quick references
 Install Python >=3.8 and [poetry](https://python-poetry.org).
 Then run the commands below to get the latest source and install the dependencies:
 
 ```bash
 git clone https://github.com/mad-lab-fau/gaitmap.git
```

