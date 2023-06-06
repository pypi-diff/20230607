# Comparing `tmp/multipie-1.1.4.tar.gz` & `tmp/multipie-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipie-1.1.4.tar", last modified: Sun Jun  4 14:49:03 2023, max compression
+gzip compressed data, was "multipie-1.1.5.tar", last modified: Tue Jun  6 23:09:26 2023, max compression
```

## Comparing `multipie-1.1.4.tar` & `multipie-1.1.5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.974689 multipie-1.1.4/
--rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.1.4/LICENSE
--rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.1.4/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-04 14:49:03.974771 multipie-1.1.4/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1727 2023-05-25 21:40:12.000000 multipie-1.1.4/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.945128 multipie-1.1.4/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-06-04 14:34:18.000000 multipie-1.1.4/multipie/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.958469 multipie-1.1.4/multipie/binary_data/
--rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.1.4/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.1.4/multipie/binary_data/CharacterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.1.4/multipie/binary_data/ClebschGordanPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.1.4/multipie/binary_data/HarmonicsPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.1.4/multipie/binary_data/ResponseTensorPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.1.4/multipie/binary_data/SymmetryOperationGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.1.4/multipie/binary_data/VirtualClusterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.1.4/multipie/binary_data/WyckoffGSet.pkl
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.958927 multipie-1.1.4/multipie/character/
--rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/character/character_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/character/character_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.959194 multipie-1.1.4/multipie/clebsch_gordan/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/clebsch_gordan/clebsch_gordan_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
--rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.1.4/multipie/const.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.967054 multipie-1.1.4/multipie/data/
--rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_atomic_multipoles.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_cartesian_to_ch_harmoncis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_character_table.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_compatibility_relation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_harmonics_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_no_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_product_decomp.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_symmetry_operation_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_symmetry_operation_sg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_tag_harmonics_alias.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_tag_point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_tag_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_transform_matrix.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_virtual_cluster_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_wyckoff_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/data/data_wyckoff_sg.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.967414 multipie-1.1.4/multipie/group/
--rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/group/point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    22492 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/group/space_group.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.968081 multipie-1.1.4/multipie/harmonics/
--rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/harmonics/harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/harmonics/harmonics_complex_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/harmonics/harmonics_complex_pg_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/harmonics/harmonics_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/harmonics/harmonics_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.968211 multipie-1.1.4/multipie/harmonics/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/harmonics/util/equivalent_operator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.968891 multipie-1.1.4/multipie/model/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2150 2023-06-01 12:24:37.000000 multipie-1.1.4/multipie/model/construct_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/model/create_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    31775 2023-06-04 14:44:20.000000 multipie-1.1.4/multipie/model/material_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/model/multipie_manager.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    17891 2023-06-01 08:23:27.000000 multipie-1.1.4/multipie/model/symmetry_adapted_model.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.969355 multipie-1.1.4/multipie/model/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/model/util/atomic_matrix_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    25780 2023-05-31 07:44:56.000000 multipie-1.1.4/multipie/model/util/create_pdf.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    24859 2023-06-01 08:23:27.000000 multipie-1.1.4/multipie/model/util/symmetry_adapted_model_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.942975 multipie-1.1.4/multipie/multipole/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.969942 multipie-1.1.4/multipie/multipole/base/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/multipole/base/base_atomic_multipole_dataset.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/multipole/base/base_atomic_multipole_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.970996 multipie-1.1.4/multipie/multipole/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    14715 2023-05-31 07:36:18.000000 multipie-1.1.4/multipie/multipole/util/atomic_orbital_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     6736 2023-06-01 08:23:27.000000 multipie-1.1.4/multipie/multipole/util/atomic_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/multipole/util/multipole_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/multipole/util/pauli.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/multipole/util/spin_orbital_basis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/multipole/util/structure_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/multipole/util/z_samb_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.971273 multipie-1.1.4/multipie/response_tensor/
--rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/response_tensor/response_tensor_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/response_tensor/response_tensor_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.971415 multipie-1.1.4/multipie/response_tensor/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/response_tensor/util/response_tensor_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.971730 multipie-1.1.4/multipie/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.1.4/multipie/scripts/create_binary.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.1.4/multipie/scripts/create_samb.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.972209 multipie-1.1.4/multipie/symmetry_operation/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/symmetry_operation/symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/symmetry_operation/symmetry_operation_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/symmetry_operation/symmetry_operation_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.972402 multipie-1.1.4/multipie/symmetry_operation/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/symmetry_operation/util/symmetry_operation_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.973943 multipie-1.1.4/multipie/tag/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_list.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_multipole.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/tag/tag_wyckoff.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.974300 multipie-1.1.4/multipie/virtual_cluster/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/virtual_cluster/virtual_cluster_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/virtual_cluster/virtual_cluster_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.974564 multipie-1.1.4/multipie/wyckoff/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.1.4/multipie/wyckoff/wyckoff_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.1.4/multipie/wyckoff/wyckoff_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-04 14:49:03.946019 multipie-1.1.4/multipie.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-04 14:49:03.000000 multipie-1.1.4/multipie.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-06-04 14:49:03.000000 multipie-1.1.4/multipie.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-04 14:49:03.000000 multipie-1.1.4/multipie.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)      116 2023-06-04 14:49:03.000000 multipie-1.1.4/multipie.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-06-04 14:49:03.000000 multipie-1.1.4/multipie.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        9 2023-06-04 14:49:03.000000 multipie-1.1.4/multipie.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      888 2023-06-04 14:49:03.975157 multipie-1.1.4/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.1.4/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.406180 multipie-1.1.5/
+-rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.1.5/LICENSE
+-rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.1.5/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-06 23:09:26.406315 multipie-1.1.5/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1727 2023-05-25 21:40:12.000000 multipie-1.1.5/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.353234 multipie-1.1.5/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-06-06 23:05:26.000000 multipie-1.1.5/multipie/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.388709 multipie-1.1.5/multipie/binary_data/
+-rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.1.5/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.1.5/multipie/binary_data/CharacterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.1.5/multipie/binary_data/ClebschGordanPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.1.5/multipie/binary_data/HarmonicsPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.1.5/multipie/binary_data/ResponseTensorPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.1.5/multipie/binary_data/SymmetryOperationGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.1.5/multipie/binary_data/VirtualClusterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.1.5/multipie/binary_data/WyckoffGSet.pkl
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.389853 multipie-1.1.5/multipie/character/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/character/character_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/character/character_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.390139 multipie-1.1.5/multipie/clebsch_gordan/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/clebsch_gordan/clebsch_gordan_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.1.5/multipie/const.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.398106 multipie-1.1.5/multipie/data/
+-rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_atomic_multipoles.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_cartesian_to_ch_harmoncis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_character_table.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_compatibility_relation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_harmonics_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_no_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_product_decomp.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_symmetry_operation_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_symmetry_operation_sg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_tag_harmonics_alias.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_tag_point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_tag_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_transform_matrix.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_virtual_cluster_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_wyckoff_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/data/data_wyckoff_sg.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.398535 multipie-1.1.5/multipie/group/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/group/point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22492 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/group/space_group.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.399343 multipie-1.1.5/multipie/harmonics/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/harmonics/harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/harmonics/harmonics_complex_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/harmonics/harmonics_complex_pg_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/harmonics/harmonics_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/harmonics/harmonics_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.399480 multipie-1.1.5/multipie/harmonics/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/harmonics/util/equivalent_operator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.400619 multipie-1.1.5/multipie/model/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2198 2023-06-06 22:09:12.000000 multipie-1.1.5/multipie/model/construct_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/model/create_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    31775 2023-06-04 14:44:20.000000 multipie-1.1.5/multipie/model/material_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/model/multipie_manager.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    17731 2023-06-06 23:04:26.000000 multipie-1.1.5/multipie/model/symmetry_adapted_model.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.401361 multipie-1.1.5/multipie/model/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/model/util/atomic_matrix_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    25780 2023-05-31 07:44:56.000000 multipie-1.1.5/multipie/model/util/create_pdf.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    24859 2023-06-01 08:23:27.000000 multipie-1.1.5/multipie/model/util/symmetry_adapted_model_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.351445 multipie-1.1.5/multipie/multipole/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.401691 multipie-1.1.5/multipie/multipole/base/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/multipole/base/base_atomic_multipole_dataset.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/multipole/base/base_atomic_multipole_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.402672 multipie-1.1.5/multipie/multipole/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14715 2023-05-31 07:36:18.000000 multipie-1.1.5/multipie/multipole/util/atomic_orbital_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6736 2023-06-01 08:23:27.000000 multipie-1.1.5/multipie/multipole/util/atomic_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/multipole/util/multipole_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/multipole/util/pauli.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/multipole/util/spin_orbital_basis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/multipole/util/structure_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/multipole/util/z_samb_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.402984 multipie-1.1.5/multipie/response_tensor/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/response_tensor/response_tensor_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/response_tensor/response_tensor_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.403129 multipie-1.1.5/multipie/response_tensor/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/response_tensor/util/response_tensor_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.403473 multipie-1.1.5/multipie/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.1.5/multipie/scripts/create_binary.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.1.5/multipie/scripts/create_samb.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.404122 multipie-1.1.5/multipie/symmetry_operation/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/symmetry_operation/symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/symmetry_operation/symmetry_operation_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/symmetry_operation/symmetry_operation_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.404320 multipie-1.1.5/multipie/symmetry_operation/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/symmetry_operation/util/symmetry_operation_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.405478 multipie-1.1.5/multipie/tag/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_list.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_multipole.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/tag/tag_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.405733 multipie-1.1.5/multipie/virtual_cluster/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/virtual_cluster/virtual_cluster_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/virtual_cluster/virtual_cluster_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.406033 multipie-1.1.5/multipie/wyckoff/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.1.5/multipie/wyckoff/wyckoff_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.1.5/multipie/wyckoff/wyckoff_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-06 23:09:26.354485 multipie-1.1.5/multipie.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-06 23:09:26.000000 multipie-1.1.5/multipie.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-06-06 23:09:26.000000 multipie-1.1.5/multipie.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-06 23:09:26.000000 multipie-1.1.5/multipie.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      116 2023-06-06 23:09:26.000000 multipie-1.1.5/multipie.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-06-06 23:09:26.000000 multipie-1.1.5/multipie.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        9 2023-06-06 23:09:26.000000 multipie-1.1.5/multipie.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      888 2023-06-06 23:09:26.406766 multipie-1.1.5/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.1.5/setup.py
```

### Comparing `multipie-1.1.4/LICENSE` & `multipie-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/PKG-INFO` & `multipie-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.1.4/README.md` & `multipie-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/__init__.py` & `multipie-1.1.5/multipie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 __top_dir__ = os.path.normpath(os.path.dirname(__file__) + "/../") + "/"
 __bin_dir__ = __top_dir__ + "multipie/binary_data/"
 
 
 # ==================================================
 from gcoreutils.string_util import class_name
 from gcoreutils.binary_manager import BinaryManager
