# Comparing `tmp/physiofit-3.0.6.tar.gz` & `tmp/physiofit-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physiofit-3.0.6.tar", max compression
+gzip compressed data, was "physiofit-3.1.0.tar", max compression
```

## Comparing `physiofit-3.0.6.tar` & `physiofit-3.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0    35147 2023-05-22 08:54:39.415783 physiofit-3.0.6/LICENSE
--rw-r--r--   0        0        0     3577 2023-05-22 08:54:39.415783 physiofit-3.0.6/README.md
--rw-r--r--   0        0        0       80 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/__init__.py
--rw-r--r--   0        0        0      966 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/__main__.py
--rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/base/__init__.py
--rw-r--r--   0        0        0    18990 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/base/fitter.py
--rw-r--r--   0        0        0    22161 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/base/io.py
--rw-r--r--   0        0        0      272 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/data/data_example.tsv
--rw-r--r--   0        0        0      366 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/example_yaml.yml
--rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__init__.py
--rw-r--r--   0        0        0      182 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6252 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/base_model.cpython-310.pyc
--rw-r--r--   0        0        0     2831 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_1.cpython-310.pyc
--rw-r--r--   0        0        0     2126 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_2.cpython-310.pyc
--rw-r--r--   0        0        0     2417 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_3.cpython-310.pyc
--rw-r--r--   0        0        0     1817 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_4.cpython-310.pyc
--rw-r--r--   0        0        0     3188 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_5.cpython-310.pyc
--rw-r--r--   0        0        0     3196 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_6.cpython-310.pyc
--rw-r--r--   0        0        0     6220 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/base_model.py
--rw-r--r--   0        0        0     3218 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_1.py
--rw-r--r--   0        0        0     2558 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_2.py
--rw-r--r--   0        0        0     2346 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_3.py
--rw-r--r--   0        0        0     1811 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_4.py
--rw-r--r--   0        0        0     4012 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_5.py
--rw-r--r--   0        0        0      101 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/template.py
--rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/tests/__init__.py
--rw-r--r--   0        0        0     1670 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/tests/conftest.py
--rw-r--r--   0        0        0     3252 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/tests/test_base.py
--rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/ui/__init__.py
--rw-r--r--   0        0        0     6499 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/ui/cli.py
--rw-r--r--   0        0        0    24255 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/ui/gui.py
--rw-r--r--   0        0        0      854 2023-05-22 08:54:39.423783 physiofit-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 physiofit-3.0.6/setup.py
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 physiofit-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-06-07 14:07:04.311319 physiofit-3.1.0/LICENSE
+-rw-r--r--   0        0        0     3577 2023-06-07 14:07:04.311319 physiofit-3.1.0/README.md
+-rw-r--r--   0        0        0       80 2023-06-07 14:07:04.315319 physiofit-3.1.0/physiofit/__init__.py
+-rw-r--r--   0        0        0      966 2023-06-07 14:07:04.315319 physiofit-3.1.0/physiofit/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:07:04.315319 physiofit-3.1.0/physiofit/base/__init__.py
+-rw-r--r--   0        0        0    18990 2023-06-07 14:07:04.315319 physiofit-3.1.0/physiofit/base/fitter.py
+-rw-r--r--   0        0        0    22432 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/base/io.py
+-rw-r--r--   0        0        0      272 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/data/data_example.tsv
+-rw-r--r--   0        0        0      538 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/data/test-data_single_exp.tsv
+-rw-r--r--   0        0        0      366 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/example_yaml.yml
+-rw-r--r--   0        0        0        0 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6252 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/base_model.cpython-310.pyc
+-rw-r--r--   0        0        0     2831 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/model_1.cpython-310.pyc
+-rw-r--r--   0        0        0     2126 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/model_2.cpython-310.pyc
+-rw-r--r--   0        0        0     2417 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/model_3.cpython-310.pyc
+-rw-r--r--   0        0        0     1817 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/model_4.cpython-310.pyc
+-rw-r--r--   0        0        0     3188 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/model_5.cpython-310.pyc
+-rw-r--r--   0        0        0     3196 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/__pycache__/model_6.cpython-310.pyc
+-rw-r--r--   0        0        0     6220 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/base_model.py
+-rw-r--r--   0        0        0     3236 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/model_1.py
+-rw-r--r--   0        0        0     2576 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/model_2.py
+-rw-r--r--   0        0        0     2364 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/model_3.py
+-rw-r--r--   0        0        0     1829 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/model_4.py
+-rw-r--r--   0        0        0     4061 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/model_5.py
+-rw-r--r--   0        0        0      101 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/models/template.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/tests/__init__.py
+-rw-r--r--   0        0        0     1670 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/tests/conftest.py
+-rw-r--r--   0        0        0     3252 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/tests/test_base.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/ui/__init__.py
+-rw-r--r--   0        0        0     6499 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/ui/cli.py
+-rw-r--r--   0        0        0    22489 2023-06-07 14:07:04.319320 physiofit-3.1.0/physiofit/ui/gui.py
+-rw-r--r--   0        0        0      854 2023-06-07 14:07:04.319320 physiofit-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 physiofit-3.1.0/setup.py
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 physiofit-3.1.0/PKG-INFO
```

### Comparing `physiofit-3.0.6/LICENSE` & `physiofit-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/README.md` & `physiofit-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/__main__.py` & `physiofit-3.1.0/physiofit/__main__.py`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/base/fitter.py` & `physiofit-3.1.0/physiofit/base/fitter.py`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/base/io.py` & `physiofit-3.1.0/physiofit/base/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -314,14 +314,18 @@
         for idx, element in enumerate(self.multiple_experiments):
             if not isinstance(element, DataFrame):
                 raise TypeError(
                     f"All the elements of multiple_experiments must be DataFrames. Wrong element type"
                     f"detected at indice {idx}"
                 )
         final_df = concat(self.multiple_experiments)
