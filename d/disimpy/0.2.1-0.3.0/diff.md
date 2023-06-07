# Comparing `tmp/disimpy-0.2.1.tar.gz` & `tmp/disimpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disimpy-0.2.1.tar", last modified: Tue Jan  4 07:59:49 2022, max compression
+gzip compressed data, was "disimpy-0.3.0.tar", last modified: Wed Jun  7 19:36:59 2023, max compression
```

## Comparing `disimpy-0.2.1.tar` & `disimpy-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2022-01-04 07:59:49.285369 disimpy-0.2.1/
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     2261 2022-01-04 07:59:49.285369 disimpy-0.2.1/PKG-INFO
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     2012 2021-12-07 11:55:50.000000 disimpy-0.2.1/README.rst
-drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2022-01-04 07:59:49.277369 disimpy-0.2.1/disimpy/
--rw-rw-r--   0 leevi     (1000) leevi     (1000)      118 2021-12-07 13:43:10.000000 disimpy-0.2.1/disimpy/__init__.py
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     3989 2022-01-04 07:56:07.000000 disimpy-0.2.1/disimpy/gradients.py
--rw-r--r--   0 leevi     (1000) leevi     (1000)    44456 2021-12-07 12:30:28.000000 disimpy-0.2.1/disimpy/simulations.py
--rw-r--r--   0 leevi     (1000) leevi     (1000)    18479 2021-12-07 11:08:17.000000 disimpy-0.2.1/disimpy/substrates.py
-drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2022-01-04 07:59:49.285369 disimpy-0.2.1/disimpy/tests/
--rw-rw-r--   0 leevi     (1000) leevi     (1000)      210 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/__init__.py
--rw-rw-r--   0 leevi     (1000) leevi     (1000)    22834 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/cylinder_mesh_closed.pkl
--rw-rw-r--   0 leevi     (1000) leevi     (1000)    20434 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/cylinder_mesh_open.pkl
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     1728 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/desired_subvoxel_indices.npy
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     3520 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/desired_triangle_indices.npy
--rw-rw-r--   0 leevi     (1000) leevi     (1000)   366274 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/example_mesh.pkl
--rw-r--r--   0 leevi     (1000) leevi     (1000)     6896 2022-01-04 07:55:30.000000 disimpy-0.2.1/disimpy/tests/example_traj.txt
--rw-rw-r--   0 leevi     (1000) leevi     (1000)    52018 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/fibre_mesh.pkl
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/misst_cylinder_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/misst_cylinder_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/misst_sphere_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/misst_sphere_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt
--rw-r--r--   0 leevi     (1000) leevi     (1000)   890928 2021-10-31 14:45:58.000000 disimpy-0.2.1/disimpy/tests/neuron-model.pkl
--rw-r--r--   0 leevi     (1000) leevi     (1000)  1484484 2021-10-30 09:30:56.000000 disimpy-0.2.1/disimpy/tests/neuron-model.stl
--rw-rw-r--   0 leevi     (1000) leevi     (1000)     3200 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/sphere_mesh.pkl
--rw-r--r--   0 leevi     (1000) leevi     (1000)     2396 2021-12-06 15:41:51.000000 disimpy-0.2.1/disimpy/tests/test_gradients.py
--rw-r--r--   0 leevi     (1000) leevi     (1000)    26768 2021-12-07 11:40:42.000000 disimpy-0.2.1/disimpy/tests/test_simulations.py
--rw-r--r--   0 leevi     (1000) leevi     (1000)    13502 2021-12-06 16:12:47.000000 disimpy-0.2.1/disimpy/tests/test_substrates.py
--rw-rw-r--   0 leevi     (1000) leevi     (1000)   686649 2021-10-30 09:21:22.000000 disimpy-0.2.1/disimpy/tests/test_traj.txt
--rw-r--r--   0 leevi     (1000) leevi     (1000)      719 2021-12-06 12:59:30.000000 disimpy-0.2.1/disimpy/tests/test_utils.py
--rw-r--r--   0 leevi     (1000) leevi     (1000)     3219 2021-12-07 12:37:05.000000 disimpy-0.2.1/disimpy/utils.py
-drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2022-01-04 07:59:49.277369 disimpy-0.2.1/disimpy.egg-info/
--rw-r--r--   0 leevi     (1000) leevi     (1000)     2261 2022-01-04 07:59:49.000000 disimpy-0.2.1/disimpy.egg-info/PKG-INFO
--rw-r--r--   0 leevi     (1000) leevi     (1000)     1120 2022-01-04 07:59:49.000000 disimpy-0.2.1/disimpy.egg-info/SOURCES.txt
--rw-r--r--   0 leevi     (1000) leevi     (1000)        1 2022-01-04 07:59:49.000000 disimpy-0.2.1/disimpy.egg-info/dependency_links.txt
--rw-r--r--   0 leevi     (1000) leevi     (1000)       36 2022-01-04 07:59:49.000000 disimpy-0.2.1/disimpy.egg-info/requires.txt
--rw-r--r--   0 leevi     (1000) leevi     (1000)        8 2022-01-04 07:59:49.000000 disimpy-0.2.1/disimpy.egg-info/top_level.txt
--rw-rw-r--   0 leevi     (1000) leevi     (1000)       38 2022-01-04 07:59:49.285369 disimpy-0.2.1/setup.cfg
--rw-r--r--   0 leevi     (1000) leevi     (1000)      609 2022-01-04 07:53:10.000000 disimpy-0.2.1/setup.py
+drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2023-06-07 19:36:59.845324 disimpy-0.3.0/
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     2238 2023-06-07 19:36:59.845324 disimpy-0.3.0/PKG-INFO
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     2009 2023-06-07 16:13:36.000000 disimpy-0.3.0/README.rst
+drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2023-06-07 19:36:59.833324 disimpy-0.3.0/disimpy/
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)      509 2023-06-07 14:40:04.000000 disimpy-0.3.0/disimpy/__init__.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     5227 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/gradients.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    44456 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/simulations.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    18557 2023-06-07 13:57:14.000000 disimpy-0.3.0/disimpy/substrates.py
+drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2023-06-07 19:36:59.845324 disimpy-0.3.0/disimpy/tests/
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)      210 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/__init__.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    22834 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/cylinder_mesh_closed.pkl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    20434 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/cylinder_mesh_open.pkl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     1728 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/desired_subvoxel_indices.npy
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     3520 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/desired_triangle_indices.npy
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)   366274 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/example_mesh.pkl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)   694926 2023-06-07 17:38:39.000000 disimpy-0.3.0/disimpy/tests/example_traj.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    52018 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/fibre_mesh.pkl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/misst_cylinder_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/misst_cylinder_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/misst_sphere_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     1300 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/misst_sphere_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)   890928 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/neuron-model.pkl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)  1484484 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/neuron-model.stl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     3200 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/sphere_mesh.pkl
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     3532 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/test_gradients.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    26768 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/test_simulations.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)    13502 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/test_substrates.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)   686649 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/test_traj.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)      719 2023-06-04 15:34:25.000000 disimpy-0.3.0/disimpy/tests/test_utils.py
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     3056 2023-06-07 14:16:18.000000 disimpy-0.3.0/disimpy/utils.py
+drwxrwxr-x   0 leevi     (1000) leevi     (1000)        0 2023-06-07 19:36:59.833324 disimpy-0.3.0/disimpy.egg-info/
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     2238 2023-06-07 19:36:59.000000 disimpy-0.3.0/disimpy.egg-info/PKG-INFO
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)     1120 2023-06-07 19:36:59.000000 disimpy-0.3.0/disimpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)        1 2023-06-07 19:36:59.000000 disimpy-0.3.0/disimpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)       74 2023-06-07 19:36:59.000000 disimpy-0.3.0/disimpy.egg-info/requires.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)        8 2023-06-07 19:36:59.000000 disimpy-0.3.0/disimpy.egg-info/top_level.txt
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)       38 2023-06-07 19:36:59.845324 disimpy-0.3.0/setup.cfg
+-rw-rw-r--   0 leevi     (1000) leevi     (1000)      694 2023-06-05 21:45:35.000000 disimpy-0.3.0/setup.py
```

### Comparing `disimpy-0.2.1/PKG-INFO` & `disimpy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: disimpy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Massively parallel diffusion MR simulator
 Home-page: https://github.com/kerkelae/disimpy
 Author: Leevi Kerkelä
 Author-email: leevi.kerkela@protonmail.com
 License: MIT