```

### Comparing `multipie-1.1.4/multipie/binary_data/BaseAtomicMultipoleDataset.pkl` & `multipie-1.1.5/multipie/binary_data/BaseAtomicMultipoleDataset.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/CharacterPGSet.pkl` & `multipie-1.1.5/multipie/binary_data/CharacterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/ClebschGordanPGSet.pkl` & `multipie-1.1.5/multipie/binary_data/ClebschGordanPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/HarmonicsPGSet.pkl` & `multipie-1.1.5/multipie/binary_data/HarmonicsPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/ResponseTensorPGSet.pkl` & `multipie-1.1.5/multipie/binary_data/ResponseTensorPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/SymmetryOperationGSet.pkl` & `multipie-1.1.5/multipie/binary_data/SymmetryOperationGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/VirtualClusterPGSet.pkl` & `multipie-1.1.5/multipie/binary_data/VirtualClusterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/binary_data/WyckoffGSet.pkl` & `multipie-1.1.5/multipie/binary_data/WyckoffGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/character/character_pg.py` & `multipie-1.1.5/multipie/character/character_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/character/character_pg_set.py` & `multipie-1.1.5/multipie/character/character_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/clebsch_gordan/clebsch_gordan_pg.py` & `multipie-1.1.5/multipie/clebsch_gordan/clebsch_gordan_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/clebsch_gordan/clebsch_gordan_pg_set.py` & `multipie-1.1.5/multipie/clebsch_gordan/clebsch_gordan_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/const.py` & `multipie-1.1.5/multipie/const.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_atomic_multipoles.py` & `multipie-1.1.5/multipie/data/data_atomic_multipoles.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_cartesian_to_ch_harmoncis.py` & `multipie-1.1.5/multipie/data/data_cartesian_to_ch_harmoncis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_character_table.py` & `multipie-1.1.5/multipie/data/data_character_table.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_compatibility_relation.py` & `multipie-1.1.5/multipie/data/data_compatibility_relation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_harmonics.py` & `multipie-1.1.5/multipie/data/data_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_harmonics_real.py` & `multipie-1.1.5/multipie/data/data_harmonics_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_no_space_group.py` & `multipie-1.1.5/multipie/data/data_no_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_product_decomp.py` & `multipie-1.1.5/multipie/data/data_product_decomp.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_symmetry_operation_pg.py` & `multipie-1.1.5/multipie/data/data_symmetry_operation_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_symmetry_operation_sg.py` & `multipie-1.1.5/multipie/data/data_symmetry_operation_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_tag_harmonics_alias.py` & `multipie-1.1.5/multipie/data/data_tag_harmonics_alias.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_tag_irrep.py` & `multipie-1.1.5/multipie/data/data_tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_tag_point_group.py` & `multipie-1.1.5/multipie/data/data_tag_point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_tag_space_group.py` & `multipie-1.1.5/multipie/data/data_tag_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_transform_matrix.py` & `multipie-1.1.5/multipie/data/data_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_virtual_cluster_real.py` & `multipie-1.1.5/multipie/data/data_virtual_cluster_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_wyckoff_pg.py` & `multipie-1.1.5/multipie/data/data_wyckoff_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/data/data_wyckoff_sg.py` & `multipie-1.1.5/multipie/data/data_wyckoff_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/group/point_group.py` & `multipie-1.1.5/multipie/group/point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/group/space_group.py` & `multipie-1.1.5/multipie/group/space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/harmonics/harmonics.py` & `multipie-1.1.5/multipie/harmonics/harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/harmonics/harmonics_complex_pg.py` & `multipie-1.1.5/multipie/harmonics/harmonics_complex_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/harmonics/harmonics_complex_pg_set.py` & `multipie-1.1.5/multipie/harmonics/harmonics_complex_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/harmonics/harmonics_pg.py` & `multipie-1.1.5/multipie/harmonics/harmonics_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/harmonics/harmonics_pg_set.py` & `multipie-1.1.5/multipie/harmonics/harmonics_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/harmonics/util/equivalent_operator.py` & `multipie-1.1.5/multipie/harmonics/util/equivalent_operator.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/model/construct_model.py` & `multipie-1.1.5/multipie/model/construct_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 # ==================================================
 def convert_samb_to_matrix_set(Z, param=None):
     """
     convert SAMB to a set of matrix.
 
     Args:
         Z (ndarray): samb matrix, [#bases, #k, dim, dim].
-        param (list, optional): parameter set(s).
+        param (list, optional): parameter set(s), [z_j] for crystal or [z_j]/[[z_j]] for molecule.
 
     Returns:
-        ndarray: matrix, [#params, #k, dim, dim].
+        ndarray: matrix, [#params/#k, dim, dim].
     """
     if param is None:
         param = [1.0] * Z.shape[0]
     param = np.array(param)
     if param.ndim == 1:
         M = [Z.transpose(1, 2, 3, 0) @ param]
     else:
