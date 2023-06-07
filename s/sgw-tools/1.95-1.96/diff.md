# Comparing `tmp/sgw_tools-1.95.tar.gz` & `tmp/sgw_tools-1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgw_tools-1.95.tar", last modified: Wed May 31 21:13:47 2023, max compression
+gzip compressed data, was "sgw_tools-1.96.tar", last modified: Wed Jun  7 21:24:51 2023, max compression
```

## Comparing `sgw_tools-1.95.tar` & `sgw_tools-1.96.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-31 21:13:08.000000 sgw_tools-1.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-31 21:13:47.831453 sgw_tools-1.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 21:13:08.000000 sgw_tools-1.95/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:13:47.831453 sgw_tools-1.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 21:13:08.000000 sgw_tools-1.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/sgw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-31 21:13:08.000000 sgw_tools-1.95/sgw_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/sgw_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 21:13:47.000000 sgw_tools-1.95/sgw_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:47.831453 sgw_tools-1.95/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:13:08.000000 sgw_tools-1.95/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-31 21:13:08.000000 sgw_tools-1.95/tests/test_biggraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 21:24:20.000000 sgw_tools-1.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 21:24:51.275636 sgw_tools-1.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 21:24:20.000000 sgw_tools-1.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:24:51.275636 sgw_tools-1.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 21:24:20.000000 sgw_tools-1.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/sgw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/sgw_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:20.000000 sgw_tools-1.96/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-06-07 21:24:20.000000 sgw_tools-1.96/tests/test_biggraph.py
```

### Comparing `sgw_tools-1.95/LICENSE` & `sgw_tools-1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.95/PKG-INFO` & `sgw_tools-1.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw_tools
-Version: 1.95
+Version: 1.96
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.95/setup.py` & `sgw_tools-1.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sgw_tools",
-    version="1.95",
+    version="1.96",
     author="Mark Hale",
     license="MIT",
     description="Spectral graph wavelet tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulquero/sgw",
     packages=find_packages(),
```

### Comparing `sgw_tools-1.95/sgw_tools/__init__.py` & `sgw_tools-1.96/sgw_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import matplotlib.pyplot as plt
 from builtins import staticmethod
 
 from .graph import LGraph
 from .graph import Hypergraph
 from .graph import BigGraph
 from .graph import BipartiteGraph
+from .graphs import RingGraph
 from .graphs import StarGraph
 from .graphs import DirectedPath
 from .graphs import DirectedRing
 from .graphs import RandomRegular
 from .filters import GWHeat
 from .filters import GaussianFilter
 from .filters import ShiftedFilter
```

### Comparing `sgw_tools-1.95/sgw_tools/filters.py` & `sgw_tools-1.96/sgw_tools/filters.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.95/sgw_tools/graph.py` & `sgw_tools-1.96/sgw_tools/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 import pygsp as gsp
 from scipy import sparse
 from scipy.linalg import eigh
 from . import util
 
 
 class LGraphFourier(gsp.graphs.fourier.GraphFourier):
-    def compute_fourier_basis(self, recompute=False, spectrum_only=False):
+    def _has_fourier_basis(self, recompute):
         if hasattr(self, '_e') and self._e is not None and hasattr(self, '_U') and self._U is not None and not recompute:
+            return True
+
+    def compute_fourier_basis(self, recompute=False, spectrum_only=False):
+        if self._has_fourier_basis(recompute):
             return
 
         assert self.L.shape == (self.N, self.N)
         if self.N > 3000:
             self.logger.warning('Computing the full eigendecomposition of a '
                                 'large matrix ({0} x {0}) may take some '
                                 'time.'.format(self.N))
@@ -236,16 +240,17 @@
                 sources, targets, _ = self.get_edge_list()
                 bounds += [np.max(self.dw[sources] + self.dw[targets])]
             # Merris, A note on Laplacian graph eigenvalues.
             if not self.is_directed():
                 W = self.W
             else:
                 W = gsp.utils.symmetrize(self.W, method='average')
