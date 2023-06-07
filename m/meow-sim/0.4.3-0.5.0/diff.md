# Comparing `tmp/meow-sim-0.4.3.tar.gz` & `tmp/meow-sim-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.4.3.tar", last modified: Tue Jun  6 21:21:53 2023, max compression
+gzip compressed data, was "meow-sim-0.5.0.tar", last modified: Wed Jun  7 04:02:56 2023, max compression
```

## Comparing `meow-sim-0.4.3.tar` & `meow-sim-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-06 21:21:47.000000 meow-sim-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 21:21:53.194868 meow-sim-0.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-06 21:21:47.000000 meow-sim-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.190868 meow-sim-0.4.3/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.190868 meow-sim-0.4.3/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.190868 meow-sim-0.4.3/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    12184 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     5962 2023-06-06 21:21:47.000000 meow-sim-0.4.3/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 21:21:53.000000 meow-sim-0.4.3/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-06 21:21:47.000000 meow-sim-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 21:21:53.194868 meow-sim-0.4.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:21:53.194868 meow-sim-0.4.3/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-06 21:21:47.000000 meow-sim-0.4.3/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-06 21:21:47.000000 meow-sim-0.4.3/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-06 21:21:47.000000 meow-sim-0.4.3/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-07 04:02:52.000000 meow-sim-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 04:02:56.360557 meow-sim-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-07 04:02:52.000000 meow-sim-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.356557 meow-sim-0.5.0/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5533 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12184 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-06-07 04:02:52.000000 meow-sim-0.5.0/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-07 04:02:56.000000 meow-sim-0.5.0/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-07 04:02:52.000000 meow-sim-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 04:02:56.360557 meow-sim-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:02:56.360557 meow-sim-0.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-07 04:02:52.000000 meow-sim-0.5.0/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-07 04:02:52.000000 meow-sim-0.5.0/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-07 04:02:52.000000 meow-sim-0.5.0/tests/test_nbs.py
```

### Comparing `meow-sim-0.4.3/LICENSE` & `meow-sim-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/PKG-INFO` & `meow-sim-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.3
+Version: 0.5.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.3/README.md` & `meow-sim-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/__init__.py` & `meow-sim-0.5.0/meow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.4.3"
+__version__ = "0.5.0"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.4.3/meow/assets/silicon.csv` & `meow-sim-0.5.0/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.0/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/base_model.py` & `meow-sim-0.5.0/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/cache.py` & `meow-sim-0.5.0/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/cell.py` & `meow-sim-0.5.0/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/cross_section.py` & `meow-sim-0.5.0/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/eme/__init__.py` & `meow-sim-0.5.0/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/eme/common.py` & `meow-sim-0.5.0/meow/eme/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,75 +19,86 @@
     conjugate_transpose: bool = DEFAULT_CONJUGATE_TRANSPOSE,
     enforce_reciprocity: bool = DEFAULT_ENFORCE_RECIPROCITY,
     enforce_lossy_unitarity: bool = DEFAULT_ENFORCE_LOSSY_UNITARITY,
 ):
     """get the S-matrix of the interface between two `CrossSection`s"""
     # overlap matrices
     inner_product = inner_product_conj if conjugate_transpose else inner_product_normal
-    transp = (lambda x: x.T.conj()) if conjugate_transpose else (lambda x: x.T)
+    conjugate = np.conj if conjugate_transpose else lambda a: a
+
     NL, NR = len(modes1), len(modes2)
     O_LL = np.array([inner_product(modes1[m], modes1[m]) for m in range(NL)])
     O_RR = np.array([inner_product(modes2[n], modes2[n]) for n in range(NR)])
     O_LR = np.array([[inner_product(modes1[m], modes2[n]) for n in range(NR)] for m in range(NL)])  # fmt: skip
     O_RL = np.array([[inner_product(modes2[m], modes1[n]) for n in range(NL)] for m in range(NR)])  # fmt: skip
 
     # extra phase correction (disabled?).
 