```

### Comparing `multipie-1.1.4/multipie/model/create_model.py` & `multipie-1.1.5/multipie/model/create_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/model/material_model.py` & `multipie-1.1.5/multipie/model/material_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/model/multipie_manager.py` & `multipie-1.1.5/multipie/model/multipie_manager.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/model/symmetry_adapted_model.py` & `multipie-1.1.5/multipie/model/symmetry_adapted_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     - atomic : { "M_#" : ["amp_#"] }
     - site_cluster : { "S_#" : ["smp_#"] }
     - bond_cluster : { "B_#" : ["bmp_#"] }
     - uniform : { "S_#"/"B_#" : ["ump_#"] }
     - structure* : { "B_#" : ["kmp_#"] }
     - Z : { ("M_#", "S_#"/"B_#") : ["z_#"] }
     - version : MultiPie version
-    - harmonics : { head : { "harm_tag" } }
+    - harmonics : { head : [TagMultipole] }
 
 - data
     - atomic : { "amp_#" : ( TagMultipole, shape, [(i, j, matrix element)] ) }
     - site_cluster : { "smp_#" : ( TagMultipole, [vector component] ) }
     - bond_cluster : { "bmp_#" : ( TagMultipole, [vector component] ) }
     - uniform : { "ump_#" : ( TagMultipole, shape, [(i, j, matrix element)] ) }
