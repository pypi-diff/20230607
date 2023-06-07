# Comparing `tmp/elex-model-1.0.8.tar.gz` & `tmp/elex-model-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elex-model-1.0.8.tar", last modified: Fri Jan 13 18:30:44 2023, max compression
+gzip compressed data, was "elex-model-1.0.9.tar", last modified: Mon Mar  6 20:57:08 2023, max compression
```

## Comparing `elex-model-1.0.8.tar` & `elex-model-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.279601 elex-model-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-01-13 18:30:44.279601 elex-model-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-01-13 18:30:35.000000 elex-model-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-13 18:30:44.279601 elex-model-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-01-13 18:30:35.000000 elex-model-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.271601 elex-model-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.275601 elex-model-1.0.8/src/elex_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-13 18:30:44.000000 elex-model-1.0.8/src/elex_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.275601 elex-model-1.0.8/src/elexmodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.275601 elex-model-1.0.8/src/elexmodel/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/distributions/GaussianModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/distributions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.275601 elex-model-1.0.8/src/elexmodel/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.275601 elex-model-1.0.8/src/elexmodel/handlers/data/
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/data/CombinedData.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/data/LiveData.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/data/ModelResults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/data/PreprocessedData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/handlers/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.275601 elex-model-1.0.8/src/elexmodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/models/BaseElectionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/models/GaussianElectionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/models/NonparametricElectionModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:44.279601 elex-model-1.0.8/src/elexmodel/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/utils/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-13 18:30:35.000000 elex-model-1.0.8/src/elexmodel/utils/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-03-06 20:57:08.577642 elex-model-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-03-06 20:56:59.000000 elex-model-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-06 20:57:08.577642 elex-model-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-06 20:56:59.000000 elex-model-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.573642 elex-model-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.573642 elex-model-1.0.9/src/elex_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 20:57:08.000000 elex-model-1.0.9/src/elex_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.573642 elex-model-1.0.9/src/elexmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/src/elexmodel/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/distributions/GaussianModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/distributions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/src/elexmodel/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/src/elexmodel/handlers/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/data/CombinedData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/data/LiveData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/data/ModelResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/data/PreprocessedData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/handlers/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/src/elexmodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/models/BaseElectionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/models/GaussianElectionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/models/NonparametricElectionModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/src/elexmodel/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/utils/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-06 20:56:59.000000 elex-model-1.0.9/src/elexmodel/utils/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:57:08.577642 elex-model-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    24150 2023-03-06 20:56:59.000000 elex-model-1.0.9/tests/test_client.py
```

### Comparing `elex-model-1.0.8/PKG-INFO` & `elex-model-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elex-model
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for the Washington Post's live election night model
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `elex-model-1.0.8/README.md` & `elex-model-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/setup.py` & `elex-model-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 LONG_DESCRIPTION = ""
 # Get the long description from the README file
 with open(os.path.join(THIS_FILE_DIR, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 # The full version, including alpha/beta/rc tags
-RELEASE = "1.0.8"
+RELEASE = "1.0.9"
 # The short X.Y version
 VERSION = ".".join(RELEASE.split(".")[:2])
 
 PROJECT = "elex-model"
 AUTHOR = "The Wapo Newsroom Engineering Team"
 COPYRIGHT = "2022, {}".format(AUTHOR)
```

### Comparing `elex-model-1.0.8/src/elex_model.egg-info/PKG-INFO` & `elex-model-1.0.9/src/elex_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elex-model
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for the Washington Post's live election night model
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `elex-model-1.0.8/src/elex_model.egg-info/SOURCES.txt` & `elex-model-1.0.9/src/elex_model.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 src/elexmodel/models/GaussianElectionModel.py
 src/elexmodel/models/NonparametricElectionModel.py
 src/elexmodel/models/__init__.py
 src/elexmodel/utils/__init__.py
 src/elexmodel/utils/constants.py
 src/elexmodel/utils/file_utils.py
 src/elexmodel/utils/math_utils.py
-src/elexmodel/utils/pandas_utils.py
+src/elexmodel/utils/pandas_utils.py
+tests/test_client.py
```

### Comparing `elex-model-1.0.8/src/elexmodel/cli.py` & `elex-model-1.0.9/src/elexmodel/cli.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/client.py` & `elex-model-1.0.9/src/elexmodel/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 class ModelClient(object):
     """
     Client for generating vote estimates
     """
 
     def __init__(self):
         super().__init__()
