# Comparing `tmp/freeflux-0.3.3.tar.gz` & `tmp/freeflux-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\cwu\Desktop\Software\FreeFlux\pypi\freeflux-0.3.3\dist\.tmp-ho6do_pt\freeflux-0.3.3.tar", last modified: Mon Apr 24 08:23:57 2023, max compression
+gzip compressed data, was "C:\Users\cwu\Desktop\Software\FreeFlux\pypi\freeflux-0.3.4\dist\.tmp-3707hrhn\freeflux-0.3.4.tar", last modified: Wed Jun  7 20:06:51 2023, max compression
```

## Comparing `freeflux-0.3.3.tar` & `freeflux-0.3.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.231616 freeflux-0.3.3/
--rw-rw-rw-   0        0        0    35149 2022-08-18 01:02:32.000000 freeflux-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     5239 2023-04-24 08:23:57.232615 freeflux-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4188 2023-04-07 06:00:51.000000 freeflux-0.3.3/README.rst
--rw-rw-rw-   0        0        0       90 2023-04-03 02:02:48.000000 freeflux-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0     1232 2023-04-24 08:23:57.237600 freeflux-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-18 21:36:18.000000 freeflux-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.057083 freeflux-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.091990 freeflux-0.3.3/src/freeflux/
--rw-rw-rw-   0        0        0      247 2023-04-24 08:23:21.000000 freeflux-0.3.3/src/freeflux/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.138865 freeflux-0.3.3/src/freeflux/analysis/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.3/src/freeflux/analysis/__init__.py
--rw-rw-rw-   0        0        0    23297 2023-04-18 21:42:54.000000 freeflux-0.3.3/src/freeflux/analysis/fit.py
--rw-rw-rw-   0        0        0    21603 2023-04-18 21:44:20.000000 freeflux-0.3.3/src/freeflux/analysis/inst_fit.py
--rw-rw-rw-   0        0        0     6538 2023-04-18 21:44:44.000000 freeflux-0.3.3/src/freeflux/analysis/inst_simulate.py
--rw-rw-rw-   0        0        0    10165 2023-04-18 21:46:20.000000 freeflux-0.3.3/src/freeflux/analysis/simulate.py
--rw-rw-rw-   0        0        0    12497 2023-04-24 08:02:13.000000 freeflux-0.3.3/src/freeflux/analysis/stats.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.166791 freeflux-0.3.3/src/freeflux/core/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.3/src/freeflux/core/__init__.py
--rw-rw-rw-   0        0        0     4989 2023-04-18 21:49:39.000000 freeflux-0.3.3/src/freeflux/core/emu.py
--rw-rw-rw-   0        0        0    12887 2023-04-24 08:02:34.000000 freeflux-0.3.3/src/freeflux/core/mdv.py
--rw-rw-rw-   0        0        0     2553 2023-03-31 21:40:13.000000 freeflux-0.3.3/src/freeflux/core/metabolite.py
--rw-rw-rw-   0        0        0    35901 2023-04-18 21:53:25.000000 freeflux-0.3.3/src/freeflux/core/model.py
--rw-rw-rw-   0        0        0    11011 2023-04-18 21:49:24.000000 freeflux-0.3.3/src/freeflux/core/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.180753 freeflux-0.3.3/src/freeflux/io/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:20.000000 freeflux-0.3.3/src/freeflux/io/__init__.py
--rw-rw-rw-   0        0        0     3147 2023-04-24 07:59:36.000000 freeflux-0.3.3/src/freeflux/io/inputs.py
--rw-rw-rw-   0        0        0    33246 2023-04-24 08:03:00.000000 freeflux-0.3.3/src/freeflux/io/results.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.190728 freeflux-0.3.3/src/freeflux/optim/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:49.000000 freeflux-0.3.3/src/freeflux/optim/__init__.py
--rw-rw-rw-   0        0        0     9270 2023-04-18 21:54:53.000000 freeflux-0.3.3/src/freeflux/optim/optim.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.204690 freeflux-0.3.3/src/freeflux/solver/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:33:01.000000 freeflux-0.3.3/src/freeflux/solver/__init__.py
--rw-rw-rw-   0        0        0     3375 2023-04-01 23:47:14.000000 freeflux-0.3.3/src/freeflux/solver/lpsolver.py
--rw-rw-rw-   0        0        0    19803 2023-04-24 08:03:20.000000 freeflux-0.3.3/src/freeflux/solver/nlpsolver.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.225635 freeflux-0.3.3/src/freeflux/utils/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.3/src/freeflux/utils/__init__.py
--rw-rw-rw-   0        0        0      496 2023-03-26 22:55:07.000000 freeflux-0.3.3/src/freeflux/utils/context.py
--rw-rw-rw-   0        0        0     1916 2023-04-01 23:41:09.000000 freeflux-0.3.3/src/freeflux/utils/progress.py
--rw-rw-rw-   0        0        0    33624 2023-04-24 08:06:34.000000 freeflux-0.3.3/src/freeflux/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.110941 freeflux-0.3.3/src/freeflux.egg-info/
--rw-rw-rw-   0        0        0     5239 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.459902 freeflux-0.3.4/
+-rw-rw-rw-   0        0        0    35149 2022-08-18 01:02:32.000000 freeflux-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     5239 2023-06-07 20:06:51.460900 freeflux-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4188 2023-04-07 06:00:51.000000 freeflux-0.3.4/README.rst
+-rw-rw-rw-   0        0        0       90 2023-04-03 02:02:48.000000 freeflux-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1232 2023-06-07 20:06:51.466884 freeflux-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-04-18 21:36:18.000000 freeflux-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.224531 freeflux-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.265422 freeflux-0.3.4/src/freeflux/
+-rw-rw-rw-   0        0        0      247 2023-06-05 21:04:50.000000 freeflux-0.3.4/src/freeflux/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.332244 freeflux-0.3.4/src/freeflux/analysis/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.4/src/freeflux/analysis/__init__.py
+-rw-rw-rw-   0        0        0    23464 2023-06-05 20:59:06.000000 freeflux-0.3.4/src/freeflux/analysis/fit.py
+-rw-rw-rw-   0        0        0    21702 2023-06-05 21:01:09.000000 freeflux-0.3.4/src/freeflux/analysis/inst_fit.py
+-rw-rw-rw-   0        0        0     6538 2023-04-18 21:44:44.000000 freeflux-0.3.4/src/freeflux/analysis/inst_simulate.py
+-rw-rw-rw-   0        0        0    10165 2023-04-18 21:46:20.000000 freeflux-0.3.4/src/freeflux/analysis/simulate.py
+-rw-rw-rw-   0        0        0    12546 2023-06-05 21:03:42.000000 freeflux-0.3.4/src/freeflux/analysis/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.372137 freeflux-0.3.4/src/freeflux/core/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.4/src/freeflux/core/__init__.py
+-rw-rw-rw-   0        0        0     4989 2023-04-18 21:49:39.000000 freeflux-0.3.4/src/freeflux/core/emu.py
+-rw-rw-rw-   0        0        0    12887 2023-04-24 08:02:34.000000 freeflux-0.3.4/src/freeflux/core/mdv.py
+-rw-rw-rw-   0        0        0     2553 2023-03-31 21:40:13.000000 freeflux-0.3.4/src/freeflux/core/metabolite.py
+-rw-rw-rw-   0        0        0    35901 2023-04-18 21:53:25.000000 freeflux-0.3.4/src/freeflux/core/model.py
+-rw-rw-rw-   0        0        0    11011 2023-04-18 21:49:24.000000 freeflux-0.3.4/src/freeflux/core/reaction.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.391086 freeflux-0.3.4/src/freeflux/io/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:20.000000 freeflux-0.3.4/src/freeflux/io/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-04-24 07:59:36.000000 freeflux-0.3.4/src/freeflux/io/inputs.py
+-rw-rw-rw-   0        0        0    33246 2023-04-24 08:03:00.000000 freeflux-0.3.4/src/freeflux/io/results.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.404052 freeflux-0.3.4/src/freeflux/optim/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:49.000000 freeflux-0.3.4/src/freeflux/optim/__init__.py
+-rw-rw-rw-   0        0        0     9270 2023-04-18 21:54:53.000000 freeflux-0.3.4/src/freeflux/optim/optim.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.426990 freeflux-0.3.4/src/freeflux/solver/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:33:01.000000 freeflux-0.3.4/src/freeflux/solver/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-04-01 23:47:14.000000 freeflux-0.3.4/src/freeflux/solver/lpsolver.py
+-rw-rw-rw-   0        0        0    19803 2023-04-24 08:03:20.000000 freeflux-0.3.4/src/freeflux/solver/nlpsolver.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.452921 freeflux-0.3.4/src/freeflux/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.4/src/freeflux/utils/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-03-26 22:55:07.000000 freeflux-0.3.4/src/freeflux/utils/context.py
+-rw-rw-rw-   0        0        0     1916 2023-04-01 23:41:09.000000 freeflux-0.3.4/src/freeflux/utils/progress.py
+-rw-rw-rw-   0        0        0    33750 2023-06-05 21:02:38.000000 freeflux-0.3.4/src/freeflux/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:06:51.293348 freeflux-0.3.4/src/freeflux.egg-info/
+-rw-rw-rw-   0        0        0     5239 2023-06-07 20:06:51.000000 freeflux-0.3.4/src/freeflux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-06-07 20:06:51.000000 freeflux-0.3.4/src/freeflux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:06:51.000000 freeflux-0.3.4/src/freeflux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-06-07 20:06:51.000000 freeflux-0.3.4/src/freeflux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 20:06:51.000000 freeflux-0.3.4/src/freeflux.egg-info/top_level.txt
```

### Comparing `freeflux-0.3.3/LICENSE` & `freeflux-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/PKG-INFO` & `freeflux-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeflux
-Version: 0.3.3
+Version: 0.3.4
 Summary: FreeFlux is a package for 13C metabolic flux analysis
 Home-page: https://github.com/Chaowu88/freeflux
 Author: Chao Wu
 Author-email: chaowu09@gmail.com
 License: GNU General Public License v3.0
 Keywords: 13c,labeling pattern,metabolic flux analysis,metabolism,biology,non-linear programming,optimization,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freeflux-0.3.3/README.rst` & `freeflux-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/setup.cfg` & `freeflux-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 7265 6566 6c75 780d 0a76 6572   = freeflux..ver