-    - structure* : { "kmp_#" : (TagMultipole, "formfactor") }
+    - structure* : { "kmp_#" : (TagMultipole, "structure factor") }
     - Z : {"z_#" : ( TagMultipole, [(coeff, "amp_#", "smp_#"/"bmp_#/ump_#")] ) }
     - Zk* : {"z_#" : ( TagMultipole, [(coeff, "amp_#", "ump_#", "kmp_#")] ) }
 """
 
 # ==================================================
 matrix_header_str = """
 == SAMB in full matrix form (* only for crystal) ===
@@ -117,46 +117,38 @@
 
         # site/bond-cluster
         rep_site_dict = {cluster_tag: site[site_list[0]][0] for cluster_tag, site_list in cluster_site.items()}
         rep_bond_dict = {cluster_tag: bond[bond_list[0]][0] for cluster_tag, bond_list in cluster_bond.items()}
 
         func = create_cluster_samb_set
         args = [g, rep_site_dict, rep_bond_dict, self._parallel]
-        site_cluster_info, site_cluster_data, bond_cluster_info, bond_cluster_data = _run(
-            "site/bond-cluster", mpm, func, *args
-        )
+        site_cluster_info, site_cluster_data, bond_cluster_info, bond_cluster_data = _run("site/bond-cluster", mpm, func, *args)
 
         # uniform
         cluster_samb_set = {S_i: [site_cluster_data[smp_i] for smp_i in lst] for S_i, lst in site_cluster_info.items()}
         cluster_samb_set |= {B_i: [bond_cluster_data[bmp_i] for bmp_i in lst] for B_i, lst in bond_cluster_info.items()}
         braket_indexes_dict = {
-            cluster_tag: [site[site_tag][2] for site_tag in site_list]
-            for cluster_tag, site_list in cluster_site.items()
+            cluster_tag: [site[site_tag][2] for site_tag in site_list] for cluster_tag, site_list in cluster_site.items()
         }
         braket_indexes_dict |= {
-            cluster_tag: [bond[bond_tag][2] for bond_tag in bond_list]
-            for cluster_tag, bond_list in cluster_bond.items()
+            cluster_tag: [bond[bond_tag][2] for bond_tag in bond_list] for cluster_tag, bond_list in cluster_bond.items()
         }
         dim = len(site)
 
         func = create_uniform_samb_set
         args = [cluster_samb_set, braket_indexes_dict, dim, self._parallel]
         uniform_info, uniform_data = _run("uniform", mpm, func, *args)
 
         # Z
         x_tag_dict = {(M_i, atomic_data[amp_i][0]): amp_i for M_i, lst in atomic_info.items() for amp_i in lst}
         if molecule:
             y_tag_dict = {(SB_i, uniform_data[ump_i][0]): ump_i for SB_i, lst in uniform_info.items() for ump_i in lst}
         else:
-            y_tag_dict = {
-                (S_i, site_cluster_data[smp_i][0]): smp_i for S_i, lst in site_cluster_info.items() for smp_i in lst
-            }
-            y_tag_dict |= {
-                (B_i, bond_cluster_data[bmp_i][0]): bmp_i for B_i, lst in bond_cluster_info.items() for bmp_i in lst
-            }
+            y_tag_dict = {(S_i, site_cluster_data[smp_i][0]): smp_i for S_i, lst in site_cluster_info.items() for smp_i in lst}
+            y_tag_dict |= {(B_i, bond_cluster_data[bmp_i][0]): bmp_i for B_i, lst in bond_cluster_info.items() for bmp_i in lst}
 
         cluster_site_bond = cluster_site | cluster_bond
         braket_site_no_dict = {S_i: site[site_list[0]][2] for S_i, site_list in cluster_site.items()}
         braket_site_no_dict |= {B_i: bond[bond_list[0]][2] for B_i, bond_list in cluster_bond.items()}
         M_SB_list = []
         for SB_i in cluster_site_bond.keys():
             for _, _, M_i in cluster_atomic[braket_site_no_dict[SB_i]]:
@@ -171,17 +163,15 @@
             bc_samb_set = {B_i: [bond_cluster_data[bmp_i] for bmp_i in lst] for B_i, lst in bond_cluster_info.items()}
 
             func = create_structure_samb_set
             args = [bc_samb_set, cluster_bond, bond, self._parallel]
             structure_info, structure_data = _run("structure", mpm, func, *args)
 
             # Zk