+        final_df = final_df.reset_index()
+        final_df[["experiments", "parameter name"]] = final_df["index"].str.split(" ", expand=True)
+        final_df.set_index(["experiments", "parameter name"], inplace=True)
+        final_df.drop("index", axis=1, inplace=True)
         final_df.to_csv(f"{str(Path(export_path))}/summary.csv")
 
 
     def output_report(self, fitter, export_path: str |list = None):
         """
         Handle creation and export of the report containing stats from monte
         carlo analysis of optimization parameters
```

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/base_model.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/base_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/model_1.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/model_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/model_2.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/model_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/model_3.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/model_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/model_4.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/model_4.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/model_5.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/model_5.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/__pycache__/model_6.cpython-310.pyc` & `physiofit-3.1.0/physiofit/models/__pycache__/model_6.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/base_model.py` & `physiofit-3.1.0/physiofit/models/base_model.py`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/models/model_1.py` & `physiofit-3.1.0/physiofit/models/model_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         self.parameters_to_estimate = None
         self.fixed_parameters = None
 
     def get_params(self):
 
         self.parameters_to_estimate = {
             "X_0" : self.vini,
-            "mu" : self.vini,
+            "growth_rate" : self.vini,
             "t_lag" : self.vini
         }
         self.bounds = Bounds(
             X_0=(1e-3, 10),
-            mu=(1e-3, 3),
+            growth_rate=(1e-3, 3),
             t_lag = (0, 0.5*self.time_vector.max())
         )
         for metabolite in self.metabolites:
             self.parameters_to_estimate.update(
                 {
                     f"{metabolite}_q" : self.vini,
                     f"{metabolite}_M0" : self.vini
```

### Comparing `physiofit-3.0.6/physiofit/models/model_2.py` & `physiofit-3.1.0/physiofit/models/model_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,20 +18,20 @@
         self.parameters_to_estimate = None
         self.fixed_parameters = None
 
     def get_params(self):
 
         self.parameters_to_estimate = {
             "X_0" : self.vini,
-            "mu" : self.vini,
+            "growth_rate" : self.vini,
             "t_lag" : self.vini
         }
         self.bounds = Bounds({
             "X_0": (1e-3, 10),
-            "mu": (1e-3, 3),
+            "growth_rate": (1e-3, 3),
             "t_lag": (0, 0.5 * self.time_vector.max()),
         })
         for metabolite in self.metabolites:
             self.parameters_to_estimate.update(
                 {
                     f"{metabolite}_q" : 1,
                     f"{metabolite}_M0" : 1
```

### Comparing `physiofit-3.0.6/physiofit/models/model_3.py` & `physiofit-3.1.0/physiofit/models/model_3.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         self.parameters_to_estimate = None
         self.fixed_parameters = None
 
     def get_params(self):
 
         self.parameters_to_estimate = {
             "X_O" : self.vini,
-            "mu" : self.vini
+            "growth_rate" : self.vini
         }
         self.fixed_parameters = {"Degradation": {
             met: 0 for met in self.metabolites
             }
         }
         self.bounds = Bounds({
             "X_0": (1e-3, 10),
-            "mu": (1e-3, 3),
+            "growth_rate": (1e-3, 3),
         })
         for metabolite in self.metabolites:
             self.parameters_to_estimate.update(
                 {
                     f"{metabolite}_q": self.vini,
                     f"{metabolite}_M0": self.vini
                 }
```

### Comparing `physiofit-3.0.6/physiofit/models/model_4.py` & `physiofit-3.1.0/physiofit/models/model_4.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,19 @@
         self.parameters_to_estimate = None
         self.fixed_parameters = None
 
     def get_params(self):
 
         self.parameters_to_estimate = {
             "X_0" : self.vini,
-            "mu" : self.vini
+            "growth_rate" : self.vini
         }
         self.bounds = Bounds({
             "X_0": (1e-3, 10),
-            "mu": (1e-3, 3)
+            "growth_rate": (1e-3, 3)
         })
         for metabolite in self.metabolites:
             self.parameters_to_estimate.update(
                 {
                     f"{metabolite}_q" : self.vini,
                     f"{metabolite}_M0" : self.vini
                 }
```

### Comparing `physiofit-3.0.6/physiofit/models/model_5.py` & `physiofit-3.1.0/physiofit/models/model_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,18 @@
                         f"{metabolite}_y_P": (1e-6, 100),
                         f"{metabolite}_p_0": (1e-6, 100)
                     }
                 )
                 break
 
         if len(self.parameters_to_estimate) != 7:
-            raise ValueError("This model expects 2 metabolites in the data file (1 substrate with name starting with 'S_' and 1 product with name starting with 'P_').")
+            raise ValueError(
+                "This model expects 2 metabolites in the data file (1 substrate with name starting with 'S_' and 1 "
+                "product with name starting with 'P_')."
+            )
 
 
     @staticmethod
     def simulate(
             params_opti: list,
             data_matrix: np.ndarray,
             time_vector: np.ndarray,
```

### Comparing `physiofit-3.0.6/physiofit/tests/conftest.py` & `physiofit-3.1.0/physiofit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/tests/test_base.py` & `physiofit-3.1.0/physiofit/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/ui/cli.py` & `physiofit-3.1.0/physiofit/ui/cli.py`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.6/physiofit/ui/gui.py` & `physiofit-3.1.0/physiofit/ui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,20 +108,20 @@
                 raise
         else:
             raise KeyError(
                 f"Wrong input file format. Accepted formats are tsv for data "
                 f"files or json for configuration files. Detected file: "
                 f"{self.data_file.name}")
 
-        if "experiments" in self.io.data.columns:
-            to_sort = ["experiments", "time"]
-        else:
-            to_sort = "time"
+        if "experiments" not in self.io.data.columns:
+            raise ValueError(
+                "'experiments' column missing from dataset"
+            )
         self.io.data = self.io.data.sort_values(
-            to_sort, ignore_index=True
+            ["experiments", "time"], ignore_index=True
         )
 
         try:
             # Initialize the list of available models
             self.io.get_models()
         except Exception:
             st.error(f"An error has occurred when listing models from the models folder: "
@@ -146,101 +146,68 @@
                 path_to_data = self.io.home_path / self.data_file.name,
                 selected_model= self.model,
                 sds = self.sd,
                 mc = self.mc,
                 iterations = self.iterations
             )
 
-            if "experiments" in self.io.data.columns:
-                full_dataframe = self.io.data.copy()
-                results_path = copy(self.io.res_path)
-                experiments = list(self.io.data["experiments"].unique())
-                self.io.multiple_experiments = []
-                for experiment in experiments:
-                    with st.spinner(f"Running optimization for {experiment}"):
-                        final_table_dict = {}
-                        self.model.data = full_dataframe[
-                            full_dataframe["experiments"] == experiment
-                        ].drop("experiments", axis=1).copy()
-
-                        self.io.res_path = results_path / experiment
-                        if not self.io.res_path.is_dir():
-                            self.io.res_path.mkdir()
-                        # Initialize the fitter object
-                        self.io.names = self.io.data.columns[1:].to_list()
-                        kwargs = self._build_fitter_kwargs()
-                        fitter = self.io.initialize_fitter(
-                            self.model.data,
-                            model=kwargs["model"],
-                            mc=kwargs["mc"],
-                            iterations=kwargs["iterations"],
-                            sd=kwargs["sd"],
-                            debug_mode=kwargs["debug_mode"]
-                        )
-                        # Do the work
-                        fitter.optimize()
-                        if self.mc:
-                            fitter.monte_carlo_analysis()
-                        fitter.khi2_test()
-                        df = pd.DataFrame.from_dict(
-                            fitter.parameter_stats,
-                            orient="columns"
-                        )
-                        df.index = [
-                            f"{experiment} {param}" for param in fitter.model.parameters_to_estimate.keys()
-                        ]
-                        st.write(df)
-                        self.io.multiple_experiments.append(df)
-
-                        # Export results
-                        self.io.output_report(fitter, self.io.res_path)
-                        self.io.plot_data(fitter)
-                        self.io.output_plots(fitter, self.io.res_path)
-                        with st.expander(f"{experiment} plots"):
-                            for fig in self.io.figures:
-                                st.pyplot(fig[1])
-                        self.io.output_pdf(fitter, self.io.res_path)
-                        # Reset figures to free memory
-                        self.io.figures = []
-                        self.config_parser.export_config(self.io.res_path)
-                self.io.data = full_dataframe
-                self.io.res_path = results_path
-                self.io.output_recap(results_path)
-            else:
-                with st.spinner("Running flux calculation..."):
+            full_dataframe = self.io.data.copy()
+            results_path = copy(self.io.res_path)
+            experiments = list(self.io.data["experiments"].unique())
+            self.io.multiple_experiments = []
+            for experiment in experiments:
+                with st.spinner(f"Running optimization for {experiment}"):
+                    # final_table_dict = {}
+                    self.model.data = full_dataframe[
+                        full_dataframe["experiments"] == experiment
+                    ].drop("experiments", axis=1).copy()
+
+                    self.io.res_path = results_path / experiment
+                    if not self.io.res_path.is_dir():
+                        self.io.res_path.mkdir()
                     # Initialize the fitter object
                     self.io.names = self.io.data.columns[1:].to_list()
                     kwargs = self._build_fitter_kwargs()
                     fitter = self.io.initialize_fitter(
-                        self.io.data,
+                        self.model.data,
                         model=kwargs["model"],
                         mc=kwargs["mc"],
                         iterations=kwargs["iterations"],
                         sd=kwargs["sd"],
                         debug_mode=kwargs["debug_mode"]
                     )
-                    # Do the work and export results
+                    # Do the work
                     fitter.optimize()
                     if self.mc:
                         fitter.monte_carlo_analysis()
                     fitter.khi2_test()
+                    df = pd.DataFrame.from_dict(
+                        fitter.parameter_stats,
+                        orient="columns"
+                    )
+                    df.index = [
+                        f"{experiment} {param}" for param in fitter.model.parameters_to_estimate.keys()
+                    ]
+                    st.write(df)
+                    self.io.multiple_experiments.append(df)
+
+                    # Export results
                     self.io.output_report(fitter, self.io.res_path)
                     self.io.plot_data(fitter)
                     self.io.output_plots(fitter, self.io.res_path)
-                    with st.expander("Plots"):
+                    with st.expander(f"{experiment} plots"):
                         for fig in self.io.figures:
                             st.pyplot(fig[1])
                     self.io.output_pdf(fitter, self.io.res_path)
                     # Reset figures to free memory
                     self.io.figures = []
                     self.config_parser.export_config(self.io.res_path)
-                st.success(
-                    f"Run is finished. Check {self.io.res_path} for "
-                    f"the results."
-                )
+            self.io.data = full_dataframe
+            self.io.res_path = results_path
+            self.io.output_recap(results_path)
 
     def silent_sim(self):
 
         self.model.simulate(
             [param for param in self.model.parameters_to_estimate.values()],
             self.model.experimental_matrix,
             self.model.time_vector,
```

### Comparing `physiofit-3.0.6/pyproject.toml` & `physiofit-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "physiofit"
-version = "3.0.6"
+version = "3.1.0"
 description = "Calculate extracellular fluxes from metabolite concentrations and biomass data"
 authors = ["llegregam <legregam@insa-toulouse.fr>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 
 [tool.poetry.scripts]
 physiofit = 'physiofit.__main__:main'
```

### Comparing `physiofit-3.0.6/setup.py` & `physiofit-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'streamlit>=1.20.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['physiofit = physiofit.__main__:main']}
 
 setup_kwargs = {
     'name': 'physiofit',
-    'version': '3.0.6',
+    'version': '3.1.0',
     'description': 'Calculate extracellular fluxes from metabolite concentrations and biomass data',
     'long_description': '# PhysioFit\n\n[![PyPI version](https://badge.fury.io/py/physiofit.svg)](https://badge.fury.io/py/physiofit)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/physiofit.svg)](https://pypi.python.org/pypi/physiofit/)\n[![Documentation Status](https://readthedocs.org/projects/physiofit/badge/?version=latest)](http://physiofit.readthedocs.io/?badge=latest)\n\n\n## What is PhysioFit?\n**PhysioFit is a scientific tool designed to quantify cell growth parameters and uptake & production fluxes**\n\nFluxes are estimated using various mathematical models by fitting time-course measurements of the concentration of\ncells and extracellular substrates and products. PhysioFit v3 includes by default the most common growth models, and\nadditional models can be implemented by users.\n\nIt is one of the routine tools that we use at the [MetaSys team](http://www.lisbp.fr/en/research/molecular-physiology-and-metabolism/metasys.html) \nand [MetaToul platform](http://www.metatoul.fr) in functional studies of metabolic systems.\n\nThe code is open-source, and available under a GPLv3 license. Additional information can be found in the following \n[publication](https://doi.org/10.1128/aem.00768-19).\n\nDetailed documentation can be found online at Read the Docs \n([https://physiofit.readthedocs.io/](https://physiofit.readthedocs.io/)).\n\n## Key features\n   * **calculation of growth rate and extracellular (uptake and production) fluxes**,\n   * default models for quantifying parameters in steady-state conditions (with and without lag & metabolite degradation\n     over time),\n   * **user-defined growth models**,\n   * Monte-Carlo sensitivity analysis to **estimate the precision of the calculated fluxes**,\n   * **evaluation of the goodness of fit and visual inspection of the fitted curves**,\n   * shipped as a **library** with both a **graphical** and **command line** interface,\n   * open-source, free and easy to install everywhere where Python 3 and pip run,\n   * **biologist-friendly**.\n\n## Quick-start\nPhysioFit requires Python 3.7 or higher and run on all platforms.\nPlease check [the documentation](https://physiofit.readthedocs.io/en/latest/quickstart.html) for complete\ninstallation and usage instructions.\n\nUse `pip` to **install PhysioFit from PyPi**:\n\n```bash\n$ pip install physiofit\n```\n\nThen, start the graphical interface with:\n\n```bash\n$ physiofit\n```\n\nPhysioFit is also available directly from command-line and as a Python library.\n\n## Bug and feature requests\nIf you have an idea on how we could improve PhysioFit please submit a new *issue*\nto [our GitHub issue tracker](https://github.com/MetaSys-LISBP/PhysioFit/issues).\n\n\n## Developers guide\n### Contributions\nContributions are very welcome! :heart:\n\nPlease work on your own fork,\nfollow [PEP8](https://www.python.org/dev/peps/pep-0008/) style guide,\nand make sure you pass all the tests before a pull request.\n\n### Local install with pip\nIn development mode, do a `pip install -e /path/to/PhysioFit` to install\nlocally the development version.\n\n### Build the documentation locally\nBuild the HTML documentation with:\n\n```bash\n$ cd doc\n$ make html\n```\n\nThe PDF documentation can be built locally by replacing `html` by `latexpdf`\nin the command above. You will need a recent latex installation.\n\n## How to cite\nPhysioFit: quantifying cell growth parameters and uptake and production fluxes.\nLe Grégam L., Guitton Y., Bellvert F., Jourdan F., Portais J.C., Millard P.\nIn preparation for publication\n\n## Authors\nLoïc Le Grégam, Pierre Millard\n\n## Contact\n:email: legregam@insa-toulouse.fr, millard@insa-toulouse.fr\n',
     'author': 'llegregam',
     'author_email': 'legregam@insa-toulouse.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `physiofit-3.0.6/PKG-INFO` & `physiofit-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physiofit
-Version: 3.0.6
+Version: 3.1.0
 Summary: Calculate extracellular fluxes from metabolite concentrations and biomass data
 License: GNU General Public License (GPL)
 Author: llegregam
 Author-email: legregam@insa-toulouse.fr
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