-00000020: 7369 6f6e 203d 2030 2e33 2e33 0d0a 6175  sion = 0.3.3..au
+00000020: 7369 6f6e 203d 2030 2e33 2e34 0d0a 6175  sion = 0.3.4..au
 00000030: 7468 6f72 203d 2043 6861 6f20 5775 0d0a  thor = Chao Wu..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2063  author_email = c
 00000050: 6861 6f77 7530 3940 676d 6169 6c2e 636f  haowu09@gmail.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2046 7265 6546 6c75 7820 6973 2061 2070   FreeFlux is a p
 00000080: 6163 6b61 6765 2066 6f72 2031 3343 206d  ackage for 13C m
 00000090: 6574 6162 6f6c 6963 2066 6c75 7820 616e  etabolic flux an
```

### Comparing `freeflux-0.3.3/src/freeflux/analysis/fit.py` & `freeflux-0.3.4/src/freeflux/analysis/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,18 +619,25 @@
             
             optModel = MFAModel(self.model, fit_measured_fluxes, solver)
             optModel.build_objective()
             optModel.build_gradient()
             optModel.build_flux_bound_constraints()
             optModel.build_initial_flux_values(ini_netfluxes = iniFluxes)
 
-            while True:
-                optTotalfluxes, optNetfluxes, *_, isSuccess = optModel.solve_flux(tol, max_iters)
-                if isSuccess:
-                    break
+            try:
+                while True:
+                    (optTotalfluxes, 
+                     optNetfluxes, 
+                     *_, 
+                     isSuccess
+                    ) = optModel.solve_flux(tol, max_iters)
+                    if isSuccess:
+                        break
+            except:
+                continue
             optTotalfluxesSet.append(optTotalfluxes)
             optNetfluxesSet.append(optNetfluxes)
             
             self.calculator._reset_measured_fluxes()
             self.calculator._reset_measured_MDVs()
                
         return optTotalfluxesSet, optNetfluxesSet