-            m = W.dot(self.dw) / self.dw  # Mean degree of adjacent vertices.
-            bounds += [np.max(self.dw + m)]
+            if not np.allclose(self.dw, 0):
+                m = W.dot(self.dw) / self.dw  # Mean degree of adjacent vertices.
+                bounds += [np.max(self.dw + m)]
             # Good review: On upper bounds for Laplacian graph eigenvalues.
             return min(bounds)
         else:
             return np.inf
 
     def has_loops(self):
         return np.any(self.W.diagonal() != 0)
@@ -490,12 +495,12 @@
 
 class BipartiteGraph(BigGraph):
     def __init__(self, W, lap_type='combinatorial', s=1, q=0, coords=None, plotting={}):
         super().__init__(W, lap_type=lap_type, s=s, q=q, coords=coords, plotting=plotting)
         if self.lap_type == 'normalized':
             self._lmax = 2
 
-    def compute_fourier_basis(self, recompute=False):
-        LGraphFourier.compute_fourier_basis(self, recompute)
+    def compute_fourier_basis(self, recompute=False, spectrum_only=False):
+        LGraphFourier.compute_fourier_basis(self, recompute=recompute, spectrum_only=spectrum_only)
         if self.lap_type == 'normalized':
             assert self.e[-1] == 2
```

### Comparing `sgw_tools-1.95/sgw_tools/graphs.py` & `sgw_tools-1.96/sgw_tools/graphs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,64 @@
 import numpy as np
 import pygsp as gsp
 from scipy import sparse
 from .graph import BigGraph
 