-Platform: UNKNOWN
 
 *******
 Disimpy
 *******
 
 Disimpy is a Python package for generating simulated diffusion-weighted MR
 signals that can be useful in the development and validation of data
 acquisition and analysis methods. The data is generated by Monte Carlo random
-walk simulations that run in massively parallel on Nvidia CUDA-capable GPUs. If
+walk simulations that run massively parallel on Nvidia CUDA-capable GPUs. If
 you use Disimpy in work that leads to a scientific publication, please cite
 [1]_, where the details about signal generation can also be found.
 
 Requirements and installation
 #############################
 
 Follow the `installation instructions
@@ -61,9 +60,7 @@
 References
 ##########
 
 .. [1] Kerkelä et al., (2020). Disimpy: A massively parallel Monte Carlo
        simulator for generating diffusion-weighted MRI data in Python. Journal
        of Open Source Software, 5(52), 2527.
        https://doi.org/10.21105/joss.02527
-
-
```

### Comparing `disimpy-0.2.1/README.rst` & `disimpy-0.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 *******
 Disimpy
 *******
 
 Disimpy is a Python package for generating simulated diffusion-weighted MR
 signals that can be useful in the development and validation of data
 acquisition and analysis methods. The data is generated by Monte Carlo random
-walk simulations that run in massively parallel on Nvidia CUDA-capable GPUs. If
+walk simulations that run massively parallel on Nvidia CUDA-capable GPUs. If
 you use Disimpy in work that leads to a scientific publication, please cite
 [1]_, where the details about signal generation can also be found.
 
 Requirements and installation
 #############################
 
 Follow the `installation instructions
```

