# Comparing `tmp/mdopt-0.3.0.tar.gz` & `tmp/mdopt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdopt-0.3.0.tar", max compression
+gzip compressed data, was "mdopt-0.4.0.tar", max compression
```

## Comparing `mdopt-0.3.0.tar` & `mdopt-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1078 2022-08-29 19:45:43.899044 mdopt-0.3.0/LICENSE.md
--rw-r--r--   0        0        0        0 2022-09-19 15:34:51.979834 mdopt-0.3.0/mdopt/__init__.py
--rw-r--r--   0        0        0        0 2022-09-19 15:34:51.980234 mdopt-0.3.0/mdopt/contractor/__init__.py
--rw-r--r--   0        0        0    10549 2022-10-27 19:28:15.445985 mdopt-0.3.0/mdopt/contractor/contractor.py
--rw-r--r--   0        0        0        0 2022-10-27 18:22:35.622621 mdopt-0.3.0/mdopt/mps/__init__.py
--rw-r--r--   0        0        0    16382 2022-10-27 19:31:42.495831 mdopt-0.3.0/mdopt/mps/canonical.py
--rw-r--r--   0        0        0    13610 2022-10-27 19:32:25.123397 mdopt-0.3.0/mdopt/mps/explicit.py
--rw-r--r--   0        0        0    16055 2022-11-01 16:55:01.417597 mdopt-0.3.0/mdopt/mps/utils.py
--rw-r--r--   0        0        0       23 2022-09-19 15:34:51.983667 mdopt-0.3.0/mdopt/optimiser/__init__.py
--rw-r--r--   0        0        0    13626 2022-10-28 23:06:28.787867 mdopt-0.3.0/mdopt/optimiser/dephasing_dmrg.py
--rw-r--r--   0        0        0    12306 2022-10-28 23:06:28.788492 mdopt-0.3.0/mdopt/optimiser/dmrg.py
--rw-r--r--   0        0        0        0 2022-09-19 15:34:51.985005 mdopt-0.3.0/mdopt/utils/__init__.py
--rw-r--r--   0        0        0    14548 2022-10-27 19:30:38.039481 mdopt-0.3.0/mdopt/utils/utils.py
--rw-r--r--   0        0        0     1121 2022-11-01 17:25:06.616891 mdopt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 mdopt-0.3.0/setup.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 mdopt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-02-07 16:00:32.106100 mdopt-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1434 2023-06-04 04:29:40.989489 mdopt-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-07 16:00:32.119334 mdopt-0.4.0/mdopt/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-07 16:00:32.119407 mdopt-0.4.0/mdopt/contractor/__init__.py
+-rw-r--r--   0        0        0    10640 2023-05-11 01:00:55.742426 mdopt-0.4.0/mdopt/contractor/contractor.py
+-rw-r--r--   0        0        0        0 2023-03-08 10:03:23.369496 mdopt-0.4.0/mdopt/mps/__init__.py
+-rw-r--r--   0        0        0    31245 2023-06-06 20:18:50.091990 mdopt-0.4.0/mdopt/mps/canonical.py
+-rw-r--r--   0        0        0    26381 2023-05-08 12:52:41.868101 mdopt-0.4.0/mdopt/mps/explicit.py
+-rw-r--r--   0        0        0    22933 2023-06-06 03:45:48.064434 mdopt-0.4.0/mdopt/mps/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:00:18.160606 mdopt-0.4.0/mdopt/optimiser/__init__.py
+-rw-r--r--   0        0        0    13767 2023-03-08 10:03:23.370998 mdopt-0.4.0/mdopt/optimiser/dephasing_dmrg.py
+-rw-r--r--   0        0        0    12325 2023-03-21 00:50:18.847156 mdopt-0.4.0/mdopt/optimiser/dmrg.py
+-rw-r--r--   0        0        0     4336 2023-04-17 04:00:18.160933 mdopt-0.4.0/mdopt/optimiser/utils.py
+-rw-r--r--   0        0        0        0 2023-02-07 16:00:32.120222 mdopt-0.4.0/mdopt/utils/__init__.py
+-rw-r--r--   0        0        0    16600 2023-06-06 03:44:55.970289 mdopt-0.4.0/mdopt/utils/utils.py
+-rw-r--r--   0        0        0     1259 2023-06-07 06:03:36.654466 mdopt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 mdopt-0.4.0/setup.py
+-rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 mdopt-0.4.0/PKG-INFO
```

### Comparing `mdopt-0.3.0/LICENSE.md` & `mdopt-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdopt-0.3.0/mdopt/contractor/contractor.py` & `mdopt-0.4.0/mdopt/contractor/contractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
-The ``mdopt.contractor.contractor`` module.
-======================================================
 This module contains the MPS-MPO contractor functions.
 """
 
 from typing import Union, List, Tuple, cast
 import numpy as np
 from opt_einsum import contract
 
 from mdopt.mps.canonical import CanonicalMPS
 from mdopt.mps.explicit import ExplicitMPS
 from mdopt.utils.utils import split_two_site_tensor
 
 
 def apply_one_site_operator(tensor: np.ndarray, operator: np.ndarray) -> np.ndarray:
     """
-    Applies a one-site operator to a canonical MPS as follows::
+    Applies a one-site operator to a MPS as follows::
 
         ----(tensor)---  ->  ---(tensor_updated)---
                |                       |
            (operator)                  |
                |                       |
 
     The operator can be non-unitary, however note
@@ -41,25 +39,24 @@
 
     Raises
     ------
     ValueError
         If the MPS tensor is not three-dimensional.
     ValueError
         If the operator tensor is not two-dimensional.
-
     """
 
     if len(tensor.shape) != 3:
         raise ValueError(
             f"A valid MPS tensor must have 3 legs while the one given has {len(tensor.shape)}."
         )
 
     if len(operator.shape) != 2:
         raise ValueError(
-            "A valid single-site operator must have 2 legs"
+            "A valid one-site operator must have 2 legs"
             f"while the one given has {len(operator.shape)}."
         )
 
     tensor_updated = contract("ijk, jl -> ilk", tensor, operator, optimize=[(0, 1)])
 
     return np.asarray(tensor_updated)
 
@@ -192,17 +189,17 @@
                    [ ]---[ ]---[ ]---...---[ ]
                     |     |     |           |
 
     The contraction proceeds as described in the supplementary notes.
 
     Parameters
     ----------
-    mps : Union[CanonicalMPS, ExplicitMPS]
+    mps : Union[ExplicitMPS, CanonicalMPS]
         The initial MPS.
-    mpo : list[np.ndarray]
+    mpo : List[np.ndarray]
         MPO as a list of tensors, where each tensor is corresponding to
         an operator applied at a certain site.
         The operators should be ordered in correspondence with the sites.
         According to our convention, each operator has legs (vL, vR, pU, pD),
         where v stands for "virtual", p -- for "physical",
         and L, R, U, D stand for "left", "right", "up", "down".
     start_site : int
@@ -211,19 +208,21 @@
         Whether to renormalise the singular values after each contraction
         involving two neigbouring MPS sites.
     chi_max : int
         Maximum bond dimension to keep.
     cut : np.float32
         Cutoff for the singular values.
     inplace : bool
-        Whether to modify the starting MPS or create a new one.
+        Whether to modify the current MPS or create a new one.
+    result_to_explicit : bool
+        Whether to tranform the result to the explicit form.
 
     Returns
     -------
-    mps : CanonicalMPS
+    mps : Union[ExplicitMPS, CanonicalMPS]
         The updated MPS in the canonical form.
 
     Raises
     ------
     ValueError
         If any of the MPO tensors is not four-dimensional.
     ValueError
@@ -234,15 +233,17 @@
 
     if not inplace:
         mps = mps.copy()
     if isinstance(mps, ExplicitMPS):
         mps = mps.mixed_canonical(start_site)
     assert isinstance(mps, CanonicalMPS)
     if mps.orth_centre != start_site:
-        mps = cast(CanonicalMPS, mps.move_orth_centre(start_site))
+        mps = cast(
+            CanonicalMPS, mps.move_orth_centre(start_site, renormalise=renormalise)
+        )
 
     for i, tensor in enumerate(mpo):
         if len(tensor.shape) != 4:
             raise ValueError(
                 f"A valid MPO tensor must have 4 legs while tensor {i} has {len(tensor.shape)}."
             )
 
@@ -268,15 +269,14 @@
             mpo[0].shape[3],
             mpo[1].shape[3],
             mps.tensors[start_site + 1].shape[2] * mpo[1].shape[1],
         )
     )
 
     for i in range(len(mpo) - 2):
-
         mps.tensors[orth_centre_index], singular_values, b_r = split_two_site_tensor(
             two_site_mps_mpo_tensor, chi_max=chi_max, cut=cut, renormalise=renormalise
         )
 
         orth_centre_index += 1
         if isinstance(mps, CanonicalMPS):
             mps.orth_centre = orth_centre_index
@@ -312,10 +312,10 @@
     )
 
     mps.tensors[orth_centre_index + 1] = contract(
         "ij, jkl -> ikl", np.diag(singular_values), b_r, optimize=[(0, 1)]
     )
 
     if result_to_explicit and isinstance(mps, CanonicalMPS):
-        return mps.explicit()
+        return mps.explicit(tolerance=mps.tolerance, renormalise=renormalise)
 
     return mps
```

### Comparing `mdopt-0.3.0/mdopt/mps/explicit.py` & `mdopt-0.4.0/mdopt/optimiser/dephasing_dmrg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,366 +1,385 @@
 """
-This module contains the :class:`ExplicitMPS` class.
-Hereafter by saying the MPS is in an explicit form we mean that
-the state is stored in the following format: for each three-dimensional tensor
-at site `i`, there exists a singular values diagonal matrix at bond ``i``::
-
-            i     i    i+1    i
-    ...---[ ]---( )---[ ]---( )---...
-                    |           |
-                    |           |
-
-For "ghost" bonds at indices ``0``, ``L-1`` (i.e., bonds of dimension 1),
-the corresponding singular value tensors at the boundaries
-would be the identities of the same dimension.
-We index sites with ``i`` from ``0`` to ``L-1``, with bond ``i`` being left of site ``i``.
-Essentially, it corresponds to storing each ``Γ[i]`` and ``Λ[i]`` as shown in
-fig.4b in reference `[1]`_.
+This module contains the :class:`DephasingDMRG` and the :class:`EffectiveDensityOperator` classes.
+
+This algorithm's main feature is that it restricts the target-state search to
+the computational basis states domain.
+In particular, we use it to find the main component of a Matrix Density Product Operator (MDPO),
+i.e., a computational basis state contributing the largest amplitude.
+
+In our notation, MDPO for ``n`` sites denotes the following object::
+
+         |      |               |       |
+         |      |               |       |
+    ----(0*)---(1*)--- ... ---(n-2*)--(n-1*)---
+    ----(0)----(1)---- ... ---(n-2)---(n-1)----
+         |      |               |       |
+         |      |               |       |
+
+An MDPO is formed by an MPS and its complex-conjugated version.
+The main idea is to find the main component of this object without
+performing the kronecker product explicitly.
 """
 
-from functools import reduce
-from copy import deepcopy
-from typing import Iterable, List, cast
+
+from typing import Union, cast
 import numpy as np
+import scipy.sparse
 from opt_einsum import contract
+from scipy.sparse.linalg import eigsh
+from tqdm import tqdm
 
 from mdopt.mps.canonical import CanonicalMPS
-from mdopt.utils.utils import kron_tensors
+from mdopt.mps.explicit import ExplicitMPS
+from mdopt.utils.utils import split_two_site_tensor
 
 
-class ExplicitMPS:
+class EffectiveDensityOperator(scipy.sparse.linalg.LinearOperator):
     """
