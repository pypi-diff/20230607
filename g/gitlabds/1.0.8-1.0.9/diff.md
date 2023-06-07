# Comparing `tmp/gitlabds-1.0.8.tar.gz` & `tmp/gitlabds-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabds-1.0.8.tar", last modified: Mon Oct 25 18:27:18 2021, max compression
+gzip compressed data, was "gitlabds-1.0.9.tar", last modified: Mon Nov  1 22:12:05 2021, max compression
```

## Comparing `gitlabds-1.0.8.tar` & `gitlabds-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 18:27:18.038828 gitlabds-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1238 2021-10-25 18:27:08.000000 gitlabds-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19834 2021-10-25 18:27:18.037828 gitlabds-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    19508 2021-10-25 18:27:08.000000 gitlabds-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 18:27:18.035828 gitlabds-1.0.8/gitlabds/
--rw-rw-rw-   0 root         (0) root         (0)      339 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4795 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/dummies.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/feature_reduction.py
--rw-rw-rw-   0 root         (0) root         (0)     3577 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/mars_modeling.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/missing_fill.py
--rw-rw-rw-   0 root         (0) root         (0)    12736 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/model_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/outliers.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2021-10-25 18:27:08.000000 gitlabds-1.0.8/gitlabds/split_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 18:27:18.037828 gitlabds-1.0.8/gitlabds.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19834 2021-10-25 18:27:17.000000 gitlabds-1.0.8/gitlabds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      377 2021-10-25 18:27:17.000000 gitlabds-1.0.8/gitlabds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-25 18:27:17.000000 gitlabds-1.0.8/gitlabds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2021-10-25 18:27:17.000000 gitlabds-1.0.8/gitlabds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-10-25 18:27:17.000000 gitlabds-1.0.8/gitlabds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-25 18:27:18.038828 gitlabds-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      883 2021-10-25 18:27:08.000000 gitlabds-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:12:05.192118 gitlabds-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2021-11-01 22:11:55.000000 gitlabds-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19923 2021-11-01 22:12:05.191118 gitlabds-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    19597 2021-11-01 22:11:55.000000 gitlabds-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:12:05.189118 gitlabds-1.0.9/gitlabds/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4795 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/dummies.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/feature_reduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/mars_modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/missing_fill.py
+-rw-rw-rw-   0 root         (0) root         (0)    12971 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/model_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5593 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/outliers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2021-11-01 22:11:55.000000 gitlabds-1.0.9/gitlabds/split_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:12:05.191118 gitlabds-1.0.9/gitlabds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19923 2021-11-01 22:12:05.000000 gitlabds-1.0.9/gitlabds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      377 2021-11-01 22:12:05.000000 gitlabds-1.0.9/gitlabds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-01 22:12:05.000000 gitlabds-1.0.9/gitlabds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2021-11-01 22:12:05.000000 gitlabds-1.0.9/gitlabds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-11-01 22:12:05.000000 gitlabds-1.0.9/gitlabds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-11-01 22:12:05.192118 gitlabds-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      883 2021-11-01 22:11:55.000000 gitlabds-1.0.9/setup.py
```

### Comparing `gitlabds-1.0.8/LICENSE` & `gitlabds-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/PKG-INFO` & `gitlabds-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabds
-Version: 1.0.8
+Version: 1.0.9
 Summary: Gitlab Data Science and Modeling Tools
 Home-page: https://gitlab.com/gitlab-data/gitlabds
 Author: Kevin Dietz
 Author-email: kdietz@gitlab.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -381,25 +381,25 @@
 - _**show_graphs**_ : Set to `True` to show visualizations
 - _**f_score**_ : Cut point for determining a correct classification. Must also set classification to `True` to enable.
 - _**classification**_ : Set to `True` to show classification model metrics (accuracy, precision, recall, F1). Set show_graphs to `True` to display confusion matrix.
 - _**algo**_ : Select the algorythm used to display additional model metrics. Currently supports `mars` and `xgb`
 
 
 #### Returns