### Comparing `disimpy-0.2.1/disimpy/gradients.py` & `disimpy-0.3.0/disimpy/gradients.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Gradient arrays are numpy.ndarray instances with shape (number of measurements,
 number of time points, 3). Gradient array elements are floats representing the
 gradient magnitude in SI units (T/m).
 """
 
 import numpy as np
 
+from . import utils
+
 
 GAMMA = 267.513e6  # Gyromagnetic ratio of the simulated spins
 
 
 def interpolate_gradient(gradient, dt, n_t):
     """Interpolate the gradient array to have `n_t` time points.
 
@@ -133,7 +135,45 @@
     for i, R in enumerate(Rs):
         if not np.isclose(np.linalg.det(R), 1) or not np.all(
             np.isclose(R.T, np.linalg.inv(R))
         ):
             raise ValueError(f"Rs[{i}] ({R}) is not a valid rotation matrix")
         g[i, :, :] = np.matmul(R, gradient[i, :, :].T).T
     return g
+
+
+def pgse(delta, DELTA, n_t, bvals, bvecs):
+    """Generate a pulsed gradient spin echo gradient array.
+
+    Parameters
+    ----------
+    delta: float
+        Diffusion encoding time.
+    DELTA : float
+        Diffusion time.
+    n_t : int
+        The number of time points in the generated gradient array. 
+    bvals : float or numpy.ndarray
+        b-value or an array of b-values.
+    bvecs : numpy.ndarray
+        b-vector or array of b-vectors.
+
+    Returns
+    -------
+    gradient : numpy.ndarray
+        Gradient array.
+    dt : float
+        Duration of a time step in the gradient array.   
+    """
+    gradient = np.zeros((1, int(1e6), 3))
+    T = delta + DELTA
+    dt = T / (gradient.shape[1] - 1)
+    gradient[0, 1 : np.round(delta / dt).astype(int), 0] = 1
+    gradient[0, -np.round(delta / dt).astype(int) : -1, 0] = -1
+    gradient, dt = interpolate_gradient(gradient, dt, n_t)
+    gradient = np.concatenate([gradient for _ in bvals], axis=0)
+    gradient = set_b(gradient, dt, bvals)
+    Rs = np.zeros((len(bvals), 3, 3))
+    for i, bvec in enumerate(bvecs):
+        Rs[i] = utils.vec2vec_rotmat(np.array([1.0, 0.0, 0.0]), bvec)
+    gradient = rotate_gradient(gradient, Rs)
+    return gradient, dt
```

### Comparing `disimpy-0.2.1/disimpy/simulations.py` & `disimpy-0.3.0/disimpy/simulations.py`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/substrates.py` & `disimpy-0.3.0/disimpy/substrates.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,33 +254,33 @@
         periodic=periodic,
         init_pos=init_pos,
         quiet=quiet,
     )
     return substrate
 
 
-@numba.jit()
+@numba.jit(nopython=True)
 def _cross_product(a, b):
     """Compiled function for calculating the cross product between two 1D
     arrays of length 3."""
     c = np.zeros(3)
     c[0] = a[1] * b[2] - a[2] * b[1]
     c[1] = a[2] * b[0] - a[0] * b[2]
     c[2] = a[0] * b[1] - a[1] * b[0]
     return c
 
 
-@numba.jit()
+@numba.jit(nopython=True)
 def _dot_product(a, b):
     """Compiled function for calculating the dot product between two 1D arrays
     of length 3."""
     return a[0] * b[0] + a[1] * b[1] + a[2] * b[2]
 
 
-@numba.jit()
+@numba.jit(nopython=True)
 def _triangle_box_overlap(triangle, box):
     """Check if a triangle overlaps with a box.
 
     Parameters
     ----------
     triangle : numpy.ndarray
         Array with shape (3, 3) where the first dimension corresponds to the
@@ -353,15 +353,15 @@
             for k in range(3):
                 p[k] = _dot_product(a, v[k])
             if np.min(p) > r or np.max(p) < -r:
                 return False
     return True
 
 
-@numba.jit()
+@numba.jit(nopython=True)
 def _interval_sv_overlap(xs, x1, x2):
     """Return the indices of subvoxels that overlap with interval [x1, x2].
 
     Parameters
     ----------
     xs : numpy.ndarray
         Array of subvoxel boundaries.
@@ -404,15 +404,15 @@
     else:
         if ll != len(xs) - 1:
             return ll, ul + 1
         else:
             return ll - 1, ul
 
 
-@numba.jit()
+@numba.jit(nopython=True)
 def _triangle_aabb(triangle):
     """Calculate the axis-aligned bounding box of a triangle and return its
     closest and furthest points to the origin.
 
     Parameters
     ----------
     triangle : numpy.ndarray
@@ -426,15 +426,15 @@
     aabb = np.zeros((2, 3))
     for i in range(3):
         aabb[0, i] = np.min(triangle[:, i])
         aabb[1, i] = np.max(triangle[:, i])
     return aabb
 
 
-@numba.jit()
+@numba.jit(nopython=True)
 def _box_subvoxel_overlap(box, xs, ys, zs):
     """Find the subvoxels which with a box overlaps and return the lowest and
     highest index of the subvoxels along each axis.
 
     Parameters
     ----------
     box : numpy.ndarray
```