-    Class for finite-size explicit matrix product states (MPS) with open boundary conditions.
+    Class to store an effective two-site density operator.
 
-    Attributes
-    ----------
-    tensors : list[np.ndarray]
-        The "physical" tensors of the MPS, one for each physical site.
-        Each tensor has legs (virtual left, physical, virtual right), in short ``(vL, i, vR)``.
-    singular_values : list[list]
-        The singular values at each of the bonds, ``singular_values[i]`` is left of ``tensors[i]``.
-        Each singular values list at each bond is normalised to 1.
-    tolerance : np.float32
-        Absolute tolerance of the normalisation of the singular value spectrum at each bond.
-    num_sites : int
-        Number of sites.
-    num_bonds : int
-        Number of non-trivial bonds, which is equal to ``num_sites - 1``.
-
-    Raises
-    ------
-    ValueError
-        If the ``tensors`` and the ``singular_values`` lists do not have corresponding lengths.
-        The number of singular value matrices should be equal to the number of tensors + 1,
-        because there are two trivial singular value matrices at each of the ghost bonds.
-    ValueError
-        If any of the MPS tensors is not three-dimensional.
-    ValueError
-        If any of the singular-values tensors is not normalised within the `tolerance` attribute.
+    To take more advantage of the ``scipy.sparse.linalg`` module, we make a special class
+    for local effective density operators extending the analogy from local effective operators.
+    It allows us to compute eigenvectors more effeciently.
+
+    The diagram displaying the contraction can be found in the supplementary notes.
     """
 
     def __init__(
         self,
-        tensors: List[np.ndarray],
-        singular_values: List[list],
-        tolerance: np.float32 = np.float32(1e-12),
-        chi_max: int = int(1e4),
+        left_environment: np.ndarray,
+        mps_target_1: np.ndarray,
+        mps_target_2: np.ndarray,
+        right_environment: np.ndarray,
     ) -> None:
+        """
+        Initialise an effective dephased density operator tensor network.
 
-        self.tensors = tensors
-        self.num_sites = len(tensors)
-        self.num_bonds = self.num_sites - 1
-        self.bond_dimensions = [self.tensors[i].shape[2] for i in range(self.num_bonds)]
-        self.phys_dimensions = [self.tensors[i].shape[1] for i in range(self.num_sites)]
-        self.singular_values = singular_values
-        self.num_singval_mat = len(singular_values)
-        self.dtype = tensors[0].dtype
-        self.tolerance = tolerance
-        self.chi_max = chi_max
-
-        if self.num_sites != self.num_singval_mat - 1:
+        Parameters
+        ----------
+        left_environment : np.ndarray
+            The left environment for the effective dephased density operator.
+        mps_target_1 : np.ndarray
+            The left target matrix product state tensor.
+        mps_target_2 : np.ndarray
+            The right target matrix product state tensor.
+        right_environment : np.ndarray
+            The right environment for the effective dephased density operator.
+
+        Raises
+        ------
+        ValueError
+            If the left environment tensor is not four-dimensional.
+        ValueError
+            If the first target MPS tensor is not three-dimensional.
+        ValueError
+            If the second target MPS tensor is not three-dimensional.
+        ValueError
+            If the right environment tensor is not four-dimensional.
+        """
+        if len(left_environment.shape) != 4:
             raise ValueError(
-                f"The number of tensors {self.num_sites} should correspond "
-                "to the number of non-trivial singular value matrices "
-                f"{len(tensors) - 1}, instead the number of "
-                f"non-trivial singular value matrices is {self.num_singval_mat - 2}."
-            )
-
-        for i, tensor in enumerate(tensors):
-            if len(tensor.shape) != 3:
-                raise ValueError(
-                    "A valid MPS tensor must have 3 legs"
-                    f"while the one given has {len(tensor.shape)}."
-                )
-
-        for i, _ in enumerate(singular_values):
-            norm = np.linalg.norm(singular_values[i])
-            if abs(norm - 1) > tolerance:
-                raise ValueError(
-                    "The norm of each singular values tensor must be 1, "
-                    f"instead the norm is {norm} at bond {i + 1}."
-                )
-
-    def __len__(self) -> int:
-        """Returns the number of sites in the MPS."""
-        return self.num_sites
-
-    def __iter__(self) -> Iterable:
-        """Returns an iterator over (singular_values, tensors) pair for each site."""
-        return zip(self.singular_values, self.tensors)
-
-    def copy(self) -> "ExplicitMPS":
-        """Returns a copy of the current MPS."""
-        return ExplicitMPS(
-            deepcopy(self.tensors),
-            deepcopy(self.singular_values),
-            self.tolerance,
-            self.chi_max,
-        )
-
-    def reverse(self) -> "ExplicitMPS":
-        """Returns a reversed version of a given MPS."""
-
-        reversed_tensors = list(np.transpose(t) for t in reversed(self.tensors))
-        reversed_singular_values = list(reversed(self.singular_values))
-
-        return ExplicitMPS(
-            reversed_tensors, reversed_singular_values, self.tolerance, self.chi_max
-        )
-
-    def conjugate(self) -> "ExplicitMPS":
-        """Returns a complex-conjugated version of the current MPS."""
-
-        conjugated_tensors = [np.conjugate(tensor) for tensor in self.tensors]
-        conjugated_sing_vals = [
-            [np.conjugate(sigma) for sigma in sing_vals]
-            for sing_vals in self.singular_values
-        ]
-        conjugated_sing_vals = cast(List[list], conjugated_sing_vals)
-        return ExplicitMPS(
-            conjugated_tensors,
-            conjugated_sing_vals,
-            self.tolerance,
-            self.chi_max,
-        )
-
-    def single_site_left_iso(self, site: int) -> np.ndarray:
-        """Computes a single-site left isometry at a given site."""
-
-        if site not in range(self.num_sites):
+                "A valid left environment tensor must have 4 legs"
+                f"while the one given has {len(left_environment.shape)}."
+            )
+        if len(mps_target_1.shape) != 3:
             raise ValueError(
-                f"Site given {site}, with the number of sites in the MPS {self.num_sites}."
+                "A valid target MPS tensor must have 3 legs"
+                f"while the one given has {len(mps_target_1.shape)}."
             )
-
-        return np.tensordot(
-            np.diag(self.singular_values[site]), self.tensors[site], (1, 0)
-        )
-
-    def single_site_right_iso(self, site: int) -> np.ndarray:
-        """Computes a single-site right isometry at a given site."""
-
-        if site not in range(self.num_sites):
+        if len(mps_target_2.shape) != 3:
             raise ValueError(
-                f"Sites given {site}, {site + 1}, "
-                f"with the number of sites in the MPS {self.num_sites}."
+                "A valid target MPS tensor must have 3 legs"
+                f"while the one given has {len(mps_target_1.shape)}."
+            )
+        if len(right_environment.shape) != 4:
+            raise ValueError(
+                "A valid right environment tensor must have 4 legs"
+                f"while the one given has {len(right_environment.shape)}."
             )
 
-        return np.tensordot(
-            self.tensors[site], np.diag(self.singular_values[site + 1]), (2, 0)
-        )
-
-    def single_site_left_iso_iter(self) -> Iterable:
-        """Returns an iterator over the left isometries for every site."""
-
-        return (self.single_site_left_iso(i) for i in range(self.num_sites))
-
-    def single_site_right_iso_iter(self) -> Iterable:
-        """Returns an iterator over the right isometries for every site."""
-
-        return (self.single_site_right_iso(i) for i in range(self.num_sites))
+        self.left_environment = left_environment
+        self.right_environment = right_environment
+        self.mps_target_1 = mps_target_1
+        self.mps_target_2 = mps_target_2
+        chi_1, chi_2 = (
+            left_environment.shape[3],
+            right_environment.shape[3],
+        )
+        d_1, d_2 = (
+            mps_target_1.shape[1],
+            mps_target_2.shape[1],
+        )
+        self.x_shape = (chi_1, d_1, d_2, chi_2)
+        self.shape = (chi_1 * d_1 * d_2 * chi_2, chi_1 * d_1 * d_2 * chi_2)
+        self.dtype = mps_target_1.dtype
+        super().__init__(shape=self.shape, dtype=self.dtype)
 
-    def two_site_left_iso(self, site: int) -> np.ndarray:
-        """Computes a two-site isometry on a given site and
-        the following one from two single-site left isometries.
+    def _matvec(self, x: np.ndarray) -> np.ndarray:
         """
+        Performs matrix-vector multiplication.
 
-        if site not in range(self.num_sites):
-            raise ValueError(
-                f"Sites given {site}, {site + 1}, "
-                f"with the number of sites in the MPS {self.num_sites}."
-            )
-
-        return np.tensordot(
-            self.single_site_left_iso(site),
-            self.single_site_left_iso(site + 1),
-            (2, 0),
-        )
+        Computes ``effective_density_operator * |x> = |x'>``.
+        This function is used by ``scipy.sparse.linalg.eigsh`` to diagonalise
+        the effective density operator with the Lanczos method, withouth generating the full matrix.
 
-    def two_site_right_iso(self, site: int) -> np.ndarray:
-        """Computes a two-site isometry on a given site and
-        the following one from two single-site right isometries.
+        Parameters
+        ----------
+        x : np.ndarray
+            The two-site tensor to be acted on by an effective density operator.
         """
 
-        if site not in range(self.num_sites):
+        two_site_tensor = np.reshape(x, self.x_shape)
+
+        if len(two_site_tensor.shape) != 4:
             raise ValueError(
-                f"Sites given {site}, {site + 1}, "
-                f"with the number of sites in the MPS {self.num_sites}."
+                f"A valid two-site tensor must have 4 legs"
+                f"while the one given has {len(two_site_tensor.shape)}."
             )
 
-        return np.tensordot(
-            self.single_site_right_iso(site),
-            self.single_site_right_iso(site + 1),
-            (2, 0),
+        copy_tensor = np.fromfunction(
+            lambda i, j, k: np.logical_and(i == j, j == k), (2, 2, 2), dtype=int
         )
 
-    def two_site_right_iso_iter(self) -> Iterable:
-        """Returns an iterator over the two-site right isometries for every site and
-        its right neighbour.
-        """
-        return (self.two_site_right_iso(i) for i in range(self.num_sites))
+        einsum_string = (
+            "ustw, ailu, ifj, jhk, bef, cgh, lom, mpn, eso, gtp, dknw -> abcd"
+        )
+        two_site_tensor = contract(
+            einsum_string,
+            two_site_tensor,
+            self.left_environment,
+            np.conjugate(self.mps_target_1),
+            np.conjugate(self.mps_target_2),
+            copy_tensor,
+            copy_tensor,
+            self.mps_target_1,
+            self.mps_target_2,
+            copy_tensor,
+            copy_tensor,
+            self.right_environment,
+            optimize=[
+                (0, 8),
+                (0, 1),
+                (0, 6),
+                (0, 5),
+                (1, 2),
+                (2, 3),
+                (3, 4),
+                (2, 3),
+                (1, 2),
+                (0, 1),
+            ],
+            use_blas=True,
+        )
 
-    def two_site_left_iso_iter(self) -> Iterable:
-        """Returns an iterator over the two-site left isometries for every site and
-        its right neighbour.
-        """
-        return (self.two_site_left_iso(i) for i in range(self.num_sites))
+        return np.reshape(two_site_tensor, self.shape[0])
 
-    def dense(self, flatten: bool = True) -> np.ndarray:
-        """Returns dense representation of the MPS.
 