-class StarGraph(gsp.graphs.Comet):
+
+class RingGraph(BigGraph):
+    def __init__(self, N, **kwargs):
+        G = gsp.graphs.Ring(N)
+        super().__init__(G.W, coords=G.coords, plotting=G.plotting, **kwargs)
+
+    def compute_fourier_basis(self, recompute=False, spectrum_only=False):
+        if self._has_fourier_basis(recompute):
+            return
+
+        if self.lap_type in ["combinatorial", "normalized", "adjacency"]:
+            N = self.N
+            tmp = [0]
+            for i in np.arange(1, N // 2 + 1):
+                tmp.append(i)
+                tmp.append(i)
+            x = np.array(tmp[:N])
+            if self.lap_type == "combinatorial":
+                self._e = 2 - 2 * np.cos(2 * np.pi * x / N)
+                if not N&1:  # bipartite
+                    self._e[-1] = 4
+            else:
+                # normalized/adjacency (identical for ring graph)
+                self._e = 1 - np.cos(2 * np.pi * x / N)
+                if not N&1:  # bipartite
+                    self._e[-1] = 2
+            self._e[0] = 0
+
+            if not spectrum_only:
+                # eigenvectors are identical for normalized/adjacency and combinatorial Laplacians
+                x_k = np.kron(np.arange(N)[:, np.newaxis], np.arange(N // 2 + 1))
+                U_cos = np.cos(2 * np.pi * x_k / N) / np.sqrt(N / 2)
+                U_sin = np.sin(2 * np.pi * x_k / N) / np.sqrt(N / 2)
+                U = np.empty((N, N))
+                U[:, 0] = U_cos[:, 0] / np.sqrt(2)
+                if N&1:
+                    U[:, 1:-1:2] = U_cos[:, 1:]
+                    U[:, -1] = U_sin[:, -1]
+                else:
+                    U[:, 1:-1:2] = U_cos[:, 1:-1]
+                    U[:, -1] = U_cos[:, -1] / np.sqrt(2)
+                U[:, 2:-1:2] = U_sin[:, 1:-1]
+                U[np.isclose(U, 0)] = 0
+                self._U = U
+        else:
+            super().compute_fourier_basis(recompute=recompute, spectrum_only=spectrum_only)
+
+
+class StarGraph(BigGraph):
     def __init__(self, N, **kwargs):
-        super().__init__(N, N-1, **kwargs)
-        self.n_vertices = self.N
-        self.n_edges = self.Ne
+        G = gsp.graphs.Comet(N, N-1)
+        super().__init__(G.W, coords=G.coords, plotting=G.plotting, **kwargs)
 
 
 class DirectedPath(BigGraph):
     def __init__(self, N, **kwargs):
         sources = np.arange(0, N-1)
         targets = np.arange(1, N)
         weights = np.ones(N-1)
```

### Comparing `sgw_tools-1.95/sgw_tools/util.py` & `sgw_tools-1.96/sgw_tools/util.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.95/sgw_tools.egg-info/PKG-INFO` & `sgw_tools-1.96/sgw_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw-tools
-Version: 1.95
+Version: 1.96
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.95/tests/test_biggraph.py` & `sgw_tools-1.96/tests/test_biggraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import scipy.linalg
 from scipy import sparse
 import networkx as nx
 
 from pygsp import graphs
 from sgw_tools import BigGraph
-from sgw_tools import StarGraph, DirectedPath, RandomRegular
+from sgw_tools import RingGraph, StarGraph, DirectedPath, RandomRegular
 
 
 class TestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls._G = BigGraph.create_from(graphs.Logo())
         cls._G.compute_fourier_basis()
@@ -317,14 +317,15 @@
                 L = graph.D.T.dot(graph.D)
                 np.testing.assert_allclose(L.toarray(), graph.L.toarray())
                 test_incidence_nx(graph)
 
     def test_difference(self):
         for lap_type in ['combinatorial', 'normalized']:
             G = BigGraph.create_from(graphs.Logo(), lap_type=lap_type)
+            G.compute_differential_operator()
             y = G.grad(self._signal)
             self.assertEqual(len(y), G.n_edges)
             z = G.div(y)
             self.assertEqual(len(z), G.n_vertices)
             np.testing.assert_allclose(z, G.L.dot(self._signal))
 
     def test_dirichlet_energy(self, n_vertices=100):
@@ -388,14 +389,43 @@
         test(W.astype(int))
         test(sparse.csr_matrix(W))
         #test(sparse.csr_matrix(W, dtype=np.float32))
         test(sparse.csr_matrix(W, dtype=int))
         test(sparse.csc_matrix(W))
         test(sparse.coo_matrix(W))
 
+    def test_ring_even_combinatorial(self):
+        self._test_ring(20, 'combinatorial')
+
+    def test_ring_odd_combinatorial(self):
+        self._test_ring(19, 'combinatorial')
+
+    def test_ring_even_normalized(self):
+        self._test_ring(20, 'normalized')
+
+    def test_ring_odd_normalized(self):
+        self._test_ring(19, 'normalized')
+
+    def _test_ring(self, n=20, lap_type='combinatorial'):
+        graph = RingGraph(n, lap_type=lap_type)
+        self.assertEqual(graph.n_vertices, n)
+        self.assertEqual(graph.n_edges, n)
+        np.testing.assert_array_equal(graph.d, n * [2])
+        np.testing.assert_allclose(np.linalg.norm(graph.coords[1:], axis=1), 1)
+        graph.compute_fourier_basis()
+        expected_evals = scipy.linalg.eigh(graph.L.toarray(), eigvals_only=True)
+        expected_evals[0] = 0
+        np.testing.assert_allclose(graph.e, expected_evals)
+        # check eigenvectors
+        L = graph.L
+        U = graph.U
+        for i, e in enumerate(graph.e):
+            np.testing.assert_almost_equal(U.T@U, np.eye(n), 10)
+            np.testing.assert_almost_equal(L @ U[:,i], e * U[:,i], 10)
+
     def test_star(self, n=20):
         graph = StarGraph(n)
         self.assertEqual(graph.n_vertices, n)
         self.assertEqual(graph.n_edges, n-1)
         np.testing.assert_array_equal(graph.d, [n-1] + (n-1) * [1])
         np.testing.assert_allclose(np.linalg.norm(graph.coords[1:], axis=1), 1)
```