+        self.conformalization_data_unit_dict = None
+        self.conformalization_data_agg_dict = None
 
     def _check_input_parameters(
         self,
         config_handler,
         office,
         estimands,
         geographic_unit_type,
@@ -82,14 +84,34 @@
             raise ValueError("beta is not valid. Has to be either an integer or a float.")
         if not isinstance(robust, bool):
             raise ValueError("robust is not valid. Has to be a boolean.")
         if handle_unreporting not in {"drop", "zero"}:
             raise ValueError("handle_unreporting must be either `drop` or `zero`")
         return True
 
+    def get_all_conformalization_data_unit(self):
+        """
+        This function collects the conformalization data from a model run. It produces a dictionary
+        with two types of data (in the gaussian case): the conformalization points that a distribution is
+        fit to, and the parameters of the resulting guassian distribution. In this unit-level function, the information for
+        one distribution is returned (all units combined). It returns None if get_estimates isn't called, as the
+        values they pull out are generated in that function.
+        """
+        return self.all_conformalization_data_unit_dict
+
+    def get_all_conformalization_data_agg(self):
+        """
+        This function collects the conformalization data from a model run. It produces a dictionary
+        with two types of data (in the gaussian case): the conformalization points that a distribution is
+        fit to, and the parameters of the resulting guassian distribution. In the agg case, distributions for each state (
+        in a multi-state model) are returned. This functions return None if get_estimates isn't called, as the
+        values they pull out are generated in that function.
+        """
+        return self.all_conformalization_data_agg_dict
+
     def get_estimates(
         self,
         current_data,  # list of lists
         election_id,
         office,
         estimands,
         prediction_intervals=[0.7, 0.9],
@@ -132,15 +154,14 @@
             "save_conformalization": save_conformalization,
         }
 
         LOG.info("Getting config: %s", election_id)
         config_handler = ConfigHandler(
             election_id, config=raw_config, s3_client=s3.S3JsonUtil(TARGET_BUCKET), save=save_config
         )
-
         self._check_input_parameters(
             config_handler,
             office,
             estimands,
             geographic_unit_type,
             features,
             aggregates,
@@ -235,48 +256,52 @@
         if len(duplicate_units) > 0:
             raise ModelClientException(f"At least one unit appears twice: {duplicate_units}")
 
         results_handler = ModelResultsHandler(
             aggregates, prediction_intervals, reporting_units, nonreporting_units, unexpected_units
         )
 
+        self.all_conformalization_data_unit_dict = {alpha: {} for alpha in prediction_intervals}
+        self.all_conformalization_data_agg_dict = {alpha: {} for alpha in prediction_intervals}
         for estimand in estimands:
             unit_predictions = model.get_unit_predictions(reporting_units, nonreporting_units, estimand)
             results_handler.add_unit_predictions(estimand, unit_predictions)
             # gets prediciton intervals for each alpha
-            alpha_to_unit_prediction_intervals = {
-                alpha: model.get_unit_prediction_intervals(
+            alpha_to_unit_prediction_intervals = {}
+            for alpha in prediction_intervals:
+                alpha_to_unit_prediction_intervals[alpha] = model.get_unit_prediction_intervals(
                     results_handler.reporting_units, results_handler.nonreporting_units, alpha, estimand
                 )
-                for alpha in prediction_intervals
-            }
+                self.all_conformalization_data_unit_dict[alpha][estimand] = model.get_all_conformalization_data_unit()
+
             results_handler.add_unit_intervals(estimand, alpha_to_unit_prediction_intervals)
 
             for aggregate in results_handler.aggregates:
                 aggregate_list = sorted(list(set(["postal_code", aggregate])), key=lambda x: AGGREGATE_ORDER.index(x))
                 estimates_df = model.get_aggregate_predictions(
                     results_handler.reporting_units,
                     results_handler.nonreporting_units,
                     results_handler.unexpected_units,
                     aggregate_list,
                     estimand,
                 )
-                alpha_to_agg_prediction_intervals = {
-                    alpha: model.get_aggregate_prediction_intervals(
+                alpha_to_agg_prediction_intervals = {}
+                for alpha in prediction_intervals:
+                    alpha_to_agg_prediction_intervals[alpha] = model.get_aggregate_prediction_intervals(
                         results_handler.reporting_units,
                         results_handler.nonreporting_units,
                         results_handler.unexpected_units,
                         aggregate_list,
                         alpha,
                         alpha_to_unit_prediction_intervals[alpha].conformalization,
                         estimand,
                         model_settings,
                     )
-                    for alpha in prediction_intervals
-                }
+                    self.all_conformalization_data_agg_dict[alpha][estimand] = model.get_all_conformalization_data_agg()
+
                 # get all of the prediction intervals here
                 results_handler.add_agg_predictions(
                     estimand, aggregate, estimates_df, alpha_to_agg_prediction_intervals
                 )
 
         results_handler.process_final_results()
         if APP_ENV != "local" and save_results:
@@ -361,14 +386,15 @@
             office,
             geographic_unit_type,
             estimands,
             estimand_baselines,
             s3_client=s3.S3CsvUtil(TARGET_BUCKET),
             historical=True,
         )
+
         results_to_return = [f"results_{estimand}" for estimand in estimands]
         geo_columns = set(["geographic_unit_fips", "postal_code"] + [a for a in self.aggregates if a != "unit"])
         preprocessed_data = preprocessed_data_handler.data[list(geo_columns) + results_to_return].copy()
         historical_current_data = preprocessed_data.merge(formatted_data, on=["postal_code", "geographic_unit_fips"])
         for estimand in estimands:
             column_name = f"results_{estimand}"
             historical_current_data = historical_current_data.assign(
```

### Comparing `elex-model-1.0.8/src/elexmodel/distributions/GaussianModel.py` & `elex-model-1.0.9/src/elexmodel/distributions/GaussianModel.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/handlers/config.py` & `elex-model-1.0.9/src/elexmodel/handlers/config.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/handlers/data/CombinedData.py` & `elex-model-1.0.9/src/elexmodel/handlers/data/CombinedData.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/handlers/data/LiveData.py` & `elex-model-1.0.9/src/elexmodel/handlers/data/LiveData.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,27 +40,25 @@
             "postal_code",
             "county_classification",
             "county_fips",
         ]  # columns we may want to sample by
         self.shuffle_dataframe = None
 
         self.data = data
-
         if data is not None:
             # passed in as a df
             data_for_estimands = self.load_data(data, estimands, historical)
             self.data = data_for_estimands
         else:
             self.data = self.get_data()
 
         self.current_reporting_data = None
 
     def get_data(self):
         file_path = self.get_live_data_file_path()
-
         # If local data file is not available, read data from s3
         if not Path(file_path).is_file():
             path_info = {
                 "election_id": self.election_id,
                 "office": self.office_id,
                 "geographic_unit_type": self.geographic_unit_type,
             }
@@ -88,15 +86,15 @@
     def load_data(self, data, estimands, historical):
         columns_to_return = ["postal_code", "geographic_unit_fips"]
         for estimand in estimands:
             if historical:
                 data[f"results_{estimand}"] = np.nan
             results_column_names = [x for x in data.columns if x.startswith("results")]
             # If this is not a historical run, then this is a live election
-            # so we are expecting that there will not be actual results  data
+            # so we are expecting that there will be actual results  data
             if not self.historical and len(results_column_names) == 0:
                 raise MockLiveDataHandlerException("This is not a test election, it is missing results data")
             if f"results_{estimand}" not in results_column_names:
                 raise MockLiveDataHandlerException("This is missing results data for estimand: ", estimand)
             columns_to_return.append(f"results_{estimand}")
         self.shuffle_dataframe = data[self.shuffle_columns].copy()
         return data[columns_to_return].copy()
@@ -116,14 +114,15 @@
         probabilities = np.ones((self.data.shape[0],))
         # if upweight is empty this forloop is skipped
         for category in upweight:  # e.g. category == "postal_code"
             weight = upweight[category]
             for value in weight:  # e.g. value == "AL"
                 indices = self.data[self.shuffle_dataframe[category] == value].index
                 probabilities[indices] = probabilities[indices] * weight[value]
+
         self.data = self.data.sample(frac=1, random_state=seed, weights=probabilities)
 
         # get indices of units that must come first
         mask = self.data.geographic_unit_fips.isin(enforce)
         first = self.data[mask]
         last = self.data[~mask]
         self.data = pd.concat([first, last]).reset_index(drop=True)
```

### Comparing `elex-model-1.0.8/src/elexmodel/handlers/data/ModelResults.py` & `elex-model-1.0.9/src/elexmodel/handlers/data/ModelResults.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/handlers/data/PreprocessedData.py` & `elex-model-1.0.9/src/elexmodel/handlers/data/PreprocessedData.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         if not Path(self.local_file_path).is_file():
             path_info = {
                 "election_id": self.election_id,
                 "office": self.office,
                 "geographic_unit_type": self.geographic_unit_type,
             }
             file_path = self.s3_client.get_file_path("preprocessed", path_info)
+
             csv_data = self.s3_client.get(file_path)
             # read data as a buffer
             preprocessed_data = StringIO(csv_data)
         else:
             # read data as a filepath
             preprocessed_data = self.local_file_path
```

### Comparing `elex-model-1.0.8/src/elexmodel/handlers/s3.py` & `elex-model-1.0.9/src/elexmodel/handlers/s3.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/logging.py` & `elex-model-1.0.9/src/elexmodel/logging.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/models/BaseElectionModel.py` & `elex-model-1.0.9/src/elexmodel/models/BaseElectionModel.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/models/GaussianElectionModel.py` & `elex-model-1.0.9/src/elexmodel/models/GaussianElectionModel.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 class GaussianElectionModel(BaseElectionModel):
     def __init__(self, model_settings={}):
         super().__init__(model_settings)
         self.model_settings = model_settings
         self.beta = model_settings.get("beta", 1)
         self.alpha_to_nonreporting_lower_bounds = {}
         self.alpha_to_nonreporting_upper_bounds = {}
+        self.modeled_bounds_agg = None
+        self.conformalization_data_agg = None
+        self.gaussian_bounds_unit = None
+        self.conformalization_data_unit = None
 
     def _compute_conf_frac(self):
         """
         Compute conformalization fraction for Gaussian model
         """
         return 0.7
 
@@ -40,22 +44,25 @@
             reporting_units,
             nonreporting_units,
             estimand,
             aggregate=[],
             alpha=alpha,
             beta=self.beta,
         )
+        self.gaussian_bounds_unit = gaussian_model
+        self.conformalization_data_unit = prediction_intervals.conformalization
 
         # gaussian model for single unit prediction intervals
         quantile = (3 + alpha) / 4
         lower_correction = stats.norm.ppf(
             q=quantile,
             loc=gaussian_model.mu_lower_bound,
             scale=np.sqrt(gaussian_model.var_inflate + 1) * gaussian_model.sigma_lower_bound,
         )
+
         upper_correction = stats.norm.ppf(
             q=quantile,
             loc=gaussian_model.mu_upper_bound,
             scale=np.sqrt(gaussian_model.var_inflate + 1) * gaussian_model.sigma_upper_bound,
         )
 
         # save for later, but need to copy to avoid changing the original
@@ -79,14 +86,21 @@
             upper + nonreporting_units[f"last_election_results_{estimand}"], nonreporting_units[f"results_{estimand}"]
         )
 
         return PredictionIntervals(
             lower.round(decimals=0), upper.round(decimals=0), prediction_intervals.conformalization
         )
 
+    # At the unit level, conformalization data is adjustment from estimated % change from baseline
+    def get_all_conformalization_data_unit(self):
+        return self.gaussian_bounds_unit, self.conformalization_data_unit
+
+    def get_all_conformalization_data_agg(self):
+        return self.modeled_bounds_agg, self.conformalization_data_agg
+
     def get_aggregate_prediction_intervals(
         self,
         reporting_units,
         nonreporting_units,
         unexpected_units,
         aggregate,
         alpha,
@@ -228,17 +242,20 @@
             else:
 
                 remaining_bounds_w_models = remaining_bounds.merge(remaining_models, how="inner", on=next_aggregate)
             # APPEND NEWLY MODELED BOUNDS TO modeled_bounds
             modeled_bounds = pd.concat([modeled_bounds, remaining_bounds_w_models])
 
         # construction conformal corrections using Gaussian models
-        # get means and standard deviations for for aggregates
+        # get means and standard deviations for aggregates
         # and add correction (which is percentile of the Gaussian at the quantile we care about)
+        self.modeled_bounds_agg = modeled_bounds
+        self.conformalization_data_agg = conformalization_data
         quantile = (3 + alpha) / 4
+
         modeled_bounds = modeled_bounds.assign(
             lb_mean=lambda x: x.nonreporting_weight_sum * x.mu_lower_bound,
             lb_sd=lambda x: x.sigma_lower_bound
             * np.sqrt(x.nonreporting_weight_ssum + x.var_inflate * np.power(x.nonreporting_weight_sum, 2)),
             ub_mean=lambda x: x.nonreporting_weight_sum * x.mu_upper_bound,
             ub_sd=lambda x: x.sigma_upper_bound
             * np.sqrt(x.nonreporting_weight_ssum + x.var_inflate * np.power(x.nonreporting_weight_sum, 2)),
@@ -265,15 +282,15 @@
                 predicted_upper=lambda x: np.maximum(
                     x[f"last_election_results_{estimand}"] + x.ub, aggregate_nonreporting_votes[f"results_{estimand}"]
                 ),
             )
             .drop(columns=f"last_election_results_{estimand}")
         )
 
-        # add results from reporting and reporting and unexpected units to get final group bounds
+        # add results from reporting  and unexpected units to get final group bounds
         aggregate_data = (
             aggregate_votes.merge(aggregate_prediction_intervals, how="outer", on=aggregate)
             .fillna({f"results_{estimand}": 0, "predicted_lower": 0, "predicted_upper": 0})
             .assign(
                 lower=lambda x: x.predicted_lower + x[f"results_{estimand}"],
                 upper=lambda x: x.predicted_upper + x[f"results_{estimand}"],
             )
```

### Comparing `elex-model-1.0.8/src/elexmodel/models/NonparametricElectionModel.py` & `elex-model-1.0.9/src/elexmodel/models/NonparametricElectionModel.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from elexmodel.models.BaseElectionModel import BaseElectionModel, PredictionIntervals
 
 
 class NonparametricElectionModel(BaseElectionModel):
     def __init__(self, model_settings={}):
         super().__init__(model_settings)
         self.robust = model_settings.get("robust", False)
+        self.conformalization_data_agg = None
+        self.conformalization_data_unit = None
 
     def _compute_conf_frac(self, n_reporting_units, alpha):
         """
         Returns fraction of reporting units to be part of conformalization set
         """
         # what happens if this is negative, which it is alpha 0.95 and n_reporting_units is 38
         return round(min(1 + (alpha + 1) / (n_reporting_units * (alpha - 1)), 0.9), 2)
@@ -48,15 +50,15 @@
         Returns upper/lower unit bounds and conformalization data (since we need that for aggregation)
         """
         conf_frac = self._compute_conf_frac(reporting_units.shape[0], alpha)
         # compute unadjusted upper/lower unit bounds and get conformalization data
         prediction_intervals = self.get_unit_prediction_interval_bounds(
             reporting_units, nonreporting_units, conf_frac, alpha, estimand
         )
-
+        self.conformalization_data_unit = prediction_intervals.conformalization
         # compute conformity scores (e_j). This is how well the the lower/upper model cover the conformalization data.
         scores = np.maximum(
             prediction_intervals.conformalization.lower_bounds, prediction_intervals.conformalization.upper_bounds
         )
 
         # our desired coverage is: the alpha-% percentile of e_j than is less than zero
         # this is roughly equivalent to alpha-% of conformalization data that is covered by initial guess
@@ -96,14 +98,21 @@
             upper + nonreporting_units[f"last_election_results_{estimand}"], nonreporting_units[f"results_{estimand}"]
         )
 
         return PredictionIntervals(
             lower.round(decimals=0), upper.round(decimals=0), prediction_intervals.conformalization
         )
 
+    # At the unit level, conformalization data is adjustment from estimated % change from baseline
+    def get_all_conformalization_data_unit(self):
+        return None, self.conformalization_data_unit
+
+    def get_all_conformalization_data_agg(self):
+        return None, self.conformalization_data_agg
+
     def get_aggregate_prediction_intervals(
         self,
         reporting_units,
         nonreporting_units,
         unexpected_units,
         aggregate,
         alpha,
@@ -142,8 +151,9 @@
                 lower=lambda x: x[f"pi_lower_{estimand}"] + x[f"results_{estimand}"],
                 upper=lambda x: x[f"pi_upper_{estimand}"] + x[f"results_{estimand}"],
             )
             .sort_values(aggregate)[aggregate + ["lower", "upper"]]
             .reset_index(drop=True)
         )
 
+        self.conformalization_data_agg = conformalization_data
         return PredictionIntervals(aggregate_data.lower.round(decimals=0), aggregate_data.upper.round(decimals=0))
```

### Comparing `elex-model-1.0.8/src/elexmodel/utils/file_utils.py` & `elex-model-1.0.9/src/elexmodel/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `elex-model-1.0.8/src/elexmodel/utils/math_utils.py` & `elex-model-1.0.9/src/elexmodel/utils/math_utils.py`

 * *Files identical despite different names*

