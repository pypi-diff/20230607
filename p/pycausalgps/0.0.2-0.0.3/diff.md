# Comparing `tmp/pycausalgps-0.0.2.tar.gz` & `tmp/pycausalgps-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycausalgps-0.0.2.tar", last modified: Mon Apr  3 21:19:29 2023, max compression
+gzip compressed data, was "dist/pycausalgps-0.0.3.tar", last modified: Wed Jun  7 20:27:28 2023, max compression
```

## Comparing `pycausalgps-0.0.2.tar` & `pycausalgps-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-03 21:19:29.227465 pycausalgps-0.0.2/
--rw-r--r--   0 nak443     (502) staff       (20)    35148 2021-04-14 20:13:44.000000 pycausalgps-0.0.2/LICENSE
--rw-r--r--   0 nak443     (502) staff       (20)       34 2020-07-10 05:31:32.000000 pycausalgps-0.0.2/MANIFEST.in
--rw-r--r--   0 nak443     (502) staff       (20)     2603 2023-04-03 21:19:29.226958 pycausalgps-0.0.2/PKG-INFO
--rw-r--r--   0 nak443     (502) staff       (20)     1439 2023-04-03 21:17:18.000000 pycausalgps-0.0.2/README.md
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-03 21:19:29.221422 pycausalgps-0.0.2/pycausalgps/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2021-04-14 14:54:15.000000 pycausalgps-0.0.2/pycausalgps/__init__.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-03 21:19:29.224843 pycausalgps-0.0.2/pycausalgps/base/
--rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/base/__init__.py
--rw-r--r--   0 nak443     (502) staff       (20)     5181 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/base/utils.py
--rw-r--r--   0 nak443     (502) staff       (20)    10192 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/gps.py
--rw-r--r--   0 nak443     (502) staff       (20)      830 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/log.py
--rw-r--r--   0 nak443     (502) staff       (20)    18195 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/pseudo_population.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-03 21:19:29.226068 pycausalgps-0.0.2/pycausalgps/rscripts/
--rw-r--r--   0 nak443     (502) staff       (20)      532 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/rscripts/__init__.py
--rw-r--r--   0 nak443     (502) staff       (20)     6805 2023-04-03 21:16:42.000000 pycausalgps-0.0.2/pycausalgps/rscripts/rfunctions.py
-drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-04-03 21:19:29.224178 pycausalgps-0.0.2/pycausalgps.egg-info/
--rw-r--r--   0 nak443     (502) staff       (20)     2603 2023-04-03 21:19:29.000000 pycausalgps-0.0.2/pycausalgps.egg-info/PKG-INFO
--rw-r--r--   0 nak443     (502) staff       (20)      396 2023-04-03 21:19:29.000000 pycausalgps-0.0.2/pycausalgps.egg-info/SOURCES.txt
--rw-r--r--   0 nak443     (502) staff       (20)        1 2023-04-03 21:19:29.000000 pycausalgps-0.0.2/pycausalgps.egg-info/dependency_links.txt
--rw-r--r--   0 nak443     (502) staff       (20)       12 2023-04-03 21:19:29.000000 pycausalgps-0.0.2/pycausalgps.egg-info/top_level.txt
--rw-r--r--   0 nak443     (502) staff       (20)       38 2023-04-03 21:19:29.227643 pycausalgps-0.0.2/setup.cfg
--rw-r--r--   0 nak443     (502) staff       (20)     1487 2023-04-03 21:18:45.000000 pycausalgps-0.0.2/setup.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/
+-rw-r--r--   0 nak443     (502) staff       (20)    35148 2021-04-14 20:13:44.000000 pycausalgps-0.0.3/LICENSE
+-rw-r--r--   0 nak443     (502) staff       (20)       34 2020-07-10 05:31:32.000000 pycausalgps-0.0.3/MANIFEST.in
+-rw-r--r--   0 nak443     (502) staff       (20)     7833 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/PKG-INFO
+-rw-r--r--   0 nak443     (502) staff       (20)     6649 2023-06-07 20:22:33.000000 pycausalgps-0.0.3/README.md
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps/
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2021-04-14 14:54:15.000000 pycausalgps-0.0.3/pycausalgps/__init__.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps/base/
+-rw-r--r--   0 nak443     (502) staff       (20)        0 2023-04-03 21:16:42.000000 pycausalgps-0.0.3/pycausalgps/base/__init__.py
+-rw-r--r--   0 nak443     (502) staff       (20)     5714 2023-05-04 22:11:50.000000 pycausalgps-0.0.3/pycausalgps/base/utils.py
+-rw-r--r--   0 nak443     (502) staff       (20)     5295 2023-06-07 20:18:56.000000 pycausalgps-0.0.3/pycausalgps/erf_helper.py
+-rw-r--r--   0 nak443     (502) staff       (20)     4022 2023-06-07 20:18:56.000000 pycausalgps-0.0.3/pycausalgps/exposure_response_function.py
+-rw-r--r--   0 nak443     (502) staff       (20)    12520 2023-05-04 22:11:50.000000 pycausalgps-0.0.3/pycausalgps/gps.py
+-rw-r--r--   0 nak443     (502) staff       (20)      830 2023-04-03 21:16:42.000000 pycausalgps-0.0.3/pycausalgps/log.py
+-rw-r--r--   0 nak443     (502) staff       (20)    27291 2023-06-07 20:18:56.000000 pycausalgps-0.0.3/pycausalgps/pseudo_population.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps/rscripts/
+-rw-r--r--   0 nak443     (502) staff       (20)      546 2023-06-07 20:18:56.000000 pycausalgps-0.0.3/pycausalgps/rscripts/__init__.py
+-rw-r--r--   0 nak443     (502) staff       (20)     8591 2023-06-07 20:18:56.000000 pycausalgps-0.0.3/pycausalgps/rscripts/rfunctions.py
+drwxr-xr-x   0 nak443     (502) staff       (20)        0 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps.egg-info/
+-rw-r--r--   0 nak443     (502) staff       (20)     7833 2023-06-07 20:27:27.000000 pycausalgps-0.0.3/pycausalgps.egg-info/PKG-INFO
+-rw-r--r--   0 nak443     (502) staff       (20)      464 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps.egg-info/SOURCES.txt
+-rw-r--r--   0 nak443     (502) staff       (20)        1 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps.egg-info/dependency_links.txt
+-rw-r--r--   0 nak443     (502) staff       (20)       12 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/pycausalgps.egg-info/top_level.txt
+-rw-r--r--   0 nak443     (502) staff       (20)       38 2023-06-07 20:27:28.000000 pycausalgps-0.0.3/setup.cfg
+-rw-r--r--   0 nak443     (502) staff       (20)     1487 2023-06-07 20:21:35.000000 pycausalgps-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pycausalgps-0.0.2/LICENSE` & `pycausalgps-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycausalgps-0.0.2/pycausalgps/base/utils.py` & `pycausalgps-0.0.3/pycausalgps/base/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,30 +35,37 @@
     Parameters
     ----------
     sample_size: int
         A number of required data samples.
     seed_val: int 
         A seed value for generating reproducible data.
     outcome_sd: int
-        TBD
+        Standard deviation used to generate the outcome in the synthetic 
+        data set.
     gps_spec: int
-        TBD
+        A numerical value (1-7) that indicates the GPS model used to generate 
+        synthetic data. See the code for more details.
     cova_spec: int
