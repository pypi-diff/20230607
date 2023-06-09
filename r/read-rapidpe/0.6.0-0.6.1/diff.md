# Comparing `tmp/read_rapidpe-0.6.0.tar.gz` & `tmp/read_rapidpe-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_rapidpe-0.6.0.tar", max compression
+gzip compressed data, was "read_rapidpe-0.6.1.tar", max compression
```

## Comparing `read_rapidpe-0.6.0.tar` & `read_rapidpe-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.6.0/README.md
--rw-r--r--   0        0        0      627 2023-06-06 23:20:26.804855 read_rapidpe-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      342 2023-06-04 17:50:03.396354 read_rapidpe-0.6.0/read_rapidpe/__init__.py
--rw-r--r--   0        0        0    11295 2023-05-13 16:31:51.989559 read_rapidpe-0.6.0/read_rapidpe/grid_point.py
--rw-r--r--   0        0        0     3620 2023-06-03 15:19:21.433555 read_rapidpe-0.6.0/read_rapidpe/io.py
--rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.6.0/read_rapidpe/p_astro.py
--rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.6.0/read_rapidpe/parser.py
--rw-r--r--   0        0        0     5890 2023-06-04 20:42:24.365320 read_rapidpe-0.6.0/read_rapidpe/plot.py
--rw-r--r--   0        0        0        0 2023-06-06 20:59:26.587831 read_rapidpe-0.6.0/read_rapidpe/plugins/__init__.py
--rw-r--r--   0        0        0     6291 2023-06-06 23:15:51.020171 read_rapidpe-0.6.0/read_rapidpe/plugins/em_bright.py
--rw-r--r--   0        0        0    35379 2023-06-06 00:08:56.172702 read_rapidpe-0.6.0/read_rapidpe/result.py
--rw-r--r--   0        0        0     8855 2023-06-03 14:39:22.849276 read_rapidpe-0.6.0/read_rapidpe/transform.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.6.1/README.md
+-rw-r--r--   0        0        0      627 2023-06-07 01:53:20.641288 read_rapidpe-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      342 2023-06-04 17:50:03.396354 read_rapidpe-0.6.1/read_rapidpe/__init__.py
+-rw-r--r--   0        0        0    11295 2023-05-13 16:31:51.989559 read_rapidpe-0.6.1/read_rapidpe/grid_point.py
+-rw-r--r--   0        0        0     3620 2023-06-03 15:19:21.433555 read_rapidpe-0.6.1/read_rapidpe/io.py
+-rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.6.1/read_rapidpe/p_astro.py
+-rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.6.1/read_rapidpe/parser.py
+-rw-r--r--   0        0        0     6030 2023-06-07 01:30:58.750555 read_rapidpe-0.6.1/read_rapidpe/plot.py
+-rw-r--r--   0        0        0        0 2023-06-06 20:59:26.587831 read_rapidpe-0.6.1/read_rapidpe/plugins/__init__.py
+-rw-r--r--   0        0        0     6291 2023-06-06 23:15:51.020171 read_rapidpe-0.6.1/read_rapidpe/plugins/em_bright.py
+-rw-r--r--   0        0        0    37550 2023-06-07 01:45:49.754474 read_rapidpe-0.6.1/read_rapidpe/result.py
+-rw-r--r--   0        0        0     8855 2023-06-03 14:39:22.849276 read_rapidpe-0.6.1/read_rapidpe/transform.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.6.1/PKG-INFO
```

### Comparing `read_rapidpe-0.6.0/README.md` & `read_rapidpe-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/pyproject.toml` & `read_rapidpe-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "read-rapidpe"
-version = "0.6.0"
+version = "0.6.1"
 description = "Read and analyse results generated by rapidpe-rift-pipe"
 authors = ["Cory Chu <cory@gwlab.page>"]
 readme = "README.md"
 packages = [{include = "read_rapidpe"}]
 homepage = "https://github.com/c0rychu/read-rapidpe"
 repository = "https://git.ligo.org/yu-kuang.chu/read-rapidpe"
```

### Comparing `read_rapidpe-0.6.0/read_rapidpe/grid_point.py` & `read_rapidpe-0.6.1/read_rapidpe/grid_point.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/read_rapidpe/io.py` & `read_rapidpe-0.6.1/read_rapidpe/io.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/read_rapidpe/p_astro.py` & `read_rapidpe-0.6.1/read_rapidpe/p_astro.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/read_rapidpe/parser.py` & `read_rapidpe-0.6.1/read_rapidpe/parser.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/read_rapidpe/plot.py` & `read_rapidpe-0.6.1/read_rapidpe/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,25 +141,30 @@
     return mc, q
 
 
 # ===============================================
 # Plotting
 # ===============================================
 
-def plot_corner(samples, zoom_in_percent=None, show_titles=True, **kwargs):
+def plot_corner(samples,
+                zoom_in_percent=None,
+                plot_range=None,
+                show_titles=True,
+                **kwargs):
     import corner
 