### Comparing `disimpy-0.2.1/disimpy/tests/cylinder_mesh_closed.pkl` & `disimpy-0.3.0/disimpy/tests/cylinder_mesh_closed.pkl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/cylinder_mesh_open.pkl` & `disimpy-0.3.0/disimpy/tests/cylinder_mesh_open.pkl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/desired_subvoxel_indices.npy` & `disimpy-0.3.0/disimpy/tests/desired_subvoxel_indices.npy`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/desired_triangle_indices.npy` & `disimpy-0.3.0/disimpy/tests/desired_triangle_indices.npy`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/example_mesh.pkl` & `disimpy-0.3.0/disimpy/tests/example_mesh.pkl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/fibre_mesh.pkl` & `disimpy-0.3.0/disimpy/tests/fibre_mesh.pkl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/misst_cylinder_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt` & `disimpy-0.3.0/disimpy/tests/misst_cylinder_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/misst_cylinder_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt` & `disimpy-0.3.0/disimpy/tests/misst_cylinder_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/misst_sphere_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt` & `disimpy-0.3.0/disimpy/tests/misst_sphere_signal_smalldelta_1ms_bigdelta_40ms_radius_5um.txt`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/misst_sphere_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt` & `disimpy-0.3.0/disimpy/tests/misst_sphere_signal_smalldelta_30ms_bigdelta_40ms_radius_5um.txt`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/neuron-model.pkl` & `disimpy-0.3.0/disimpy/tests/neuron-model.pkl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/neuron-model.stl` & `disimpy-0.3.0/disimpy/tests/neuron-model.stl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/sphere_mesh.pkl` & `disimpy-0.3.0/disimpy/tests/sphere_mesh.pkl`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/test_gradients.py` & `disimpy-0.3.0/disimpy/tests/test_gradients.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains tests of the gradients module."""
 
 import numpy as np
 import numpy.testing as npt
 