-        TBD
-
+        A numerical value (1-2) to modify the covariates. See the code for 
+        more details.
+        
     Returns
     -------
     data: pd.DataFrame
         A dataframe containing the generated data.
 
     >>> md = generate_syn_pop(100)
     >>> len(md)
     100
     """
     
+    if sample_size < 1:
+        raise ValueError("sample_size must be greater than 0")
+
+
     random.seed(seed_val)
 
     mean = [0,0,0,0]
     cov = [[1,0,0,0],[0,1,0,0],[0,0,1,0],[0,0,0,1]]
     cf = np.random.multivariate_normal(mean, cov, sample_size).T
 
     cf5 = np.random.choice([-2,-1,0,1,2], size = sample_size, replace=True)
@@ -66,43 +73,39 @@
 
     if  gps_spec == 1:
         treat = ((- 0.8 + 0.1 * cf[0] + 0.1 * cf[1] - 0.1 * cf[2] +
                     0.2 * cf[3] + 0.1 * cf5 + 0.1 * cf6) * 9 + 17  +
                     np.random.normal(loc=0.0, scale = 5, size=sample_size))
 
     elif gps_spec == 2:
-
         treat = ((- 0.8 + 0.1 * cf[0,:] + 0.1 * cf[1,:] - 0.1 * cf[2,:]
                   + 0.2 * cf[3,:] + 0.1 * cf5 + 0.1 * cf6) * 15 + 22 +
                    np.random.standard_t(size=sample_size,df=2))
 
         treat = pd.DataFrame({'t':treat})
         treat.loc[treat.t < -5, 't'] = -5
         treat.loc[treat.t > 25, 't'] = 25
 
         treat = treat['t'].tolist() 
 
     elif gps_spec == 3:
-        
         treat = ((- 0.8 + 0.1 * cf[ 0, :] + 0.1 * cf[ 1, :]- 0.1 *cf[ 2,:] 
            + 0.2 * cf [3, :]
            + 0.1 * cf5 + 0.1 * cf6) * 9
            + 1.5 * pow(cf[ 2, :],2) 
            + np.random.normal(loc=0, scale = 5, size=sample_size) + 15)
 
     elif gps_spec == 4:
-        
         treat = (49 * np.exp((-0.8 + 0.1 * cf[ 0,:] 
                 + 0.1 * cf[ 1, :] - 0.1 * cf[ 2, :]
                 + 0.2 * cf[ 3, :] + 0.1 * cf5 + 0.1 * cf6))
                 / (1 + np.exp((-0.8 + 0.1 * cf[0,:] 
                 + 0.1 * cf[ 1, :] - 0.1 * cf[ 3, :]
                 + 0.2 * cf[ 3, :] + 0.1 * cf5 + 0.1 * cf6))) - 6 
                 + np.random.normal(loc=0, scale=5, size=sample_size))
-        
     elif gps_spec == 5:
         treat = (42 / (1 + np.exp((-0.8 + 0.1 * cf[ 0, :] 
                 + 0.1 * cf[ 1, :]- 0.1 * cf[ 3, :]
                 + 0.2 * cf[3,:] + 0.1 * cf5 + 0.1 * cf6))) - 18 
                 + np.random.normal(loc=0, scale=5, size=sample_size))
     elif gps_spec == 6:
         treat = (np.log(abs(-0.8 + 0.1 * cf[ 0, :] + 0.1 * cf[ 1, :] 
@@ -125,32 +128,33 @@
                   (2 * cf5[i]) - (2 * cf6[i]) +
                   (treat[i]-20) * (0.1 + 0.1 * cf[3,i] + 0.1 * cf5[i] +
                    0.1 * pow(cf[2,i],2) - pow(0.13,2) * pow(treat[i] - 20,2)))
                 ) + np.random.normal(loc=0, scale=outcome_sd,size=1))[0]
 
 
     if cova_spec == 1:
-        pass
+        raise NotImplementedError("cova_spec 1 not implemented yet.")
     elif cova_spec == 2:
-        cf[1,:] = np.exp(cf[0,:]/2)
-        cf[2,:] = (cf[1,:]/(1+np.exp(cf[0,:])))+10
-        cf[3,:] = (cf[0,:] * cf[2,:]/25 + 0.6) ^ 3
-        cf[4,:] = (cf[1,:] + cf[3,:] + 20) ^ 2
+        cf[0,:] = np.exp(cf[0,:]/2)
+        cf[1,:] = (cf[1,:]/(1+np.exp(cf[0,:])))+10
+        cf[2,:] = (cf[0,:] * cf[2,:]/25 + 0.6) ** 3
+        cf[3,:] = (cf[1,:] + cf[3,:] + 20) ** 2
     else:
         raise ValueError(f"cova_spec:  {cova_spec} is not a valid value.")
 
     
-    data = pd.DataFrame({'Y':Y, 
-                                   'treat':treat,
-                                   'cf1':cf[0,:],
-                                   'cf2':cf[1,:],
-                                   'cf3':cf[2,:],
-                                   'cf4':cf[3,:],
-                                   'cf5':cf5,
-                                   'cf6':cf6})
+    data = pd.DataFrame({'id': range(1,sample_size+1),
+                         'Y':Y, 
+                         'treat':treat,
+                         'cf1':cf[0,:],
+                         'cf2':cf[1,:],
+                         'cf3':cf[2,:],
+                         'cf4':cf[3,:],
+                         'cf5':cf5,
+                         'cf6':cf6})
 
     return data
 
 
 
 def human_readible_size(nbytes):
     """
@@ -158,8 +162,13 @@
     """
     suffixes = ['B', 'KB', 'MB', 'GB', 'TB', 'PB']
     i = 0
     while nbytes >= 1024 and i < len(suffixes)-1:
         nbytes /= 1024.
         i += 1
 
-    return f"{nbytes:.2f} {suffixes[i]}"
+    return f"{nbytes:.2f} {suffixes[i]}"
+
+
+
+if __name__ == "__main__":
+    data = generate_syn_pop(sample_size=1000, seed_val=456, outcome_sd=0.25, gps_spec=1, cova_spec=2)
```

### Comparing `pycausalgps-0.0.2/pycausalgps/gps.py` & `pycausalgps-0.0.3/pycausalgps/gps.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,27 +21,68 @@
     Create a GPS object based on provided parameters.
 
     GPS object supports continuous treatment with numerical or categorical
     confounders.
 
     Parameters
     ----------
+
     data: pd.DataFrame
         A pandas DataFrame that contains the data for the GPS computation.
     params : dict
-        A dictionary of gps parameters.
+        A dictionary of gps parameters. This includes the folowing required
+        parameters:
+
+            - gps_density: str
+                A string that indicates the density estimation method to be
+                used. Available options are "normal" and "kernel".
+            - exposure_column: str  
+                A string that indicates the name of the exposure column.
+            - covariate_column_num: list
+                A list of strings that indicates the names of the numerical
+                covariate columns.
+            - covariate_column_cat: list
+                A list of strings that indicates the names of the categorical
+                covariate columns.
+            - libs: dict
+                A dictionary of libraries and their parameters. Currently only
+                xgboost is supported. Any parameters for hypertuning the 
+                xgboost model can be passed including:
+
+                    - n_estimators: int
+                        Number of trees to fit.
+                    - learning_rate: float
+                        Learning rate for the xgboost model.
+                    - max_depth: int
+                        Maximum depth of a tree.
+                    - test_rate: float
+                        The proportion of the data to be used for testing.
+                    - random_state: int
+                        Random state for the xgboost model.
+
+    Returns
+    -------
+
+    GeneralizedPropensityScore object that includes the following attributes:
+        - data: pd.DataFrame
+            The gps and auxilary columns.
+        - gps_minmax: list
+            A list of the minimum and maximum gps values.
+        - training_report: dict
+            A dictionary of the training report for the xgboost model.
     """
     
     def __init__(self, data: pd.DataFrame, params: dict) -> None:
-
         self.data = data
         self.params = params
         self.training_report = {}
         self.results = None
-        self.compute_gps()
+        self._check_data()
+        self._check_params()
+        self._compute_gps()
 
     @property
     def data(self) -> pd.DataFrame:
         return self.__data
     
     @data.setter
     def data(self, value: pd.DataFrame) -> None:
@@ -62,23 +103,43 @@
 
     def __str__(self) -> str:
         return f"GeneralizedPropensityScore({len(self.data)} rows)"
 
     def __repr__(self) -> str:
         return (f"GeneralizedPropensityScore(data={self.data},"
                 f"params={self.params})")
+    
+
+    def _check_data(self):
+        """
+        Check if the data is in the correct format.
+        """
+        #TODO: add more checks
+        pass
+
+    def _check_params(self):
+        """
+        Check if the params are in the correct format.
+        """
+
+        required_params = ["gps_density", "exposure_column", 
+                           "covariate_column_num", "covariate_column_cat", 
+                           "libs"]
+        
+        for param in required_params:
+            if not param in self.params.keys():
+                raise ValueError(f"Required parameter {param} is missing.")
 
     def compute_gps(self) -> None:
         """
         Returns Generalized Propensity Score (GPS) value based on input 
         parameters.
         """
 
-        libs = nested_get(self.params,
-                          ["gps_params", "libs"])
+        libs = nested_get(self.params, ["libs"])
         
         first_level_keys = list(libs.keys())
         
         if len(first_level_keys) > 1:
             raise ValueError("Multiple libraries are not supported yet.")
         
         lib_name = first_level_keys[0]