-        Warning: will cause memory overload for number of sites > ~20!
-        """
+class DephasingDMRG:
+    """
+    Class holding the Dephasing Density Matrix Renormalisation Group algorithm with two-site updates
+    for a finite-size system with open-boundary conditions.
 
-        tensors = list(self.single_site_right_iso_iter())
-        dense = reduce(lambda a, b: np.tensordot(a, b, (-1, 0)), tensors)
+    Attributes
+    ----------
+    mps : Union[ExplicitMPS, CanonicalMPS]
+        MPS serving as a current approximation of the target state.
+    mps_target : Union[ExplicitMPS, CanonicalMPS]
+        The target MPS in the right-canonical form.
+        This MPS is used to construct the dephased MDPO.
+    chi_max : int
+        The highest bond dimension of an MPS allowed.
+    mode : str
+        The eigensolver mode. Available options:
+            | ``LM`` : Largest (in magnitude) eigenvalues.
+            | ``SM`` : Smallest (in magnitude) eigenvalues.
+            | ``LA`` : Largest (algebraic) eigenvalues.
+            | ``SA`` : Smallest (algebraic) eigenvalues.
+    cut : np.float32
+        The lower boundary of the spectrum, i.e., all
+        the singular values smaller than that will be discarded.
+    silent : bool
+        Whether to show/hide the progress bar.
+    """
 
-        if flatten:
-            return dense.flatten()
+    def __init__(
+        self,
+        mps: Union[ExplicitMPS, CanonicalMPS],
+        mps_target: Union[ExplicitMPS, CanonicalMPS],
+        chi_max: int = int(1e4),
+        cut: np.float32 = np.float32(1e-12),
+        mode: str = "SA",
+        silent: bool = False,
+        copy: bool = True,
+    ) -> None:
+        """
+        Raises
+        ------
+        ValueError
+            If the current MPS and the target MPS do not have the same lengths.
+        """
+        if len(mps) != len(mps_target):
+            raise ValueError(
+                f"The MPS has length {len(mps)},"
+                f"the target MPS has length {len(mps_target)},"
+                "but the lengths should be equal."
+            )
+        if copy:
+            self.mps = mps.copy()
+        if isinstance(self.mps, CanonicalMPS):
+            self.mps = self.mps.right_canonical()
+        self.mps = mps
+        self.left_environments = [np.zeros(shape=(1,), dtype=np.float32)] * len(mps)
+        self.right_environments = [np.zeros(shape=(1,), dtype=np.float32)] * len(mps)
+        mps_target = mps_target.right_canonical()
+        self.mps_target = mps_target
+        self.chi_max = chi_max
+        self.cut = cut
+        self.mode = mode
+        self.silent = silent
+
+        start_bond_dim = self.mps_target.tensors[0].shape[0]
+        chi = mps.tensors[0].shape[0]
+        left_environment = np.zeros(
+            [chi, start_bond_dim, start_bond_dim, chi], dtype=np.float32
+        )
+        right_environment = np.zeros(
+            [chi, start_bond_dim, start_bond_dim, chi], dtype=np.float32
+        )
+        left_environment[:, 0, 0, :] = np.eye(chi, dtype=np.float32)
+        right_environment[:, start_bond_dim - 1, start_bond_dim - 1, :] = np.eye(
+            chi, dtype=np.float32
+        )
+        self.left_environments[0] = left_environment
+        self.right_environments[-1] = right_environment
+        for i in reversed(range(1, len(mps))):
+            self.update_right_environment(i)
 
-        return dense
+    def sweep(self) -> None:
+        """
+        One Dephasing DMRG sweep.
 
-    def density_mpo(self) -> List[np.ndarray]:
+        A method performing one Dephasing DMRG sweep, which consists of
+        two series of ``update_bond`` sweeps which go back and forth.
         """
-        Returns the MPO representation (as a list of tensors)
-        of the density matrix defined by a given MPS.
-        This operation is depicted in the following picture::
 
-                   i          j
-              a    |          |        c           i     j
-            ...---(*)---O*---(*)---O*---...    ab  |     |  cd
-                                        --> ...---[ ]---[ ]---...
-            ...---( )---O----( )---O----...        |     |
-              b    |          |        d           k     l
-                   k          l
+        for i in range(self.mps.num_sites - 1):
+            self.update_bond(i)
 
-        In the cartoon, `{i,j,k,l}` and `{a,b,c,d}` are single indices,
-        while `ab` and `cd` denote multi indices.
-        Here, the ( )'s represent the MPS tensors, the O's ---
-        the singular values tensors, the [ ]'s --- the MPO tensors.
-        The MPS with the physical legs up is complex-conjugated element-wise,
-        this is denoted by the star sign.
-        The empty line between the MPS and its complex-conjugated version
-        stands for the tensor (kronecker) product.
+        for i in reversed(range(self.mps.num_sites - 1)):
+            self.update_bond(i)
 
-        Each tensor in the MPO list has legs (vL, vR, pU, pD),
-        where v stands for "virtual", p -- for "physical",
-        and L, R, U, D stand for "left", "right", "up", "down".
+    def update_bond(self, i: int) -> None:
+        """
+        Updates the bond between sites ``i`` and ``i+1``.
         """
 
-        tensors = list(self.single_site_right_iso_iter())
+        j = i + 1
 
-        mpo = map(
-            lambda t: kron_tensors(
-                t, t, conjugate_second=True, merge_physicals=False
-            ).transpose((0, 3, 2, 1)),
-            tensors,
+        effective_density_operator = EffectiveDensityOperator(
+            self.left_environments[i],
+            self.mps_target.tensors[i],
+            self.mps_target.tensors[j],
+            self.right_environments[j],
         )
 
-        return list(mpo)
-
-    def entanglement_entropy(self) -> np.ndarray:
-        """Returns the entanglement entropy for bipartitions at each of the bonds."""
-
-        def xlogx(arg: float) -> float:
-            if arg == 0.0:
-                return 0.0
-            return arg * np.log(arg)
+        if isinstance(self.mps, ExplicitMPS):
+            initial_guess = self.mps.two_site_right_iso(i).reshape(
+                effective_density_operator.shape[0]
+            )
+        if isinstance(self.mps, CanonicalMPS):
+            self.mps = cast(CanonicalMPS, self.mps.move_orth_centre(i))
+            initial_guess = self.mps.two_site_tensor_next(i).reshape(
+                effective_density_operator.shape[0]
+            )
 
-        entropy = np.zeros(shape=(self.num_bonds,), dtype=np.float32)
+        _, eigenvectors = eigsh(
+            effective_density_operator,
+            k=1,
+            which=self.mode,
+            return_eigenvectors=True,
+            v0=initial_guess,
+            tol=1e-8,
+        )
+        x = eigenvectors[:, 0].reshape(effective_density_operator.x_shape)
+        left_iso_i, singular_values_j, right_iso_j = split_two_site_tensor(
+            x, chi_max=self.chi_max, cut=self.cut, renormalise=True
+        )
+
+        if isinstance(self.mps, CanonicalMPS):
+            self.mps.tensors[i] = np.tensordot(
+                left_iso_i, np.diag(singular_values_j), (1, 0)
+            )
+            self.mps.orth_centre = i
+            self.mps.tensors[j] = right_iso_j
 
-        for bond in range(self.num_bonds):
-            singular_values = self.singular_values[bond].copy()
-            singular_values[singular_values < self.tolerance] = 0
-            singular_values2 = [
-                singular_value**2 for singular_value in singular_values
-            ]
-            entropy[bond] = -1 * np.sum(
-                np.fromiter((xlogx(s) for s in singular_values2), dtype=np.float32)
+        if isinstance(self.mps, ExplicitMPS):
+            self.mps.tensors[i] = np.tensordot(
+                np.linalg.inv(np.diag(self.mps.singular_values[i])), left_iso_i, (1, 0)
+            )
+            self.mps.tensors[j] = np.tensordot(
+                right_iso_j,
+                np.linalg.inv(np.diag(self.mps.singular_values[j + 1])),
+                (2, 0),
             )
-        return entropy
+            self.mps.singular_values[j] = singular_values_j
 
-    def right_canonical(self) -> CanonicalMPS:
-        """Returns the MPS in the right-canonical form given the MPS in the explicit form.
+        self.update_left_environment(i)
+        self.update_right_environment(j)
 
