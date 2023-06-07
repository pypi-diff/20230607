# Comparing `tmp/timetomodel-0.7.2.tar.gz` & `tmp/timetomodel-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetomodel-0.7.2.tar", last modified: Mon Mar 20 15:16:45 2023, max compression
+gzip compressed data, was "timetomodel-0.7.3.tar", last modified: Wed Jun  7 13:36:55 2023, max compression
```

## Comparing `timetomodel-0.7.2.tar` & `timetomodel-0.7.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-03-20 15:16:45.699274 timetomodel-0.7.2/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       93 2023-03-19 14:07:04.000000 timetomodel-0.7.2/.gitignore
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      511 2023-03-19 14:07:04.000000 timetomodel-0.7.2/.pre-commit-config.yaml
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       91 2023-03-19 14:07:04.000000 timetomodel-0.7.2/.travis.yml
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1065 2023-03-19 14:07:04.000000 timetomodel-0.7.2/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5387 2023-03-20 15:16:45.699274 timetomodel-0.7.2/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     7536 2023-03-19 14:07:04.000000 timetomodel-0.7.2/Readme.md
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-03-20 15:16:45.699274 timetomodel-0.7.2/img/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)   113271 2023-03-19 14:07:04.000000 timetomodel-0.7.2/img/solar-forecast-evaluation.png
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      512 2023-03-20 15:16:45.703274 timetomodel-0.7.2/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5783 2023-03-20 15:15:51.000000 timetomodel-0.7.2/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-03-20 15:16:45.699274 timetomodel-0.7.2/timetomodel/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2117 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      482 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/exceptions.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     8368 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/featuring.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3595 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/forecasting.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5418 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/modelling.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    27983 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/speccing.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-03-20 15:16:45.699274 timetomodel-0.7.2/timetomodel/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        0 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/tests/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5355 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/tests/test_forecasting.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10503 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/tests/test_series_specs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3054 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/tests/test_timeutils.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3742 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/tests/utils.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4323 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/transforming.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-03-20 15:16:45.699274 timetomodel-0.7.2/timetomodel/utils/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        0 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/utils/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2234 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/utils/debug_utils.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2778 2023-03-19 14:07:04.000000 timetomodel-0.7.2/timetomodel/utils/time_utils.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-03-20 15:16:45.699274 timetomodel-0.7.2/timetomodel.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5387 2023-03-20 15:16:45.000000 timetomodel-0.7.2/timetomodel.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      735 2023-03-20 15:16:45.000000 timetomodel-0.7.2/timetomodel.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-03-20 15:16:45.000000 timetomodel-0.7.2/timetomodel.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       92 2023-03-20 15:16:45.000000 timetomodel-0.7.2/timetomodel.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       12 2023-03-20 15:16:45.000000 timetomodel-0.7.2/timetomodel.egg-info/top_level.txt
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-07 13:36:55.124870 timetomodel-0.7.3/
+-rw-r--r--   0 felix     (1000) felix     (1000)       93 2021-11-01 14:16:35.000000 timetomodel-0.7.3/.gitignore
+-rw-r--r--   0 felix     (1000) felix     (1000)      511 2021-11-01 14:16:35.000000 timetomodel-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 felix     (1000) felix     (1000)       91 2021-11-01 14:16:35.000000 timetomodel-0.7.3/.travis.yml
+-rw-r--r--   0 felix     (1000) felix     (1000)     1065 2021-11-01 14:16:35.000000 timetomodel-0.7.3/LICENSE
+-rw-rw-r--   0 felix     (1000) felix     (1000)     6208 2023-06-07 13:36:55.124870 timetomodel-0.7.3/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     7536 2021-11-01 14:16:35.000000 timetomodel-0.7.3/Readme.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-07 13:36:55.116870 timetomodel-0.7.3/img/
+-rw-r--r--   0 felix     (1000) felix     (1000)   113271 2021-11-01 14:16:35.000000 timetomodel-0.7.3/img/solar-forecast-evaluation.png
+-rw-r--r--   0 felix     (1000) felix     (1000)      512 2023-06-07 13:36:55.124870 timetomodel-0.7.3/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)     5792 2023-06-07 13:32:44.000000 timetomodel-0.7.3/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-07 13:36:55.120870 timetomodel-0.7.3/timetomodel/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2117 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      482 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/exceptions.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8374 2023-05-06 22:03:06.000000 timetomodel-0.7.3/timetomodel/featuring.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3598 2023-05-06 22:03:06.000000 timetomodel-0.7.3/timetomodel/forecasting.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5418 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/modelling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    27989 2023-05-06 22:03:05.000000 timetomodel-0.7.3/timetomodel/speccing.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-07 13:36:55.120870 timetomodel-0.7.3/timetomodel/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5355 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/tests/test_forecasting.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10503 2021-11-01 14:16:44.000000 timetomodel-0.7.3/timetomodel/tests/test_series_specs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3054 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/tests/test_timeutils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3748 2023-05-06 22:03:06.000000 timetomodel-0.7.3/timetomodel/tests/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4323 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/transforming.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-07 13:36:55.124870 timetomodel-0.7.3/timetomodel/utils/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/utils/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2234 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/utils/debug_utils.py
+-rwxrwxrwx   0 felix     (1000) felix     (1000)     1177 2020-02-20 10:50:05.000000 timetomodel-0.7.3/timetomodel/utils/log_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2778 2021-11-01 14:16:35.000000 timetomodel-0.7.3/timetomodel/utils/time_utils.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-07 13:36:55.120870 timetomodel-0.7.3/timetomodel.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     6208 2023-06-07 13:36:54.000000 timetomodel-0.7.3/timetomodel.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      766 2023-06-07 13:36:54.000000 timetomodel-0.7.3/timetomodel.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-06-07 13:36:54.000000 timetomodel-0.7.3/timetomodel.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       99 2023-06-07 13:36:54.000000 timetomodel-0.7.3/timetomodel.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       12 2023-06-07 13:36:54.000000 timetomodel-0.7.3/timetomodel.egg-info/top_level.txt
```

### Comparing `timetomodel-0.7.2/LICENSE` & `timetomodel-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/PKG-INFO` & `timetomodel-0.7.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,124 @@
 Metadata-Version: 2.1
 Name: timetomodel