```

### Comparing `freeflux-0.3.3/src/freeflux/analysis/inst_fit.py` & `freeflux-0.3.4/src/freeflux/analysis/inst_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,23 +508,26 @@
             
             optModel = InstMFAModel(self.model, fit_measured_fluxes, solver)
             optModel.build_objective()
             optModel.build_gradient()
             optModel.build_flux_and_conc_bound_constraints()
             optModel.build_initial_flux_and_conc_values(ini_netfluxes = iniFluxes)
             
-            while True:
-                (optTotalfluxes, 
-                 optNetfluxes, 
-                 optConcs, 
-                 *_, 
-                 isSuccess
-                ) = optModel.solve_flux(tol, max_iters)
-                if isSuccess:
-                    break
+            try:
+                while True:
+                    (optTotalfluxes, 
+                     optNetfluxes, 
+                     optConcs, 
+                      *_, 
+                     isSuccess
+                    ) = optModel.solve_flux(tol, max_iters)
+                    if isSuccess:
+                        break
+            except:
+                continue
             optTotalfluxesSet.append(optTotalfluxes)
             optNetfluxesSet.append(optNetfluxes)
             optConcsSet.append(optConcs)
             
             self.calculator._reset_measured_fluxes()
             self.calculator._reset_measured_inst_MDVs()