@@ -90,56 +151,59 @@
             for key in ["gps", "e_gps_pred", "e_gps_std", "w_resid"]:
                 if not key in gps_res.keys():
                     raise ValueError(f"Key {key} does not exist in "
                                      f"the gps_res.")
             
             gps_min, gps_max = gps_res["gps"].min(), gps_res["gps"].max()
             gps_standardized = (gps_res["gps"] - gps_min) / (gps_max - gps_min)    
-            self.results = {"data":pd.DataFrame(
+            results = {"data":pd.DataFrame(
                                        {"id": self.data["id"],
                                         "gps": gps_res["gps"],
                                         "gps_standardized": gps_standardized,
                                         "e_gps_pred": gps_res["e_gps_pred"],
                                         "e_gps_std_pred": gps_res["e_gps_std"],
                                         "w_resid": gps_res["w_resid"]}),
-                                "gps_minmax":[gps_min, gps_max],
-                                "training_report": self.training_report
+                        "gps_minmax":[gps_min, gps_max],
+                        "gps_density": self.params["gps_density"],
+                        "training_report": self.training_report,
             }
-           
+            return results
+
         else:
             LOGGER.warning(f" GPS computing approach (approach): "
                            f" {self.params['approach']}  is not defined.")
+            return None
+
 
+    def _compute_gps(self) -> None:
+        """
+        Compute GPS based on the provided parameters.
+        """
+        self.results = self.compute_gps()
 
     def compute_gps_xgboost(self) -> dict:
         """
         Compute GPS using XGBoost library.
         """
 
         # select columns that needs to be included.
         # TODO: add checks to make sure that all columns exist.
         # TODO: Move all core functions under base module. The user should be able to compute 
         # different parameters without using the class (provided that all information is given).
         
         # preprocess data   
-        num_cols = nested_get(self.params,
-                              ["gps_params", 
-                               "covariate_column_num"])
+        num_cols = nested_get(self.params, ["covariate_column_num"])
         
         X_num = self.data[num_cols]
 
-        exposure_col = nested_get(self.params,
-                                    ["gps_params",
-                                     "exposure_column"])
+        exposure_col = nested_get(self.params, ["exposure_column"])
 
         y = self.data[exposure_col]
  
-        cat_cols = nested_get(self.params,
-                              ["gps_params",
-                               "covariate_column_cat"])
+        cat_cols = nested_get(self.params, ["covariate_column_cat"])
 
         X_cat = self.data[cat_cols]
         X_cat = X_cat.copy()
 
         # Pandas read these comlumns as object.
         for cl in cat_cols:
             X_cat.loc[:,cl] = X_cat.loc[:,cl].astype('category')
@@ -159,33 +223,32 @@
         standard = preprocessing.StandardScaler().fit(X_.loc[:,num_cols])
         # TODO: Added the following line to avoid SettingWithCopyWarning. 
         # Need to check if this is the right way to do it.
         X_ = X_.copy()
         X_.loc[:,num_cols] = standard.transform(X_.loc[:,num_cols])       
 
         # get hyperparameters
-        hyper_params = nested_get(self.params,
-                          ["gps_params", "libs", "xgboost"])
+        hyper_params = nested_get(self.params, ["libs", "xgboost"])
 
 
-        if self.params.get("gps_params").get("model") == "parametric":
+        if self.params.get("gps_density") == "normal":
 
             e_gps_pred, training_report = self.xgb_train_it(X_, 
                                                             y.squeeze(), 
                                                             hyper_params)
             self.training_report["training_model"] = training_report
             e_gps_tmp = (e_gps_pred - y.to_numpy())
             e_gps_std = np.std(e_gps_tmp)
             gps = norm.pdf(y.to_numpy().squeeze(), e_gps_pred, e_gps_std)
             return dict(gps=gps, 
                         e_gps_pred=e_gps_pred, 
                         e_gps_std=e_gps_std,
                         w_resid=None)
 
-        elif self.params.get("gps_params").get("model") == "non-parametric":
+        elif self.params.get("gps_density") == "kernel":
 
             e_gps_pred, training_report = self.xgb_train_it(X_,
                                                             y.squeeze(), 
                                                             hyper_params)
             
             self.training_report["training_model"] = training_report
             target = np.abs(e_gps_pred - y.squeeze())
@@ -202,17 +265,17 @@
             kernel = stats.gaussian_kde(w_resid)
             gps = kernel(w_resid)
             return dict(gps=gps,
                         e_gps_pred=e_gps_pred, 
                         e_gps_std=e_gps_std_pred, 
                         w_resid=w_resid)
         else:
-            LOGGER.warning(f"gps_model: '{self.params['gps_model']}'"
+            LOGGER.warning(f"gps_density: '{self.params['gps_density']}'"
                            f" is not defined."
-                           f" Available models: parametric, non-parametric.")
+                           f" Available options: normal, kernel.")
             return dict()
 
     @staticmethod
     def xgb_train_it(X: pd.DataFrame, 
                      target: pd.Series, 
                      params: dict) -> tuple:
         """ Create XGBoost regressor model 
@@ -238,23 +301,25 @@
 
         # Collect hyperparameters
         n_estimators = params.get("n_estimators", 100)
         learning_rate = params.get("learning_rate", 0.1)
         test_size = params.get("test_rate", 0.2)
         max_depth = params.get("max_depth", 3)
         random_state = params.get("random_state", 42)
+        n_jobs = params.get("n_jobs", 1)
 
         LOGGER.debug(f"XGBoost used parameters: n_estimators={n_estimators}, "
                      f"learning_rate={learning_rate}, test_size={test_size}, "
                      f"random_state={random_state}, "
                      f"max_depth={max_depth}.")
 
         xgb = XGBRegressor(n_estimators = n_estimators,
                            learning_rate = learning_rate,
-                           max_depth = max_depth)                 
+                           max_depth = max_depth,
+                           n_jobs=n_jobs)                 
         
         X_train, X_val, y_train, y_val = train_test_split(X, target,
                                     test_size = test_size, 
                                     random_state = random_state)
         # Fit on train data
         xgb.fit(X_train, y_train)
 
@@ -277,18 +342,14 @@
         Returns
         -------
         dict
             Dictionary of results
         """
         return self.results
 
-if __name__ == "__main__":
-
-    pass
-
```

### Comparing `pycausalgps-0.0.2/pycausalgps/log.py` & `pycausalgps-0.0.3/pycausalgps/log.py`

 * *Files identical despite different names*

### Comparing `pycausalgps-0.0.2/pycausalgps/pseudo_population.py` & `pycausalgps-0.0.3/pycausalgps/pseudo_population.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,380 +1,402 @@
 """
 pseudo_population.py
 ====================
 The core module for the PseudoPopulation class.
 """
 
-import json
-import hashlib
 from collections import Counter
+from dataclasses import dataclass
+from concurrent.futures import ProcessPoolExecutor
 
 import numpy as np
 import pandas as pd
+from tqdm import tqdm
 import matplotlib.pyplot as plt
 from scipy.stats import gaussian_kde, norm
 from matplotlib.gridspec import GridSpec
 
+
 from pycausalgps.log import LOGGER
-from pycausalgps.database import Database
 from pycausalgps.base.utils import nested_get
 from pycausalgps.rscripts.rfunctions import (compute_density,
                                              compute_absolute_weighted_corr)
 
 class PseudoPopulation:
+    """
+    The PseudoPopulation class is used to compute the pseudo-population.
 
-    def __init__(self, project_params, gps_params, 
-                       pspop_params, db_path) -> None:
-        self.project_params = project_params
-        self.gps_params = gps_params
-        self.pspop_params = pspop_params
-        self.db_path = db_path
-        self.hash_value = None
-        self.pspop_id = None
-        self.counter_weight = None
-        self.covariate_balance = None
-        self._generate_hash()
-        self._connect_to_database()
-
+    Parameters
+    ----------
 
-    def _generate_hash(self) -> None:
-        """
-        Generate a hash value for the pseudo-population object.
-        """
-
-        hash_string = json.dumps(self.pspop_params, sort_keys=True)
-
-        if self.gps_params.get("hash_value"):
-            hash_string = self.gps_params.get("hash_value") + hash_string
-            self.hash_value = hashlib.sha256(
-                hash_string.encode("utf-8")).hexdigest()
-            # generating random id for the pseudo-population
-            self.pspop_id = hashlib.shake_256(self.hash_value.encode()).hexdigest(8)
-            self.pspop_params["hash_value"] = self.hash_value
-        else:
-            LOGGER.warning("Project hash value is not assigned. " +\
-                           "This can happen becuase of running the class individually. " +\
-                           "Hash value cannot be generated. ")
+    data: pd.DataFrame
+        The dataframe containing the data (covariate and exposure columns).
+    gps_data: dict
+        The dictionary containing the GPS data. The required keys are:
+        - gps_data: pd.DataFrame
+            The dataframe containing the GPS data, and its auxiliary columns.
+        - gps_model: str
+    params: dict
+        The dictionary containing the parameters for computing the 
+        pseudo-population. The required parameters are:
+        - approach: str
+            The approach to compute the pseudo-population. The available
+            approaches are: "weighting" and "matching".
+        - exposure_column: str  
+            A string that indicates the name of the exposure column.
+        - covariate_column_num: list
+            A list of strings that indicates the names of the numerical
+            covariate columns.
+        - covariate_column_cat: list
+            A list of strings that indicates the names of the categorical
+            covariate columns.
+
+    """
+
+    APPROACH_WEIGHTING = "weighting"
+    APPROACH_MATCHING = "matching"
+    GPS_DENSITY_NORMAL = "normal"
+    GPS_DENSITY_KERNEL = "kernel"
+
+    def __init__(self, data: pd.DataFrame, gps_data: dict, params: dict):
+
+        self.data = data
+        self.params = params
+        self.gps_data = gps_data
+        self.compiling_report = {}
+        self.counter_weight = None
+        self.generate_pseudo_population()
 
-            
-    def _connect_to_database(self):
-        """
-        Connect to the database.
-        """
-        if self.db_path is None:
-            raise Exception("Database is not defined.")
-            
-        self.db = Database(self.db_path)
+    @property
+    def data(self) -> pd.DataFrame:
+        return self.__data
     
+    @data.setter
+    def data(self, value: pd.DataFrame) -> None:
+        if not isinstance(value, pd.DataFrame):
+            raise ValueError("Data must be a pandas DataFrame.")
+        self.__data = value
+
+    @property
+    def params(self) -> dict:
+        return self.__params
+    
+    @params.setter
+    def params(self, value: dict) -> None:
+        #TODO: Check if the params are in the correct format.
+        if not isinstance(value, dict):
+            raise ValueError("Params must be a dictionary.")
+        self.__params = value
+
+    @property
+    def gps_data(self) -> dict:
+        return self.__gps_data
+    
+    @gps_data.setter
+    def gps_data(self, value: dict) -> None:
+        #TODO: check if the gps_data is in the correct format.
+        if not isinstance(value, dict):
+            raise ValueError("GPS data must be a dictionary.")
+        self.__gps_data = value
+
     def generate_pseudo_population(self) -> None:
         """
         Compute the pseudo-population.
         """
+        self.exposure_data_col_name = self.params.get("exposure_column")
+        self.covariate_col_num = self.params.get("covariate_column_num")
+        self.covariate_col_cat = self.params.get("covariate_column_cat")
         
-        # For computing pspop we need to have the following:
-        # 1. gps_params (gps values, estimated exposure, estimated exposure std,
-        #                w_resid)
-        # 2. pspop_params (approach, caliper, scale, 
-
-        if self.pspop_params.get("pspop_params").get("approach") == "weighting":
-            counter_weight = self._compute_pspop_weighting()
-            self.counter_weight = counter_weight["counter_weight"]
+        if self.params.get("approach") == self.APPROACH_WEIGHTING:
+            self.counter_weight = self._compute_pspop_weighting() 
             self._compute_covariate_balance()
-        elif self.pspop_params.get("pspop_params").get("approach") == "matching":
-            counter_weight = self._compute_pspop_matching()
-            self.counter_weight = counter_weight["counter_weight"]
+        elif self.params.get("approach") == self.APPROACH_MATCHING:
+            (
+             self.counter_weight, 
+             self.counter_weight_list
+            ) = self._compute_pspop_matching()
             self._compute_covariate_balance()
         else:
             raise Exception("Approach is not defined.")
-
-
-    def load_exposure(self) -> None:
-        """
-        Load the exposure values.
-        """
-        exposure_path = self.project_params.get("data").get("exposure_path")
-
-        # load exposure values.
-        exposure_data = pd.read_csv(exposure_path)
-        LOGGER.debug(f"Exposure data shape: {exposure_data.shape}")
-
-        if not isinstance(exposure_data, pd.DataFrame):
-            raise Exception("Exposure data is not a dataframe.")
-
-        if "id" not in exposure_data.columns:
-            raise Exception("Exposure data does not have id column.")
-        
-        return exposure_data
-
-    def load_confounders(self) -> tuple:
-        """
-        Load the confounder values.
-        """
-        covariate_path = self.project_params.get("data").get("covariate_path")
-
-        # load confounder values.
-        covariate_data = pd.read_csv(covariate_path)
-        LOGGER.debug(f"Confounder data shape: {covariate_data.shape}")
-        
-        # select the comlumns that are used in the gps
-        covariate_col_num = nested_get(self.gps_params,
-                                            ["gps_params","pred_model",
-                                            "covariate_column_num"])
-        covariate_col_cat = nested_get(self.gps_params,
-                                            ["gps_params", "pred_model", 
-                                            "covariate_column_cat"])
-        
-        if covariate_col_num is not None:
-            covariate_data_num = covariate_data[covariate_col_num]
-        else:
-            covariate_data_num = None
-        
-        if covariate_col_cat is not None:
-            covariate_data_cat = covariate_data[covariate_col_cat]
-        else:
-            covariate_data_cat = None
-
-
-        return covariate_data_num, covariate_data_cat
-
-
-    def _compute_pspop_weighting(self) -> None:
+    
+    
+    def _compute_pspop_weighting(self) -> pd.DataFrame:
         """
         Compute the pseudo-population using weighting.
         """
         
         # The weight of each sample is equal to the probablity of getting 
         # that exposure in the data over the probablity of getting that 
         # exposure given the covariates (GPS).
 
         # temp test
         compute_density_with_r = True
         
-        # load exposure values. 
-        exposure_data = self.load_exposure()
-
-        exposure_data_col_name = nested_get(self.gps_params,
-                                                ["gps_params", "pred_model", 
-                                                "exposure_column"])
-
         # compute density of the exposure in the data.
         if compute_density_with_r:
             # compute density with R.
-            w_val = exposure_data[exposure_data_col_name].to_numpy()
+            w_val = self.data[self.exposure_data_col_name].to_numpy()
             data_density = compute_density(w_val, w_val)
             print("Density was computed with R.")
         else:
-            exp_data = exposure_data[exposure_data_col_name]
+            exp_data = self.data[self.exposure_data_col_name]
             kde = gaussian_kde(exp_data)
             data_density = kde(exp_data)
+
         
- 
-        # Extract the gps object from the database.
-        gps_obj = self.db.get_value(self.gps_params.get("hash_value"))
-        
-        ipw = data_density / gps_obj._data.get("_data")["gps"].to_numpy()
-        
-        value = pd.DataFrame({"id": exposure_data["id"], "counter_weight": ipw})
+        ipw = data_density / self.gps_data.get("data")["gps"].to_numpy()            
+        value = pd.DataFrame({"id": self.gps_data.get("data")["id"], 
+                              "counter_weight": ipw})
 
         return value
   
+    @staticmethod
+    def compute_min_idx(i, a, b, scale, c_minus_d):
+        tmp_vals = np.abs(a - b[i]) * scale + c_minus_d
+        min_idx = np.argmin(tmp_vals)
+        return min_idx
+
+    @staticmethod
+    def compute_min_idx_proc(args):
+        i, a, b, scale, c_minus_d = args
+        tmp_vals = np.abs(a - b[i]) * scale + c_minus_d
+        min_idx = np.argmin(tmp_vals)
+        return min_idx
+    
+    @staticmethod
+    def compute_min_idx_proc_chunk(args):
+        start_idx, chunk_size, a, b, scale, c_minus_d = args
+        out_chunk = np.full(chunk_size, -1,  dtype=np.int)  # Initialize with np.nan
+        for i in range(chunk_size):
+            idx = start_idx + i
+            if idx >= len(b):
+                break
+            tmp_vals = np.abs(a - b[idx]) * scale + c_minus_d
+            min_idx = np.argmin(tmp_vals)
+            out_chunk[i] = min_idx
+        return out_chunk
+
+
+    def _process_exposure_level(self, w):
+
+        # load gps object from gps_data
+        gps_min, gps_max = self.gps_data.get("gps_minmax")
+        gps_density = self.gps_data.get("gps_density")
+        if gps_density == self.GPS_DENSITY_KERNEL:
+            w_resid = self.gps_data.get("data")["w_resid"]
+     
+        # load exposure values
+        obs_exposure_data = self.data[["id", self.exposure_data_col_name]]
+        w_min, w_max = (min(obs_exposure_data[self.exposure_data_col_name]), 
+                        max(obs_exposure_data[self.exposure_data_col_name]))
 
-    def _compute_pspop_matching(self) -> None:
+        # controlling parameters
+        delta = nested_get(self.params,
+                                ["control_params", 
+                                "caliper"])
+        scale = nested_get(self.params,
+                                ["control_params",
+                                "scale"])
+        
+        dist_measure = nested_get(self.params, 
+                                 ["control_params", 
+                                  "dist_measure"])
+
+        
+        if gps_density == self.GPS_DENSITY_NORMAL:
+            p_w = norm.pdf(w, 
+                           self.gps_data.get("data")["e_gps_pred"], 
+                           self.gps_data.get("data")["e_gps_std_pred"])
+        elif gps_density == self.GPS_DENSITY_KERNEL:
+            w_new = ((w - self.gps_data.get("data")["e_gps_pred"]) 
+                      / self.gps_data.get("data")["e_gps_std_pred"])
+            p_w = compute_density(w_resid, w_new)
+        else:
+            raise Exception("GPS model is not defined.")
+           
+
+        # select subset of data that are within the caliper value.
+        subset_idx = np.where(np.abs(
+            obs_exposure_data[self.exposure_data_col_name] - w) <= delta)[0]
+        subset_row = obs_exposure_data.iloc[subset_idx]["id"]
+
+        if len(subset_row) == 0:
+            LOGGER.debug(f"No data found within the caliper value ({delta}) " 
+                         f"for the requested exposure level: {w}.")
+            return (w, Counter(None))
+
+
+        # standardize GPS and Exposure values.
+        std_w = (w - w_min)/(w_max - w_min)
+        std_gps = (p_w - gps_min)/(gps_max - gps_min)
+
+        # all data (observational data where w is requested w.)
+        # std_w: scaler
+        # std_gps: vector
+        all_curated_data = pd.DataFrame({"id": obs_exposure_data["id"],
+                                         "std_w": std_w,
+                                         "std_gps": std_gps})
+        
+        # subset of data (actual standardized data that are within the caliper value.)
+        # std_w_subset: vector
+        # std_gps_subset: vector
+        std_w_subset = ((obs_exposure_data[obs_exposure_data["id"].
+                        isin(subset_row)][self.exposure_data_col_name] - w_min)) / (w_max - w_min)
+        
+        # TODO: use query.
+        std_gps_subset = (self.gps_data.get("data")[self.gps_data.get("data")["id"].isin(subset_row)]["gps_standardized"])
+
+        # a: subset of data with standardized GPS (std_gps_subset)
+        # b: all data with estimated GPS based on requested exposure level. (std_gps)
+        # c: subset of data with standardized exposure (std_w_subset)
+        # d: the exposure level that is requested. (std_w)
+        
+        a = std_gps_subset.to_numpy()
+        b = std_gps
+        c = std_w_subset.to_numpy()
+        d = std_w
+
+        c_minus_d = abs(c - d)*(1-scale)
+
+        # compute closest sample from subset of data to these hypothetical samples.
+        # TODO: make this a fucntion
+        len_b = len(b)
+        #len_a = len(a)
+        out = np.zeros(len_b)
+
+        # chunk_size = int(nested_get(self.params, ["run_params", "chunk_size"]))
+        # num_chunks = int(np.ceil(len_b / chunk_size))
+
+        # with ProcessPoolExecutor(max_workers=n_thread) as executor:
+        #     args_list = [(i * chunk_size, chunk_size, a, b, scale, c_minus_d) for i in range(num_chunks)]
+        #     results = list(executor.map(self.compute_min_idx_proc_chunk, args_list))
+
+        # # Flatten the results and assign them back to the 'out' array
+        # out = np.concatenate([chunk[chunk != -1] for chunk in results])
+
+    
+        for i in range(len_b):
+            tmp_vals = np.abs(a - b[i]) * scale + c_minus_d
+            min_idx = np.argmin(tmp_vals)
+            out[i] = min_idx
+
+        # Get the id based on the index.
+        selected_id = subset_row.iloc[out].to_numpy()
+        tmp_freq_table = Counter(selected_id)
+        #counter_weight.update(tmp_freq_table)   
+        
+        return (w, tmp_freq_table)
+    
+
+    
+    def _compute_pspop_matching(self):
 
         """ 
         Compute the pseudo-population using matching approach.
         """
 
         # We need: 
         # Original GPS value and mean and standard deviation.
         # Original exposure value.
         # Requested exposure level. 
         # Caliper value.
         # Scale value.
 
-        
-        # load gps object from the database.
-        gps_obj = self.db.get_value(self.gps_params.get("hash_value"))
-        gps_min, gps_max = gps_obj._data.get("gps_minmax")
-        gps_model = gps_obj.gps_params.get("gps_params").get("model")
-        if gps_model == "non-parametric":
-            w_resid = gps_obj.w_resid
-     
-        # load exposure values
-        obs_exposure_data = self.load_exposure()
-        w_min, w_max = (min(obs_exposure_data["exposure"]), 
-                        max(obs_exposure_data["exposure"]))
-
-        # controlling parameters
-        delta = nested_get(self.pspop_params,
-                               ["pspop_params", 
-                                "controlling_params", 
-                                "caliper"])
-        scale = nested_get(self.pspop_params,
-                                ["pspop_params",
-                                 "controlling_params",
-                                 "scale"])
-        distance_metric = nested_get(self.pspop_params, 
-                                          ["pspop_params",
-                                           "controlling_params", 
-                                           "distance_metric"])
+        obs_exposure_data = self.data[["id", self.exposure_data_col_name]]
+        w_min, w_max = (min(obs_exposure_data[self.exposure_data_col_name]), 
+                max(obs_exposure_data[self.exposure_data_col_name]))
 
         # collect requested exposure level.
-        req_exposure = nested_get(self.pspop_params, 
-                                       ["pspop_params", 
-                                        "controlling_params", 
-                                        "bin_seq"])
+        req_exposure = nested_get(self.params, 
+                                 ["control_params", 
+                                  "bin_seq"])
         
+        delta = nested_get(self.params,
+                                ["control_params", 
+                                "caliper"])
+
         # check if req_exposure is string
         if isinstance(req_exposure, str):
             req_exposure = eval(req_exposure)
 
         if req_exposure is None:
             req_exposure = np.arange(w_min+delta/2, w_max, delta)
-
-
-        for i, w in enumerate(req_exposure):
-            
-            if gps_model == "parametric":
-                p_w = norm.pdf(w, 
-                               gps_obj._data.get("_data")["e_gps_pred"], 
-                               gps_obj._data.get("_data")["e_gps_std_pred"])
-            elif gps_model == "non-parametric":
-                w_new = ((w - gps_obj._data.get("_data")["e_gps_pred"]) 
-                         / gps_obj._data.get("_data")["e_gps_std_pred"])
-                p_w = compute_density(w_resid, w_new)
-            else:
-                raise Exception("GPS model is not defined.")
-           
-
-
-            # select subset of data that are within the caliper value.
-            subset_idx = np.where(np.abs(obs_exposure_data["exposure"] - w) <= delta)[0]
-            subset_row = obs_exposure_data.iloc[subset_idx]["id"]
-
-            # standardize GPS and Exposure values.
-            std_w = (w - w_min)/(w_max - w_min)
-            std_gps = (p_w - gps_min)/(gps_max - gps_min)
-
-            # all data (observational data where w is requested w.)
-            # std_w: scaler
-            # std_gps: vector
-            all_curated_data = pd.DataFrame({"id": obs_exposure_data["id"],
-                                             "std_w": std_w,
-                                             "std_gps": std_gps})
-            
-            # subset of data (actual standardized data that are within the caliper value.)
-            # std_w_subset: vector
-            # std_gps_subset: vector
-            std_w_subset = ((obs_exposure_data[obs_exposure_data["id"].
-                            isin(subset_row)]["exposure"] - w_min)) / (w_max - w_min)
-            
-            # TODO: use query.
-            std_gps_subset = (gps_obj._data.get("_data")[gps_obj.
-                              _data.get("_data")["id"].
-                              isin(subset_row)]["gps_standardized"])
-
-            # a: subset of data with standardized GPS (std_gps_subset)
-            # b: all data with estimated GPS based on requested exposure level. (std_gps)
-            # c: subset of data with standardized exposure (std_w_subset)
-            # d: the exposure level that is requested. (std_w)
-            
-            a = std_gps_subset.to_numpy()
-            b = std_gps
-            c = std_w_subset.to_numpy()
-            d = std_w
-
-            c_minus_d = abs(c - d)*(1-scale)
-
-            # compute closest sample from subset of data to these hypothetical samples.
-            # TODO: make this a fucntion
-            len_b = len(b)
-            len_a = len(a)
-            out = np.zeros(len_b)
-
-            # counter_weight = pd.DataFrame.from_dict({key: 0 for key in 
-            #                                          obs_exposure_data["id"]}, 
-            #                                          orient="index", 
-            #                                          columns=['counter_weight'])
-
-            counter_weight = Counter({key: 0 for key in obs_exposure_data["id"]})
+     
+        counter_weight = Counter({key: 0 for key in obs_exposure_data["id"]})
+        counter_weight_list = []
  
-            # Brute force method.
-            for i in range(len_b):
-                for j in range(len_a):
-
-                    subtract_val = abs(a[j] - b[i])*scale
-
-                    tmp_val = subtract_val + c_minus_d[j]
-
-                    if (j == 0):
-                        min_val = tmp_val
-                        min_idx = j
-                        continue
-
-                    if (tmp_val < min_val):
-                        min_val = tmp_val
-                        min_idx = j
-                out[i] = min_idx
-            
-            # Solution with numpy, but it will consume more memory.
-            # Keeping this for future reference.
-            out2 = np.argmin(np.abs(np.subtract.outer(a, b))*scale 
-                            + c_minus_d[:, np.newaxis], axis=0)
+        n_thread = int(nested_get(self.params, ["run_params", "n_thread"]))
 
+        with ProcessPoolExecutor(max_workers=n_thread) as executor:
+            results = list(tqdm(executor.map(self._process_exposure_level, 
+                                             req_exposure), 
+                                             total=len(req_exposure), 
+                                             desc="Processing exposure levels"))
             
+        # Process the results and update the counter_weight and counter_weight_list
+        for w, tmp_freq_table in results:
+            counter_weight_list.append(CounterWeightData(w, tmp_freq_table))
+    
+        for i_counter_weight in counter_weight_list:
+            counter_weight.update(i_counter_weight.counter_weight)
+    
 
-            # Get the id based on the index.
-            selected_id = subset_row.iloc[out].to_numpy()
-            tmp_freq_table = Counter(selected_id)
-            counter_weight.update(tmp_freq_table)   
-
+        for i_counter_weight in counter_weight_list:
+            counter_weight.update(i_counter_weight.counter_weight)
+        
         counter_weight_dict = dict(counter_weight)
         counter_weight_df = pd.DataFrame(list(counter_weight_dict.items()), 
                                                    columns=["id", "counter_weight"])
 
-        return counter_weight_df
+        return counter_weight_df, counter_weight_list
 
             
-
-
-
     def _compute_covariate_balance(self) -> None:
         """
         Compute covariate balance.
         """
         if self.counter_weight is None:
-            raise Exception("Counter weight is not defined. " +\
-                "Try generating the pseudo-population first.")
+            raise Exception(f"Counter weight is not defined. " 
+                             "Try generating the pseudo-population first.")
 
-        # load exposure values.
-        exposure_data = self.load_exposure()
-        exp_data = exposure_data[self.gps_params.get("gps_params").get("pred_model").get("exposure_column")].to_numpy()
+        
+        # merge the counter weight with the original data.
+        # TODO: warn users if there is a discrepancy in ids.
+        self.merged_data = pd.merge(self.data, self.counter_weight, on="id")
+               
+        # load the exposure data.
+        exp_data = self.merged_data[self.exposure_data_col_name].to_numpy()
 
         # load the confounders.
-        covariate_data_num, covariate_data_cat = self.load_confounders()
+        covariate_data_num = self.merged_data[self.covariate_col_num]
+        covariate_data_cat = self.merged_data[self.covariate_col_cat]
+        counter_weight = self.merged_data["counter_weight"].to_numpy()
 
         # compute weighted correlation between the confounders and the exposure.
         covariate_balance = compute_absolute_weighted_corr(exp_data, 
-                                                           self.counter_weight, 
+                                                           counter_weight, 
                                                            covariate_data_num,
                                                            covariate_data_cat) 
 
-        original_data_covariate_balance = compute_absolute_weighted_corr(exp_data,
-                                                                         np.ones(self.counter_weight.shape),
-                                                                         covariate_data_num,
-                                                                         covariate_data_cat)                    
+        original_data_covariate_balance = compute_absolute_weighted_corr(
+            exp_data,
+            np.ones(counter_weight.shape),
+            covariate_data_num,
+            covariate_data_cat)                    
 
         cov_balance_current = covariate_balance
-        cov_balance_current.rename(columns = {'value':'current'}, inplace = True)
+        cov_balance_current.rename(columns = {'value':'current'}, 
+                                   inplace = True)
         cov_balance_original = original_data_covariate_balance
-        cov_balance_original.rename(columns = {'value':'original'}, inplace = True)
+        cov_balance_original.rename(columns = {'value':'original'}, 
+                                    inplace = True)
 
 
-        cov_balance = pd.merge(cov_balance_current, cov_balance_original, on='name')
+        cov_balance = pd.merge(cov_balance_current, cov_balance_original, 
+                               on='name')
 
         self.covariate_balance = cov_balance
 
 
     def plot_cov_balance(self) -> None:
         """
         Plot the covariate balance.
@@ -444,22 +466,248 @@
         ax3.axis('off')
         xlim3 = ax3.get_xlim()
         ylim3 = ax3.get_ylim()
 
         hyper_param_3 = {"fontsize": 8, "ha":"left", "va":"center"}
 
         ax3.text(xlim3[0], ylim3[1]-0.05, 'Data Info', **hyper_param_1)
-        ax3.text(xlim3[0], ylim3[1]-0.15, 
-                 f'GPS Object ID: {self.gps_params.get("gps_id")}', 
-                 **hyper_param_3)
-        ax3.text(xlim3[0], ylim3[1]-0.2,
-                    f'GPS hash value: {self.gps_params.get("hash_value")}',
-                    **hyper_param_3)
-        ax3.text(xlim3[0], ylim3[1]-0.25,
-                    f'Pseudo population ID: {self.pspop_id}',
-                    **hyper_param_3)
-        ax3.text(xlim3[0], ylim3[1]-0.3,
-                    f'Pseudo population hash value: {self.hash_value}',
-                    **hyper_param_3)
+        # ax3.text(xlim3[0], ylim3[1]-0.15, 
+        #          f'GPS Object ID: {self.gps_params.get("gps_id")}', 
+        #          **hyper_param_3)
+        # ax3.text(xlim3[0], ylim3[1]-0.2,
+        #             f'GPS hash value: {self.gps_params.get("hash_value")}',
+        #             **hyper_param_3)
+        # ax3.text(xlim3[0], ylim3[1]-0.25,
+        #             f'Pseudo population ID: {self.pspop_id}',
+        #             **hyper_param_3)
+        # ax3.text(xlim3[0], ylim3[1]-0.3,
+        #             f'Pseudo population hash value: {self.hash_value}',
+        #             **hyper_param_3)
 
         fig.suptitle("Covariate Balance", fontsize=16)
-        plt.show()   
+        plt.show()   
+
+
+    def get_results(self) -> dict:
+        """
+        Get the results of generating the pseudo-population.
+        """
+
+        results = {"data": self.merged_data,
+                   "params": self.params,
+                   "compiling_report": self.compiling_report,
+                   "covariate_balance": self.covariate_balance}
+        
+        return results
+
+    def get_individual_counter_weight(self) -> list:
+        """
+        Get the counter-weight for each individual exposure.
+        """
+
+        if self.counter_weight_list is None:
+            raise Exception("Counter-weight is not defined. " +\
+                "Try generating the pseudo-population first.")
+
+        return self.counter_weight_list
+
+
+
+
+
+
+@dataclass    
+class CounterWeightData:
+    w: float
+    counter_weight: np.ndarray
+
+    
+    
+    
+    # Old code 
+
+
+
+# def process_exposure_level_2(w, gps_data, data, 
+#                                   exposure_data_col_name, params,
+#                                   GPS_DENSITY_NORMAL, GPS_DENSITY_KERNEL):
+
+#         # load gps object from gps_data
+#         gps_min, gps_max = gps_data.get("gps_minmax")
+#         gps_density = gps_data.get("gps_density")
+#         if gps_density == GPS_DENSITY_KERNEL:
+#             w_resid = gps_data.get("data")["w_resid"]
+     
+#         # load exposure values
+#         obs_exposure_data = data[["id", exposure_data_col_name]]
+#         w_min, w_max = (min(obs_exposure_data[exposure_data_col_name]), 
+#                         max(obs_exposure_data[exposure_data_col_name]))
+
+#         # controlling parameters
+#         delta = nested_get(params,
+#                                 ["control_params", 
+#                                 "caliper"])
+#         scale = nested_get(params,
+#                                 ["control_params",
+#                                 "scale"])
+        
+#         dist_measure = nested_get(params, 
+#                                  ["control_params", 
+#                                   "dist_measure"])
+
+        
+#         if gps_density == GPS_DENSITY_NORMAL:
+#             p_w = norm.pdf(w, 
+#                            gps_data.get("data")["e_gps_pred"], 
+#                            gps_data.get("data")["e_gps_std_pred"])
+#         elif gps_density == GPS_DENSITY_KERNEL:
+#             w_new = ((w - gps_data.get("data")["e_gps_pred"]) 
+#                       / gps_data.get("data")["e_gps_std_pred"])
+#             p_w = compute_density(w_resid, w)
+#         else:
+#             raise Exception("GPS model is not defined.")
+           
+
+#         # select subset of data that are within the caliper value.
+#         subset_idx = np.where(np.abs(
+#             obs_exposure_data[exposure_data_col_name] - w) <= delta)[0]
+#         subset_row = obs_exposure_data.iloc[subset_idx]["id"]
+
+#         if len(subset_row) == 0:
+#             LOGGER.debug(f"No data found within the caliper value ({delta}) " 
+#                          f"for the requested exposure level: {w}.")
+#             return (w, Counter(None))
+
+
+#         # standardize GPS and Exposure values.
+#         std_w = (w - w_min)/(w_max - w_min)
+#         std_gps = (p_w - gps_min)/(gps_max - gps_min)
+
+#         # all data (observational data where w is requested w.)
+#         # std_w: scaler
+#         # std_gps: vector
+#         all_curated_data = pd.DataFrame({"id": obs_exposure_data["id"],
+#                                             "std_w": std_w,
+#                                             "std_gps": std_gps})
+        
+#         # subset of data (actual standardized data that are within the caliper value.)
+#         # std_w_subset: vector
+#         # std_gps_subset: vector
+#         std_w_subset = ((obs_exposure_data[obs_exposure_data["id"].
+#                         isin(subset_row)][exposure_data_col_name] - w_min)) / (w_max - w_min)
+        
+#         # TODO: use query.
+#         std_gps_subset = (gps_data.get("data")[gps_data.get("data")["id"].isin(subset_row)]["gps_standardized"])
+
+#         # a: subset of data with standardized GPS (std_gps_subset)
+#         # b: all data with estimated GPS based on requested exposure level. (std_gps)
+#         # c: subset of data with standardized exposure (std_w_subset)
+#         # d: the exposure level that is requested. (std_w)
+        
+#         a = std_gps_subset.to_numpy()
+#         b = std_gps
+#         c = std_w_subset.to_numpy()
+#         d = std_w
+
+#         c_minus_d = abs(c - d)*(1-scale)
+
+#         # compute closest sample from subset of data to these hypothetical samples.
+#         # TODO: make this a fucntion
+#         len_b = len(b)
+#         #len_a = len(a)
+#         out = np.zeros(len_b)
+
+#         # chunk_size = int(nested_get(self.params, ["run_params", "chunk_size"]))
+        
+#         # num_chunks = int(np.ceil(len_b / chunk_size))
+
+#         # with ProcessPoolExecutor(max_workers=n_thread) as executor:
+#         #     args_list = [(i * chunk_size, chunk_size, a, b, scale, c_minus_d) for i in range(num_chunks)]
+#         #     results = list(executor.map(self.compute_min_idx_proc_chunk, args_list))
+
+#         # # Flatten the results and assign them back to the 'out' array
+#         # out = np.concatenate([chunk[chunk != -1] for chunk in results])
+
+    
+#         for i in range(len_b):
+#             tmp_vals = np.abs(a - b[i]) * scale + c_minus_d
+#             min_idx = np.argmin(tmp_vals)
+#             out[i] = min_idx
+
+#         # Get the id based on the index.
+#         selected_id = subset_row.iloc[out].to_numpy()
+#         tmp_freq_table = Counter(selected_id)
+#         #counter_weight.update(tmp_freq_table)   
+        
+#         return (w, tmp_freq_table)
+    
+
+# if __name__ == "__main__":
+
+#     from pycausalgps.base.utils import generate_syn_pop
+#     from pycausalgps.gps import GeneralizedPropensityScore
+
+#     gps_params = {"gps_density": "normal",
+#                   "exposure_column": "treat",
+#                   "covariate_column_num": ["cf1", 
+#                                            "cf2", 
+#                                            "cf3", 
+#                                            "cf4", 
+#                                            "cf6"],
+#                   "covariate_column_cat": ["cf5"],
+#                   "libs":{
+#                           "xgboost":{
+#                                  "n_estimators": 100,
+#                                  "max_depth": 3,
+#                                  "learning_rate": 0.1,
+#                                  "test_rate": 0.2,
+#                                  "random_state": 42
+#                                  }
+#                              }
+#     }
+    
+#     data = generate_syn_pop(sample_size=1000, 
+#                             seed_val=456, 
+#                             outcome_sd=0.25, 
+#                             gps_spec=1, 
+#                             cova_spec=2)
+        
+#     gps = GeneralizedPropensityScore(data, gps_params)
+#     results = gps.get_results()
+#     gps_data = {
+#         'data' : results.get("data"),
+#         'gps_density' : results.get("gps_density"),
+#         'gps_minmax': results.get("gps_minmax")}
+
+#     # merged_df = pd.merge(data, gps_data, on='id')
+#     # merged_df
+
+#     # pspop_params = {"approach" : "weighting", 
+#     #                 "exposure_column": "treat",
+#     #                 "covariate_column_num": ["cf1", 
+#     #                                          "cf2", 
+#     #                                          "cf3", 
+#     #                                          "cf4", 
+#     #                                          "cf6"],
+#     #                 "covariate_column_cat": ["cf5"]}
+    
+
+#     pspop_params = {"approach" : "matching", 
+#                 "exposure_column": "treat",
+#                 "covariate_column_num": ["cf1", 
+#                                          "cf2", 
+#                                          "cf3", 
+#                                          "cf4", 
+#                                          "cf6"],
+#                 "covariate_column_cat": ["cf5"],
+#                 "control_params": {"caliper": 1.0,
+#                                    "scale": 0.5,
+#                                    "dist_measure": "l1",
+#                                    "bin_seq": None},
+#                 "run_params": {"n_thread": 12,
+#                                "chunk_size": 500}}
+
+#     pspop = PseudoPopulation(data=data, 
+#                             gps_data=gps_data, 
+#                             params=pspop_params)
+    
+
```

### Comparing `pycausalgps-0.0.2/pycausalgps/rscripts/__init__.py` & `pycausalgps-0.0.3/pycausalgps/rscripts/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 # import R's "utils" package
 utils = importr('utils')
 utils.chooseCRANmirror(ind=1) # select the first mirror in the list
 
 # define packages to be installed
-packnames = ('polycor', 'locpol', 'wCorr')
+packnames = ('polycor', 'locpol', 'wCorr', 'gnm', 'gam')
 
 # Install packages if not installed
 names_to_install = [x for x in packnames if not rpackages.isinstalled(x)]
 
 if len(names_to_install) > 0:
     utils.install_packages(StrVector(names_to_install))
```

### Comparing `pycausalgps-0.0.2/pycausalgps/rscripts/rfunctions.py` & `pycausalgps-0.0.3/pycausalgps/rscripts/rfunctions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 rfunctions.py
 =============
 Main module to define the R functions to be used in the package.
 """
 
+import os
 
 import numpy as np
 import pandas as pd
 
 from rpy2 import robjects
 from rpy2.robjects import pandas2ri
 from rpy2.robjects.conversion import localconverter
@@ -15,23 +16,21 @@
 
 
 #### Compute density function --------------------------------------------------
 # R 
 # Check if function is defined
 # TODO: Check if there is a better way to fix the path.
 if 'compute_density' not in robjects.globalenv:
+    
     try:
-        robjects.r('''
-            compute_density <- function(x0, x1){
-                tmp_density <- stats::density(x0, na.rm = TRUE)
-                dnst <- stats::approx(tmp_density$x, tmp_density$y, xout = x1,
-                                      rule = 2)$y
-            return(dnst)
-           }
-        ''')
+        r_file_path = os.path.join(os.path.dirname(__file__), 
+                                   'compute_density.r')
+
+        robjects.r(f'source("{r_file_path}")')
+
     except Exception as e:
         print('Error in loading the R function: compute_density')
         print(e)
 
 
 
 # Python 
@@ -77,77 +76,20 @@
 
 #### Compute absolute weighted corr function -----------------------------------
 
 # R
 # Check if function is defined
 if 'absolute_weighted_corr' not in robjects.globalenv:
     try:
-        robjects.r('''
-            absolute_weighted_corr_df <- function(w,
-                                      vw,
-                                      c_num,
-                                      c_cat){
-  
-  
- 
-                # detect numeric columns
-                col_n <- colnames(c_num)
-              
-                # detect factorial columns
-                col_f <- colnames(c_cat)
-              
-                c_cat[] <- lapply(c_cat, as.factor)
-              
-                absolute_corr_n <- absolute_corr_f <- NULL
-              
-                if (length(col_n) > 0) {
-                  absolute_corr_n<- sapply(col_n,function(i){
-                    abs(wCorr::weightedCorr(x = w,
-                                            y = c_num[,i],
-                                            weights = vw,
-                                            method = c("spearman")))})
-                  absolute_corr_n <- unlist(absolute_corr_n)
-                  names(absolute_corr_n) <- col_n
-                }
-              
-                if (length(col_f) > 0) {
-                  internal_fun<- function(i){
-                    abs(wCorr::weightedCorr(x = w,
-                                            y = c_cat[, i],
-                                            weights = vw,
-                                            method = c("Polyserial")))}
-              
-                  absolute_corr_f <- c()
-                  for (item in col_f){
-                    if (length(unique(c_cat[[item]])) == 1 ){
-                      absolute_corr_f <- c(absolute_corr_f, NA)
-                    } else {
-                      absolute_corr_f <- c(absolute_corr_f, internal_fun(item))
-                    }
-                  }
-                  names(absolute_corr_f) <- col_f
-                }
-              
-                absolute_corr <- c(absolute_corr_n, absolute_corr_f)
-              
-                if (sum(is.na(absolute_corr)) > 0){
-                  warning(paste("The following features generated missing values: ",
-                                names(absolute_corr)[is.na(absolute_corr)],
-                                "\nIn computing mean covariate balance, they will be ignored."))
-                }
-              
-                df <- data.frame(name = character(), value = numeric())
-              
-                for (i in names(absolute_corr)){
-                  df <- rbind(df, data.frame(name=i, value=absolute_corr[[i]]))
-                }
-              
-                return(df)
-            }
-        ''')
+
+        r_file_path = os.path.join(os.path.dirname(__file__), 
+                                   'absolute_weighted_corr_df.r')
+
+        robjects.r(f'source("{r_file_path}")')
+
     except Exception as e:
         print('Error in loading the R function: absolute_weighted_corr')
         print(e)
 
 # Python
 
 def compute_absolute_weighted_corr(w:np.array, 
@@ -195,14 +137,151 @@
 
     return results_python
 
 
 #### ---------------------------------------------------------------------------
 
 
+### Compute parametric exposure response function ------------------------------
+
+# R
+# TODO: Check if there is a better way to fix the path.
+if 'r_estimate_pmetric_erf' not in robjects.globalenv:
+    
+    try:
+        r_file_path = os.path.join(os.path.dirname(__file__), 
+                                   'r_estimate_pmetric_erf.r')
+
+        robjects.r(f'source("{r_file_path}")')
+
+    except Exception as e:
+        print('Error in loading the R function: compute_density')
+        print(e)
+
+
+# Python
+def estimate_pmetric_erf(formula:str,
+                         family:str,
+                         data:pd.DataFrame) -> any:
+    
+
+    # Convert pandas dataframe to R dataframe
+    with localconverter(robjects.default_converter + pandas2ri.converter):
+        r_data = robjects.conversion.py2rpy(data)
+    
+    # collect the function from R
+    r_estimate_pmetric_erf = robjects.globalenv['r_estimate_pmetric_erf']
+
+    # call the function
+    results = r_estimate_pmetric_erf(formula, 
+                                     family, 
+                                     r_data)
+    
+    # Convert results to python
+    with localconverter(robjects.default_converter + 
+                        robjects.pandas2ri.converter):
+        py_results = robjects.conversion.rpy2py(results)
+
+    return py_results
+    
+#### ---------------------------------------------------------------------------
+
+## Compute semiparametric exposure response function ---------------------------
+
+# R
+# TODO: Check if there is a better way to fix the path.
+if 'r_estimate_semipmetric_erf' not in robjects.globalenv:
+    
+    try:
+        r_file_path = os.path.join(os.path.dirname(__file__), 
+                                   'r_estimate_semipmetric_erf.r')
+
+        robjects.r(f'source("{r_file_path}")')
+
+    except Exception as e:
+        print('Error in loading the R function: compute_density')
+        print(e)
+
+
+# Python
+def estimate_semipmetric_erf(formula:str,
+                             family:str,
+                             data:pd.DataFrame) -> any:
+    
+
+    # Convert pandas dataframe to R dataframe
+    with localconverter(robjects.default_converter + pandas2ri.converter):
+        r_data = robjects.conversion.py2rpy(data)
+    
+    # collect the function from R
+    r_estimate_semipmetric_erf = robjects.globalenv['r_estimate_semipmetric_erf']
+
+    # call the function
+    results = r_estimate_semipmetric_erf(formula, 
+                                         family, 
+                                         r_data)
+    
+    # Convert results to python
+    with localconverter(robjects.default_converter + 
+                        robjects.pandas2ri.converter):
+        py_results = robjects.conversion.rpy2py(results)
+
+    return py_results
+    
+#### ---------------------------------------------------------------------------
+
+
+#### locpol function -----------------------------------------------------------
+
+# R
+if 'r_locpol' not in robjects.globalenv:
+        
+    try:
+        r_file_path = os.path.join(os.path.dirname(__file__), 
+                                'r_locpol.r')
+
+        robjects.r(f'source("{r_file_path}")')
+
+    except Exception as e:
+        print('Error in loading the R function: r_locpol')
+        print(e)
+
+# Python
+
+def locpol(data: pd.DataFrame, formula: str, bw: float, w_vals:np.array) -> any:
+
+    # Convert pandas dataframe to R dataframe
+    with localconverter(robjects.default_converter + pandas2ri.converter):
+        r_data = robjects.conversion.py2rpy(data)
+
+    # Convert numpy array to R vector
+    if not isinstance(w_vals, robjects.vectors.FloatVector):
+        w_vals = robjects.FloatVector(w_vals)
+
+    # Convert bw to R vector
+    if not isinstance(bw, robjects.vectors.FloatVector):
+        bw = robjects.FloatVector([bw])
+
+    # collect the function from R
+    r_locpol = robjects.globalenv['r_locpol']
+
+    # call the function
+    results = r_locpol(data = r_data,
+                       formula = formula, 
+                       bw = bw,
+                       w_vals = w_vals)
+
+    # Convert results to python (R vector to numpy array)
+    with localconverter(robjects.default_converter + 
+                        robjects.pandas2ri.converter):
+        py_results = robjects.conversion.rpy2py(results)
+
+    return py_results
+
+
 
 if __name__ == "__main__":
     x0 = np.random.normal(0, 1, 100)
     x1 = np.random.normal(0, 1, 100)
     dnsty = compute_density(x0, x1)
     #print(dnsty)
```

### Comparing `pycausalgps-0.0.2/setup.py` & `pycausalgps-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pycausalgps", 
-    version="0.0.2",
+    version="0.0.3",
     author="Naeem Khoshnevis, Xiao Wu, Danielle Braun",
     author_email="nkhoshnevis@g.harvard.edu, xw2892@cumc.columbia.edu, dbraun@mail.harvard.edu",
     maintainer="Naeem Khoshnevis",
     maintainer_email = "nkhoshnevis@g.harvard.edu",
     description="Matching on generalized propensity scores with continuous exposures",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

