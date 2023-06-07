# Comparing `tmp/meow-sim-0.5.0.tar.gz` & `tmp/meow-sim-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.0.tar", last modified: Wed Jun  7 04:02:56 2023, max compression
+gzip compressed data, was "meow-sim-0.5.1.tar", last modified: Wed Jun  7 14:51:36 2023, max compression
```

## Comparing `meow-sim-0.5.0.tar` & `meow-sim-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-07 04:02:52.000000 meow-sim-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 04:02:56.360557 meow-sim-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-07 04:02:52.000000 meow-sim-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.356557 meow-sim-0.5.0/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5533 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12184 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-07 04:02:52.000000 meow-sim-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 04:02:56.360557 meow-sim-0.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-07 04:02:52.000000 meow-sim-0.5.0/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-07 04:02:52.000000 meow-sim-0.5.0/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-07 04:02:52.000000 meow-sim-0.5.0/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.654299 meow-sim-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-07 14:51:31.000000 meow-sim-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 14:51:36.650298 meow-sim-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-07 14:51:31.000000 meow-sim-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5533 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12861 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7658 2023-06-07 14:51:31.000000 meow-sim-0.5.1/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-07 14:51:36.000000 meow-sim-0.5.1/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-07 14:51:31.000000 meow-sim-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 14:51:36.654299 meow-sim-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 14:51:36.650298 meow-sim-0.5.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-07 14:51:31.000000 meow-sim-0.5.1/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-07 14:51:31.000000 meow-sim-0.5.1/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-07 14:51:31.000000 meow-sim-0.5.1/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.0/LICENSE` & `meow-sim-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/PKG-INFO` & `meow-sim-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.0/README.md` & `meow-sim-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/__init__.py` & `meow-sim-0.5.1/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.0/meow/assets/silicon.csv` & `meow-sim-0.5.1/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.1/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/base_model.py` & `meow-sim-0.5.1/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/cache.py` & `meow-sim-0.5.1/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/cell.py` & `meow-sim-0.5.1/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/cross_section.py` & `meow-sim-0.5.1/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/eme/__init__.py` & `meow-sim-0.5.1/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/eme/common.py` & `meow-sim-0.5.1/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/eme/sax.py` & `meow-sim-0.5.1/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/environment.py` & `meow-sim-0.5.1/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/fde/lumerical.py` & `meow-sim-0.5.1/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/fde/tidy3d.py` & `meow-sim-0.5.1/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/gds_structures.py` & `meow-sim-0.5.1/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/geometries.py` & `meow-sim-0.5.1/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/integrate.py` & `meow-sim-0.5.1/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/materials.py` & `meow-sim-0.5.1/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/mesh.py` & `meow-sim-0.5.1/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow/mode.py` & `meow-sim-0.5.1/meow/mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
 from scipy.linalg import norm
 
 from .base_model import BaseModel
 from .cross_section import CrossSection
 from .integrate import integrate_2d
+from .visualize import _figsize_visualize_mode
 
 
 class Mode(BaseModel):
     """A `Mode` contains the field information for a given `CrossSection`."""
 
     neff: complex = Field(description="the effective index of the mode")
     cs: CrossSection = Field(
@@ -116,49 +117,60 @@
         title=None,
         fields=None,
         ax=None,
         n_cmap=None,
         mode_cmap=None,
         num_levels=8,
         operation=lambda x: np.abs(x) ** 2,
+        show=True,
     ):
         import matplotlib.pyplot as plt  # fmt: skip
         from matplotlib import colors  # fmt: skip
+        from mpl_toolkits.axes_grid1 import make_axes_locatable  # fmt: skip
+        W, H = _figsize_visualize_mode(self.cs, 6.4)
 
-        if fields is None or len(fields) == 0:
+        if not fields:
             fields = ["Ex"]
 
         if len(fields) > 1:
+            if len(fields) > 2:
+                max_width = 15
+                current_width = len(fields) * W
+                W, H = _figsize_visualize_mode(self.cs, 6.4 * max_width / current_width)
             if ax is None:
-                _, ax = plt.subplots(len(fields), 1, figsize=(5, len(fields) * 3))
+                _, ax = plt.subplots(1, len(fields), figsize=(len(fields) * W, H))
             if len(ax) < len(fields):
                 raise ValueError(
                     f"Not enough axes supplied for the number of fields "
                     f"to plot! {len(ax)} < {len(fields)}."
                 )
             for field, ax_ in zip(fields, ax):
                 self._visualize(
-                    field,
+                    title=title,
+                    fields=[field],
                     ax=ax_,
                     n_cmap=n_cmap,
                     mode_cmap=mode_cmap,
                     num_levels=num_levels,
+                    operation=operation,
+                    show=False,
                 )
+            if show:
+                plt.show()
             return
 
         field = fields[0]
         valid_fields = ["Ex", "Ey", "Ez", "Hx", "Hy", "Hz", "Px", "Py", "Pz"]
         if field not in valid_fields:
             raise ValueError(
                 f"Invalid field {field!r}. Valid fields: {', '.join(valid_fields)}."
             )
 
         if ax is None:
             ax = plt.gca()
-            plt.axis("scaled")
         plt.sca(ax)
 
         x, y = "x", "y"  # currently only propagation in z supported, see Mesh2d
         c = field[-1]
         if n_cmap is None:
             n_cmap = colors.LinearSegmentedColormap.from_list(
                 name="c_cmap", colors=["#ffffff", "#c1d9ed"]
@@ -166,30 +178,35 @@
         if mode_cmap is None:
             mode_cmap = "inferno"
         X = getattr(self.mesh, f"X{c}")
         Y = getattr(self.mesh, f"Y{c}")
         mode = operation(getattr(self, field))
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
-            plt.contour(X, Y, mode, cmap=mode_cmap, levels=np.linspace(mode.min(), mode.max(), num_levels))  # fmt: skip
-        plt.colorbar(label="mode")
+            levels = np.linspace(mode.min(), mode.max(), num_levels + 1)[1:]
+            plt.contour(X, Y, mode, cmap=mode_cmap, levels=levels)  # fmt: skip
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.05)
+        plt.colorbar(cax=cax)
+        plt.sca(ax)
 
         n = np.real(getattr(self.cs, f"n{c}"))
         plt.pcolormesh(X, Y, n, cmap=n_cmap)
-        plt.colorbar(label="n")
         plt.xlabel(x)
         plt.ylabel(y)
         plt.grid(True, alpha=0.4)
         if title is None:
             plt.title(f"{field} [neff={float(np.real(self.neff)):.6f}]")
         else:
             plt.title(title)
         plt.xlim(X.min(), X.max())
         plt.ylim(Y.min(), Y.max())
-        plt.show()
+        plt.axis("scaled")
+        if show:
+            plt.show()
 
     def save(self, filename):
         with open(filename, "wb") as file:
             pickle.dump(self, file)
 
     @classmethod
     def load(cls, filename):
```

### Comparing `meow-sim-0.5.0/meow/structures.py` & `meow-sim-0.5.1/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.1/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.0/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.1/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/pyproject.toml` & `meow-sim-0.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.0/tests/test_deserialization.py` & `meow-sim-0.5.1/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/tests/test_mode_operators.py` & `meow-sim-0.5.1/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.0/tests/test_nbs.py` & `meow-sim-0.5.1/tests/test_nbs.py`

 * *Files identical despite different names*