+    if conjugate_transpose:
+        O_LL = np.real(O_LL)
+        O_RR = np.real(O_RR)
+
     # ignoring the phase seems to corresponds best with lumerical.
-    # O_LL = np.abs(O_LL)
-    # O_RR = np.abs(O_RR)
 
     # alternative phase correction (probably worth testing this out)
+    # Question: is this not just a conjugation?
     # O_LL = O_LL*np.exp(-1j*np.angle(O_LL))
     # O_RR = O_RR*np.exp(-1j*np.angle(O_RR))
 
     # yet another alternative phase correction (probably worth testing this out too)
     # O_LR = O_LR*np.diag(np.exp(-1j*np.angle(np.diag(O_LR))))
     # O_RL = O_RL*np.diag(np.exp(-1j*np.angle(np.diag(O_RL))))
 
     # transmission L->R
-    LHS = O_LR + transp(O_RL)
+    LHS = conjugate(O_LR) + O_RL.T
     RHS = np.diag(2 * O_LL)
+
+    # print(f"LHS: {LHS}")
+    # vis(LHS)
+
+    # print(f"RHS: {RHS}")
+    # vis(RHS)
+
     T_LR, _, _, _ = np.linalg.lstsq(LHS, RHS, rcond=None)
 
     # HACK: we don't expect gain --> invert singular values that lead to gain
     # see: https://github.com/BYUCamachoLab/emepy/issues/12
     U, t, V = np.linalg.svd(T_LR, full_matrices=False)
     t = np.where(t > 1, 1 / t, t)
     T_LR = U @ np.diag(t) @ V
 
     # transmission R->L
-    LHS = O_RL + transp(O_LR)
+    LHS = conjugate(O_RL) + O_LR.T
     RHS = np.diag(2 * O_RR)
     T_RL, _, _, _ = np.linalg.lstsq(LHS, RHS, rcond=None)
 
     # HACK: we don't expect gain --> invert singular values that lead to gain
     U, t, V = np.linalg.svd(T_RL, full_matrices=False)
     t = np.where(t > 1, 1 / t, t)
     T_RL = U @ np.diag(t) @ V
 
     # reflection
-    R_LR = np.diag(1 / (2 * O_LL)) @ (transp(O_RL) - O_LR) @ T_LR  # type: ignore
-    R_RL = np.diag(1 / (2 * O_RR)) @ (transp(O_LR) - O_RL) @ T_RL  # type: ignore
+    R_LR = np.diag(1 / (2 * O_LL)) @ (O_RL.T - conjugate(O_LR)) @ T_LR  # type: ignore
+    R_RL = np.diag(1 / (2 * O_RR)) @ (O_LR.T - conjugate(O_RL)) @ T_RL  # type: ignore
 
     # s-matrix
     S = np.concatenate(
         [
             np.concatenate([R_LR, T_RL], 1),
             np.concatenate([T_LR, R_RL], 1),
         ],
         0,
     )
 
-    # enforce S@S.H is diagonal
-    if enforce_lossy_unitarity:  # HACK!
+    # enforce S@S.H is diagonal: HACK!
+    if enforce_lossy_unitarity:
         U, s, V = np.linalg.svd(S)
         S = np.diag(s) @ U @ V
 
-    # ensure reciprocity:
+    # ensure reciprocity: HACK?
     if enforce_reciprocity:
         S = 0.5 * (S + S.T)
 
     # create port map
     in_ports = [f"left@{i}" for i in range(len(modes1))]
     out_ports = [f"right@{i}" for i in range(len(modes2))]
     port_map = {p: i for i, p in enumerate(in_ports + out_ports)}