-Version: 0.7.2
+Version: 0.7.3
 Summary: Sane handling of time series data for forecast modelling - with production usage in mind.
 Home-page: https://github.com/seitabv/timetomodel
 Author: Seita BV
 Author-email: nicolas@seita.nl
 License: UNKNOWN
+Description: # timetomodel
+        
+        Time series forecasting is a modern data science & engineering challenge.
+        
+        We noticed that these two worlds, data science and engineering of time series forecasting, are not very compatible.
+        Often, work from the data scientist has to be re-implemented by engineers to be used in production.
+        
+        `timetomodel` was created to change that. It describes the data treatment of a model, and also automates common data treatment tasks like building data for training and testing.
+        
+        As a *data scientist*, experiment with a model in your notebook.
+        Load data from static files (e.g. CSV) and try out lags, regressors and so on.
+        Compare plots and mean square errors of the models you developed.
+        
+        As an *engineer*, take over the model description and use it in your production code.
+        Often, this would entail not much more than changing the data source (e.g from CSV to a column in the database).
+        
+        `timetomodel` is supposed to wrap around any fit/predict type model, e.g. from statsmodels or scikit-learn (some work needed here to ensure support).
+        
+        
+        ## Features
+        
+        Here are some features for both data scientists and engineers to enjoy:
+        
+        * Describe how to load data for outcome and regressor variables. Load from Pandas objects, CSV files, Pandas pickles or databases via SQLAlchemy.
+        * Create train & test data, including lags.
+        * Timezone awareness support.
+        * Custom data transformations, after loading (e.g. to remove duplicate) or only for forecasting (e.g. to apply a BoxCox transformation).
+        * Evaluate a model by RMSE, and plot the cumulative error.
+        * Support for creating rolling forecasts.
+        
+        
+        ## Installation
+        
+        ``pip install timetomodel``
+        
+        ## Example
+        
+        Here is an example where we describe a solar time series problem, and use ``statsmodels.OLS``, a linear regression model, to forecast one hour ahead:
+        
+            import pandas as pd
+            import pytz
+            from datetime import datetime, timedelta
+            from statsmodels.api import OLS
+            from timetomodel import speccing, ModelState, create_fitted_model, evaluate_models
+            from timetomodel.transforming import BoxCoxTransformation
+            from timetomodel.forecasting import make_rolling_forecasts
+        
+            data_start = datetime(2015, 3, 1, tzinfo=pytz.utc)
+            data_end = datetime(2015, 10, 31, tzinfo=pytz.utc)
+        
+            #### Solar model - 1h ahead  ####
+        
+            # spec outcome variable
+            solar_outcome_var_spec = speccing.CSVFileSeriesSpecs(
+                file_path="data.csv",
+                time_column="datetime",
+                value_column="solar_power",
+                name="solar power",
+                feature_transformation=BoxCoxTransformation(lambda2=0.1)
+            )
+            # spec regressor variable
+            regressor_spec_1h = speccing.CSVFileSeriesSpecs(
+                file_path="data.csv",
+                time_column="datetime",
+                value_column="irradiation_forecast1h",
+                name="irradiation forecast",
+                feature_transformation=BoxCoxTransformation(lambda2=0.1)
+            )
+            # spec whole model treatment
+            solar_model1h_specs = speccing.ModelSpecs(
+                outcome_var=solar_outcome_var_spec,
+                model=OLS,
+                frequency=timedelta(minutes=15),
+                horizon=timedelta(hours=1),
+                lags=[lag * 96 for lag in range(1, 8)],  # 7 days (data has daily seasonality)
+                regressors=[regressor_spec_1h],
+                start_of_training=data_start + timedelta(days=30),
+                end_of_testing=data_end,
+                ratio_training_testing_data=2/3,
+                remodel_frequency=timedelta(days=14)  # re-train model every two weeks
+            )
+        
+            solar_model1h = create_fitted_model(solar_model1h_specs, "Linear Regression Solar Horizon 1h")
+            # solar_model_1h is now an OLS model object which can be pickled and re-used.
+            # With the solar_model1h_specs in hand, your production code could always re-train a new one,
+            # if the model has become outdated.
+        
+            # For data scientists: evaluate model
+            evaluate_models(m1=ModelState(solar_model1h, solar_model1h_specs))
+        
+        ![Evaluation result](https://raw.githubusercontent.com/SeitaBV/timetomodel/master/img/solar-forecast-evaluation.png)
+        
+            # For engineers a): Change data sources to use database (hinted)
+            solar_model1h_specs.outcome_var = speccing.DBSeriesSpecs(query=...)
+            solar_model1h_specs.regressors[0] = speccing.DBSeriesSpecs(query=...)
+        
+            # For engineers b): Use model to make forecasts for an hour
+            forecasts, model_state = make_rolling_forecasts(
+                start=datetime(2015, 11, 1, tzinfo=pytz.utc),
+                end=datetime(2015, 11, 1, 1, tzinfo=pytz.utc),
+                model_specs=solar_model1h_specs
+            )
+            # model_state might have re-trained a new model automatically, by honoring the remodel_frequency
+        
+            
 Keywords: time series,forecasting
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# timetomodel
-
-Time series forecasting is a modern data science & engineering challenge.
-
-We noticed that these two worlds, data science and engineering of time series forecasting, are not very compatible.
-Often, work from the data scientist has to be re-implemented by engineers to be used in production.
-
-`timetomodel` was created to change that. It describes the data treatment of a model, and also automates common data treatment tasks like building data for training and testing.
-
-As a *data scientist*, experiment with a model in your notebook.
-Load data from static files (e.g. CSV) and try out lags, regressors and so on.
-Compare plots and mean square errors of the models you developed.
-
-As an *engineer*, take over the model description and use it in your production code.
-Often, this would entail not much more than changing the data source (e.g from CSV to a column in the database).
-
-`timetomodel` is supposed to wrap around any fit/predict type model, e.g. from statsmodels or scikit-learn (some work needed here to ensure support).
-
-
-## Features
-
-Here are some features for both data scientists and engineers to enjoy:
-
-* Describe how to load data for outcome and regressor variables. Load from Pandas objects, CSV files, Pandas pickles or databases via SQLAlchemy.
-* Create train & test data, including lags.
-* Timezone awareness support.
-* Custom data transformations, after loading (e.g. to remove duplicate) or only for forecasting (e.g. to apply a BoxCox transformation).
-* Evaluate a model by RMSE, and plot the cumulative error.
-* Support for creating rolling forecasts.
-
-
-## Installation
-
-``pip install timetomodel``
-
-## Example
-
-Here is an example where we describe a solar time series problem, and use ``statsmodels.OLS``, a linear regression model, to forecast one hour ahead:
-
-    import pandas as pd
-    import pytz
-    from datetime import datetime, timedelta
-    from statsmodels.api import OLS
-    from timetomodel import speccing, ModelState, create_fitted_model, evaluate_models
-    from timetomodel.transforming import BoxCoxTransformation
-    from timetomodel.forecasting import make_rolling_forecasts
-
-    data_start = datetime(2015, 3, 1, tzinfo=pytz.utc)
-    data_end = datetime(2015, 10, 31, tzinfo=pytz.utc)
-
-    #### Solar model - 1h ahead  ####
-
-    # spec outcome variable
-    solar_outcome_var_spec = speccing.CSVFileSeriesSpecs(
-        file_path="data.csv",
-        time_column="datetime",
-        value_column="solar_power",
-        name="solar power",
-        feature_transformation=BoxCoxTransformation(lambda2=0.1)
-    )
-    # spec regressor variable
-    regressor_spec_1h = speccing.CSVFileSeriesSpecs(
-        file_path="data.csv",
-        time_column="datetime",
-        value_column="irradiation_forecast1h",
-        name="irradiation forecast",
-        feature_transformation=BoxCoxTransformation(lambda2=0.1)
-    )
-    # spec whole model treatment
-    solar_model1h_specs = speccing.ModelSpecs(
-        outcome_var=solar_outcome_var_spec,
-        model=OLS,
-        frequency=timedelta(minutes=15),
-        horizon=timedelta(hours=1),
-        lags=[lag * 96 for lag in range(1, 8)],  # 7 days (data has daily seasonality)
-        regressors=[regressor_spec_1h],
-        start_of_training=data_start + timedelta(days=30),
-        end_of_testing=data_end,
-        ratio_training_testing_data=2/3,
-        remodel_frequency=timedelta(days=14)  # re-train model every two weeks
-    )
-
-    solar_model1h = create_fitted_model(solar_model1h_specs, "Linear Regression Solar Horizon 1h")
-    # solar_model_1h is now an OLS model object which can be pickled and re-used.
-    # With the solar_model1h_specs in hand, your production code could always re-train a new one,
-    # if the model has become outdated.
-
-    # For data scientists: evaluate model
-    evaluate_models(m1=ModelState(solar_model1h, solar_model1h_specs))
-
-![Evaluation result](https://raw.githubusercontent.com/SeitaBV/timetomodel/master/img/solar-forecast-evaluation.png)
-
-    # For engineers a): Change data sources to use database (hinted)
-    solar_model1h_specs.outcome_var = speccing.DBSeriesSpecs(query=...)
-    solar_model1h_specs.regressors[0] = speccing.DBSeriesSpecs(query=...)
-
-    # For engineers b): Use model to make forecasts for an hour
-    forecasts, model_state = make_rolling_forecasts(
-        start=datetime(2015, 11, 1, tzinfo=pytz.utc),
-        end=datetime(2015, 11, 1, 1, tzinfo=pytz.utc),
-        model_specs=solar_model1h_specs
-    )
-    # model_state might have re-trained a new model automatically, by honoring the remodel_frequency
-
-    
-
```

### Comparing `timetomodel-0.7.2/Readme.md` & `timetomodel-0.7.3/Readme.md`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/img/solar-forecast-evaluation.png` & `timetomodel-0.7.3/img/solar-forecast-evaluation.png`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/setup.cfg` & `timetomodel-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/setup.py` & `timetomodel-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 setup(
     name="timetomodel",
     description="Sane handling of time series data for forecast modelling - with production usage in mind.",
     author="Seita BV",
     author_email="nicolas@seita.nl",
     url="https://github.com/seitabv/timetomodel",
     keywords=["time series", "forecasting"],
-    version="0.7.2",
+    version="0.7.3",
     install_requires=[
-        "pandas",
+        "pandas >= 1.4.0",
         "statsmodels",
         "scikit-learn",
         "matplotlib",
         "numpy",
         "scipy",
         "pytz",
         "python-dateutil >= 2.5",
```

### Comparing `timetomodel-0.7.2/timetomodel/__init__.py` & `timetomodel-0.7.3/timetomodel/__init__.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/featuring.py` & `timetomodel-0.7.3/timetomodel/featuring.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,23 @@
             "a tuple of two datetime objects or one datetime object."
         )
 
     pd_frequency = timedelta_to_pandas_freq_str(specs.frequency)
 
     # easy cases: one or two datetime objects
     if isinstance(time_range, datetime):
-        return pd.date_range(time_range, time_range, closed="left", freq=pd_frequency)
+        return pd.date_range(time_range, time_range, inclusive="left", freq=pd_frequency)
     elif isinstance(time_range, tuple):
         if not timedelta_fits_into(specs.frequency, time_range[1] - time_range[0]):
             raise Exception(
                 "Start & end period (%s to %s) does not cleanly fit a multiple of the model frequency (%s)"
                 % (time_range[0], time_range[1], specs.frequency)
             )
         return pd.date_range(
-            time_range[0], time_range[1], closed="left", freq=pd_frequency
+            time_range[0], time_range[1], inclusive="left", freq=pd_frequency
         )
 
     # special cases: "train" or "test" - we have to calculate from model specs
     length_of_data = specs.end_of_testing - specs.start_of_training
     if time_range == "train":
         end_of_training = (
             specs.start_of_training + length_of_data * specs.ratio_training_testing_data
```

### Comparing `timetomodel-0.7.2/timetomodel/forecasting.py` & `timetomodel-0.7.3/timetomodel/forecasting.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     feature_frame: pd.DataFrame = construct_features(
         (model_specs.start_of_training, end), model_specs
     )
 
     pd_frequency = timedelta_to_pandas_freq_str(model_specs.frequency)
     values = pd.Series(
         index=pd.date_range(
-            start, end, freq=pd_frequency, closed="left", tz=start.tzinfo
+            start, end, freq=pd_frequency, inclusive="left", tz=start.tzinfo
         )
     )
     time_step = start
     model = None
     logger.info("Forecasting from %s to %s" % (start, end))
     while time_step < end:
         model, specs = update_model(
```

### Comparing `timetomodel-0.7.2/timetomodel/modelling.py` & `timetomodel-0.7.3/timetomodel/modelling.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/speccing.py` & `timetomodel-0.7.3/timetomodel/speccing.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,27 +129,27 @@
         with downsampling_method and upsampling_method names (e.g. "mean" and "pad", respectively),
         an optional event_resolution, and keyword params which are to be passed into `pandas.Series.resample`.
         For example:
 
         ```
         resampling_config=dict(
             event_resolution=timedelta(hours=1),
-            closed="left",
+            inclusive="left",
             downsampling_method="sum",
             upsampling_method="reverse_sum",
         )
         ```
 
         Here:
         - the event resolution describes that, before resampling,
           each data point denotes a value over a 1-hour period.
           Being explicit about the event resolution is especially important when the data frequency
           is not the same as the event resolution, for example, in the case of
           upsampling a time series containing hourly averages with only one data point per day.
-        - closed="left" will become an argument to `pandas.Series.resample`.
+        - inclusive="left" will become an argument to `pandas.Series.resample`.
           It denotes that each period in the time series is indexed by its start time.
         - When downsampling, `pandas.Series.resample().sum()` will be called.
         - When upsampling, `pandas.Series.resample().reverse_sum()` will be called.
         Acceptable values for downsampling_method and upsampling_method are (string names of) possible
         re-sample methods offered by pandas plus a timetomodel-version of "reverse_sum".
         "mean" and "pad" are the default values for downsampling and upsampling, respectively.
```

### Comparing `timetomodel-0.7.2/timetomodel/tests/test_forecasting.py` & `timetomodel-0.7.3/timetomodel/tests/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/tests/test_series_specs.py` & `timetomodel-0.7.3/timetomodel/tests/test_series_specs.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/tests/test_timeutils.py` & `timetomodel-0.7.3/timetomodel/tests/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/tests/utils.py` & `timetomodel-0.7.3/timetomodel/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     """
     Create a dummy model. data increases linearly, regressor is constant (useless).
     Use two different ways to define Series specs to test them.
     """
     dt_range = pd.date_range(
         data_start,
         data_start + timedelta(hours=data_range_in_hours),
-        closed="left",
+        inclusive="left",
         freq="1H",
     )
     reg_range = pd.date_range(
         data_start,
         data_start + timedelta(hours=data_range_in_hours) + timedelta(days=1),
-        closed="left",
+        inclusive="left",
         freq="1H",
     )  # 1 additional day of regressor data is available
     outcome_values = [0]
     regressor_values = [5]
     for i in range(1, len(dt_range)):
         outcome_values.append(outcome_values[i - 1] + 1)
     for i in range(1, len(reg_range)):
```

### Comparing `timetomodel-0.7.2/timetomodel/transforming.py` & `timetomodel-0.7.3/timetomodel/transforming.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/utils/debug_utils.py` & `timetomodel-0.7.3/timetomodel/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel/utils/time_utils.py` & `timetomodel-0.7.3/timetomodel/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `timetomodel-0.7.2/timetomodel.egg-info/PKG-INFO` & `timetomodel-0.7.3/timetomodel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,124 @@
 Metadata-Version: 2.1
 Name: timetomodel
-Version: 0.7.2
+Version: 0.7.3
 Summary: Sane handling of time series data for forecast modelling - with production usage in mind.
 Home-page: https://github.com/seitabv/timetomodel
 Author: Seita BV
 Author-email: nicolas@seita.nl
 License: UNKNOWN
+Description: # timetomodel
+        
+        Time series forecasting is a modern data science & engineering challenge.
+        
+        We noticed that these two worlds, data science and engineering of time series forecasting, are not very compatible.
+        Often, work from the data scientist has to be re-implemented by engineers to be used in production.
+        
+        `timetomodel` was created to change that. It describes the data treatment of a model, and also automates common data treatment tasks like building data for training and testing.
+        
+        As a *data scientist*, experiment with a model in your notebook.
+        Load data from static files (e.g. CSV) and try out lags, regressors and so on.
+        Compare plots and mean square errors of the models you developed.
+        
+        As an *engineer*, take over the model description and use it in your production code.
+        Often, this would entail not much more than changing the data source (e.g from CSV to a column in the database).
+        
+        `timetomodel` is supposed to wrap around any fit/predict type model, e.g. from statsmodels or scikit-learn (some work needed here to ensure support).
+        
+        
+        ## Features
+        
+        Here are some features for both data scientists and engineers to enjoy:
+        
+        * Describe how to load data for outcome and regressor variables. Load from Pandas objects, CSV files, Pandas pickles or databases via SQLAlchemy.
+        * Create train & test data, including lags.
+        * Timezone awareness support.
+        * Custom data transformations, after loading (e.g. to remove duplicate) or only for forecasting (e.g. to apply a BoxCox transformation).
+        * Evaluate a model by RMSE, and plot the cumulative error.
+        * Support for creating rolling forecasts.
+        
+        
+        ## Installation
+        
+        ``pip install timetomodel``
+        
+        ## Example
+        
+        Here is an example where we describe a solar time series problem, and use ``statsmodels.OLS``, a linear regression model, to forecast one hour ahead:
+        
+            import pandas as pd
+            import pytz
+            from datetime import datetime, timedelta
+            from statsmodels.api import OLS
+            from timetomodel import speccing, ModelState, create_fitted_model, evaluate_models
+            from timetomodel.transforming import BoxCoxTransformation
+            from timetomodel.forecasting import make_rolling_forecasts
+        
+            data_start = datetime(2015, 3, 1, tzinfo=pytz.utc)
+            data_end = datetime(2015, 10, 31, tzinfo=pytz.utc)
+        
+            #### Solar model - 1h ahead  ####
+        
+            # spec outcome variable
+            solar_outcome_var_spec = speccing.CSVFileSeriesSpecs(
+                file_path="data.csv",
+                time_column="datetime",
+                value_column="solar_power",
+                name="solar power",
+                feature_transformation=BoxCoxTransformation(lambda2=0.1)
+            )
+            # spec regressor variable
+            regressor_spec_1h = speccing.CSVFileSeriesSpecs(
+                file_path="data.csv",
+                time_column="datetime",
+                value_column="irradiation_forecast1h",
+                name="irradiation forecast",
+                feature_transformation=BoxCoxTransformation(lambda2=0.1)
+            )
+            # spec whole model treatment
+            solar_model1h_specs = speccing.ModelSpecs(
+                outcome_var=solar_outcome_var_spec,
+                model=OLS,
+                frequency=timedelta(minutes=15),
+                horizon=timedelta(hours=1),
+                lags=[lag * 96 for lag in range(1, 8)],  # 7 days (data has daily seasonality)
+                regressors=[regressor_spec_1h],
+                start_of_training=data_start + timedelta(days=30),
+                end_of_testing=data_end,
+                ratio_training_testing_data=2/3,
+                remodel_frequency=timedelta(days=14)  # re-train model every two weeks
+            )
+        
+            solar_model1h = create_fitted_model(solar_model1h_specs, "Linear Regression Solar Horizon 1h")
+            # solar_model_1h is now an OLS model object which can be pickled and re-used.
+            # With the solar_model1h_specs in hand, your production code could always re-train a new one,
+            # if the model has become outdated.
+        
+            # For data scientists: evaluate model
+            evaluate_models(m1=ModelState(solar_model1h, solar_model1h_specs))
+        
+        ![Evaluation result](https://raw.githubusercontent.com/SeitaBV/timetomodel/master/img/solar-forecast-evaluation.png)
+        
+            # For engineers a): Change data sources to use database (hinted)
+            solar_model1h_specs.outcome_var = speccing.DBSeriesSpecs(query=...)
+            solar_model1h_specs.regressors[0] = speccing.DBSeriesSpecs(query=...)
+        
+            # For engineers b): Use model to make forecasts for an hour
+            forecasts, model_state = make_rolling_forecasts(
+                start=datetime(2015, 11, 1, tzinfo=pytz.utc),
+                end=datetime(2015, 11, 1, 1, tzinfo=pytz.utc),
+                model_specs=solar_model1h_specs
+            )
+            # model_state might have re-trained a new model automatically, by honoring the remodel_frequency
+        
+            
 Keywords: time series,forecasting
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# timetomodel
-
-Time series forecasting is a modern data science & engineering challenge.
-
-We noticed that these two worlds, data science and engineering of time series forecasting, are not very compatible.
-Often, work from the data scientist has to be re-implemented by engineers to be used in production.
-
-`timetomodel` was created to change that. It describes the data treatment of a model, and also automates common data treatment tasks like building data for training and testing.
-
-As a *data scientist*, experiment with a model in your notebook.
-Load data from static files (e.g. CSV) and try out lags, regressors and so on.
-Compare plots and mean square errors of the models you developed.
-
-As an *engineer*, take over the model description and use it in your production code.
-Often, this would entail not much more than changing the data source (e.g from CSV to a column in the database).
-
-`timetomodel` is supposed to wrap around any fit/predict type model, e.g. from statsmodels or scikit-learn (some work needed here to ensure support).
-
-
-## Features
-
-Here are some features for both data scientists and engineers to enjoy:
-
-* Describe how to load data for outcome and regressor variables. Load from Pandas objects, CSV files, Pandas pickles or databases via SQLAlchemy.
-* Create train & test data, including lags.
-* Timezone awareness support.
-* Custom data transformations, after loading (e.g. to remove duplicate) or only for forecasting (e.g. to apply a BoxCox transformation).
-* Evaluate a model by RMSE, and plot the cumulative error.
-* Support for creating rolling forecasts.
-
-
-## Installation
-
-``pip install timetomodel``
-
-## Example
-
-Here is an example where we describe a solar time series problem, and use ``statsmodels.OLS``, a linear regression model, to forecast one hour ahead:
-
-    import pandas as pd
-    import pytz
-    from datetime import datetime, timedelta
-    from statsmodels.api import OLS
-    from timetomodel import speccing, ModelState, create_fitted_model, evaluate_models
-    from timetomodel.transforming import BoxCoxTransformation
-    from timetomodel.forecasting import make_rolling_forecasts
-
-    data_start = datetime(2015, 3, 1, tzinfo=pytz.utc)
-    data_end = datetime(2015, 10, 31, tzinfo=pytz.utc)
-
-    #### Solar model - 1h ahead  ####
-
-    # spec outcome variable
-    solar_outcome_var_spec = speccing.CSVFileSeriesSpecs(
-        file_path="data.csv",
-        time_column="datetime",
-        value_column="solar_power",
-        name="solar power",
-        feature_transformation=BoxCoxTransformation(lambda2=0.1)
-    )
-    # spec regressor variable
-    regressor_spec_1h = speccing.CSVFileSeriesSpecs(
-        file_path="data.csv",
-        time_column="datetime",
-        value_column="irradiation_forecast1h",
-        name="irradiation forecast",
-        feature_transformation=BoxCoxTransformation(lambda2=0.1)
-    )
-    # spec whole model treatment
-    solar_model1h_specs = speccing.ModelSpecs(
-        outcome_var=solar_outcome_var_spec,
-        model=OLS,
-        frequency=timedelta(minutes=15),
-        horizon=timedelta(hours=1),
-        lags=[lag * 96 for lag in range(1, 8)],  # 7 days (data has daily seasonality)
-        regressors=[regressor_spec_1h],
-        start_of_training=data_start + timedelta(days=30),
-        end_of_testing=data_end,
-        ratio_training_testing_data=2/3,
-        remodel_frequency=timedelta(days=14)  # re-train model every two weeks
-    )
-
-    solar_model1h = create_fitted_model(solar_model1h_specs, "Linear Regression Solar Horizon 1h")
-    # solar_model_1h is now an OLS model object which can be pickled and re-used.
-    # With the solar_model1h_specs in hand, your production code could always re-train a new one,
-    # if the model has become outdated.
-
-    # For data scientists: evaluate model
-    evaluate_models(m1=ModelState(solar_model1h, solar_model1h_specs))
-
-![Evaluation result](https://raw.githubusercontent.com/SeitaBV/timetomodel/master/img/solar-forecast-evaluation.png)
-
-    # For engineers a): Change data sources to use database (hinted)
-    solar_model1h_specs.outcome_var = speccing.DBSeriesSpecs(query=...)
-    solar_model1h_specs.regressors[0] = speccing.DBSeriesSpecs(query=...)
-
-    # For engineers b): Use model to make forecasts for an hour
-    forecasts, model_state = make_rolling_forecasts(
-        start=datetime(2015, 11, 1, tzinfo=pytz.utc),
-        end=datetime(2015, 11, 1, 1, tzinfo=pytz.utc),
-        model_specs=solar_model1h_specs
-    )
-    # model_state might have re-trained a new model automatically, by honoring the remodel_frequency
-
-    
-
```

### Comparing `timetomodel-0.7.2/timetomodel.egg-info/SOURCES.txt` & `timetomodel-0.7.3/timetomodel.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 timetomodel/tests/__init__.py
 timetomodel/tests/test_forecasting.py
 timetomodel/tests/test_series_specs.py
 timetomodel/tests/test_timeutils.py
 timetomodel/tests/utils.py
 timetomodel/utils/__init__.py
 timetomodel/utils/debug_utils.py
+timetomodel/utils/log_utils.py
 timetomodel/utils/time_utils.py
```