```

### Comparing `freeflux-0.3.3/src/freeflux/analysis/inst_simulate.py` & `freeflux-0.3.4/src/freeflux/analysis/inst_simulate.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/analysis/simulate.py` & `freeflux-0.3.4/src/freeflux/analysis/simulate.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/analysis/stats.py` & `freeflux-0.3.4/src/freeflux/analysis/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,19 @@
     '''
     
     chi2Lb = chi2.ppf((1-confidence_level)/2, dof)
     chi2Ub = chi2.ppf((1+confidence_level)/2, dof)
     
     flag = '' if chi2Lb <= obj_value <= chi2Ub else 'not '
     
-    print(f'SSR {obj_value:.2f} {flag}acceptable, which is {flag}in [{chi2Lb}, {chi2Ub}]'
-          f'of {confidence_level*100}%% confidence level by chi2 test')
+    print(
+        f'SSR {obj_value:.2f} {flag}acceptable,'
+        f' which is {flag}in [{round(chi2Lb, 2)}, {round(chi2Ub, 2)}]'
+        f' of the {confidence_level*100}%% confidence level by chi2 test'
+    )
 
 
 def _normal_probability(resids, show_fig, output_dir):
     '''
     Parameters
     ----------
     resids: array
```

### Comparing `freeflux-0.3.3/src/freeflux/core/emu.py` & `freeflux-0.3.4/src/freeflux/core/emu.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/core/mdv.py` & `freeflux-0.3.4/src/freeflux/core/mdv.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/core/metabolite.py` & `freeflux-0.3.4/src/freeflux/core/metabolite.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/core/model.py` & `freeflux-0.3.4/src/freeflux/core/model.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/core/reaction.py` & `freeflux-0.3.4/src/freeflux/core/reaction.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/io/inputs.py` & `freeflux-0.3.4/src/freeflux/io/inputs.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/io/results.py` & `freeflux-0.3.4/src/freeflux/io/results.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/optim/optim.py` & `freeflux-0.3.4/src/freeflux/optim/optim.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/solver/lpsolver.py` & `freeflux-0.3.4/src/freeflux/solver/lpsolver.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/solver/nlpsolver.py` & `freeflux-0.3.4/src/freeflux/solver/nlpsolver.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/utils/progress.py` & `freeflux-0.3.4/src/freeflux/utils/progress.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.3/src/freeflux/utils/utils.py` & `freeflux-0.3.4/src/freeflux/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,15 +632,15 @@
                 else:
                     mdvs = [ChainMap(simMDVs, self.model.substrate_MDVs)[emu] 
                             for emu in sourceEMU]
                     sourceMDV = reduce(conv, mdvs)
                 Y.append(sourceMDV)    
             Y = np.array(Y)
             