```

### Comparing `meow-sim-0.4.3/meow/eme/sax.py` & `meow-sim-0.5.0/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/environment.py` & `meow-sim-0.5.0/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/fde/lumerical.py` & `meow-sim-0.5.0/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/fde/tidy3d.py` & `meow-sim-0.5.0/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/gds_structures.py` & `meow-sim-0.5.0/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/geometries.py` & `meow-sim-0.5.0/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/integrate.py` & `meow-sim-0.5.0/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/materials.py` & `meow-sim-0.5.0/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/mesh.py` & `meow-sim-0.5.0/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/mode.py` & `meow-sim-0.5.0/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/structures.py` & `meow-sim-0.5.0/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/meow/visualize.py` & `meow-sim-0.5.0/meow/visualize.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from jaxlib.xla_extension import DeviceArray  # fmt: skip # type: ignore
 except ImportError:
     DeviceArray = None
 
 
-def _visualize_s_matrix(S, fmt=".3f", title=None, show=True):
+def _visualize_s_matrix(S, fmt=".3f", title=None, show=True, phase=False):
     import matplotlib.pyplot as plt  # fmt: skip
 
     Z = np.abs(S)
     y, x = np.arange(Z.shape[0])[::-1], np.arange(Z.shape[1])
     Y, X = np.meshgrid(y, x)
 
     plt.figure(figsize=(2 * x.shape[0] / 3, 2 * y.shape[0] / 3))
@@ -45,18 +45,24 @@
     )
     coords_ = coords_[::-1]  # reverse
     labels = ["" for _ in coords_]
     plt.yticks(coords_ + 0.5, labels)
     plt.ylim(coords_[-1] - 0.5, coords_[0] + 0.5)
     plt.grid(True)
 
-    for x, y, z in zip(X.ravel(), Y.ravel(), Z[::-1].T.ravel()):
-        if z > 0.0005:
+    for x, y, z in zip(X.ravel(), Y.ravel(), S[::-1].T.ravel()):
+        if np.abs(z) > 0.0005:
+            if phase:
+                z = np.angle(z) * 180 / np.pi
             text = eval(f"f'{{z:{fmt}}}'")  # 😅
-            plt.text(x, y, text, ha="center", va="center")
+            text = text.replace("+", "\n+")
+            text = text.replace("-", "\n-")
+            if text[0] == "\n":
+                text = text[1:]
+            plt.text(x, y, text, ha="center", va="center", fontsize=8)
 
     if title is not None:
         plt.title(title)
 
     if show:
         plt.show()
 
@@ -170,27 +176,28 @@
     """
     from .base_model import BaseModel  # fmt: skip
     from .mode import Mode  # fmt: skip
     from .structures import Structure, visualize_structures  # fmt: skip
 
     # if isinstance(obj, Mode):
     #    return _visualize_mode(obj)
+
     if isinstance(obj, list) and all(isinstance(o, Mode) for o in obj):
         return _visualize_modes(obj)
     elif isinstance(obj, BaseModel):
         return obj._visualize(**kwargs)
     elif _is_s_matrix(obj) and plt is not None:
         _visualize_s_matrix(obj, **kwargs)
     elif (
         _is_two_tuple(obj)
         and _is_s_matrix(obj[0])
         and isinstance(obj[1], dict)
         and plt is not None
     ):
-        _visualize_s_pm_matrix(obj, **kwargs)
+        _visualize_s_matrix(obj, **kwargs)
     elif gf is not None and isinstance(obj, gf.Component):
         _visualize_gdsfactory(obj, **kwargs)
     else:
         try:
             (*objs,) = obj  # type: ignore
         except TypeError:
             return obj
```

### Comparing `meow-sim-0.4.3/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.0/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.4.3
+Version: 0.5.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.4.3/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.0/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/pyproject.toml` & `meow-sim-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.4.3"
+version = "0.5.0"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.4.3/tests/test_deserialization.py` & `meow-sim-0.5.0/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/tests/test_mode_operators.py` & `meow-sim-0.5.0/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.4.3/tests/test_nbs.py` & `meow-sim-0.5.0/tests/test_nbs.py`

 * *Files identical despite different names*