-        (see eq.19 in https://scipost.org/10.21468/SciPostPhysLectNotes.5 for reference),
+    def update_right_environment(self, i: int) -> None:
         """
-
-        return CanonicalMPS(
-            list(self.single_site_right_iso_iter()),
-            orth_centre=None,
-            tolerance=self.tolerance,
-            chi_max=self.chi_max,
-        )
-
-    def left_canonical(self) -> CanonicalMPS:
-        """Returns the MPS in the left-canonical form given the MPS in the explicit form.
-
-        (see eq.19 in https://scipost.org/10.21468/SciPostPhysLectNotes.5 for reference),
+        Compute the ``right_environment`` right of site ``i-1``
+        from the ``right_environment`` right of site ``i``.
         """
 
-        return CanonicalMPS(
-            list(self.single_site_left_iso_iter()),
-            orth_centre=None,
-            tolerance=self.tolerance,
-            chi_max=self.chi_max,
-        )
+        right_environment = self.right_environments[i]
 
-    def mixed_canonical(self, orth_centre: int) -> CanonicalMPS:
-        """Returns the MPS in the mixed-canonical form
-        with the orthogonality centre being located at `orth_centre`.
+        if isinstance(self.mps, ExplicitMPS):
+            right_iso = self.mps.one_site_right_iso(i)
+        if isinstance(self.mps, CanonicalMPS):
+            self.mps = cast(CanonicalMPS, self.mps.move_orth_centre(i - 1))
+            right_iso = self.mps.one_site_tensor(i)
+
+        right_environment = contract(
+            "ijkl, omi, pmj, qnk, rnl -> opqr",
+            right_environment,
+            right_iso,
+            np.conjugate(self.mps_target.tensors[i]),
+            self.mps_target.tensors[i],
+            np.conjugate(right_iso),
+            optimize=[(0, 2), (0, 1), (0, 1), (0, 1)],
+        )
+        self.right_environments[i - 1] = right_environment
 
-        Parameters
-            orth_centre_index: int
-                An integer which can take values `0, 1, ..., num_sites-1`.
-                Denotes the position of the orthogonality centre --
-                the only non-isometry in the new MPS.
+    def update_left_environment(self, i: int) -> None:
+        """
+        Compute the ``left_environment`` left of site ``i+1``
+        from the  ``left_environment`` left of site ``i``.
         """
 
-        if orth_centre not in range(self.num_sites):
-            raise ValueError(
-                f"Orthogonality centre index given {orth_centre}, "
-                f"with the number of sites in the MPS {self.num_sites}."
-            )
-
-        mixed_can_mps = []
-
-        for i in range(orth_centre):
-            mixed_can_mps.append(self.single_site_left_iso(i))
+        left_environment = self.left_environments[i]
 
-        orth_centre_tensor = contract(
-            "ij, jkl, lm -> ikm",
-            np.diag(self.singular_values[orth_centre]),
-            self.tensors[orth_centre],
-            np.diag(self.singular_values[orth_centre + 1]),
-            optimize=[(0, 1), (0, 1)],
+        if isinstance(self.mps, ExplicitMPS):
+            left_iso = self.mps.one_site_left_iso(i)
+        if isinstance(self.mps, CanonicalMPS):
+            self.mps = cast(CanonicalMPS, self.mps.move_orth_centre(i + 1))
+            left_iso = self.mps.one_site_tensor(i)
+
+        left_environment = contract(
+            "ijkl, imo, jmp, knq, lnr -> opqr",
+            left_environment,
+            left_iso,
+            np.conjugate(self.mps_target.tensors[i]),
+            self.mps_target.tensors[i],
+            np.conjugate(left_iso),
+            optimize=[(0, 2), (0, 1), (0, 1), (0, 1)],
         )
-        mixed_can_mps.append(orth_centre_tensor)
+        self.left_environments[i + 1] = left_environment
 
-        for i in range(orth_centre + 1, self.num_sites):
-            mixed_can_mps.append(self.single_site_right_iso(i))
+    def run(self, num_iter: int = 1) -> None:
+        """
+        Run the algorithm, i.e., run the ``sweep`` method for ``num_iter`` number of times.
+        """
 
-        return CanonicalMPS(
-            mixed_can_mps,
-            orth_centre=orth_centre,
-            tolerance=self.tolerance,
-            chi_max=self.chi_max,
-        )
+        for _ in tqdm(range(num_iter), disable=self.silent):
+            self.sweep()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mdopt-0.3.0/mdopt/mps/utils.py` & `mdopt-0.4.0/mdopt/mps/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 The ``mdopt.mps.utils`` module.
 ===========================================
 This module contains various MPS utilities.
 """
 
-from typing import Union, Optional, cast
+from typing import Union, Optional, List, cast
 from functools import reduce
 import numpy as np
 from opt_einsum import contract
 
 from mdopt.utils.utils import svd
 from mdopt.mps.canonical import CanonicalMPS
 from mdopt.mps.explicit import ExplicitMPS
 
 
 def create_state_vector(num_sites: int, phys_dim: int = int(2)) -> np.ndarray:
     """
-    Creates a uniform random complex quantum state in the form of a state vector.
+    Creates a random uniform complex-valued vector of norm 1.
 
     Parameters
     ----------
     num_sites : int
         Number of degrees of freedom.
     phys_dim : int
         Number of dimensions of each degree of freedom.
@@ -29,15 +29,15 @@
     -------
     state_vector : np.ndarray
         The resulting state vector.
     """
 
     state_vector = np.random.uniform(
         size=(phys_dim**num_sites)
-    ) + 1j * np.random.uniform(size=(phys_dim**num_sites))
+    ) + 1j * np.random.uniform(size=phys_dim**num_sites)
     state_vector /= np.linalg.norm(state_vector)
 
     return state_vector
 
 
 def find_orth_centre(
     mps: CanonicalMPS, return_orth_flags: bool = False, tolerance: float = 1e-12
@@ -52,19 +52,19 @@
     return_orth_flags : bool
         Whether to return if each tensor is a right or a left isometry.
     tolerance : float
         Numerical tolerance for checking the isometry property.
 
     Returns
     -------
-    orth_centres : list[int]
+    orth_centres : List[int]
         Indices of sites at which tensors are orthogonality centres.
-    orth_flags_left : Optional[list[bool]]
+    orth_flags_left : Optional[List[bool]]
         Boolean variables for each tensor corresponding to being a left isometry.
-    orth_flags_right : Optional[list[bool]]
+    orth_flags_right : Optional[List[bool]]
         Boolean variables for each tensor corresponding to being a right isometry.
 
     Raises
     ------
     ValueError
         If an :class:`ExplicitMPS` instance is passed as an input.
         They do not have orthogonality centres by definition.
@@ -78,15 +78,14 @@
     num_sites = mps.num_sites
 
     orth_flags_left = []
     orth_flags_right = []
     orth_centres = []
 
     for i, tensor in enumerate(mps.tensors):
-
         to_be_identity_left = np.asarray(
             contract("ijk, ijl -> kl", tensor, np.conjugate(tensor), optimize=[(0, 1)])
         )
         to_be_identity_right = np.asarray(
             contract("ijk, ljk -> il", tensor, np.conjugate(tensor), optimize=[(0, 1)])
         )
 
@@ -154,15 +153,14 @@
         raise ValueError(
             "Orthogonality centre is undefined for an Explicit MPS instance."
         )
 
     flags_left = []
     flags_right = []
     for _, tensor in enumerate(mps.tensors):
-
         to_be_identity_left = np.asarray(
             contract("ijk, ijl -> kl", tensor, np.conjugate(tensor), optimize=[(0, 1)])
         )
         to_be_identity_right = np.asarray(
             contract("ijk, ljk -> il", tensor, np.conjugate(tensor), optimize=[(0, 1)])
         )
 
@@ -186,24 +184,24 @@
     orth_centres = find_orth_centre(mps)
     if_canonical = len(orth_centres) == 1
 
     return if_canonical
 
 
 def inner_product(
-    mps_1: Union[CanonicalMPS, ExplicitMPS], mps_2: Union[CanonicalMPS, ExplicitMPS]
+    mps_1: Union[ExplicitMPS, CanonicalMPS], mps_2: Union[ExplicitMPS, CanonicalMPS]
 ) -> Union[np.float32, np.complex128]:
     """
     Returns an inner product between 2 Matrix Product States.
 
     Parameters
     ----------
-    mps_1 : Union[CanonicalMPS, ExplicitMPS]
+    mps_1 : Union[ExplicitMPS, CanonicalMPS]
         The first MPS in the inner product.
-    mps_1 : Union[CanonicalMPS, ExplicitMPS]
+    mps_1 : Union[ExplicitMPS, CanonicalMPS]
         The second MPS in the inner product.
 
     Returns
     -------
     product : Union[np.float32, np.complex128]
         The value of the inner product.
 
@@ -228,40 +226,42 @@
         mps_1 = mps_1.right_canonical()
     if isinstance(mps_2, ExplicitMPS):
         mps_2 = mps_2.right_canonical()
 
     tensors = []
 
     for i in range(num_sites):
-
         dims_1 = mps_1.tensors[i].shape
         dims_2 = mps_2.tensors[i].shape
 
         tensors.append(
             contract(
                 "ijk, ljm -> ilkm",
                 mps_1.tensors[i],
                 mps_2.tensors[i],
                 optimize=[(0, 1)],
             ).reshape((dims_1[0] * dims_2[0], dims_1[2] * dims_2[2]))
         )
 
-    product = reduce(lambda a, b: np.tensordot(a, b, (-1, 0)), tensors)
+    product = reduce(lambda a, b: np.tensordot(a, b, (-1, 0)), tensors)[0][0]
+
+    if np.isclose(np.imag(product), 0):
+        return np.float32(np.real(product))
 
-    return product[0][0]
+    return np.complex128(product)
 
 
 def mps_from_dense(
     state_vector: np.ndarray,
     phys_dim: int = int(2),
     chi_max: int = int(1e4),
     tolerance: np.float32 = np.float32(1e-12),
     form: str = "Explicit",
     orth_centre: Optional[int] = None,
-) -> Union[CanonicalMPS, ExplicitMPS]:
+) -> Union[ExplicitMPS, CanonicalMPS]:
     """
     Builds an MPS from a dense (state-vector) from.
 
     Parameters
     ----------
     state_vector : np.ndarray
         The initial state vector.
@@ -279,15 +279,15 @@
             | ``Left-canonical`` : The :class:`CanonicalMPS` left-canonical form.
             | ``Mixed-canonical`` : The :class:`CanonicalMPS` mixed-canonical form.
     orth_centre : Optional[int]
         The orthogonal centre position for the mixed-canonical form.
 
     Returns
     -------
-    mps : Union[CanonicalMPS, ExplicitMPS]
+    mps : Union[ExplicitMPS, CanonicalMPS]
         The resulting MPS.
 
     Raises
     ------
     ValueError
         If the vector's length does not correspond to the physical dimension.
     """
@@ -309,15 +309,14 @@
         state_vector, chi_max=chi_max, renormalise=False
     )
 
     tensors.append(np.expand_dims(v_r, -1))
     singular_values.append(singular_values_local)
 
     while state_vector.shape[0] >= phys_dim:
-
         state_vector = np.matmul(state_vector, np.diag(singular_values_local))
 
         bond_dim = state_vector.shape[-1]
         state_vector = state_vector.reshape((-1, phys_dim * bond_dim))
         state_vector, singular_values_local, v_r = svd(
             state_vector, chi_max=chi_max, renormalise=False
         )
@@ -325,15 +324,14 @@
 
         tensors.insert(0, v_r)
         singular_values.insert(0, singular_values_local)
 
     singular_values.append([1.0])
 
     for i, _ in enumerate(tensors):
-
         tensors[i] = np.tensordot(
             tensors[i], np.linalg.inv(np.diag(singular_values[i + 1])), (2, 0)
         )
 
     if form == "Right-canonical":
         return ExplicitMPS(
             tensors, singular_values, tolerance=tolerance, chi_max=chi_max
@@ -352,15 +350,15 @@
 
 
 def create_simple_product_state(
     num_sites: int,
     which: str = "0",
     phys_dim: int = 2,
     form: str = "Explicit",
-) -> Union[CanonicalMPS, ExplicitMPS]:
+) -> Union[ExplicitMPS, CanonicalMPS]:
     r"""
     Creates a simple product-state MPS.
 
     Parameters
     ----------
     num_sites : int
         The number of sites.
@@ -376,15 +374,15 @@
         The form of the MPS. Available options:
             | ``Explicit`` : The :class:`ExplicitMPS` form (by default).
             | ``Right-canonical`` : The :class:`CanonicalMPS` right-canonical form.
             | ``Left-canonical`` : The :class:`CanonicalMPS` left-canonical form.
 
     Returns
     -------
-    mps : Union[CanonicalMPS, ExplicitMPS]
+    mps : Union[ExplicitMPS, CanonicalMPS]
         The resulting MPS.
 
     Raises
     ------
     ValueError
         If the chosen form is mixed-canonical.
         This form is not available for product states.
@@ -418,15 +416,15 @@
         raise ValueError("Mixed-canonical form is not defined for a product state.")
 
     return ExplicitMPS(tensors, singular_values)
 
 
 def create_custom_product_state(
     string: str, phys_dim: int = 2, form: str = "Explicit"
-) -> Union[CanonicalMPS, ExplicitMPS]:
+) -> Union[ExplicitMPS, CanonicalMPS]:
     r"""
     Creates a custom product-state MPS defined by the ``string`` argument.
 
     Parameters
     ----------
     string : str
         The string defining the product-state MPS. Available characters: ``0``, ``1``, ``+``.
@@ -437,15 +435,15 @@
         The form of the MPS. Available options:
             | ``Explicit`` : The :class:`ExplicitMPS` form (by default).
             | ``Right-canonical`` : The :class:`CanonicalMPS` right-canonical form.
             | ``Left-canonical`` : The :class:`CanonicalMPS` left-canonical form.
 
     Returns
     -------
-    mps : Union[CanonicalMPS, ExplicitMPS]
+    mps : Union[ExplicitMPS, CanonicalMPS]
         The resulting MPS.
 
     Raises
     ------
     ValueError
         If a symbol inside the ``string`` argument does not belong to the available set.
     ValueError
@@ -462,15 +460,14 @@
     The state is renormalized at the end.
     """
 
     num_sites = len(string)
     tensors = []
 
     for symbol in string:
-
         tensor = np.zeros((phys_dim,))
         if symbol == "0":
             tensor[0] = 1.0
         elif symbol == "1":
             tensor[-1] = 1.0
         elif symbol == "+":
             for i in range(phys_dim):
@@ -488,7 +485,206 @@
         return ExplicitMPS(tensors, singular_values).right_canonical()
     if form == "Left-canonical":
         return ExplicitMPS(tensors, singular_values).left_canonical()
     if form == "Mixed-canonical":
         raise ValueError("Mixed-canonical form is not defined for a product state.")
 
     return ExplicitMPS(tensors, singular_values)
+
+
+def marginalise(
+    mps: Union[ExplicitMPS, CanonicalMPS],
+    sites_to_marginalise: List[int],
+    canonicalise: bool = False,
+) -> Union[CanonicalMPS, np.float32, np.complex128]:
+    r"""
+    Computes a marginal over a subset of sites of an MPS.
+    This function was created to not act inplace.
+    For the inplace version, take a look into the
+    corresponding methods of available MPS classes.
+
+    Parameters
+    ----------
+    mps : Union[ExplicitMPS, CanonicalMPS]
+        The MPS we operate upon.
+    sites_to_marginalise : List[int]
+        The sites to marginalise over.
+    canonicalise : bool
+        Whether to put the result in the canonical form,
+        i.e., whether to sweep with SVDs over the left bonds.
+
+    Notes
+    -----
+    The algorithm proceeds by starting from the bond possessing the
+    maximum dimension and contracting the marginalised tensors into
+    the tensors left untouched. This subroutine proceeds until the
+    list of sites to marginalise is empty.
+    An example of marginalising is shown in the following diagram::
+
+        ---(0)---(1)---(2)---(3)---    ---(2)---(3)---
+            |     |     |     |     ->     |     |
+            |     |     |     |            |     |
+           (t)   (t)
+
+    Here, the ``(t)`` (trace) tensor is a tensor consisting af all 1's.
+    """
+
+    mps = mps.copy()
+    sites_all = list(range(mps.num_sites))
+
+    if isinstance(mps, ExplicitMPS):
+        mps = mps.right_canonical()
+
+    if sites_to_marginalise == []:
+        return mps
+
+    if sites_to_marginalise == sites_all:
+        plus_state = create_simple_product_state(
+            num_sites=mps.num_sites, which="+", phys_dim=mps.phys_dimensions[0]
+        )
+        return inner_product(mps, plus_state) * np.prod(mps.phys_dimensions)  # type: ignore
+
+    for site in sites_to_marginalise:
+        if site not in sites_all:
+            raise ValueError(
+                "The list of sites to marginalise must be a subset of the list of all sites."
+            )
+
+    # This subroutine will be used to update the list of sites to marginalise on the fly.
+    def _update_sites_routine(site_checked, site):
+        if site_checked < site:
+            return site_checked
+        if site_checked > site:
+            return site_checked - 1
+        return None
+
+    # This subroutine will be used to update the MPS attributes on the fly.
+    def _update_attributes_routine(
+        tensors, num_sites, bond_dims, sites_all, sites_to_marg, site
+    ):
+        del tensors[site]
+        try:
+            del bond_dims[site]
+        except IndexError:
+            pass
+        sites_to_marg = [
+            _update_sites_routine(site_checked, site)
+            for site_checked in sites_to_marg
+            if site_checked != site
+        ]
+        return tensors, num_sites - 1, bond_dims, sites_all[:-1], sites_to_marg
+
+    # Contracting in the "+" tensors.
+    for site in sites_to_marginalise:
+        phys_dim = mps.phys_dimensions[site]
+        trace_tensor = np.ones((phys_dim,)) / np.sqrt(phys_dim)
+        mps.tensors[site] = np.tensordot(mps.tensors[site], trace_tensor, (1, 0))
+
+    bond_dims = mps.bond_dimensions
+
+    while sites_to_marginalise:
+        try:
+            site = int(np.argmax(bond_dims))
+        except ValueError:
+            site = sites_to_marginalise[0]
+
+        # Checking all possible tensor layouts on a given bond.
+        try:
+            if mps.tensors[site].ndim == 2 and mps.tensors[site + 1].ndim == 3:
+                mps.tensors[site + 1] = np.tensordot(
+                    mps.tensors[site], mps.tensors[site + 1], (-1, 0)
+                )
+                (
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                ) = _update_attributes_routine(
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                    site,
+                )
+            elif mps.tensors[site].ndim == 3 and mps.tensors[site + 1].ndim == 2:
+                mps.tensors[site] = np.tensordot(
+                    mps.tensors[site], mps.tensors[site + 1], (-1, 0)
+                )
+                (
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                ) = _update_attributes_routine(
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                    site + 1,
+                )
+            elif mps.tensors[site].ndim == 2 and mps.tensors[site + 1].ndim == 2:
+                mps.tensors[site] = np.tensordot(
+                    mps.tensors[site], mps.tensors[site + 1], (-1, 0)
+                )
+                (
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                ) = _update_attributes_routine(
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                    site + 1,
+                )
+        except IndexError:
+            if mps.tensors[site].ndim == 2 and mps.tensors[site - 1].ndim == 3:
+                mps.tensors[site - 1] = np.tensordot(
+                    mps.tensors[site - 1], mps.tensors[site], (-1, 0)
+                )
+                (
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                ) = _update_attributes_routine(
+                    mps.tensors,
+                    mps.num_sites,
+                    bond_dims,
+                    sites_all,
+                    sites_to_marginalise,
+                    site,
+                )
+        else:
+            try:
+                del bond_dims[site]
+            except IndexError:
+                pass
+
+    if canonicalise:
+        return cast(
+            CanonicalMPS,
+            CanonicalMPS(
+                tensors=mps.tensors,
+                orth_centre=mps.num_sites - 1,
+                tolerance=mps.tolerance,
+                chi_max=mps.chi_max,
+            ).move_orth_centre(0, renormalise=False),
+        )
+
+    return cast(
+        CanonicalMPS,
+        CanonicalMPS(
+            tensors=mps.tensors,
+            orth_centre=mps.num_sites - 1,
+            tolerance=mps.tolerance,
+            chi_max=mps.chi_max,
+        ),
+    )
```

### Comparing `mdopt-0.3.0/mdopt/optimiser/dephasing_dmrg.py` & `mdopt-0.4.0/mdopt/optimiser/dmrg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,262 +1,229 @@
 """
-This module contains the :class:`DephasingDMRG` and the :class:`EffectiveDensityOperator` classes.
-
-This algorithm's main feature is that it restricts the target-state search to
-the computational basis states domain.
-In particular, we use it to find the main component of a Matrix Density Product Operator (MDPO),
-i.e., a computational basis state contributing the largest amplitude.
-
-In our notation, MDPO for ``n`` sites denotes the following object::
-
-         |      |               |       |
-         |      |               |       |
-    ----(0*)---(1*)--- ... ---(n-2*)--(n-1*)---
-    ----(0)----(1)---- ... ---(n-2)---(n-1)----
-         |      |               |       |
-         |      |               |       |
-
-An MDPO is formed by an MPS and its complex-conjugated version.
-The main idea is to find the main component of this object without
-performing the kronecker product explicitly.
+This module contains the :class:`DMRG` and the :class:`EffectiveOperator` classes.
+The class structure is inspired by TenPy.
 """
 
-
-from typing import Union, cast
+from typing import Union, List, cast
 import numpy as np
 import scipy.sparse
 from opt_einsum import contract
 from scipy.sparse.linalg import eigsh
 from tqdm import tqdm
 
 from mdopt.mps.canonical import CanonicalMPS
 from mdopt.mps.explicit import ExplicitMPS
 from mdopt.utils.utils import split_two_site_tensor
 
 
-class EffectiveDensityOperator(scipy.sparse.linalg.LinearOperator):
-    """
-    Class to store an effective two-site density operator.
+class EffectiveOperator(scipy.sparse.linalg.LinearOperator):
+    r"""Class to store an effective two-site operator.
 
-    To take more advantage of the ``scipy.sparse.linalg`` module, we make a special class
-    for local effective density operators extending the analogy from local effective operators.
+    In order to take more advantage of the ``scipy.sparse.linalg`` module,
+    we make a special class for local effective operators.
     It allows us to compute eigenvectors more effeciently.
 
-    The diagram displaying the contraction can be found in the supplementary notes.
+    Such effective operator is to be diagonalised in the
+    ``update_bond`` method of the :class:`DMRG` class::
+
+        ---uL                    uR---
+        |        i          j        |
+        |  vL    |          |    vR  |
+        (L)----(mpo_l)----(mpo_r)----(R)
+        |        |          |        |
+        |        k          l        |
+        ---dL                    dR---
+
+    In our convention, the legs of left/right environments (tensors ``L``/``R`` in the cartoon)
+    are ordered as follows: ``(uL/uR, vL/vR, dL/dR)`` which means "(up, virtual, down)".
     """
 
     def __init__(
         self,
         left_environment: np.ndarray,
-        mps_target_1: np.ndarray,
-        mps_target_2: np.ndarray,
+        mpo_tensor_left: np.ndarray,
+        mpo_tensor_right: np.ndarray,
         right_environment: np.ndarray,
     ) -> None:
         """
-        Initialise an effective dephased density operator tensor network.
+        Initialises an effective operator tensor network.
 
         Parameters
         ----------
         left_environment : np.ndarray
-            The left environment for the effective dephased density operator.
-        mps_target_1 : np.ndarray
-            The left target matrix product state tensor.
-        mps_target_2 : np.ndarray
-            The right target matrix product state tensor.
+            The left environment for the effective operator.
+        mpo_tensor_left : np.ndarray
+            The left MPO tensor.
+        mpo_tensor_right : np.ndarray
+            The right MPO tensor.
         right_environment : np.ndarray
-            The right environment for the effective dephased density operator.
-
-        Raises
-        ------
-        ValueError
-            If the left environment tensor is not four-dimensional.
-        ValueError
-            If the first target MPS tensor is not three-dimensional.
-        ValueError
-            If the second target MPS tensor is not three-dimensional.
-        ValueError
-            If the right environment tensor is not four-dimensional.
+            The right environment for the effective operator.
         """
-        if len(left_environment.shape) != 4:
+
+        if len(left_environment.shape) != 3:
             raise ValueError(
-                "A valid left environment tensor must have 4 legs"
+                "A valid left environment tensor must have 3 legs"
                 f"while the one given has {len(left_environment.shape)}."
             )
-        if len(mps_target_1.shape) != 3:
+        if len(mpo_tensor_left.shape) != 4:
             raise ValueError(
-                "A valid target MPS tensor must have 3 legs"
-                f"while the one given has {len(mps_target_1.shape)}."
+                "A valid mpo left tensor must have 4 legs"
+                f"while the one given has {len(mpo_tensor_left.shape)}."
             )
-        if len(mps_target_2.shape) != 3:
+        if len(mpo_tensor_right.shape) != 4:
             raise ValueError(
-                "A valid target MPS tensor must have 3 legs"
-                f"while the one given has {len(mps_target_1.shape)}."
+                "A valid mpo right tensor must have 4 legs"
+                f"while the one given has {len(mpo_tensor_right.shape)}."
             )
-        if len(right_environment.shape) != 4:
+        if len(right_environment.shape) != 3:
             raise ValueError(
-                "A valid right environment tensor must have 4 legs"
+                "A valid right environment tensor must have 3 legs"
                 f"while the one given has {len(right_environment.shape)}."
             )
 
         self.left_environment = left_environment
         self.right_environment = right_environment
-        self.mps_target_1 = mps_target_1
-        self.mps_target_2 = mps_target_2
+        self.mpo_tensor_left = mpo_tensor_left
+        self.mpo_tensor_right = mpo_tensor_right
         chi_1, chi_2 = (
-            left_environment.shape[3],
-            right_environment.shape[3],
+            left_environment.shape[2],
+            right_environment.shape[2],
         )
         d_1, d_2 = (
-            mps_target_1.shape[1],
-            mps_target_2.shape[1],
+            mpo_tensor_left.shape[3],
+            mpo_tensor_right.shape[3],
         )
         self.x_shape = (chi_1, d_1, d_2, chi_2)
         self.shape = (chi_1 * d_1 * d_2 * chi_2, chi_1 * d_1 * d_2 * chi_2)
-        self.dtype = mps_target_1.dtype
+        self.dtype = mpo_tensor_left.dtype
         super().__init__(shape=self.shape, dtype=self.dtype)
 
     def _matvec(self, x: np.ndarray) -> np.ndarray:
         """
         Performs matrix-vector multiplication.
 
-        Computes ``effective_density_operator * |x> = |x'>``.
-        This function is used by ``scipy.sparse.linalg.eigsh`` to diagonalise
-        the effective density operator with the Lanczos method, withouth generating the full matrix.
+        Computes ``effective_operator * |x> = |x'>``.
+        This function is being used by ``scipy.sparse.linalg.eigsh`` to diagonalise
+        the effective operator with the Lanczos method, without generating the full matrix.
 
         Parameters
         ----------
         x : np.ndarray
-            The two-site tensor to be acted on by an effective density operator.
+            The two-site tensor on which acts an effective operator.
         """
 
         two_site_tensor = np.reshape(x, self.x_shape)
 
         if len(two_site_tensor.shape) != 4:
             raise ValueError(
                 f"A valid two-site tensor must have 4 legs"
                 f"while the one given has {len(two_site_tensor.shape)}."
             )
 
-        copy_tensor = np.fromfunction(
-            lambda i, j, k: np.logical_and(i == j, j == k), (2, 2, 2), dtype=int
-        )
-
-        einsum_string = (
-            "ustw, ailu, ifj, jhk, bef, cgh, lom, mpn, eso, gtp, dknw -> abcd"
-        )
+        einsum_string = "ijkl, mni, nopj, oqrk, sql -> mprs"
         two_site_tensor = contract(
             einsum_string,
             two_site_tensor,
             self.left_environment,
-            np.conjugate(self.mps_target_1),
-            np.conjugate(self.mps_target_2),
-            copy_tensor,
-            copy_tensor,
-            self.mps_target_1,
-            self.mps_target_2,
-            copy_tensor,
-            copy_tensor,
+            self.mpo_tensor_left,
+            self.mpo_tensor_right,
             self.right_environment,
-            optimize=[
-                (0, 8),
-                (0, 1),
-                (0, 6),
-                (0, 5),
-                (1, 2),
-                (2, 3),
-                (3, 4),
-                (2, 3),
-                (1, 2),
-                (0, 1),
-            ],
+            optimize=[(0, 1), (0, 3), (0, 2), (0, 1)],
             use_blas=True,
         )
 
         return np.reshape(two_site_tensor, self.shape[0])
 
 
-class DephasingDMRG:
+class DMRG:
     """
-    Class holding the Dephasing Density Matrix Renormalisation Group algorithm with two-site updates
+    Class storing the DMRG methods.
+
+    Class holding the Density Matrix Renormalisation Group algorithm with two-site updates
     for a finite-size system with open-boundary conditions.
 
     Attributes
     ----------
     mps : Union[ExplicitMPS, CanonicalMPS]
         MPS serving as a current approximation of the target state.
-    mps_target : Union[ExplicitMPS, CanonicalMPS]
-        The target MPS in the right-canonical form.
-        This MPS is used to construct the dephased MDPO.
+    mpo : List[np.ndarray]
+        The MPO of which the target state is to be computed.
+        Each tensor in the MPO list has legs ``(vL, vR, pU, pD)``,
+        where ``v`` stands for "virtual", ``p`` -- for "physical",
+        and ``L``, ``R``, ``U``, ``D`` -- for "left", "right", "up", "down" accordingly.
     chi_max : int
         The highest bond dimension of an MPS allowed.
+    cut : np.float32
+        The lower boundary of the spectrum, i.e., all the
+        singular values smaller than that will be discarded.
     mode : str
         The eigensolver mode. Available options:
             | ``LM`` : Largest (in magnitude) eigenvalues.
             | ``SM`` : Smallest (in magnitude) eigenvalues.
             | ``LA`` : Largest (algebraic) eigenvalues.
             | ``SA`` : Smallest (algebraic) eigenvalues.
-    cut : np.float32
-        The lower boundary of the spectrum, i.e., all
-        the singular values smaller than that will be discarded.
     silent : bool
         Whether to show/hide the progress bar.
+    copy : bool
+        Whether to copy the input MPS or modify inplace.
     """
 
     def __init__(
         self,
         mps: Union[ExplicitMPS, CanonicalMPS],
-        mps_target: Union[ExplicitMPS, CanonicalMPS],
+        mpo: List[np.ndarray],
         chi_max: int = int(1e4),
         cut: np.float32 = np.float32(1e-12),
         mode: str = "SA",
         silent: bool = False,
         copy: bool = True,
     ) -> None:
-        if len(mps) != len(mps_target):
+        if len(mps) != len(mpo):
             raise ValueError(
                 f"The MPS has length {len(mps)},"
-                f"the target MPS has length {len(mps_target)},"
+                f"the MPO has length {len(mpo)},"
                 "but the lengths should be equal."
             )
+        for i, tensor in enumerate(mpo):
+            if len(tensor.shape) != 4:
+                raise ValueError(
+                    f"A valid MPO tensor must have 4 legs while tensor {i} has {len(tensor.shape)}."
+                )
+        if mode not in ["SA", "LA", "SM", "LM"]:
+            raise ValueError("Invalid eigensolver mode given.")
+
+        self.mps = mps
         if copy:
             self.mps = mps.copy()
         if isinstance(self.mps, CanonicalMPS):
             self.mps = self.mps.right_canonical()
-        self.mps = mps
         self.left_environments = [np.zeros(shape=(1,), dtype=np.float32)] * len(mps)
         self.right_environments = [np.zeros(shape=(1,), dtype=np.float32)] * len(mps)
-        mps_target = mps_target.right_canonical()
-        self.mps_target = mps_target
+        self.mpo = mpo
         self.chi_max = chi_max
         self.cut = cut
         self.mode = mode
         self.silent = silent
 
-        start_bond_dim = self.mps_target.tensors[0].shape[0]
+        start_bond_dim = self.mpo[0].shape[0]
         chi = mps.tensors[0].shape[0]
-        left_environment = np.zeros(
-            [chi, start_bond_dim, start_bond_dim, chi], dtype=np.float32
-        )
-        right_environment = np.zeros(
-            [chi, start_bond_dim, start_bond_dim, chi], dtype=np.float32
-        )
-        left_environment[:, 0, 0, :] = np.eye(chi, dtype=np.float32)
-        right_environment[:, start_bond_dim - 1, start_bond_dim - 1, :] = np.eye(
-            chi, dtype=np.float32
-        )
+        left_environment = np.zeros([chi, start_bond_dim, chi], dtype=np.float32)
+        right_environment = np.zeros([chi, start_bond_dim, chi], dtype=np.float32)
+        left_environment[:, 0, :] = np.eye(chi, dtype=np.float32)
+        right_environment[:, start_bond_dim - 1, :] = np.eye(chi, dtype=np.float32)
         self.left_environments[0] = left_environment
         self.right_environments[-1] = right_environment
         for i in reversed(range(1, len(mps))):
             self.update_right_environment(i)
 
     def sweep(self) -> None:
         """
-        One Dephasing DMRG sweep.
+        One DMRG sweep.
 
-        A method performing one Dephasing DMRG sweep, which consists of
+        A method performing one DMRG sweep, which consists of
         two series of ``update_bond`` sweeps which go back and forth.
         """
 
         for i in range(self.mps.num_sites - 1):
             self.update_bond(i)
 
         for i in reversed(range(self.mps.num_sites - 1)):
@@ -265,47 +232,47 @@
     def update_bond(self, i: int) -> None:
         """
         Updates the bond between sites ``i`` and ``i+1``.
         """
 
         j = i + 1
 
-        effective_density_operator = EffectiveDensityOperator(
+        effective_hamiltonian = EffectiveOperator(
             self.left_environments[i],
-            self.mps_target.tensors[i],
-            self.mps_target.tensors[j],
+            self.mpo[i],
+            self.mpo[j],
             self.right_environments[j],
         )
 
         if isinstance(self.mps, ExplicitMPS):
             initial_guess = self.mps.two_site_right_iso(i).reshape(
-                effective_density_operator.shape[0]
+                effective_hamiltonian.shape[0]
             )
         if isinstance(self.mps, CanonicalMPS):
             self.mps = cast(CanonicalMPS, self.mps.move_orth_centre(i))
             initial_guess = self.mps.two_site_tensor_next(i).reshape(
-                effective_density_operator.shape[0]
+                effective_hamiltonian.shape[0]
             )
 
         _, eigenvectors = eigsh(
-            effective_density_operator,
+            effective_hamiltonian,
             k=1,
             which=self.mode,
             return_eigenvectors=True,
             v0=initial_guess,
             tol=1e-8,
         )
-        x = eigenvectors[:, 0].reshape(effective_density_operator.x_shape)
+        x = eigenvectors[:, 0].reshape(effective_hamiltonian.x_shape)
         left_iso_i, singular_values_j, right_iso_j = split_two_site_tensor(
             x, chi_max=self.chi_max, cut=self.cut, renormalise=True
         )
 
         if isinstance(self.mps, CanonicalMPS):
             self.mps.tensors[i] = np.tensordot(
-                left_iso_i, np.diag(singular_values_j), (1, 0)
+                left_iso_i, np.diag(singular_values_j), (2, 0)
             )
             self.mps.orth_centre = i
             self.mps.tensors[j] = right_iso_j
 
         if isinstance(self.mps, ExplicitMPS):
             self.mps.tensors[i] = np.tensordot(
                 np.linalg.inv(np.diag(self.mps.singular_values[i])), left_iso_i, (1, 0)
@@ -325,55 +292,53 @@
         Compute the ``right_environment`` right of site ``i-1``
         from the ``right_environment`` right of site ``i``.
         """
 
         right_environment = self.right_environments[i]
 
         if isinstance(self.mps, ExplicitMPS):
-            right_iso = self.mps.single_site_right_iso(i)
+            right_iso = self.mps.one_site_right_iso(i)
         if isinstance(self.mps, CanonicalMPS):
             self.mps = cast(CanonicalMPS, self.mps.move_orth_centre(i - 1))
-            right_iso = self.mps.single_site_tensor(i)
+            right_iso = self.mps.one_site_tensor(i)
 
         right_environment = contract(
-            "ijkl, omi, pmj, qnk, rnl -> opqr",
-            right_environment,
+            "ijk, lnjm, omp, knp -> ilo",
             right_iso,
-            np.conjugate(self.mps_target.tensors[i]),
-            self.mps_target.tensors[i],
+            self.mpo[i],
             np.conjugate(right_iso),
-            optimize=[(0, 2), (0, 1), (0, 1), (0, 1)],
+            right_environment,
+            optimize=[(0, 3), (0, 2), (0, 1)],
         )
         self.right_environments[i - 1] = right_environment
 
     def update_left_environment(self, i: int) -> None:
         """
         Compute the ``left_environment`` left of site ``i+1``
-        from the  ``left_environment`` left of site ``i``.
+        from the ``left_environment`` left of site ``i``.
         """
 
         left_environment = self.left_environments[i]
 
         if isinstance(self.mps, ExplicitMPS):
-            left_iso = self.mps.single_site_left_iso(i)
+            left_iso = self.mps.one_site_left_iso(i)
         if isinstance(self.mps, CanonicalMPS):
             self.mps = cast(CanonicalMPS, self.mps.move_orth_centre(i + 1))
-            left_iso = self.mps.single_site_tensor(i)
+            left_iso = self.mps.one_site_tensor(i)
 
         left_environment = contract(
-            "ijkl, imo, jmp, knq, lnr -> opqr",
-            left_environment,
+            "ijk, lnjm, omp, ilo -> knp",
             left_iso,
-            np.conjugate(self.mps_target.tensors[i]),
-            self.mps_target.tensors[i],
+            self.mpo[i],
             np.conjugate(left_iso),
-            optimize=[(0, 2), (0, 1), (0, 1), (0, 1)],
+            left_environment,
+            optimize=[(0, 3), (0, 2), (0, 1)],
         )
         self.left_environments[i + 1] = left_environment
 
     def run(self, num_iter: int = 1) -> None:
         """
-        Run the algorithm, i.e., run the ``sweep`` method for ``num_iter`` number of times.
+        Run the algorithm, i.e., run the ``sweep`` method for ``num_iter`` number of iterations.
         """
 
         for _ in tqdm(range(num_iter), disable=self.silent):
             self.sweep()
```

### Comparing `mdopt-0.3.0/mdopt/utils/utils.py` & `mdopt-0.4.0/mdopt/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def svd(
     mat: np.ndarray,
     cut: np.float32 = np.float32(1e-12),
     chi_max: int = int(1e4),
     renormalise: bool = False,
 ) -> Tuple[np.ndarray, list, np.ndarray]:
     """
-    Performs the Singular Value Decomposition with different features.
+    Performs Singular Value Decomposition with different features.
 
     Parameters
     ----------
     mat : np.ndarray
         Matrix provided as a tensor with 2 dimensions.
     cut : np.float32
         Singular values smaller than this will be discarded.
@@ -35,15 +35,15 @@
         The singular values, sorted in non-increasing order.
     v_r : np.ndarray
         Unitary matrix having right singular vectors as rows.
 
     Raises
     ------
     ValueError
-        If the `np.ndarray` provided is not two-dimensional.
+        If the ``np.ndarray`` provided is not two-dimensional.
     """
 
     if len(mat.shape) != 2:
         raise ValueError(
             f"A valid matrix must have 2 dimensions while the one given has {len(mat.shape)}."
         )
     try:
@@ -146,64 +146,88 @@
 
 
 def split_two_site_tensor(
     tensor: np.ndarray,
     chi_max: int = int(1e4),
     cut: np.float32 = np.float32(1e-12),
     renormalise: bool = False,
-) -> Tuple[np.ndarray, list, np.ndarray]:
+    strategy: str = "svd",
+) -> Tuple:
     """
-    Split a two-site MPS tensor according to the following diagram::
+    Split a two-site MPS tensor according to the following diagram
+    (in case of the SVD strategy, similarly but without the singular vals for the others)::
 
+                                             m         n
        i ---(tensor)--- l     ->    i ---(A)---diag(S)---(B)--- l
-             |   |                         |               |
-             j   k                         j               k
+             |   |                        |               |
+             j   k                        j               k
 
     Parameters
     ----------
     tensor : np.ndarray
         Two-site tensor ``(i, j, k, l)``.
     chi_max : int
         Maximum number of singular values to keep.
     cut : np.float32
         Discard any singular values smaller than eps.
+    renormalise : bool
+        Whether to renormalise the singular value spectrum after the cut.
+    strategy : str
+        Which strategy to use for the splitting.
+        Available options: ``svd``, ``qr``, ``rq``.
 
     Returns
     -------
     a_l : np.ndarray
         Left isometry ``(i, j, m)``.
     singular_values : np.ndarray
         List of singular values.
     b_r : np.ndarray
-        Right isometry ``(m, k, l)``.
+        Right isometry ``(n, k, l)``.
 
     Raises
     ------
     ValueError
         If the tensor is not four-dimensional.
     """
 
     if len(tensor.shape) != 4:
         raise ValueError(
             "A valid two-site tensor must have 4 legs"
             f"while the one given has {len(tensor.shape)}."
         )
 
-    chi_v_l, d_l, d_r, chi_v_r = tensor.shape
-    tensor = tensor.reshape((chi_v_l * d_l, d_r * chi_v_r))
+    if strategy not in ["svd", "qr", "rq"]:
+        raise ValueError("The strategy must be one of 'svd', 'qr', 'rq'.")
 
-    u_l, singular_values, v_r = svd(
-        tensor, cut=cut, chi_max=chi_max, renormalise=renormalise
-    )
+    chi_v_l, phys_l, phys_r, chi_v_r = tensor.shape
+    tensor = tensor.reshape((chi_v_l * phys_l, phys_r * chi_v_r))
 
-    chi_v_cut = len(singular_values)
-    a_l = u_l.reshape((chi_v_l, d_l, chi_v_cut))
-    b_r = v_r.reshape((chi_v_cut, d_r, chi_v_r))
+    if strategy == "svd":
+        u_l, singular_values, v_r = svd(
+            tensor, cut=cut, chi_max=chi_max, renormalise=renormalise
+        )
+        chi_v_cut = len(singular_values)
+        u_l = u_l.reshape((chi_v_l, phys_l, chi_v_cut))
+        v_r = v_r.reshape((chi_v_cut, phys_r, chi_v_r))
+        return u_l, singular_values, v_r  # pylint: disable=unbalanced-tuple-unpacking
+
+    if strategy == "qr":
+        q_l, r_r = np.linalg.qr(tensor, mode="reduced")
+        q_l = q_l.reshape((chi_v_l, phys_l, -1))
+        r_r = r_r.reshape((-1, phys_r, chi_v_r))
+        return q_l, r_r  # pylint: disable=unbalanced-tuple-unpacking
+
+    if strategy == "rq":
+        r_l, q_r = scipy.linalg.rq(tensor, mode="economic")
+        r_l = r_l.reshape((chi_v_l, phys_l, -1))
+        q_r = q_r.reshape((-1, phys_r, chi_v_r))
+        return r_l, q_r  # pylint: disable=unbalanced-tuple-unpacking
 
-    return a_l, singular_values, b_r
+    return tuple()
 
 
 def create_random_mpo(
     num_sites: int,
     bond_dimensions: List[int],
     phys_dim: int,
     which: str = "uniform",
@@ -212,26 +236,26 @@
     Creates a random complex-valued Matrix Product Operator.
 
     Parameters
     ----------
     num_sites : int
         The number of sites for the MPO.
         This will be equal to the number of tensors.
-    bond_dimensions : list[int]
+    bond_dimensions : List[int]
         A list of bond dimensions.
     phys_dim : int
         Physical dimension of the tensors.
     which : str
         Specifies the distribution from which
         the matrix elements are being taken.
         Options: "uniform", "normal", "randint".
 
     Returns
     -------
-    mpo : list[np.ndarray]
+    mpo : List[np.ndarray]
         The resulting MPO.
 
     Notes
     -----
     The ``bond_dimensions`` argument should be given as a list of right virtual dimensions
     without the last trivial virtual dimension. Thus, the length of the list is ``num_sites - 1``.
 
@@ -277,15 +301,15 @@
     mpo: List[np.ndarray], interlace: bool = False, group: bool = False
 ) -> np.ndarray:
     """
     Creates a matrix from an MPO.
 
     Parameters
     ----------
-    mpo : list[np.ndarray]
+    mpo : List[np.ndarray]
         The MPO to convert to a matrix.
     interlace : bool
         Whether to interlace the matrix' legs or not.
     group : bool
         Whether to group the matrix' legs or not, see the notes.
         Grouping means merging all the up legs into one leg and the same for the down legs.
 
@@ -336,15 +360,14 @@
     matrix = (
         np.tensordot(mpo[0], mpo[1], (1, 0))
         .transpose((0, 3, 1, 2, 4, 5))
         .reshape((-1, mpo[1].shape[1], phys_dim**2, phys_dim**2))
     )
 
     for i in range(num_sites - 2):
-
         matrix = (
             np.tensordot(matrix, mpo[i + 2], (1, 0))
             .transpose((0, 3, 1, 2, 4, 5))
             .reshape(
                 (-1, mpo[i + 2].shape[1], phys_dim ** (i + 3), phys_dim ** (i + 3))
             )
         )
@@ -361,37 +384,41 @@
     return matrix
 
 
 def mpo_from_matrix(
     matrix: np.ndarray,
     num_sites: int,
     interlaced: bool = True,
+    orthogonalise: bool = False,
     phys_dim: int = 2,
     chi_max: int = int(1e4),
 ) -> List[np.ndarray]:
     """
     Creates an MPO from a matrix.
 
     Parameters
     ----------
     matrix : np.ndarray
         The matrix to convert to an MPO.
         Can be given with either physical legs grouped together or merged (see notes).
     num_sites : int
         The number of sites in the MPO.
     interlaced : bool
-        Whether the matrix legs are interlaced or not.
+        Whether the matrix' legs are interlaced or not.
+    orthogonalise: bool
+        Whether to make the MPO tensors isometric
+        with respect to 2 physical legs and one virtual.
     phys_dim : int
         Local dimension of the physical legs.
     chi_max : int
         Maximum bond dimension allowed in the MPO.
 
     Returns
     -------
-    mpo : list[np.ndarray]
+    mpo : List[np.ndarray]
         The resulting Matrix Product Operator.
 
     Raises
     ------
     ValueError
         If the matrix' shape does not correspond to ``phys_dim`` and ``num_sites``.
 
@@ -400,14 +427,21 @@
     If ``interlaced==True``, the matrix' legs are considered to go as
     ``(p0U, p0D, p1U, p1D, ...)``, which means physical legs sticking up and down with site number.
     If ``interlaced==False``, the matrix' legs are considered to go as
     ``(p0D, p1D, ..., p0U, p1U, ...)``, which means listing first all physical legs sticking down
     with the site number, and then all physical legs sticking up.
     This is done to adjust the matrix to the ``@`` numpy-native matrix-vector multiplication.
 
+    If ``orthogonalise==True``, the singular values at each bond are being carried further to the
+    orthogonality centre thus making all the tensors except the latter isometric.
+    The orthogonality centre is then isometric up to a multiplier which would be its norm.
+    If ``orthogonalise==False``, the singular values at each bond are being splitted by taking
+    the square root and distribbuted to both MPO tensors at each bond thus leaving all the tensors
+    nonisometric. There is no orthogonality centre in this case.
+
     An example of a matrix with ungrouped legs on three sites::
 
           p0U p1U p2U
          __|___|___|__
         |            |
         |____________|
            |   |   |
@@ -415,15 +449,14 @@
 
     Each tensor in the ``mpo`` list has legs ``(vL, vR, pU, pD)``, where ``v`` stands for "virtual",
     ``p`` -- for "physical", and ``L, R, U, D`` -- for "left", "right", "up", "down" accordingly.
     """
 
     hilbert_space_dim = phys_dim**num_sites
     phys_dims = [phys_dim] * num_sites * 2
-    mps_dim = phys_dim**2
 
     # Checking the matrix has correct shapes for
     # a given physical dimension and number of sites.
     if (matrix.shape != tuple([hilbert_space_dim] * 2)) and (
         matrix.shape != tuple(phys_dims)
     ):
         raise ValueError(
@@ -441,32 +474,39 @@
     # Dealing with possible interlacing.
     if not interlaced:
         correct_order = list([i + num_sites, i] for i in range(num_sites))
         matrix = matrix.transpose(list(chain.from_iterable(correct_order)))
 
     # Treating the MPO as an MPS with squared physical dimensions.
     mpo = []
+    mps_dim = phys_dim**2
     matrix = matrix.reshape((-1, mps_dim))
     matrix, singular_values, v_r = svd(matrix, chi_max=chi_max, renormalise=False)
-    v_r = np.matmul(np.diag(np.sqrt(singular_values)), v_r)
+    if not orthogonalise:
+        v_r = np.matmul(np.diag(np.sqrt(singular_values)), v_r)
     mpo.append(np.expand_dims(v_r, -1))
     while matrix.shape[0] >= mps_dim:
-        matrix = np.matmul(matrix, np.diag(np.sqrt(singular_values)))
+        if not orthogonalise:
+            singular_values = list(np.sqrt(np.array(singular_values)))
+        matrix = np.matmul(matrix, np.diag(singular_values))
         bond_dim = matrix.shape[-1]
         matrix = matrix.reshape((-1, mps_dim * bond_dim))
         matrix, singular_values, v_r = svd(matrix, chi_max=chi_max, renormalise=False)
-        v_r = np.matmul(np.diag(np.sqrt(singular_values)), v_r)
+        if not orthogonalise:
+            v_r = np.matmul(np.diag(np.sqrt(singular_values)), v_r)
         v_r = v_r.reshape((-1, mps_dim, bond_dim))
         mpo.insert(0, v_r)
 
     # Contracting in the orthogonality centre.
+    if not orthogonalise:
+        singular_values = list(np.sqrt(np.array(singular_values)))
     mpo[0] = contract(
         "ij, jk, klm",
         matrix,
-        np.diag(np.sqrt(singular_values)),
+        np.diag(singular_values),
         mpo[0],
         optimize=[(0, 1), (0, 1)],
     )
 
     # Converting the MPS back to the MPO.
     mpo = [tensor.transpose((0, 2, 1)) for tensor in mpo]
     mpo = [
```

### Comparing `mdopt-0.3.0/pyproject.toml` & `mdopt-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 [tool.poetry]
 name = "mdopt"
-version = "0.3.0"
-description = "Discrete optimization in the tensor-network (specifically, MPS-MPO) language."
+version = "0.4.0"
+description = "Discrete optimisation in the tensor-network (specifically, MPS-MPO) language."
 authors = [
-    "Aleksandr Berezutskii <berezutskii@phystech.edu>",
+    "Aleksandr Berezutskii <berezutskii.aleksandr@gmail.com>",
 ]
 maintainers = [
-    "Aleksandr Berezutskii <berezutskii@phystech.edu>"
+    "Aleksandr Berezutskii <berezutskii.aleksandr@gmail.com>"
 ]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 scipy = "^1.9.2"
-numpy = "^1.20.1"
 opt-einsum = "^3.3.0"
 more-itertools = ">=8.12,<10.0"
-matplotlib = "^3.6.1"
-threadpoolctl = {version="^3.1.0", optional = true}
+threadpoolctl = "^3.1.0"
 tqdm = "^4.64.1"
 qecstruct = "^0.2.9"
+qecsim = "^1.0b9"
+numpy = "1.24.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-pylint = "^2.15.3"
-setuptools = "^65.3.0"
-mypy = "^0.982"
+black = ">=22.3,<24.0"
+pylint = "^2.17.4"
+setuptools = "^67.8.0"
+mypy = "^1.3"
+ipykernel = "^6.23.1"
+notebook = "^6.5.3"
+jupyter = "^1.0.0"
+matplotlib = "^3.7.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-coverage = "^6.4.4"
-pytest-cov = "^3.0.0"
-pytest = "^7.1.3"
+coverage = ">=6.4.4,<8.0.0"
+pytest-cov = ">=3,<5"
+pytest = "^7.3.0"
 py = "^1.11.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^5.2.3"
-sphinx-rtd-theme = "^1.0.0"
+matplotlib = "^3.7.0"
+Sphinx = "^6.2.1"
+sphinx-rtd-theme = "^1.2.1"
 sphinxcontrib-napoleon = "^0.7"
-myst-parser = "^0.18.0"
+myst-parser = "^1.0.0"
+nbsphinx = "^0.9.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