-            X = pinv2(A)@B@Y
+            X = pinv2(A, check_finite = True)@B@Y
         
             simMDVs.update(zip(productEMUs, X))
             
         simMDVs = {emu.id: mdv for emu, mdv in simMDVs.items()}
         
         return simMDVs
                     
@@ -663,15 +663,15 @@
             
             lambA, fluxidsA, productEMUs = self.model.matrix_As[size]
             lambB, fluxidsB, sourceEMUs = self.model.matrix_Bs[size]
             
             A = lambA(*self.model.total_fluxes[fluxidsA])
             B = lambB(*self.model.total_fluxes[fluxidsB])
             
-            Ainv = pinv2(A)
+            Ainv = pinv2(A, check_finite = True)
             
             Ader = self.model.matrix_As_der_p[size]   
             Bder = self.model.matrix_Bs_der_p[size]   
             
             Y = []
             Yder = []
             for sourceEMU in sourceEMUs:
@@ -738,18 +738,18 @@
                     lambA, fluxidsA, productEMUs = self.model.matrix_As[size]
                     lambB, fluxidsB, sourceEMUs = self.model.matrix_Bs[size]
                     lambM, metabids =  self.model.matrix_Ms[size]
                     
                     A = lambA(*self.model.total_fluxes[fluxidsA])
                     B = lambB(*self.model.total_fluxes[fluxidsB])
                     M = lambM(*self.model.concentrations[metabids])
-                    Minv = pinv2(M)
+                    Minv = pinv2(M, check_finite = True)
                     
                     F = Minv@A
-                    Finv = pinv2(F)
+                    Finv = pinv2(F, check_finite = True)
                     I = np.eye(*F.shape)
                     Phi = expm(F*deltat)
                     Gamma = (Phi - I)@Finv
                     Omega = (Gamma/deltat - I)@Finv
                     
                     X_t0 = Xs[t0][size]
                     
@@ -828,23 +828,23 @@
                     lambA, fluxidsA, productEMUs = self.model.matrix_As[size]
                     lambB, fluxidsB, sourceEMUs = self.model.matrix_Bs[size]
                     lambM, metabids =  self.model.matrix_Ms[size]
             
                     A = lambA(*self.model.total_fluxes[fluxidsA])
                     B = lambB(*self.model.total_fluxes[fluxidsB])
                     M = lambM(*self.model.concentrations[metabids])
-                    Minv = pinv2(M)
+                    Minv = pinv2(M, check_finite = True)
                     
                     Ader = self.model.matrix_As_der_p[size]   
                     Bder = self.model.matrix_Bs_der_p[size]   
                     Mder = self.model.matrix_Ms_der_p[size]   
                     Minvder = -Minv@Mder@Minv
                     
                     F = Minv@A
-                    Finv = pinv2(F)
+                    Finv = pinv2(F, check_finite = True)
                     I = np.eye(*F.shape)
                     Phi = expm(F*deltat)
                     Gamma = (Phi - I)@Finv
                     Omega = (Gamma/deltat - I)@Finv
                     
                     X_t0 = Xs[t0][size]
```

### Comparing `freeflux-0.3.3/src/freeflux.egg-info/PKG-INFO` & `freeflux-0.3.4/src/freeflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeflux
-Version: 0.3.3
+Version: 0.3.4
 Summary: FreeFlux is a package for 13C metabolic flux analysis
 Home-page: https://github.com/Chaowu88/freeflux
 Author: Chao Wu
 Author-email: chaowu09@gmail.com
 License: GNU General Public License v3.0
 Keywords: 13c,labeling pattern,metabolic flux analysis,metabolism,biology,non-linear programming,optimization,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freeflux-0.3.3/src/freeflux.egg-info/SOURCES.txt` & `freeflux-0.3.4/src/freeflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

