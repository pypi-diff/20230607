# Comparing `tmp/vstt-0.28.0.tar.gz` & `tmp/vstt-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.28.0.tar", last modified: Tue Jun  6 13:38:55 2023, max compression
+gzip compressed data, was "vstt-0.29.0.tar", last modified: Wed Jun  7 12:11:58 2023, max compression
```

## Comparing `vstt-0.28.0.tar` & `vstt-0.29.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.980248 vstt-0.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-06 13:38:44.000000 vstt-0.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-06 13:38:55.980248 vstt-0.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-06 13:38:44.000000 vstt-0.28.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-06 13:38:44.000000 vstt-0.28.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:38:55.980248 vstt-0.28.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.976248 vstt-0.28.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.976248 vstt-0.28.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-06 13:38:44.000000 vstt-0.28.0/src/vstt/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.980248 vstt-0.28.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 13:38:55.000000 vstt-0.28.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:38:55.980248 vstt-0.28.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 13:38:44.000000 vstt-0.28.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.959209 vstt-0.29.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 12:11:42.000000 vstt-0.29.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-07 12:11:58.959209 vstt-0.29.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-07 12:11:42.000000 vstt-0.29.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 12:11:42.000000 vstt-0.29.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:11:58.963209 vstt-0.29.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.951209 vstt-0.29.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.955209 vstt-0.29.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.955209 vstt-0.29.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.959209 vstt-0.29.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_vstt.py
```

### Comparing `vstt-0.28.0/LICENSE` & `vstt-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/PKG-INFO` & `vstt-0.29.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.28.0
+Version: 0.29.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.28.0/README.md` & `vstt-0.29.0/README.md`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/pyproject.toml` & `vstt-0.29.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/__main__.py` & `vstt-0.29.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/common.py` & `vstt-0.29.0/src/vstt/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import copy
 import logging
 from typing import Any
-from typing import Dict
+from typing import Mapping
 from typing import Type
 from typing import TypeVar
 
 from vstt.types import DisplayOptions
 from vstt.types import Metadata
 from vstt.types import Trial
 
@@ -26,15 +26,15 @@
     if correct_type in (float, int) and type(var) in (float, int):
         # int instead of float or vice versa is ok
         return True
     return False
 
 
 def import_typed_dict(
-    input_dict: Dict, default_typed_dict: VsttTypedDict
+    input_dict: Mapping[str, Any], default_typed_dict: VsttTypedDict
 ) -> VsttTypedDict:
     # start with a valid typed dict with default values
     output_dict = copy.deepcopy(default_typed_dict)
     for key, default_value in output_dict.items():
         if key in input_dict:
             # import all valid keys from input_dict
             correct_type = type(default_value)
```

### Comparing `vstt-0.28.0/src/vstt/display.py` & `vstt-0.29.0/src/vstt/display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/display_widget.py` & `vstt-0.29.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/experiment.py` & `vstt-0.29.0/src/vstt/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 from vstt.display import default_display_options
 from vstt.display import import_display_options
 from vstt.meta import default_metadata
 from vstt.meta import import_metadata
 from vstt.stat import append_stats_data_to_excel
 from vstt.stat import stats_dataframe
 from vstt.trial import default_trial
-from vstt.trial import import_trial
-from vstt.trial import validate_trial
+from vstt.trial import import_and_validate_trial
 
 
 class Experiment:
     def __init__(self, filename: Optional[str] = None):
         self.filename = "default-experiment.psydat"
         self.has_unsaved_changes = False
         self.metadata = default_metadata()
@@ -31,16 +30,16 @@
         self.trial_list = [default_trial()]
         self.trial_handler_with_results: Optional[TrialHandlerExt] = None
         self.stats: Optional[pd.DataFrame] = None
         if filename is not None:
             self.load_file(filename)
 
     def create_trialhandler(self) -> TrialHandlerExt:
-        for trial in self.trial_list:
-            validate_trial(trial)
+        for index, trial in enumerate(self.trial_list):
+            self.trial_list[index] = import_and_validate_trial(trial)
         return TrialHandlerExt(
             self.trial_list,
             nReps=1,
             method="sequential",
             originPath=-1,
             extraInfo={
                 "display_options": self.display_options,
@@ -143,30 +142,28 @@
         filename: str,
         metadata_dict: Dict,
         display_options_dict: Dict,
         trial_dict_list: List[Dict],
     ) -> None:
         self.metadata = import_metadata(metadata_dict)
         self.display_options = import_display_options(display_options_dict)
-        self.trial_list = []
-        for trial_dict in trial_dict_list:
-            trial = import_trial(trial_dict)
-            validate_trial(trial)
-            self.trial_list.append(trial)
+        self.trial_list = [
+            import_and_validate_trial(trial_dict) for trial_dict in trial_dict_list
+        ]
         self.trial_handler_with_results = None
         self.stats = None
         self.has_unsaved_changes = True
         self.filename = str(pathlib.Path(filename).with_suffix(".psydat"))
 
     def import_and_validate_trial_handler(self, trial_handler: TrialHandlerExt) -> None:
         # psychopy trial handler converts empty trial list [] -> [None]
         if trial_handler.trialList == [None]:
             trial_handler.trialList = []
-        for trial in trial_handler.trialList:
-            validate_trial(trial)
+        for index, trial in enumerate(trial_handler.trialList):
+            trial_handler.trialList[index] = import_and_validate_trial(trial)
         self.trial_list = trial_handler.trialList
         if not trial_handler.extraInfo:
             trial_handler.extraInfo = {}
         self.metadata = import_metadata(
             trial_handler.extraInfo.get("metadata", default_metadata())
         )
         self.display_options = import_display_options(
```

### Comparing `vstt-0.28.0/src/vstt/geom.py` & `vstt-0.29.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/gui.py` & `vstt-0.29.0/src/vstt/gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/joystick_wrapper.py` & `vstt-0.29.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/meta.py` & `vstt-0.29.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/meta_widget.py` & `vstt-0.29.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/results_widget.py` & `vstt-0.29.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/stat.py` & `vstt-0.29.0/src/vstt/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
 
 def _get_dat(
     data: Dict, key: str, index: Tuple, i_target: int, default_value: Any
 ) -> Any:
     ar = data.get(key)
     if ar is None:
-        logging.warning(
+        logging.debug(
             f"Key '{key}' not found in data, using default value {default_value}"
         )
         return default_value
     try:
         return ar[index][i_target]
     except IndexError:
-        logging.warning(
+        logging.debug(
             f"Index error for key '{key}', index '{index}', i_target '{i_target}', using default value {default_value}"
         )
     return default_value
 
 
 def _get_target_data(
     trial_handler: TrialHandlerExt, index: Tuple, i_target: int
```

### Comparing `vstt-0.28.0/src/vstt/task.py` & `vstt-0.29.0/src/vstt/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Union
 
 import numpy as np
 from psychopy.clock import Clock
 from psychopy.data import TrialHandlerExt
 from psychopy.event import Mouse
 from psychopy.hardware.keyboard import Keyboard
@@ -83,24 +84,29 @@
         self.cursor.setPos(np.array([0.0, 0.0]))
         if trial["show_cursor"]:
             self.drawables.append(self.cursor)
         self.point_rotator = PointRotator(trial["cursor_rotation_degrees"])
         self.joystick_point_updater = JoystickPointUpdater(
             trial["cursor_rotation_degrees"], trial["joystick_max_speed"], win.size
         )
-        self.cursor_path = ShapeStim(
-            win, vertices=[(0, 0)], lineColor="white", closeShape=False
-        )
-        self.prev_cursor_path = ShapeStim(
-            win, vertices=[(0, 0)], lineColor="white", closeShape=False
+        self._cursor_path = ShapeStim(
+            win, vertices=[(0.0, 0.0)], lineColor="white", closeShape=False
         )
+        self._cursor_path_vertices: List[Tuple[float, float]] = []
         self.clock = Clock()
         if trial["show_cursor_path"]:
-            self.drawables.append(self.cursor_path)
-            self.drawables.append(self.prev_cursor_path)
+            self.drawables.append(self._cursor_path)
+
+    def cursor_path_add_vertex(
+        self, vertex: Tuple[float, float], clear_existing: bool = False
+    ) -> None:
+        if clear_existing:
+            self._cursor_path_vertices = []
+        self._cursor_path_vertices.append(vertex)
+        self._cursor_path.vertices = self._cursor_path_vertices
 
 
 def _contains_mixed_length_numpy_arrays(items: Iterable) -> bool:
     return (
         len(set([item.shape if isinstance(item, np.ndarray) else 1 for item in items]))
         > 1
     )
@@ -224,24 +230,20 @@
             stop_waiting_time = (num_completed_targets + 1) * trial["target_duration"]
             stop_target_time = stop_waiting_time + trial["target_duration"]
         for target_index in _get_target_indices(index, trial):
             t0 = tm.clock.getTime()
             is_central_target = target_index == trial["num_targets"]
             mouse_times = []
             mouse_positions = []
-            if is_central_target:
-                tm.prev_cursor_path.vertices = tm.cursor_path.vertices
-                tm.cursor_path.vertices = [tm.cursor_path.vertices[-1]]
-            else:
+            if not is_central_target:
                 if trial["automove_cursor_to_center"]:
                     mouse_pos = np.array([0.0, 0.0])
                     self.mouse.setPos(mouse_pos)
                     tm.cursor.setPos(mouse_pos)
-                tm.cursor_path.vertices = [mouse_pos]
-                tm.prev_cursor_path.vertices = [(0, 0)]
+                tm.cursor_path_add_vertex(mouse_pos, clear_existing=True)
                 if not trial["fixed_target_intervals"]:
                     stop_waiting_time = t0 + trial["inter_target_duration"]
                 if stop_waiting_time > t0:
                     # no target displayed
                     vis.update_target_colors(
                         tm.targets, trial["show_inactive_targets"], None
                     )
@@ -263,15 +265,15 @@
                             else:
                                 mouse_pos = tm.point_rotator(self.mouse.getPos())
                         mouse_times.append(tm.clock.getTime())
                         mouse_positions.append(mouse_pos)
                         if trial["show_cursor"]:
                             tm.cursor.setPos(mouse_pos)
                         if trial["show_cursor_path"]:
-                            tm.cursor_path.vertices = mouse_positions
+                            tm.cursor_path_add_vertex(mouse_pos)
                         should_continue_waiting = (
                             tm.clock.getTime() + minimum_window_for_flip
                             < stop_waiting_time
                         )
             # display current target
             t0 = tm.clock.getTime()
             vis.update_target_colors(
@@ -288,15 +290,18 @@
             else:
                 tm.data.target_pos.append(tm.targets.xys[target_index])
                 tm.data.to_target_num_timestamps_before_visible.append(len(mouse_times))
             target_size = trial["target_size"]
             if is_central_target:
                 target_size = trial["central_target_size"]
             if not trial["fixed_target_intervals"]:
-                stop_target_time = t0 + trial["target_duration"]
+                if is_central_target:
+                    stop_target_time = t0 + trial["central_target_duration"]
+                else:
+                    stop_target_time = t0 + trial["target_duration"]
             dist_correct = 1.0
             # ensure we get at least one flip
             should_continue_target = True
             while should_continue_target:
                 vis.draw_and_flip(self.win, tm.drawables, self.kb)
                 if trial["use_joystick"]:
                     mouse_pos = tm.joystick_point_updater(
@@ -305,15 +310,15 @@
                 else:
                     mouse_pos = tm.point_rotator(self.mouse.getPos())
                 if trial["show_cursor"]:
                     tm.cursor.setPos(mouse_pos)
                 mouse_times.append(tm.clock.getTime())
                 mouse_positions.append(mouse_pos)
                 if trial["show_cursor_path"]:
-                    tm.cursor_path.vertices = mouse_positions
+                    tm.cursor_path_add_vertex(mouse_pos)
                 dist_correct, dist_any = to_target_dists(
                     mouse_pos,
                     tm.targets.xys,
                     target_index,
                     trial["add_central_target"],
                 )
                 if trial["ignore_incorrect_targets"] or is_central_target:
```

### Comparing `vstt-0.28.0/src/vstt/trial.py` & `vstt-0.29.0/src/vstt/trial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import copy
+from typing import Any
 from typing import Dict
 from typing import List
+from typing import Mapping
 from typing import Optional
 
 import numpy as np
 from psychopy.gui import DlgFromDict
 from vstt.common import import_typed_dict
 from vstt.types import Trial
 
@@ -28,14 +30,15 @@
         "target_order": "clockwise",
         "target_indices": "0 1 2 3 4 5 6 7",
         "add_central_target": True,
         "show_target_labels": False,
         "target_labels": "0 1 2 3 4 5 6 7",
         "fixed_target_intervals": False,
         "target_duration": 5.0,
+        "central_target_duration": 5.0,
         "inter_target_duration": 1.0,
         "target_distance": 0.4,
         "target_size": 0.04,
         "central_target_size": 0.02,
         "show_inactive_targets": True,
         "ignore_incorrect_targets": True,
         "play_sound": True,
@@ -63,14 +66,15 @@
         "target_order": "Target order",
         "target_indices": "Target indices",
         "add_central_target": "Add a central target",
         "show_target_labels": "Display target labels",
         "target_labels": "Target labels",
         "fixed_target_intervals": "Fixed target display intervals",
         "target_duration": "Target display duration (secs)",
+        "central_target_duration": "Central target display duration (secs)",
         "inter_target_duration": "Delay between targets (secs)",
         "target_distance": "Distance to targets (screen height fraction)",
         "target_size": "Target size (screen height fraction)",
         "central_target_size": "Central target size (screen height fraction)",
         "show_inactive_targets": "Show inactive targets",
         "ignore_incorrect_targets": "Ignore cursor hitting incorrect target",
         "play_sound": "Play a sound on target display",
@@ -104,25 +108,23 @@
             order_of_targets.append(target_order)
     trial["target_order"] = order_of_targets
     dialog = DlgFromDict(
         trial, title="Trial settings", labels=trial_labels(), sortKeys=False
     )
     if not dialog.OK:
         return None
-    return validate_trial(trial)
+    return import_and_validate_trial(trial)
 
 
-def import_trial(trial_dict: dict) -> Trial:
-    return import_typed_dict(trial_dict, default_trial())
-
-
-def validate_trial(trial: Trial) -> Trial:
+def import_and_validate_trial(trial_or_dict: Mapping[str, Any]) -> Trial:
+    trial = import_typed_dict(trial_or_dict, default_trial())
     # make any negative time durations zero
     for duration in [
         "target_duration",
+        "central_target_duration",
         "inter_target_duration",
         "post_trial_delay",
         "post_block_delay",
     ]:
         if trial[duration] < 0.0:  # type: ignore
             trial[duration] = 0.0  # type: ignore
     # convert string of target indices to a numpy array of ints
```

### Comparing `vstt-0.28.0/src/vstt/trials_widget.py` & `vstt-0.29.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/types.py` & `vstt-0.29.0/src/vstt/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     target_order: Union[str, List]
     target_indices: str
     add_central_target: bool
     show_target_labels: bool
     target_labels: str
     fixed_target_intervals: bool
     target_duration: float
+    central_target_duration: float
     inter_target_duration: float
     target_distance: float
     target_size: float
     central_target_size: float
     show_inactive_targets: bool
     ignore_incorrect_targets: bool
     play_sound: bool
```

### Comparing `vstt-0.28.0/src/vstt/update.py` & `vstt-0.29.0/src/vstt/update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/src/vstt/vis.py` & `vstt-0.29.0/src/vstt/vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,15 @@
                     pos=row.target_pos,
                     fillColor=colors[row.target_index],
                 )
             )
     # paths to center
     if (
         display_options["to_center_paths"]
+        and conditions["add_central_target"]
         and not conditions["automove_cursor_to_center"]
     ):
         for _, row in stats_df.iterrows():
             drawables.append(
                 ShapeStim(
                     win,
                     vertices=row.to_center_mouse_positions,
```

### Comparing `vstt-0.28.0/src/vstt.egg-info/PKG-INFO` & `vstt-0.29.0/src/vstt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.28.0
+Version: 0.29.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.28.0/src/vstt.egg-info/SOURCES.txt` & `vstt-0.29.0/src/vstt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_display.py` & `vstt-0.29.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_display_widget.py` & `vstt-0.29.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_experiment.py` & `vstt-0.29.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_geom.py` & `vstt-0.29.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_gui.py` & `vstt-0.29.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_joystick_wrapper.py` & `vstt-0.29.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_meta.py` & `vstt-0.29.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_meta_widget.py` & `vstt-0.29.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_results_widget.py` & `vstt-0.29.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_stat.py` & `vstt-0.29.0/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_task.py` & `vstt-0.29.0/tests/test_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,16 +193,25 @@
     data = experiment.trial_handler_with_results.data
     for success_name in ["to_target_success", "to_center_success"]:
         assert np.all(data[success_name][0][0] == expected_success)
     # first to_target timestamps should start at ~0,
     # at ~target_duration the first target is displayed for target_duration secs,
     # subsequent ones should be displayed every ~target_duration starting from ~2*target_duration
     all_to_target_timestamps = data["to_target_timestamps"][0][0]
-    # require timestamps to be accurate within 0.1s
-    # On CI the fps / dropped frames can be erratic so this is a conservative value.
-    # If running on real hardware these should actually be within 2/fps
-    delta = 0.1
-    assert abs(all_to_target_timestamps[0][0]) < delta
-    assert abs(all_to_target_timestamps[0][-1] - 2 * target_duration) < delta
+    # require timestamps to be accurate within 0.5s
+    allowed_error_on_timestamp = 0.5
+    # this is a weak requirement to avoid tests failing on CI where many frames can get dropped
+    # if running tests locally allowed_error_on_timestamp should be ~2/fps
+    assert abs(all_to_target_timestamps[0][0]) < allowed_error_on_timestamp
+    assert (
+        abs(all_to_target_timestamps[0][-1] - 2 * target_duration)
+        < allowed_error_on_timestamp
+    )
     for count, to_target_timestamps in enumerate(all_to_target_timestamps[1:]):
-        assert abs(to_target_timestamps[0] - (count + 2) * target_duration) < delta
-        assert abs(to_target_timestamps[-1] - (count + 3) * target_duration) < delta
+        assert (
+            abs(to_target_timestamps[0] - (count + 2) * target_duration)
+            < allowed_error_on_timestamp
+        )
+        assert (
+            abs(to_target_timestamps[-1] - (count + 3) * target_duration)
+            < allowed_error_on_timestamp
+        )
```

### Comparing `vstt-0.28.0/tests/test_trial.py` & `vstt-0.29.0/tests/test_trial.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         vstt.trial.describe_trials(trials)
         == "  - 1 repeat of 8 clockwise targets\n  - 3 repeats of 1 fixed target"
     )
 
 
 def test_default_trial() -> None:
     trial = vstt.trial.default_trial()
-    assert len(trial) == 30
+    assert len(trial) == len(vstt.trial.trial_labels())
     assert isinstance(trial["target_indices"], str)
     assert len(trial["target_indices"].split(" ")) == trial["num_targets"]
 
 
 def test_trial_labels() -> None:
     trial = vstt.trial.default_trial()
     labels = vstt.trial.trial_labels()
@@ -51,14 +51,15 @@
         "target_order": "clockwise",
         "target_indices": "0 1 2 3 4 5",
         "add_central_target": True,
         "show_target_labels": False,
         "target_labels": "0 1 2 3 4 5",
         "fixed_target_intervals": False,
         "target_duration": 3,
+        "central_target_duration": 3,
         "inter_target_duration": 0,
         "target_distance": 0.3,
         "target_size": 0.03,
         "central_target_size": 0.01,
         "show_inactive_targets": False,
         "ignore_incorrect_targets": True,
         "play_sound": True,
@@ -74,84 +75,88 @@
         "post_trial_display_results": True,
         "post_block_delay": 2.0,
         "post_block_display_results": False,
         "show_delay_countdown": False,
         "enter_to_skip_delay": True,
     }
     # all valid keys are imported
-    trial = vstt.trial.import_trial(trial_dict)
+    trial = vstt.trial.import_and_validate_trial(trial_dict)
     for key in trial:
         assert trial[key] == trial_dict[key]  # type: ignore
     # if any keys are missing, default values are used instead
     missing_keys = [
         "weight",
         "cursor_rotation_degrees",
         "post_trial_delay",
         "post_block_display_results",
     ]
     for key in missing_keys:
         trial_dict.pop(key)
     # unknown keys are ignored
     trial_dict["unknown_key1"] = "ignore me"
     trial_dict["unknown_key2"] = False
-    trial = vstt.trial.import_trial(trial_dict)
+    trial = vstt.trial.import_and_validate_trial(trial_dict)
     for key in trial:
         if key in missing_keys:
             assert trial[key] == default_trial[key]  # type: ignore
         else:
             assert trial[key] == trial_dict[key]  # type: ignore
 
 
 def test_validate_trial_durations() -> None:
     trial = vstt.trial.default_trial()
     # positive durations are not modified
     trial["target_duration"] = 1
+    trial["central_target_duration"] = 1
     trial["inter_target_duration"] = 0.1
     trial["post_trial_delay"] = 0.2
     trial["post_block_delay"] = 0.7
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert vtrial["target_duration"] == 1
+    assert vtrial["central_target_duration"] == 1
     assert vtrial["inter_target_duration"] == 0.1
     assert vtrial["post_trial_delay"] == 0.2
     assert vtrial["post_block_delay"] == 0.7
     # negative durations are cast to zero
     trial["target_duration"] = -1
+    trial["central_target_duration"] = -0.8
     trial["inter_target_duration"] = -0.1
     trial["post_trial_delay"] = -0.2
     trial["post_block_delay"] = -0.7
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert vtrial["target_duration"] == 0
+    assert vtrial["central_target_duration"] == 0
     assert vtrial["inter_target_duration"] == 0
     assert vtrial["post_trial_delay"] == 0
     assert vtrial["post_block_delay"] == 0
 
 
 def test_validate_trial_target_order() -> None:
     trial = vstt.trial.default_trial()
     assert isinstance(trial["target_indices"], str)
     # clockwise
     trial["target_order"] = "clockwise"
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert isinstance(vtrial["target_indices"], str)
     assert vtrial["target_indices"] == "0 1 2 3 4 5 6 7"
     # anti-clockwise
     trial["target_order"] = "anti-clockwise"
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert isinstance(vtrial["target_indices"], str)
     assert vtrial["target_indices"] == "7 6 5 4 3 2 1 0"
     # random
     trial["target_order"] = "random"
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert isinstance(vtrial["target_indices"], str)
     assert len(set(vtrial["target_indices"].split(" "))) == 8
     # fixed & valid
     trial["target_order"] = "fixed"
     trial["target_indices"] = "0 1 2 3 4 5 6 7"
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert isinstance(vtrial["target_indices"], str)
     assert vtrial["target_indices"] == "0 1 2 3 4 5 6 7"
     # fixed & invalid - clipped to nearest valid indices
     trial["target_order"] = "fixed"
     trial["target_indices"] = "-2 8 1 5 12 -5"
-    vtrial = vstt.trial.validate_trial(trial)
+    vtrial = vstt.trial.import_and_validate_trial(trial)
     assert isinstance(vtrial["target_indices"], str)
     assert vtrial["target_indices"] == "0 7 1 5 7 0"
```

### Comparing `vstt-0.28.0/tests/test_trials_widget.py` & `vstt-0.29.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_update.py` & `vstt-0.29.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.28.0/tests/test_vis.py` & `vstt-0.29.0/tests/test_vis.py`

 * *Files identical despite different names*