-    if zoom_in_percent is None:
-        plot_range = None
-    else:
-        plot_range = []
-        for key in samples.keys():
-            a = np.percentile(samples[key], zoom_in_percent/2.0)
-            b = np.percentile(samples[key], 100.0-zoom_in_percent/2.0)
-            plot_range.append((a, b))
+    if plot_range is None:
+        if zoom_in_percent is None:
+            plot_range = None
+        else:
+            plot_range = []
+            for key in samples.keys():
+                a = np.percentile(samples[key], zoom_in_percent/2.0)
+                b = np.percentile(samples[key], 100.0-zoom_in_percent/2.0)
+                plot_range.append((a, b))
     return corner.corner(samples,
                          show_titles=show_titles,
                          range=plot_range,
                          **kwargs)
 
 
 def plot_grid(res, posterior_samples=True):
```

### Comparing `read_rapidpe-0.6.0/read_rapidpe/plugins/em_bright.py` & `read_rapidpe-0.6.1/read_rapidpe/plugins/em_bright.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/read_rapidpe/result.py` & `read_rapidpe-0.6.1/read_rapidpe/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         if iparam_search == "[mass1,mass2]":
             if distant_coord == "mchirp_q":
                 return ["chirp_mass", "mass_ratio"]
             elif distant_coord == "mchirp_eta":
                 return ["chirp_mass", "symmetric_mass_ratio"]
             else:
                 raise NotImplementedError("distance_coordinates not supported")
-        elif iparam_search == "[mass2,mass2,spin1z,spin2z]":
+        elif iparam_search == "[mass1,mass2,spin1z,spin2z]":
             if distant_coord == "mchirp_q":
                 return ["chirp_mass", "mass_ratio", "chi_eff", "chi_a"]
             elif distant_coord == "mchirp_eta":
                 return ["chirp_mass", "symmetric_mass_ratio", "chi_eff", "chi_a"]  # noqa E501
             else:
                 raise NotImplementedError("distance_coordinates not supported")
         else:
@@ -930,23 +930,80 @@
 
             if legend:
                 plt.legend(loc=legend_loc, fontsize="8", fancybox=False)
 
     def plot_corner(self,
                     columns=["mass_1", "mass_2"],
                     title=None,
+                    true_params=True,
+                    figsize=None,
                     **kwargs):
         from .plot import plot_corner
+        from matplotlib.lines import Line2D
+        import corner
 
         samples = {}
         for col in columns:
             try:
                 samples[col] = self.posterior_samples[col]
             except KeyError:
                 pass
 
         fig = plot_corner(samples, **kwargs)
 
+        if true_params:
+            legend = False
+            legend_elements = []
+            inj = False
+            pipe = False
+
+            x_inj = []
+            for col in columns:
+                try:
+                    x_inj.append(self.injection_info[col])
+                    legend = True
+                    inj = True
+                except (KeyError, AttributeError):
+                    x_inj.append(None)
+            if inj:
+                corner.overplot_lines(fig, x_inj, color="r")
+                corner.overplot_points(fig,
+                                       [x_inj],
+                                       marker="*",
+                                       markersize=10,
+                                       color="r",
+                                       label="Injection")
+                legend_elements.append(
+                    Line2D([0], [0], marker="*", color="r", markersize=10, label="Injection")  # noqa: E501
+                )
+
+            x_pipe = []
+            for col in columns:
+                try:
+                    x_pipe.append(self.event_info["intrinsic_param"][col])
+                    legend = True
+                    pipe = True
+                except (KeyError, AttributeError):
+                    x_pipe.append(None)
+            if pipe:
+                corner.overplot_lines(fig, x_pipe, color="b")
+                corner.overplot_points(fig,
+                                       [x_pipe],
+                                       marker="o",
+                                       color="b",
+                                       label="Search Pipeline")
+                legend_elements.append(
+                    Line2D([0], [0], marker="o", color="b", label="Search Pipeline")  # noqa: E501
+                )
+
+            if legend:
+                fig.legend(handles=legend_elements,
+                           bbox_to_anchor=(0.93, 0.85))
+
+        if figsize is not None:
+            fig.set_figwidth(figsize[0])
+            fig.set_figheight(figsize[1])
+
         if title is not None:
             fig.suptitle(title, y=1.05)
 
         return fig
```

### Comparing `read_rapidpe-0.6.0/read_rapidpe/transform.py` & `read_rapidpe-0.6.1/read_rapidpe/transform.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.6.0/PKG-INFO` & `read_rapidpe-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read-rapidpe
-Version: 0.6.0
+Version: 0.6.1
 Summary: Read and analyse results generated by rapidpe-rift-pipe
 Home-page: https://github.com/c0rychu/read-rapidpe
 Author: Cory Chu
 Author-email: cory@gwlab.page
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