-from disimpy import gradients, utils
+from .. import gradients, utils
 
 
 def example_gradient():
     T = 80e-3
     gradient = np.zeros((1, 1000, 3))
     gradient[0, 1:201, 0] = 0.1
     gradient[0, -201:-1, 0] = -0.1
@@ -68,7 +68,42 @@
     Rs = R[np.newaxis, :, :]
     rotated_g = gradients.rotate_gradient(gradient, Rs)
     d = rotated_g[0, 5, :]
     npt.assert_almost_equal(k / np.linalg.norm(k), d / np.linalg.norm(d))
     Rs = np.ones((1, 3, 3))
     npt.assert_raises(ValueError, gradients.rotate_gradient, gradient=gradient, Rs=Rs)
     return
+
+
+def test_pgse():
+    delta = 15e-3
+    DELTA = 50e-3
+    bvals = np.array([1e9, 2e9, 3e9])
+    bvecs = np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]])
+    n_t = int(1e4)
+    gradient, dt = gradients.pgse(delta, DELTA, n_t, bvals, bvecs)
+    npt.assert_equal(gradient.shape, (len(bvals), n_t, 3))
+    npt.assert_equal(np.all(gradient[:, 0, :] == 0), True)
+    npt.assert_equal(np.all(gradient[:, -1, :] == 0), True)
+    npt.assert_almost_equal(np.sum(gradient, axis=1), 0)
+    for i in range(3):
+        npt.assert_almost_equal(
+            np.sum(
+                (np.abs(gradient[i, 0 : int(n_t / 2), :]) > np.finfo(float).resolution)
+            )
+            * dt,
+            delta,
+            5,
+        )
+        npt.assert_almost_equal(
+            np.sum(
+                (np.abs(gradient[i, int(n_t / 2) : :, :]) > np.finfo(float).resolution)
+            )
+            * dt,
+            delta,
+            5,
+        )
+    npt.assert_almost_equal(gradients.calc_b(gradient, dt) / 1e9, bvals / 1e9)
+    npt.assert_almost_equal(
+        gradient[:, 1] / np.linalg.norm(gradient[:, 1], axis=1), bvecs
+    )
+    return
```

### Comparing `disimpy-0.2.1/disimpy/tests/test_simulations.py` & `disimpy-0.3.0/disimpy/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/test_substrates.py` & `disimpy-0.3.0/disimpy/tests/test_substrates.py`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/test_traj.txt` & `disimpy-0.3.0/disimpy/tests/test_traj.txt`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/tests/test_utils.py` & `disimpy-0.3.0/disimpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `disimpy-0.2.1/disimpy/utils.py` & `disimpy-0.3.0/disimpy/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,40 +74,38 @@
     ax.set_zlabel("z")
     ax.ticklabel_format(style="sci", scilimits=(0, 0))
     fig.tight_layout()
     plt.show()
     return
 
 
-def show_mesh(substrate):
+def show_mesh(substrate, seed=123):
     """Visualize a triangular mesh with random triangle colours.
 
     Parameters
     ----------
     substrate : disimpy.substrates._Substrate
         Substrate object containing the triangular mesh.
+    seed : int, optional
+        Seed for pseudorandom number generation.
 
     Returns
     -------
     None
     """
-    np.random.seed(123)
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        # The code below often resulted in a runtime warning so ignore warnings
-        # as a temporary solution
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection="3d")
-        for idx in substrate.faces:
-            tri = Poly3DCollection(substrate.vertices[idx], alpha=0.5)
-            tri.set_facecolor(np.random.random(3))
-            ax.add_collection3d(tri)
-        ax.set_xlim([0, substrate.voxel_size[0]])
-        ax.set_ylim([0, substrate.voxel_size[1]])
-        ax.set_zlim([0, substrate.voxel_size[2]])
-        ax.set_xlabel("x")
-        ax.set_ylabel("y")
-        ax.set_zlabel("z")
-        ax.ticklabel_format(style="sci", scilimits=(0, 0))
-        fig.tight_layout()
-        plt.show()
+    np.random.seed(seed)
+    fig = plt.figure()
+    ax = fig.add_subplot(111, projection="3d")
+    for idx in substrate.faces:
+        tri = Poly3DCollection([substrate.vertices[idx]], alpha=0.5)
+        tri.set_facecolor(np.random.random(3))
+        ax.add_collection3d(tri)
+    ax.set_xlim([0, substrate.voxel_size[0]])
+    ax.set_ylim([0, substrate.voxel_size[1]])
+    ax.set_zlim([0, substrate.voxel_size[2]])
+    ax.set_xlabel("x")
+    ax.set_ylabel("y")
+    ax.set_zlabel("z")
+    ax.ticklabel_format(style="sci", scilimits=(0, 0))
+    fig.tight_layout()
+    plt.show()
     return
```

