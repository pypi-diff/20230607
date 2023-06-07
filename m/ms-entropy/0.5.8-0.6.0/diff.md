# Comparing `tmp/ms_entropy-0.5.8.tar.gz` & `tmp/ms_entropy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.5.8.tar", last modified: Sun May 28 06:21:42 2023, max compression
+gzip compressed data, was "ms_entropy-0.6.0.tar", last modified: Wed Jun  7 06:59:45 2023, max compression
```

## Comparing `ms_entropy-0.5.8.tar` & `ms_entropy-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/
--rw-rw-r--   0 yli       (1000) yli       (1000)    11357 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3396 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/__init__.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy/entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    28087 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy/file_io/
--rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/lbm2_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1728 2023-05-28 06:20:51.000000 ms_entropy-0.5.8/ms_entropy/file_io/mgf_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/msp_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     3916 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/mzml_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/shared.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/file_io/spec_file.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/ms_entropy/tools/
--rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/ms_entropy/tools/tools.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-28 06:21:42.394945 ms_entropy-0.5.8/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       85 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-28 06:21:42.000000 ms_entropy-0.5.8/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-05-28 06:20:24.000000 ms_entropy-0.5.8/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-28 06:21:42.398944 ms_entropy-0.5.8/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1682 2023-05-28 06:21:13.000000 ms_entropy-0.5.8/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-06-07 06:59:45.333669 ms_entropy-0.6.0/
+-rw-rw-r--   0 yli       (1000) yli       (1000)    11357 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-06-07 06:59:45.333669 ms_entropy-0.6.0/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3503 2023-06-01 01:18:58.000000 ms_entropy-0.6.0/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-06-07 06:59:45.329669 ms_entropy-0.6.0/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-06-07 06:59:45.329669 ms_entropy-0.6.0/ms_entropy/entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/entropy_search/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    28753 2023-06-07 06:56:23.000000 ms_entropy-0.6.0/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    17592 2023-06-07 06:58:09.000000 ms_entropy-0.6.0/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-06-07 06:59:45.333669 ms_entropy-0.6.0/ms_entropy/file_io/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/file_io/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/file_io/lbm2_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1728 2023-05-28 06:20:51.000000 ms_entropy-0.6.0/ms_entropy/file_io/mgf_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/file_io/msp_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3916 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/file_io/mzml_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/file_io/shared.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/file_io/spec_file.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-06-07 06:59:45.333669 ms_entropy-0.6.0/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/tools/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/tools/fast_spectrum.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/ms_entropy/tools/tools.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-06-07 06:59:45.333669 ms_entropy-0.6.0/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-06-07 06:59:45.000000 ms_entropy-0.6.0/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-06-07 06:59:45.000000 ms_entropy-0.6.0/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-06-07 06:59:45.000000 ms_entropy-0.6.0/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       86 2023-06-07 06:59:45.000000 ms_entropy-0.6.0/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-06-07 06:59:45.000000 ms_entropy-0.6.0/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-05-28 06:20:24.000000 ms_entropy-0.6.0/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-06-07 06:59:45.333669 ms_entropy-0.6.0/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1683 2023-06-07 06:59:13.000000 ms_entropy-0.6.0/setup.py
```

### Comparing `ms_entropy-0.5.8/LICENSE` & `ms_entropy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/README.md` & `ms_entropy-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 We are continuously improving the code, and the latest version of the code can be found under the `ms_entropy` folder.
 
 You can find a brief introduction below, or you can find a more detailed documentation here: [https://flashentropysearch.readthedocs.io](https://flashentropysearch.readthedocs.io/).
 
 ## GUI
 You can find the Graphical user interface (GUI) here: [Entropy Search](https://github.com/YuanyueLi/EntropySearch/releases)
+![Screenshot for GUI 1](./docs/images/GUI_start.png)
+![Screenshot for GUI 2](./docs/images/GUI_result.png)
 
 ## In brief
 
 ### Installation
 
 Python >= 3.8, C compiler and Python development headers are required.
```

### Comparing `ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.6.0/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.6.0/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,17 +99,17 @@
                 similarity = intensity_ab * log2f(intensity_ab) - intensity_a * log2f(intensity_a) - intensity_b * log2f(intensity_b);'''
             )
             entropy_similarity = cp.zeros(self.total_spectra_num, dtype=np.float32)
 
         # Go through all the peaks in the spectrum
         for mz_query, intensity_query in peaks:
             # Determine the mz index range
-            product_mz_idx_min = _find_location_from_array_with_index(
+            product_mz_idx_min = self._find_location_from_array_with_index(
                 mz_query - ms2_tolerance_in_da, library_mz, library_mz_idx_start, 'left', index_number_in_one_da)
-            product_mz_idx_max = _find_location_from_array_with_index(
+            product_mz_idx_max = self._find_location_from_array_with_index(
                 mz_query + ms2_tolerance_in_da, library_mz, library_mz_idx_start, 'right', index_number_in_one_da)
 
             if target == "cpu" and search_type == 0:
                 intensity_library = library_peaks_intensity[product_mz_idx_min: product_mz_idx_max]
                 modified_idx = library_spec_idx[product_mz_idx_min: product_mz_idx_max]
                 entropy_similarity[modified_idx] += self._score_peaks_with_cpu(intensity_query, intensity_library)
             elif target == "cpu" and search_type != 0:
@@ -160,17 +160,17 @@
         peaks = self._preprocess_peaks(peaks)
 
         # Go through all peak in the spectrum and determine the mz index range
         product_peak_match_idx_min = np.zeros(peaks.shape[0], dtype=np.uint64)
         product_peak_match_idx_max = np.zeros(peaks.shape[0], dtype=np.uint64)
         for peak_idx, (mz_query, _) in enumerate(peaks):
             # Determine the mz index range
-            product_mz_idx_min = _find_location_from_array_with_index(
+            product_mz_idx_min = self._find_location_from_array_with_index(
                 mz_query - ms2_tolerance_in_da, all_ions_mz, all_ions_mz_idx_start, 'left', index_number_in_one_da)
-            product_mz_idx_max = _find_location_from_array_with_index(
+            product_mz_idx_max = self._find_location_from_array_with_index(
                 mz_query + ms2_tolerance_in_da, all_ions_mz, all_ions_mz_idx_start, 'right', index_number_in_one_da)
 
             product_peak_match_idx_min[peak_idx] = product_mz_idx_min
             product_peak_match_idx_max[peak_idx] = product_mz_idx_max
 
         if target == "cpu":
             entropy_similarity = np.zeros(self.total_spectra_num, dtype=np.float32)
@@ -187,31 +187,31 @@
 
                 entropy_similarity[modified_idx_product] += modified_value_product
 
                 ###############################################################
                 # Match the neutral loss ions
                 mz_nl = precursor_mz-mz
                 # Determine the mz index range
-                neutral_loss_mz_idx_min = _find_location_from_array_with_index(
+                neutral_loss_mz_idx_min = self._find_location_from_array_with_index(
                     mz_nl - ms2_tolerance_in_da, all_nl_mass, all_nl_mass_idx_start, 'left', index_number_in_one_da)
-                neutral_loss_mz_idx_max = _find_location_from_array_with_index(
+                neutral_loss_mz_idx_max = self._find_location_from_array_with_index(
                     mz_nl + ms2_tolerance_in_da, all_nl_mass, all_nl_mass_idx_start, 'right', index_number_in_one_da)
 
                 # Calculate the entropy similarity for this matched peak
                 modified_idx_nl = all_nl_spec_idx[neutral_loss_mz_idx_min: neutral_loss_mz_idx_max]
                 modified_value_nl = self._score_peaks_with_cpu(intensity, all_nl_intensity[neutral_loss_mz_idx_min: neutral_loss_mz_idx_max])
 
                 # Check if the neutral loss ion is already matched to other query peak as a product ion
                 nl_matched_product_ion_idx = all_ions_idx_for_nl[neutral_loss_mz_idx_min: neutral_loss_mz_idx_max]
                 s1 = np.searchsorted(product_peak_match_idx_min, nl_matched_product_ion_idx, side='right')
                 s2 = np.searchsorted(product_peak_match_idx_max-1, nl_matched_product_ion_idx, side='left')
                 modified_value_nl[s1 > s2] = 0
 
                 # Check if this query peak is already matched to a product ion in the same library spectrum
-                duplicate_idx_in_nl = _intersect1d(modified_idx_product, modified_idx_nl)
+                duplicate_idx_in_nl = self._remove_duplicate_with_cpu(modified_idx_product, modified_idx_nl, self.total_spectra_num)
                 modified_value_nl[duplicate_idx_in_nl] = 0
 
                 entropy_similarity[modified_idx_nl] += modified_value_nl
             return entropy_similarity
 
         elif target == "gpu":
             import cupy as cp
@@ -240,43 +240,78 @@
                 entropy_similarity_modification_list.append((modified_idx_product, modified_value_product.get()))
                 del modified_value_product
 
                 ###############################################################
                 # Match the neutral loss ions
                 mz_nl = precursor_mz-mz
                 # Determine the mz index range
-                neutral_loss_mz_idx_min = _find_location_from_array_with_index(
+                neutral_loss_mz_idx_min = self._find_location_from_array_with_index(
                     mz_nl - ms2_tolerance_in_da, all_nl_mass, all_nl_mass_idx_start, 'left', index_number_in_one_da)
-                neutral_loss_mz_idx_max = _find_location_from_array_with_index(
+                neutral_loss_mz_idx_max = self._find_location_from_array_with_index(
                     mz_nl + ms2_tolerance_in_da, all_nl_mass, all_nl_mass_idx_start, 'right', index_number_in_one_da)
 
                 # Calculate the entropy similarity for this matched peak
                 modified_idx_nl = all_nl_spec_idx[neutral_loss_mz_idx_min: neutral_loss_mz_idx_max]
                 modified_value_nl = self._score_peaks_gpu(entropy_transform, intensity, cp.array(
                     all_nl_intensity[neutral_loss_mz_idx_min: neutral_loss_mz_idx_max]))
 
                 # Check if the neutral loss ion is already matched to other query peak as a product ion
                 nl_matched_product_ion_idx = cp.array(all_ions_idx_for_nl[neutral_loss_mz_idx_min: neutral_loss_mz_idx_max])
                 s1 = cp.searchsorted(product_peak_match_idx_min_gpu, nl_matched_product_ion_idx, side='right')
                 s2 = cp.searchsorted(product_peak_match_idx_max_gpu, nl_matched_product_ion_idx, side='left')
                 modified_value_nl[s1 > s2] = 0
 
                 # Check if this query peak is already matched to a product ion in the same library spectrum
-                duplicate_idx_in_nl = _intersect1d_with_gpu(modified_idx_product, modified_idx_nl)
+                duplicate_idx_in_nl = self._remove_duplicate_with_gpu(modified_idx_product, modified_idx_nl, self.total_spectra_num)
                 modified_value_nl[duplicate_idx_in_nl] = 0
 
                 entropy_similarity_modification_list.append((modified_idx_nl, modified_value_nl.get()))
 
             entropy_similarity = cp.zeros(self.total_spectra_num, dtype=np.float32)
             for modified_idx, modified_value in entropy_similarity_modification_list:
                 entropy_similarity.scatter_add(cp.array(modified_idx), cp.array(modified_value))
             return entropy_similarity.get()
         else:
             raise ValueError("target should be cpu or gpu")
 
+    def _remove_duplicate_with_cpu(self, array_1, array_2, max_element):
+        if len(array_1) + len(array_2) < 4_000_000:
+            # When len(array_1) + len(array_2) < 4_000_000, this method is faster than array method
+            aux = np.concatenate((array_1, array_2))
+            aux_sort_indices = np.argsort(aux, kind="mergesort")
+            aux = aux[aux_sort_indices]
+            mask = aux[1:] == aux[:-1]
+            array2_indices = aux_sort_indices[1:][mask] - array_1.size
+            return array2_indices
+        else:
+            # When len(array_1) + len(array_2) > 4_000_000, this method is faster than sort method
+            note = np.zeros(max_element, dtype=np.int8)
+            note[array_1] = 1
+            duplicate_idx = np.where(note[array_2] == 1)[0]
+            return duplicate_idx
+
+
+    def _remove_duplicate_with_gpu(self, array_1, array_2, max_element):
+        import cupy as cp
+        if len(array_1) + len(array_2) < 4_000_000:
+            # When len(array_1) + len(array_2) < 4_000_000, this method is faster than array method
+            aux = cp.array(np.concatenate((array_1, array_2)))
+            aux_sort_indices = cp.argsort(aux)
+            aux = aux[aux_sort_indices]
+            mask = aux[1:] == aux[:-1]
+            ar2_indices = aux_sort_indices[1:][mask] - array_1.size
+            return ar2_indices
+
+        else:
+            # When len(array_1) + len(array_2) > 4_000_000, this method is faster than sort method
+            note = cp.zeros(max_element, dtype=np.int8)
+            note[array_1] = 1
+            duplicate_idx = cp.where(note[array_2] == 1)[0]
+            return duplicate_idx
+
     def build_index(self, all_spectra_list: list,  max_indexed_mz: float = 1500.00005):
         """
         Build the index for the MS/MS spectra library.
 
         The spectra provided to this function should be a dictionary in the format of {"precursor_mz": precursor_mz, "peaks": peaks}.
         The precursor_mz is the precursor m/z value of the MS/MS spectrum;
         The peaks is a numpy array which has been processed by the function "clean_spectrum".
@@ -317,56 +352,55 @@
             assert peaks.shape[0] <= 1 or np.min(peaks[1:, 0] - peaks[:-1, 0]) > self.max_ms2_tolerance_in_da * 2, \
                 "The peaks array should be sorted by m/z, and the m/z difference between two adjacent peaks should be larger than 2 * max_ms2_tolerance_in_da."
 
             # Preprocess the peaks array.
             peaks = self._preprocess_peaks(peaks)
 
             # Assign the product ion m/z
-            peak_data.view(np.float32).reshape(total_peaks_num, -1)[peak_idx:(peak_idx + peaks.shape[0]), 0] = peaks[:, 0]
+            peak_data_item = peak_data[peak_idx:(peak_idx + peaks.shape[0])]
+            peak_data_item["ion_mz"] = peaks[:, 0]
             # Assign the neutral loss mass
-            peak_data.view(np.float32).reshape(total_peaks_num, -1)[peak_idx:(peak_idx + peaks.shape[0]), 1] = precursor_mz - peaks[:, 0]
+            peak_data_item["nl_mass"] = precursor_mz - peaks[:, 0]
             # Assign the intensity
-            peak_data.view(np.float32).reshape(total_peaks_num, -1)[peak_idx:(peak_idx + peaks.shape[0]), 2] = peaks[:, 1]
+            peak_data_item["intensity"] = peaks[:, 1]
             # Assign the spectrum index
-            peak_data.view(np.uint32).reshape(total_peaks_num, -1)[peak_idx:(peak_idx + peaks.shape[0]), 3] = idx
+            peak_data_item["spec_idx"] = idx
             # Set the peak index
             peak_idx += peaks.shape[0]
 
         ############## Step 2: Build the index by sort with product ions. ##############
         self.index = self._generate_index_from_peak_data(peak_data, max_indexed_mz)
         return self.index
 
     def _generate_index_from_peak_data(self, peak_data, max_indexed_mz):
-        total_peaks_num = peak_data.shape[0]
-
         # Sort with precursor m/z.
         peak_data.sort(order="ion_mz")
 
         # Record the m/z, intensity, and spectrum index information for product ions.
-        all_ions_mz = np.copy(peak_data.view(np.float32).reshape(total_peaks_num, -1)[:, 0])
-        all_ions_intensity = np.copy(peak_data.view(np.float32).reshape(total_peaks_num, -1)[:, 2])
-        all_ions_spec_idx = np.copy(peak_data.view(np.uint32).reshape(total_peaks_num, -1)[:, 3])
+        all_ions_mz = np.copy(peak_data["ion_mz"])
+        all_ions_intensity = np.copy(peak_data["intensity"])
+        all_ions_spec_idx = np.copy(peak_data["spec_idx"])
 
         # Assign the index of the product ions.
-        peak_data.view(np.uint64).reshape(total_peaks_num, -1)[:, 2] = np.arange(0, self.total_peaks_num, dtype=np.uint64)
+        peak_data["peak_idx"] = np.arange(0, self.total_peaks_num, dtype=np.uint64)
 
         # Build index for fast access to the ion's m/z.
         max_mz = min(np.max(all_ions_mz), max_indexed_mz)
         search_array = np.arange(0., max_mz, self.mz_index_step)
         all_ions_mz_idx_start = np.searchsorted(all_ions_mz, search_array, side='left').astype(np.int64)
 
         ############## Step 3: Build the index by sort with neutral loss mass. ##############
         # Sort with the neutral loss mass.
         peak_data.sort(order="nl_mass")
 
         # Record the m/z, intensity, spectrum index, and product ions index information for neutral loss ions.
-        all_nl_mass = np.copy(peak_data.view(np.float32).reshape(total_peaks_num, -1)[:, 1])
-        all_nl_intensity = np.copy(peak_data.view(np.float32).reshape(total_peaks_num, -1)[:, 2])
-        all_nl_spec_idx = np.copy(peak_data.view(np.uint32).reshape(total_peaks_num, -1)[:, 3])
-        all_ions_idx_for_nl = np.copy(peak_data.view(np.uint64).reshape(total_peaks_num, -1)[:, 2])
+        all_nl_mass = peak_data["nl_mass"]
+        all_nl_intensity = peak_data["intensity"]
+        all_nl_spec_idx = peak_data["spec_idx"]
+        all_ions_idx_for_nl = peak_data["peak_idx"]
 
         # Build the index for fast access to the neutral loss mass.
         max_mz = min(np.max(all_nl_mass), max_indexed_mz)
         search_array = np.arange(0., max_mz, self.mz_index_step)
         all_nl_mass_idx_start = np.searchsorted(all_nl_mass, search_array, side='left').astype(np.int64)
 
         ############## Step 4: Save the index. ##############
@@ -387,14 +421,30 @@
         modified_value = intensity_mix * np.log2(intensity_mix) \
             - intensity_library * np.log2(intensity_library) - intensity_query * np.log2(intensity_query)
         return modified_value
 
     def _score_peaks_gpu(self, entropy_transform, intensity_query, intensity_library):
         return entropy_transform(intensity_library, intensity_query)
 
+    def _find_location_from_array_with_index(self, wanted_mz, mz_array, mz_idx_start_array, side, index_number):
+        mz_min_int = (np.floor(wanted_mz*index_number)).astype(int)
+        mz_max_int = mz_min_int + 1
+
+        if mz_min_int >= len(mz_idx_start_array):
+            mz_idx_search_start = mz_idx_start_array[-1]
+        else:
+            mz_idx_search_start = mz_idx_start_array[mz_min_int].astype(int)
+
+        if mz_max_int >= len(mz_idx_start_array):
+            mz_idx_search_end = len(mz_array)
+        else:
+            mz_idx_search_end = mz_idx_start_array[mz_max_int].astype(int)+1
+
+        return mz_idx_search_start + np.searchsorted(mz_array[mz_idx_search_start:mz_idx_search_end], wanted_mz, side=side)
+
     def save_memory_for_multiprocessing(self):
         """
         Move the numpy array in the index to shared memory in order to save memory. 
         This function is not required when you only use one thread to search the MS/MS spectra.
         When use multiple threads, this function is also not required but highly recommended, as it avoids the memory copy and saves a lot of memory and time.
         """
         if self._init_for_multiprocessing:
@@ -443,15 +493,14 @@
             "total_spectra_num": int(self.total_spectra_num),
             'total_peaks_num': int(self.total_peaks_num),
             "max_ms2_tolerance_in_da": float(self.max_ms2_tolerance_in_da),
         }
         with open(path_data / 'information.json', 'w') as f:
             json.dump(information, f)
 
-
 def _convert_numpy_array_to_shared_memory(np_array, array_c_type=None):
     """
     The char table of shared memory can be find at:
     https://docs.python.org/3/library/struct.html#format-characters
     https://docs.python.org/3/library/array.html#module-array (This one is wrong!)
     The documentation of numpy.frombuffer can be find at:
     https://docs.scipy.org/doc/numpy/reference/generated/numpy.frombuffer.html
@@ -462,42 +511,7 @@
     if array_c_type is None:
         array_c_type = np_array.dtype.char
     base = multiprocessing.Array(array_c_type, num, lock=False)
     np_array_new = np.frombuffer(base, dtype=np_array.dtype).reshape(dim)
     np_array_new[:] = np_array
     return np_array_new
 
-
-def _find_location_from_array_with_index(wanted_mz, mz_array, mz_idx_start_array, side, index_number):
-    mz_min_int = (np.floor(wanted_mz*index_number)).astype(int)
-    mz_max_int = mz_min_int + 1
-
-    if mz_min_int >= len(mz_idx_start_array):
-        mz_idx_search_start = mz_idx_start_array[-1]
-    else:
-        mz_idx_search_start = mz_idx_start_array[mz_min_int].astype(int)
-
-    if mz_max_int >= len(mz_idx_start_array):
-        mz_idx_search_end = len(mz_array)
-    else:
-        mz_idx_search_end = mz_idx_start_array[mz_max_int].astype(int)+1
-
-    return mz_idx_search_start + np.searchsorted(mz_array[mz_idx_search_start:mz_idx_search_end], wanted_mz, side=side)
-
-
-def _intersect1d(ar1, ar2):
-    aux = np.concatenate((ar1, ar2))
-    aux_sort_indices = np.argsort(aux, kind='mergesort')
-    aux = aux[aux_sort_indices]
-    mask = aux[1:] == aux[:-1]
-    ar2_indices = aux_sort_indices[1:][mask] - ar1.size
-    return ar2_indices
-
-
-def _intersect1d_with_gpu(ar1, ar2):
-    import cupy as cp
-    aux = cp.array(np.concatenate((ar1, ar2)))
-    aux_sort_indices = cp.argsort(aux)
-    aux = aux[aux_sort_indices]
-    mask = aux[1:] == aux[:-1]
-    ar2_indices = aux_sort_indices[1:][mask] - ar1.size
-    return ar2_indices
```

### Comparing `ms_entropy-0.5.8/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.6.0/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.6.0/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.6.0/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/file_io/mzml_file.py` & `ms_entropy-0.6.0/ms_entropy/file_io/mzml_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/file_io/shared.py` & `ms_entropy-0.6.0/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/file_io/spec_file.py` & `ms_entropy-0.6.0/ms_entropy/file_io/spec_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.c` & `ms_entropy-0.6.0/ms_entropy/tools/fast_entropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/tools/fast_entropy.pyx` & `ms_entropy-0.6.0/ms_entropy/tools/fast_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.c` & `ms_entropy-0.6.0/ms_entropy/tools/fast_spectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/tools/fast_spectrum.pyx` & `ms_entropy-0.6.0/ms_entropy/tools/fast_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy/tools/tools.py` & `ms_entropy-0.6.0/ms_entropy/tools/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.6.0/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.8/setup.py` & `ms_entropy-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.5.8',
+    version='0.6.0',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=find_packages(where='.', exclude=['tests', 'docs', 'examples', 'manuscript', 'dist', 'build']),
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
         "cython >= 0.29",
         "lz4 >= 4.3.2",
         "msgpack >= 1.0.5",
         # "pymzml>=2.5.2",
         "pyteomics == 4.6"
     ],
     extras_require={
-        "gpu": ["cupy >= 8.3.0"]
+        "gpu": ["cupy >= 12.0.0"]
     },
     keywords=[
         "ms entropy",
         "ms spectral entropy",
         "spectral entropy",
         "spectral similarity",
         "entropy similarity",
```