-            bc_samb_set = {
-                B_i: [(bmp_i, bond_cluster_data[bmp_i][1]) for bmp_i in lst] for B_i, lst in bond_cluster_info.items()
-            }
+            bc_samb_set = {B_i: [(bmp_i, bond_cluster_data[bmp_i][1]) for bmp_i in lst] for B_i, lst in bond_cluster_info.items()}
             u_samb_set = [(ump_i, m) for ump_i, (_, m) in uniform_data.items()]
             k_samb_set = [(kmp_i, fk) for kmp_i, (_, fk) in structure_data.items()]
 
             func = create_zk_samb_set
             args = [z_data, bc_samb_set, u_samb_set, k_samb_set, cluster_bond, bond, dim, self._parallel]
             zk_data = _run("Zk", mpm, func, *args)
 
@@ -271,17 +261,15 @@
             "uniform": uniform_data,
             "Z": z_data,
         }
         if not self._model["info"]["molecule"]:
             structure_data = {
                 kmp_i: (str(tag), str(fk).replace("'", "")) for kmp_i, (tag, fk) in self["data"]["structure"].items()
             }
-            zk_data = {
-                z_i: (str(tag), [tuple(map(str, v)) for v in lst]) for z_i, (tag, lst) in self["data"]["Zk"].items()
-            }
+            zk_data = {z_i: (str(tag), [tuple(map(str, v)) for v in lst]) for z_i, (tag, lst) in self["data"]["Zk"].items()}
             data["structure"] = structure_data
             data["Zk"] = zk_data
 
         return {"info": info, "data": data}
 
     # ==================================================
     def create_matrix(self, full=False, fmt="sympy"):