-- Print of model metrics.
+- Prints and dataframes for model metrics and lift.
 
 #### Examples:
 		
 ```
-#Display model metrics from an XGBoost model. Show classification metrics using a cut point of 0.30 F-Score
-gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=True, f_score = 0.3, classification=True, algo='xgb')
+#Display model metrics from an XGBoost model. Return classification metrics using a cut point of 0.30 F-Score
+model_metrics, lift, class_metrics = gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=True, f_score = 0.3, classification=True, algo='xgb')
 ```
 ```
-#Display model metrics from a MARS model. Do not show classification metrics and suppress visualizations
-gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=False, classification=False, algo='mars')
+#Display model metrics from a MARS model. Do not return classification metrics and suppress visualizations
+model_metrics, lift = gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=False, classification=False, algo='mars')
 ```
 </details>
 
 ## Gitlab Data Science
 
 The [handbook](https://about.gitlab.com/handbook/business-technology/data-team/organization/data-science/) is the single source of truth for all of our documentation.
```

### Comparing `gitlabds-1.0.8/README.md` & `gitlabds-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -368,25 +368,25 @@
 - _**show_graphs**_ : Set to `True` to show visualizations
 - _**f_score**_ : Cut point for determining a correct classification. Must also set classification to `True` to enable.
 - _**classification**_ : Set to `True` to show classification model metrics (accuracy, precision, recall, F1). Set show_graphs to `True` to display confusion matrix.
 - _**algo**_ : Select the algorythm used to display additional model metrics. Currently supports `mars` and `xgb`
 
 
 #### Returns
-- Print of model metrics.
+- Prints and dataframes for model metrics and lift.
 
 #### Examples:
 		
 ```
-#Display model metrics from an XGBoost model. Show classification metrics using a cut point of 0.30 F-Score
-gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=True, f_score = 0.3, classification=True, algo='xgb')
+#Display model metrics from an XGBoost model. Return classification metrics using a cut point of 0.30 F-Score
+model_metrics, lift, class_metrics = gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=True, f_score = 0.3, classification=True, algo='xgb')
 ```
 ```
-#Display model metrics from a MARS model. Do not show classification metrics and suppress visualizations
-gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=False, classification=False, algo='mars')
+#Display model metrics from a MARS model. Do not return classification metrics and suppress visualizations
+model_metrics, lift = gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=False, classification=False, algo='mars')
 ```
 </details>
 
 ## Gitlab Data Science
 
 The [handbook](https://about.gitlab.com/handbook/business-technology/data-team/organization/data-science/) is the single source of truth for all of our documentation.
```

### Comparing `gitlabds-1.0.8/gitlabds/dummies.py` & `gitlabds-1.0.9/gitlabds/dummies.py`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/gitlabds/feature_reduction.py` & `gitlabds-1.0.9/gitlabds/feature_reduction.py`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/gitlabds/mars_modeling.py` & `gitlabds-1.0.9/gitlabds/mars_modeling.py`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/gitlabds/missing_fill.py` & `gitlabds-1.0.9/gitlabds/missing_fill.py`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/gitlabds/model_metrics.py` & `gitlabds-1.0.9/gitlabds/model_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
               ]
 
     metricx = pd.DataFrame(metricx, columns=['metric', 'train', 'test'])
     metricx['deviation_pct'] = (metricx['test'] - metricx['train']) / metricx['train']
     
     print('\nModel Metrics')
     format_dict = {'train':'{0:,.4}', 'test': '{0:.4}', 'deviation_pct': '{:.2%}'}
+
+    metricx.set_index('metric', inplace=True)
     display(metricx.style.format(format_dict))
     
     # Determine log-loss cutpoint
     multi=10000
     class_ratio = [np.round(score_test['actual'].mean(),3), 1-np.round(score_test['actual'].mean(),3)]
     
     actuals=[]
@@ -110,14 +112,15 @@
         
         classification_metricx = pd.DataFrame(classification_metricx, columns=['metric', 'train', 'test'])
         classification_metricx['deviation_pct'] = (classification_metricx['test'] - classification_metricx['train']) / classification_metricx['train']
         
         print('Classification Metrics')
         print(f'Using an F-Score of {f_score}')
         format_dict = {'train':'{0:,.4}', 'test': '{0:.4}', 'deviation_pct': '{:.2%}'}
+        classification_metricx.set_index('metric', inplace=True)
         display(classification_metricx.style.format(format_dict))
         
         print('Accuracy: % of Accurate Predictions. (True Positives + True Negatives) / Total Population')
         print('Precision: % of true positives to all positives. True Positives / (True Positives + False Positives)')
         print('Recall: % of postive cases accurately classified. True Positives / (True Positives + False Negatives)')
         print('F1 Score: The harmonic mean between precision and recall.')
             
@@ -241,9 +244,15 @@
         plt.title('lift')
         plt.ylabel("% of Total Outcome")
         plt.xticks(np.arange(1, 11, step=1))
         plt.show()
             
     print('\nLift/Gains Table')
     display(lift)
-     
-    return
+    
+    if classification == True:
+        return metricx, lift, classification_metricx
+    
+    else:
+        return metricx, lift
+    
+
```

### Comparing `gitlabds-1.0.8/gitlabds/outliers.py` & `gitlabds-1.0.9/gitlabds/outliers.py`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/gitlabds/split_data.py` & `gitlabds-1.0.9/gitlabds/split_data.py`

 * *Files identical despite different names*

### Comparing `gitlabds-1.0.8/gitlabds.egg-info/PKG-INFO` & `gitlabds-1.0.9/gitlabds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabds
-Version: 1.0.8
+Version: 1.0.9
 Summary: Gitlab Data Science and Modeling Tools
 Home-page: https://gitlab.com/gitlab-data/gitlabds
 Author: Kevin Dietz
 Author-email: kdietz@gitlab.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -381,25 +381,25 @@
 - _**show_graphs**_ : Set to `True` to show visualizations
 - _**f_score**_ : Cut point for determining a correct classification. Must also set classification to `True` to enable.
 - _**classification**_ : Set to `True` to show classification model metrics (accuracy, precision, recall, F1). Set show_graphs to `True` to display confusion matrix.
 - _**algo**_ : Select the algorythm used to display additional model metrics. Currently supports `mars` and `xgb`
 
 
 #### Returns
-- Print of model metrics.
+- Prints and dataframes for model metrics and lift.
 
 #### Examples:
 		
 ```
-#Display model metrics from an XGBoost model. Show classification metrics using a cut point of 0.30 F-Score
-gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=True, f_score = 0.3, classification=True, algo='xgb')
+#Display model metrics from an XGBoost model. Return classification metrics using a cut point of 0.30 F-Score
+model_metrics, lift, class_metrics = gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=True, f_score = 0.3, classification=True, algo='xgb')
 ```
 ```
-#Display model metrics from a MARS model. Do not show classification metrics and suppress visualizations
-gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=False, classification=False, algo='mars')
+#Display model metrics from a MARS model. Do not return classification metrics and suppress visualizations
+model_metrics, lift = gitlabds.model_metrics(model=model, x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, show_graphs=False, classification=False, algo='mars')
 ```
 </details>
 
 ## Gitlab Data Science
 
 The [handbook](https://about.gitlab.com/handbook/business-technology/data-team/organization/data-science/) is the single source of truth for all of our documentation.
```

### Comparing `gitlabds-1.0.8/setup.py` & `gitlabds-1.0.9/setup.py`

 * *Files identical despite different names*