### Comparing `disimpy-0.2.1/disimpy.egg-info/PKG-INFO` & `disimpy-0.3.0/disimpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: disimpy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Massively parallel diffusion MR simulator
 Home-page: https://github.com/kerkelae/disimpy
 Author: Leevi Kerkelä
 Author-email: leevi.kerkela@protonmail.com
 License: MIT
-Platform: UNKNOWN
 
 *******
 Disimpy
 *******
 
 Disimpy is a Python package for generating simulated diffusion-weighted MR
 signals that can be useful in the development and validation of data
 acquisition and analysis methods. The data is generated by Monte Carlo random
-walk simulations that run in massively parallel on Nvidia CUDA-capable GPUs. If
+walk simulations that run massively parallel on Nvidia CUDA-capable GPUs. If
 you use Disimpy in work that leads to a scientific publication, please cite
 [1]_, where the details about signal generation can also be found.
 
 Requirements and installation
 #############################
 
 Follow the `installation instructions
@@ -61,9 +60,7 @@
 References
 ##########
 
 .. [1] Kerkelä et al., (2020). Disimpy: A massively parallel Monte Carlo
        simulator for generating diffusion-weighted MRI data in Python. Journal
        of Open Source Software, 5(52), 2527.
        https://doi.org/10.21105/joss.02527
-
-
```

### Comparing `disimpy-0.2.1/disimpy.egg-info/SOURCES.txt` & `disimpy-0.3.0/disimpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