```

### Comparing `multipie-1.1.4/multipie/model/util/create_pdf.py` & `multipie-1.1.5/multipie/model/util/create_pdf.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/model/util/symmetry_adapted_model_util.py` & `multipie-1.1.5/multipie/model/util/symmetry_adapted_model_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/base/base_atomic_multipole_dataset.py` & `multipie-1.1.5/multipie/multipole/base/base_atomic_multipole_dataset.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/base/base_atomic_multipole_set.py` & `multipie-1.1.5/multipie/multipole/base/base_atomic_multipole_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/atomic_orbital_util.py` & `multipie-1.1.5/multipie/multipole/util/atomic_orbital_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/atomic_samb_util.py` & `multipie-1.1.5/multipie/multipole/util/atomic_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/multipole_util.py` & `multipie-1.1.5/multipie/multipole/util/multipole_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/pauli.py` & `multipie-1.1.5/multipie/multipole/util/pauli.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/spin_orbital_basis.py` & `multipie-1.1.5/multipie/multipole/util/spin_orbital_basis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/structure_samb_util.py` & `multipie-1.1.5/multipie/multipole/util/structure_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/multipole/util/z_samb_util.py` & `multipie-1.1.5/multipie/multipole/util/z_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/response_tensor/response_tensor_pg.py` & `multipie-1.1.5/multipie/response_tensor/response_tensor_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/response_tensor/response_tensor_pg_set.py` & `multipie-1.1.5/multipie/response_tensor/response_tensor_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/response_tensor/util/response_tensor_util.py` & `multipie-1.1.5/multipie/response_tensor/util/response_tensor_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/scripts/create_binary.py` & `multipie-1.1.5/multipie/scripts/create_binary.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/scripts/create_samb.py` & `multipie-1.1.5/multipie/scripts/create_samb.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/symmetry_operation/symmetry_operation.py` & `multipie-1.1.5/multipie/symmetry_operation/symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/symmetry_operation/symmetry_operation_g.py` & `multipie-1.1.5/multipie/symmetry_operation/symmetry_operation_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/symmetry_operation/symmetry_operation_g_set.py` & `multipie-1.1.5/multipie/symmetry_operation/symmetry_operation_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/symmetry_operation/util/symmetry_operation_util.py` & `multipie-1.1.5/multipie/symmetry_operation/util/symmetry_operation_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag.py` & `multipie-1.1.5/multipie/tag/tag.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_group.py` & `multipie-1.1.5/multipie/tag/tag_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_irrep.py` & `multipie-1.1.5/multipie/tag/tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_list.py` & `multipie-1.1.5/multipie/tag/tag_list.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_multipole.py` & `multipie-1.1.5/multipie/tag/tag_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_response_tensor.py` & `multipie-1.1.5/multipie/tag/tag_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_symmetry_operation.py` & `multipie-1.1.5/multipie/tag/tag_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/tag/tag_wyckoff.py` & `multipie-1.1.5/multipie/tag/tag_wyckoff.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/virtual_cluster/virtual_cluster_pg.py` & `multipie-1.1.5/multipie/virtual_cluster/virtual_cluster_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/virtual_cluster/virtual_cluster_pg_set.py` & `multipie-1.1.5/multipie/virtual_cluster/virtual_cluster_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/wyckoff/wyckoff_g.py` & `multipie-1.1.5/multipie/wyckoff/wyckoff_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie/wyckoff/wyckoff_g_set.py` & `multipie-1.1.5/multipie/wyckoff/wyckoff_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/multipie.egg-info/PKG-INFO` & `multipie-1.1.5/multipie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.1.4/multipie.egg-info/SOURCES.txt` & `multipie-1.1.5/multipie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multipie-1.1.4/setup.cfg` & `multipie-1.1.5/setup.cfg`

 * *Files identical despite different names*

