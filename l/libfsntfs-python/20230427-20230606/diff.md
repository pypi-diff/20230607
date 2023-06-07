# Comparing `tmp/libfsntfs-python-20230427.tar.gz` & `tmp/libfsntfs-python-20230606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfsntfs-python-20230427.tar", last modified: Sat Apr 29 07:47:21 2023, max compression
+gzip compressed data, was "libfsntfs-python-20230606.tar", last modified: Wed Jun  7 04:06:26 2023, max compression
```

## Comparing `libfsntfs-python-20230427.tar` & `libfsntfs-python-20230606.tar`

### file list

```diff
@@ -1,1228 +1,1228 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32273 2023-04-29 07:19:08.000000 libfsntfs-20230427/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-04-29 07:18:41.000000 libfsntfs-20230427/libfcache/libfcache_date_time.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/common/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/config_msc.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/byte_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/common.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/system_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-04-27 16:30:55.000000 libfsntfs-20230427/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-04-29 07:19:24.000000 libfsntfs-20230427/common/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/types.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/config_winapi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19504 2023-04-29 07:19:24.000000 libfsntfs-20230427/common/config.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26844 2023-04-29 07:19:08.000000 libfsntfs-20230427/common/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/file_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18422 2023-04-29 07:19:07.000000 libfsntfs-20230427/common/config.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-04-27 16:31:00.000000 libfsntfs-20230427/common/wide_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31244 2023-04-29 07:19:08.000000 libfsntfs-20230427/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-29 07:18:45.000000 libfsntfs-20230427/libfguid/libfguid_extern.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15806 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_root_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14680 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_volume_information_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      989 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libfsntfs.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35342 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_security_descriptor_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4880 2023-04-27 16:37:43.000000 libfsntfs-20230427/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17795 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15392 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_security_descriptor_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15536 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7132 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_profiler.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41944 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_compressed_data_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    30411 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_cluster_block_stream.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36317 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    27561 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_file_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6049 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_path_hint.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6798 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_compressed_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24256 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_name.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    67794 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_entry_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100428 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_compressed_block_data_handle.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3436 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13832 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_txf_data_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   132840 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_data_stream.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29815 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23213 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_attribute_list_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libfdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_rwlock.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5750 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_tools_info_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_rwlock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14589 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_entry_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8845 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_usn_change_journal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8643 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_extent.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15448 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46804 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9173 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_node_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11496 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_fixup_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51596 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   110531 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_file_system.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_getopt.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    92729 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_cluster_block_vector.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3811 2023-04-27 16:38:07.000000 libfsntfs-20230427/tests/test_tools.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28465 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_standard_information_values.c
--rwxrw-r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10623 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_compression_unit_data_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15740 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31281 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_volume_name_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12560 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_data_run.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14474 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/pyfsntfs_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10373 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_security_descriptor_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-04-27 16:31:37.000000 libfsntfs-20230427/tests/test_runner.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10854 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_volume_information_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26241 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_directory_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23425 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_reparse_point_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39431 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_reparse_point_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)   127782 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_compression.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/pyfsntfs_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63509 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2007 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10606 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   138313 2023-04-29 07:19:09.000000 libfsntfs-20230427/tests/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9580 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35036 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_directory_entries_tree.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libfcache.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35794 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft_attribute_list_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   259855 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7195 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_compression_unit_descriptor.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9191 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_index_value.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14810 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_volume_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59086 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft_entry.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3186 2023-04-28 04:00:25.000000 libfsntfs-20230427/tests/test_fsntfsinfo_bodyfile.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43120 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_file_name_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15477 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_logged_utility_stream_values.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     2248 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/test_fsntfsinfo.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21070 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft_entry_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14191 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_object_identifier_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    60997 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_cluster_block_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33492 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft_metadata_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13974 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_bitmap_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19485 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_cluster_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35027 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_volume_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9333 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_sds_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12477 2023-04-27 16:33:04.000000 libfsntfs-20230427/tests/fsntfs_test_mft_attribute_list.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    92276 2023-04-27 16:31:04.000000 libfsntfs-20230427/tests/fsntfs_test_compressed_block_vector.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31800 2023-04-29 07:19:08.000000 libfsntfs-20230427/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-04-29 07:18:32.000000 libfsntfs-20230427/libclocale/libclocale_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-04-29 07:19:07.000000 libfsntfs-20230427/missing
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3775 2022-04-25 19:40:39.000000 libfsntfs-20230427/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56136 2023-04-29 07:19:04.000000 libfsntfs-20230427/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35306 2023-04-29 07:19:08.000000 libfsntfs-20230427/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-04-29 07:18:26.000000 libfsntfs-20230427/libbfio/libbfio_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-04-27 16:30:55.000000 libfsntfs-20230427/COPYING
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      684 2023-04-27 16:30:55.000000 libfsntfs-20230427/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/include/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      509 2023-04-27 16:30:55.000000 libfsntfs-20230427/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64032 2023-04-27 16:31:00.000000 libfsntfs-20230427/include/libfsntfs.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/include/libfsntfs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4079 2023-04-27 16:31:01.000000 libfsntfs-20230427/include/libfsntfs/definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2023-04-27 16:31:01.000000 libfsntfs-20230427/include/libfsntfs/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-04-29 07:19:24.000000 libfsntfs-20230427/include/libfsntfs/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-04-27 16:31:01.000000 libfsntfs-20230427/include/libfsntfs/features.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5224 2023-04-27 16:31:01.000000 libfsntfs-20230427/include/libfsntfs/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2023-04-29 07:19:24.000000 libfsntfs-20230427/include/libfsntfs/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2023-04-29 07:19:24.000000 libfsntfs-20230427/include/libfsntfs/definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2023-04-27 16:31:01.000000 libfsntfs-20230427/include/libfsntfs/codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-04-27 16:31:01.000000 libfsntfs-20230427/include/libfsntfs/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29864 2023-04-29 07:19:08.000000 libfsntfs-20230427/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64032 2023-04-29 07:19:24.000000 libfsntfs-20230427/include/libfsntfs.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/fsntfstools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3074 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   220309 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/info_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1245 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/digest_hash.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31066 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/mount_file_system.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28494 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/mount_fuse.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libcpath.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5420 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/mount_dokan.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24694 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/mount_file_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15540 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/fsntfsmount.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2568 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/mount_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2724 2020-11-29 18:25:27.000000 libfsntfs-20230427/fsntfstools/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libhmac.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16556 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/mount_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfusn.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11770 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/fsntfsinfo.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_getopt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfwnt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37237 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/mount_file_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_i18n.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_output.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9033 2023-04-27 16:33:04.000000 libfsntfs-20230427/fsntfstools/info_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3298 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/digest_hash.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      989 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libfsntfs.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5731 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36644 2023-04-29 07:19:08.000000 libfsntfs-20230427/fsntfstools/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4584 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_output.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2023-04-27 16:31:03.000000 libfsntfs-20230427/fsntfstools/fsntfstools_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-04-29 07:19:07.000000 libfsntfs-20230427/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-04-29 07:19:08.000000 libfsntfs-20230427/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2023-04-29 07:19:24.000000 libfsntfs-20230427/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/libfsntfs-python3.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/libfsntfs.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2023-04-27 16:31:05.000000 libfsntfs-20230427/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/libfsntfs-tools.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/source/format
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/libfsntfs-dev.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      778 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/rules
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2240 2023-04-27 16:30:55.000000 libfsntfs-20230427/dpkg/control
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/libfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94428 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2062 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2829 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_data_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23416 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9488 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_txf_data_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8562 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_root_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8711 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17036 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_bitmap_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libfwnt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2102 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_profiler.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1909 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_secure.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_object_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compression.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8832 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4582 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8311 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4610 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_data.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3924 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_mft_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8168 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1286 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_fixup_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2486 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_reparse_point.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_data.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5402 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19845 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_name_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1984 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_vector.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7382 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2289 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_txf_data_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    28629 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_data_stream.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2503 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_standard_information.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2005 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_io_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    32475 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_notify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_name.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23871 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_data_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13362 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_node.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15709 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6367 2022-01-13 18:43:42.000000 libfsntfs-20230427/libfsntfs/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12727 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_vector.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2392 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4404 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_data_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    29282 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    76620 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3756 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8183 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_profiler.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12897 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_value.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16323 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_support.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7850 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_buffer_data_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3159 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index_value.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_sds_index_value.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22935 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_name.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libfcache.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_volume_information.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17017 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_extent.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4217 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7978 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index_value.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3360 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_directory_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12001 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    25038 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_directory_entries_tree.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20903 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_data_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2786 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_data_run.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_descriptor.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15319 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19315 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_debug.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2253 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libfdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19566 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19693 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    39153 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2349 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_path_hint.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    63403 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_directory_entries_tree.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3381 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_data_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4428 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_metadata_file.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_vector.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_node_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12385 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_vector.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8597 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_path_hint.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7029 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_fixup_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_error.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2815 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9737 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_data_run.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2373 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9103 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_descriptor.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_index.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22736 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2201 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_bitmap_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3207 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_name_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3248 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_volume_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3475 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20087 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4131 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_extent.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3833 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7027 2023-04-29 07:19:24.000000 libfsntfs-20230427/libfsntfs/libfsntfs_definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_buffer_data_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16683 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    25638 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_stream.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libcthreads.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    54282 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_metadata_file.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17815 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2427 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_mft_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_debug.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2448 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_node.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15170 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_directory_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9290 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12076 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_data_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4008 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_system.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2574 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_support.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3227 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libfdatetime.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55595 2023-04-29 07:19:08.000000 libfsntfs-20230427/libfsntfs/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2318 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_file_name.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18720 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_usn_change_journal.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    60465 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    28966 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_name_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7849 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_logged_utility_stream_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_logged_utility_stream_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6301 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_txf_data.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3874 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6767 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_node_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_extern.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_root_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13040 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_vector.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2807 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4755 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_name_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1107 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs.rc.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21101 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_logged_utility_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20304 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    48386 2023-04-27 16:47:38.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_system.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)   168965 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_file_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1621 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2144 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_value.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2604 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6361 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5429 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_io_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_vector.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libcdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11491 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_sds_index_value.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/fsntfs_mft_attribute_list.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13566 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1105 2023-04-29 07:19:24.000000 libfsntfs-20230427/libfsntfs/libfsntfs.rc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2420 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_data_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4088 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_compression.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_index_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-04-27 16:31:02.000000 libfsntfs-20230427/libfsntfs/libfsntfs_usn_change_journal.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34415 2023-04-29 07:19:08.000000 libfsntfs-20230427/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-04-29 07:18:44.000000 libfsntfs-20230427/libfdatetime/libfdatetime_filetime.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32564 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-04-29 07:18:31.000000 libfsntfs-20230427/libcfile/libcfile_notify.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35469 2023-04-29 07:19:09.000000 libfsntfs-20230427/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_access_control_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2023-04-29 07:18:48.000000 libfsntfs-20230427/libfwnt/libfwnt_debug.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34654 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-04-29 07:18:39.000000 libfsntfs-20230427/libcthreads/libcthreads_queue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       93 2023-04-27 16:31:00.000000 libfsntfs-20230427/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      757 2023-04-27 16:30:55.000000 libfsntfs-20230427/libfsntfs.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/pyfsntfs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_data_streams.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3169 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_name_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23172 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23389 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_attribute_flags.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11552 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2911 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_guid.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_object_identifier_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2477 2018-08-18 07:35:36.000000 libfsntfs-20230427/pyfsntfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9341 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_attributes.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3400 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_standard_information_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9524 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_reparse_point_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_python.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27912 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_data_stream.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_object_io_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_datetime.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_security_descriptor_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1361 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8966 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9649 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36819 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1180 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_guid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_attributes.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5347 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_name_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2918 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_file_entries.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23602 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_standard_information_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_name_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2297 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_usn_change_journal.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6679 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_information_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_reparse_point_attribute.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10060 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_object_identifier_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entries.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    78655 2023-04-29 07:19:09.000000 libfsntfs-20230427/pyfsntfs/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16625 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_datetime.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_integer.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5521 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_security_descriptor_attribute.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9481 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entries.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_information_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95899 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22909 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10377 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_attribute_flags.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10659 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute_types.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10741 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10577 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_usn_change_journal.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    33964 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3199 2023-04-27 16:33:04.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_data_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9495 2023-04-27 16:31:03.000000 libfsntfs-20230427/pyfsntfs/pyfsntfs_data_streams.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-04-29 07:19:07.000000 libfsntfs-20230427/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31842 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-04-29 07:18:36.000000 libfsntfs-20230427/libcpath/libcpath_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30798 2023-04-27 16:31:05.000000 libfsntfs-20230427/manuals/libfsntfs.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      166 2016-02-02 07:37:21.000000 libfsntfs-20230427/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28810 2023-04-29 07:19:09.000000 libfsntfs-20230427/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2097 2023-04-27 16:31:05.000000 libfsntfs-20230427/manuals/fsntfsinfo.1
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/libfusn/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2327 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/fusn_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12280 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      817 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26484 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4234 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31827 2023-04-29 07:19:08.000000 libfsntfs-20230427/libfusn/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-04-29 07:18:47.000000 libfsntfs-20230427/libfusn/libfusn_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-14 03:51:49.000000 libfsntfs-20230427/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6467 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6357 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfcache/libfcache.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6873 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6511 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_information_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6095 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfsmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7848 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/fsntfsmount/fsntfsmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_node_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_directory_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6149 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_bitmap_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6059 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6352 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5324 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_name_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6158 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_buffer_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_path_hint/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6035 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compression_unit_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_name_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6083 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6306 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_entry_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_name_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6077 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6300 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compression_unit_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84253 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/libfsntfs.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_root_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6170 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_data_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_entry_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6496 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20944 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfsntfs/libfsntfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_reparse_point_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6089 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5786 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_object_identifier_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_standard_information_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5889 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute_list_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6176 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_system/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/pyfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10166 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/pyfsntfs/pyfsntfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_logged_utility_stream_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6143 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfusn/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfusn/libfusn.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_node/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_attribute_list_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_usn_change_journal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6238 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_txf_data_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_reparse_point_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_metadata_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6824 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29124 2023-04-29 07:19:09.000000 libfsntfs-20230427/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_fixup_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5892 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_directory_entries_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6169 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6502 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6411 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_sds_index_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_index/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6178 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5874 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_profiler/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_information_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfsinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7641 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/fsntfsinfo/fsntfsinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_extent/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6038 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_name_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_index_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6113 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_entry_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_name/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6032 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-04-27 16:31:37.000000 libfsntfs-20230427/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/msvscpp/fsntfs_test_data_run/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6128 2023-04-27 16:33:04.000000 libfsntfs-20230427/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50222 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45801 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34374 2023-04-29 07:19:09.000000 libfsntfs-20230427/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48185 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45844 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40792 2023-04-29 07:18:50.000000 libfsntfs-20230427/libhmac/libhmac_md5_context.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-04-27 16:31:37.000000 libfsntfs-20230427/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-04-29 07:19:07.000000 libfsntfs-20230427/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-27 16:30:55.000000 libfsntfs-20230427/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/ossfuzz/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3119 2023-04-27 16:31:02.000000 libfsntfs-20230427/ossfuzz/file_entry_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2025 2021-05-02 04:50:03.000000 libfsntfs-20230427/ossfuzz/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2023-04-27 16:31:02.000000 libfsntfs-20230427/ossfuzz/volume_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      977 2023-04-27 16:31:02.000000 libfsntfs-20230427/ossfuzz/ossfuzz_libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38215 2023-04-29 07:19:09.000000 libfsntfs-20230427/ossfuzz/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2430 2023-04-27 16:31:02.000000 libfsntfs-20230427/ossfuzz/mft_metadata_file_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-04-27 16:31:02.000000 libfsntfs-20230427/ossfuzz/ossfuzz_libbfio.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-04-29 07:19:09.000000 libfsntfs-20230427/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1999923 2023-04-29 07:19:06.000000 libfsntfs-20230427/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55366 2023-04-29 07:19:09.000000 libfsntfs-20230427/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-04-29 07:18:53.000000 libfsntfs-20230427/libuna/libuna_codepage_iso_8859_16.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3957 2023-04-27 16:30:55.000000 libfsntfs-20230427/libfsntfs.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44234 2023-04-29 07:19:08.000000 libfsntfs-20230427/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11939 2022-01-12 13:35:10.000000 libfsntfs-20230427/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/m4/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-09-05 06:42:38.000000 libfsntfs-20230427/m4/libuna.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2022-02-13 11:48:13.000000 libfsntfs-20230427/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-14 03:51:49.000000 libfsntfs-20230427/m4/gettext.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-18 13:59:08.000000 libfsntfs-20230427/m4/tests.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libfusn.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-14 03:51:49.000000 libfsntfs-20230427/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-04-29 07:19:00.000000 libfsntfs-20230427/m4/ltoptions.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2019-12-16 19:17:55.000000 libfsntfs-20230427/m4/libfwnt.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2020-09-21 04:08:13.000000 libfsntfs-20230427/m4/lib-ld.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-14 03:51:49.000000 libfsntfs-20230427/m4/lib-link.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2020-11-29 18:18:15.000000 libfsntfs-20230427/m4/libhmac.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-17 03:27:32.000000 libfsntfs-20230427/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-04-29 07:19:00.000000 libfsntfs-20230427/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-14 03:51:49.000000 libfsntfs-20230427/m4/nls.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libclocale.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-03-21 15:40:29.000000 libfsntfs-20230427/m4/libfdata.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-14 03:51:49.000000 libfsntfs-20230427/m4/host-cpu-c-abi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-04-29 07:19:01.000000 libfsntfs-20230427/m4/ltversion.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-02-06 02:34:47.000000 libfsntfs-20230427/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-14 03:51:50.000000 libfsntfs-20230427/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-04-29 07:19:01.000000 libfsntfs-20230427/m4/lt~obsolete.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libcfile.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    27306 2022-12-03 08:47:43.000000 libfsntfs-20230427/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-14 03:51:50.000000 libfsntfs-20230427/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2013-09-14 20:39:31.000000 libfsntfs-20230427/m4/pthread.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-12-13 07:44:48.000000 libfsntfs-20230427/m4/common.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libcerror.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2020-09-21 04:08:13.000000 libfsntfs-20230427/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-04-29 07:19:00.000000 libfsntfs-20230427/m4/ltsugar.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-02-06 02:34:47.000000 libfsntfs-20230427/m4/libfcache.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2019-05-09 05:43:09.000000 libfsntfs-20230427/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-14 03:51:49.000000 libfsntfs-20230427/m4/intlmacosx.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-08-18 07:16:18.000000 libfsntfs-20230427/m4/types.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2020-11-27 18:36:28.000000 libfsntfs-20230427/m4/libbfio.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-04-27 16:30:55.000000 libfsntfs-20230427/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31189 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-04-29 07:18:29.000000 libfsntfs-20230427/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31676 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-04-29 07:18:35.000000 libfsntfs-20230427/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-04-29 07:19:00.000000 libfsntfs-20230427/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-04-29 07:19:07.000000 libfsntfs-20230427/compile
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/pyfsntfs-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2954 2023-04-27 16:30:58.000000 libfsntfs-20230427/pyfsntfs-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77798 2023-04-29 07:19:09.000000 libfsntfs-20230427/pyfsntfs-python2/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-14 03:51:49.000000 libfsntfs-20230427/config.rpath
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-04-29 07:19:09.000000 libfsntfs-20230427/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:20.000000 libfsntfs-20230427/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-14 03:51:50.000000 libfsntfs-20230427/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-14 03:51:50.000000 libfsntfs-20230427/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2010-12-09 10:42:14.000000 libfsntfs-20230427/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-14 03:51:50.000000 libfsntfs-20230427/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2010-12-14 11:01:34.000000 libfsntfs-20230427/po/Makevars.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-09 12:44:04.000000 libfsntfs-20230427/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-14 03:51:50.000000 libfsntfs-20230427/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2010-12-09 10:42:14.000000 libfsntfs-20230427/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1811 2023-04-29 07:19:24.000000 libfsntfs-20230427/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-14 03:51:50.000000 libfsntfs-20230427/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-14 03:51:50.000000 libfsntfs-20230427/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2010-12-09 10:42:13.000000 libfsntfs-20230427/po/boldquot.sed
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:19.000000 libfsntfs-20230427/pyfsntfs-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2954 2023-04-27 16:30:58.000000 libfsntfs-20230427/pyfsntfs-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77798 2023-04-29 07:19:09.000000 libfsntfs-20230427/pyfsntfs-python3/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:18.000000 libfsntfs-20230427/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35029 2023-04-29 07:19:08.000000 libfsntfs-20230427/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2023-04-29 07:18:42.000000 libfsntfs-20230427/libfdata/libfdata_range.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34248 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-04-29 07:18:28.000000 libfsntfs-20230427/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2023-04-27 16:34:42.000000 libfsntfs-20230427/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-29 07:47:17.000000 libfsntfs-20230427/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32622 2023-04-29 07:19:08.000000 libfsntfs-20230427/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-04-29 07:18:38.000000 libfsntfs-20230427/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2794 2023-04-29 07:19:24.000000 libfsntfs-20230427/libfsntfs.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8666 2023-04-27 16:30:55.000000 libfsntfs-20230427/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      355 2023-04-29 07:47:21.722344 libfsntfs-20230427/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32273 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-06-06 19:50:43.000000 libfsntfs-20230606/libfcache/libfcache_date_time.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/common/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/config_msc.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/byte_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/common.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/system_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-06-06 18:54:53.000000 libfsntfs-20230606/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-06-06 19:51:24.000000 libfsntfs-20230606/common/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/types.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/config_winapi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19504 2023-06-06 19:51:24.000000 libfsntfs-20230606/common/config.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26844 2023-06-06 19:51:08.000000 libfsntfs-20230606/common/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/file_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18422 2023-06-06 19:51:07.000000 libfsntfs-20230606/common/config.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-06-06 18:55:01.000000 libfsntfs-20230606/common/wide_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-06-06 19:50:48.000000 libfsntfs-20230606/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-06-06 19:50:48.000000 libfsntfs-20230606/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31244 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-06-06 19:50:47.000000 libfsntfs-20230606/libfguid/libfguid_extern.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15806 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index_root_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14680 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_volume_information_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      989 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libfsntfs.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35342 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_security_descriptor_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4880 2023-06-06 18:56:13.000000 libfsntfs-20230606/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17795 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15392 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_security_descriptor_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15536 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7132 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_profiler.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41944 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_compressed_data_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    30411 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_cluster_block_stream.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36317 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    27561 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_file_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6049 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_path_hint.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6798 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_compressed_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24256 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_name.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    67794 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_index_entry_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100428 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_compressed_block_data_handle.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3436 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13832 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_txf_data_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   132840 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_data_stream.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29815 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23213 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_attribute_list_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libfdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_rwlock.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5750 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_tools_info_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_rwlock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14589 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index_entry_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8845 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_usn_change_journal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8643 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_extent.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15448 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46804 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9173 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index_node_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11496 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_fixup_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51596 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   110531 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_file_system.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_getopt.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    92729 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_cluster_block_vector.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3811 2023-06-06 18:56:13.000000 libfsntfs-20230606/tests/test_tools.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28465 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_standard_information_values.c
+-rwxrw-r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10623 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_compression_unit_data_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15740 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31281 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_volume_name_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12560 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_data_run.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14474 2023-06-06 18:56:13.000000 libfsntfs-20230606/tests/pyfsntfs_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10373 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_security_descriptor_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11116 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_volume_information_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26241 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_directory_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23687 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_reparse_point_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39431 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_reparse_point_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)   127782 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_compression.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/pyfsntfs_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63509 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2007 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10606 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   138313 2023-06-06 19:51:09.000000 libfsntfs-20230606/tests/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9580 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35036 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_directory_entries_tree.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libfcache.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35794 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft_attribute_list_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   259855 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7195 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_compression_unit_descriptor.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9191 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15072 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_volume_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59086 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft_entry.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3186 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/test_fsntfsinfo_bodyfile.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43120 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_file_name_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15477 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_logged_utility_stream_values.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     2248 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/test_fsntfsinfo.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21070 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft_entry_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14191 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_object_identifier_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    60997 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_cluster_block_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33492 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft_metadata_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13974 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_bitmap_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19485 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_cluster_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35027 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_volume_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9333 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_sds_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12477 2023-06-06 18:55:58.000000 libfsntfs-20230606/tests/fsntfs_test_mft_attribute_list.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    92276 2023-06-06 18:55:06.000000 libfsntfs-20230606/tests/fsntfs_test_compressed_block_vector.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31800 2023-06-06 19:51:08.000000 libfsntfs-20230606/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-06-06 19:50:35.000000 libfsntfs-20230606/libclocale/libclocale_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-06-06 19:51:08.000000 libfsntfs-20230606/missing
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3775 2022-04-25 19:40:39.000000 libfsntfs-20230606/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56136 2023-06-06 19:51:04.000000 libfsntfs-20230606/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35306 2023-06-06 19:51:08.000000 libfsntfs-20230606/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-06-06 19:50:30.000000 libfsntfs-20230606/libbfio/libbfio_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-06-06 18:54:53.000000 libfsntfs-20230606/COPYING
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      684 2023-06-06 18:54:53.000000 libfsntfs-20230606/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/include/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      509 2023-06-06 18:54:53.000000 libfsntfs-20230606/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64032 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/include/libfsntfs/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4079 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs/definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-06-06 19:51:24.000000 libfsntfs-20230606/include/libfsntfs/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs/features.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5224 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2023-06-06 19:51:24.000000 libfsntfs-20230606/include/libfsntfs/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2023-06-06 19:51:24.000000 libfsntfs-20230606/include/libfsntfs/definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs/codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-06-06 18:55:01.000000 libfsntfs-20230606/include/libfsntfs/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29864 2023-06-06 19:51:08.000000 libfsntfs-20230606/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64032 2023-06-06 19:51:24.000000 libfsntfs-20230606/include/libfsntfs.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:24.000000 libfsntfs-20230606/fsntfstools/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3074 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   220309 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/info_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1245 2023-06-06 18:55:04.000000 libfsntfs-20230606/fsntfstools/digest_hash.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31066 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/mount_file_system.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2023-06-06 18:55:04.000000 libfsntfs-20230606/fsntfstools/fsntfstools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28494 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/mount_fuse.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libcpath.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5420 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/mount_dokan.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24694 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/mount_file_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15540 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/fsntfsmount.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2568 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/mount_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2724 2020-11-29 18:25:27.000000 libfsntfs-20230606/fsntfstools/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libhmac.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16556 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/mount_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfusn.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11770 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/fsntfsinfo.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 18:55:04.000000 libfsntfs-20230606/fsntfstools/fsntfstools_getopt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfwnt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37237 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/mount_file_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_i18n.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_output.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9033 2023-06-06 18:56:13.000000 libfsntfs-20230606/fsntfstools/info_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3298 2023-06-06 18:55:04.000000 libfsntfs-20230606/fsntfstools/digest_hash.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      989 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libfsntfs.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5731 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36644 2023-06-06 19:51:08.000000 libfsntfs-20230606/fsntfstools/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4584 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_output.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2023-06-06 18:55:05.000000 libfsntfs-20230606/fsntfstools/fsntfstools_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-06-06 19:51:08.000000 libfsntfs-20230606/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-06-06 19:51:08.000000 libfsntfs-20230606/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      122 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2023-06-06 19:51:24.000000 libfsntfs-20230606/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/libfsntfs-python3.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/libfsntfs.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2023-06-06 18:55:06.000000 libfsntfs-20230606/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/libfsntfs-tools.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/source/format
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/libfsntfs-dev.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      778 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/rules
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2240 2023-06-06 18:54:53.000000 libfsntfs-20230606/dpkg/control
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94428 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2062 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2829 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_data_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23416 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9488 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_txf_data_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8562 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_root_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8711 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17036 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_bitmap_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libfwnt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2102 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_profiler.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1909 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_secure.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_object_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compression.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8832 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4582 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8311 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4610 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_data.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3924 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_mft_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8168 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1286 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_fixup_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2486 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_reparse_point.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_data.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5402 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19845 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_name_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1984 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_vector.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7382 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2289 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_txf_data_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    28629 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_data_stream.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2503 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_standard_information.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2005 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_io_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    32475 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_notify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_name.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23871 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_data_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13362 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_node.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15709 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6367 2022-01-13 18:43:42.000000 libfsntfs-20230606/libfsntfs/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12727 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_vector.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2392 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4404 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_data_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    29282 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    77724 2023-06-06 19:17:16.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3756 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8183 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_profiler.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12897 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_value.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16323 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_support.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7850 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_buffer_data_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3159 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index_value.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_sds_index_value.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22935 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_name.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libfcache.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_volume_information.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17017 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_extent.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4217 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7978 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index_value.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3360 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_directory_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12001 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    25038 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_directory_entries_tree.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20903 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_data_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2786 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_data_run.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_descriptor.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15319 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19315 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_debug.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2253 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libfdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19566 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19693 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    39152 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2349 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_path_hint.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    63403 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_directory_entries_tree.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3381 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_data_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4428 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_metadata_file.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_vector.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_node_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12385 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_vector.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8597 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_path_hint.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7029 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_fixup_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_error.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2815 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9737 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_data_run.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2373 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9103 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_descriptor.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_index.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22736 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2201 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_bitmap_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3207 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_name_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3248 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_volume_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3475 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20087 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4131 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_extent.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3833 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7027 2023-06-06 19:51:24.000000 libfsntfs-20230606/libfsntfs/libfsntfs_definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_buffer_data_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16683 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    25638 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_stream.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libcthreads.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    54282 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_metadata_file.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17815 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2427 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_mft_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_debug.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2448 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_node.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15170 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_directory_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9290 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12076 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_data_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4008 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_system.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2574 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_support.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3227 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libfdatetime.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55595 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfsntfs/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2318 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_file_name.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18720 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_usn_change_journal.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    60465 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    28966 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_name_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7849 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_logged_utility_stream_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_logged_utility_stream_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6301 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_txf_data.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3874 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6767 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_node_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_extern.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_root_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13040 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_vector.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2807 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4755 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_name_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1107 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs.rc.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21101 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_logged_utility_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20304 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    48386 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_system.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)   168965 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_file_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1621 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2144 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_value.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2604 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6361 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5429 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_io_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_vector.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libcdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11491 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_sds_index_value.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/fsntfs_mft_attribute_list.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13566 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1105 2023-06-06 19:51:24.000000 libfsntfs-20230606/libfsntfs/libfsntfs.rc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2420 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_data_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4088 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_compression.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_index_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-06-06 18:55:03.000000 libfsntfs-20230606/libfsntfs/libfsntfs_usn_change_journal.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34415 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-06-06 19:50:46.000000 libfsntfs-20230606/libfdatetime/libfdatetime_filetime.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32564 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-06-06 19:50:34.000000 libfsntfs-20230606/libcfile/libcfile_notify.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35469 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_access_control_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2023-06-06 19:50:51.000000 libfsntfs-20230606/libfwnt/libfwnt_debug.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34654 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-06-06 19:50:42.000000 libfsntfs-20230606/libcthreads/libcthreads_queue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       93 2023-06-06 18:55:01.000000 libfsntfs-20230606/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      757 2023-06-06 18:54:53.000000 libfsntfs-20230606/libfsntfs.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:24.000000 libfsntfs-20230606/pyfsntfs/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_data_streams.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3169 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_name_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23172 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23389 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_attribute_flags.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11552 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2911 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_guid.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_object_identifier_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2477 2018-08-18 07:35:36.000000 libfsntfs-20230606/pyfsntfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9341 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_attributes.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3400 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_standard_information_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9524 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_reparse_point_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_python.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27912 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_data_stream.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_object_io_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_datetime.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_security_descriptor_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1361 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8966 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9649 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36819 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1180 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_guid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_attributes.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5347 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_name_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2918 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_file_entries.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23602 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_standard_information_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_name_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2297 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_usn_change_journal.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6679 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_information_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_reparse_point_attribute.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10060 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_object_identifier_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entries.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    78655 2023-06-06 19:51:09.000000 libfsntfs-20230606/pyfsntfs/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16625 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_datetime.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_integer.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5521 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_security_descriptor_attribute.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9481 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entries.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_information_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95899 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22909 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10377 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_attribute_flags.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10659 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute_types.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10741 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10577 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_usn_change_journal.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    33964 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3199 2023-06-06 18:56:13.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_data_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9495 2023-06-06 18:55:04.000000 libfsntfs-20230606/pyfsntfs/pyfsntfs_data_streams.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-06-06 19:51:08.000000 libfsntfs-20230606/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31842 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-06-06 19:50:39.000000 libfsntfs-20230606/libcpath/libcpath_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:24.000000 libfsntfs-20230606/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30798 2023-06-06 18:55:06.000000 libfsntfs-20230606/manuals/libfsntfs.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      166 2016-02-02 07:37:21.000000 libfsntfs-20230606/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28810 2023-06-06 19:51:09.000000 libfsntfs-20230606/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2097 2023-06-06 18:55:06.000000 libfsntfs-20230606/manuals/fsntfsinfo.1
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libfusn/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2327 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/fusn_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12280 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      817 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26484 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4234 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31827 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfusn/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-06-06 19:50:49.000000 libfsntfs-20230606/libfusn/libfusn_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-14 03:51:49.000000 libfsntfs-20230606/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6467 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6357 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfcache/libfcache.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6873 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6511 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_information_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6095 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfsmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7848 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/fsntfsmount/fsntfsmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_node_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_directory_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6149 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_bitmap_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6059 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6352 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5324 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_name_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6158 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_buffer_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_path_hint/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6035 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compression_unit_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_name_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6083 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6306 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_entry_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_name_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6077 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6300 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compression_unit_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84253 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/libfsntfs.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_root_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6170 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_data_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_entry_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6496 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20944 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfsntfs/libfsntfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_reparse_point_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6089 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5786 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_object_identifier_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_standard_information_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5889 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute_list_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6176 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_system/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/pyfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10166 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/pyfsntfs/pyfsntfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_logged_utility_stream_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6143 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfusn/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfusn/libfusn.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_node/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_attribute_list_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_usn_change_journal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6238 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_txf_data_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_reparse_point_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_metadata_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6824 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29124 2023-06-06 19:51:09.000000 libfsntfs-20230606/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_fixup_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5892 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_directory_entries_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6169 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6502 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6411 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_sds_index_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_index/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6178 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5874 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_profiler/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_information_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfsinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7641 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/fsntfsinfo/fsntfsinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_extent/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6038 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_name_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_index_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6113 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_entry_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_name/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6032 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-06-06 18:55:37.000000 libfsntfs-20230606/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/msvscpp/fsntfs_test_data_run/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6128 2023-06-06 18:55:58.000000 libfsntfs-20230606/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50222 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45801 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34374 2023-06-06 19:51:09.000000 libfsntfs-20230606/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48185 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45844 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40792 2023-06-06 19:50:52.000000 libfsntfs-20230606/libhmac/libhmac_md5_context.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-06-06 18:55:37.000000 libfsntfs-20230606/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-06-06 19:51:08.000000 libfsntfs-20230606/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-06 18:54:53.000000 libfsntfs-20230606/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:25.000000 libfsntfs-20230606/ossfuzz/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3119 2023-06-06 18:55:03.000000 libfsntfs-20230606/ossfuzz/file_entry_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2025 2021-05-02 04:50:03.000000 libfsntfs-20230606/ossfuzz/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2023-06-06 18:55:03.000000 libfsntfs-20230606/ossfuzz/volume_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      977 2023-06-06 18:55:03.000000 libfsntfs-20230606/ossfuzz/ossfuzz_libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38215 2023-06-06 19:51:09.000000 libfsntfs-20230606/ossfuzz/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2430 2023-06-06 18:55:03.000000 libfsntfs-20230606/ossfuzz/mft_metadata_file_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-06-06 18:55:03.000000 libfsntfs-20230606/ossfuzz/ossfuzz_libbfio.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-06-06 19:51:09.000000 libfsntfs-20230606/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1999923 2023-06-06 19:51:06.000000 libfsntfs-20230606/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55366 2023-06-06 19:51:09.000000 libfsntfs-20230606/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-06-06 19:50:55.000000 libfsntfs-20230606/libuna/libuna_codepage_iso_8859_16.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3957 2023-06-06 18:54:53.000000 libfsntfs-20230606/libfsntfs.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44234 2023-06-06 19:51:08.000000 libfsntfs-20230606/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11939 2022-01-12 13:35:10.000000 libfsntfs-20230606/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/m4/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-09-05 06:42:38.000000 libfsntfs-20230606/m4/libuna.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2022-02-13 11:48:13.000000 libfsntfs-20230606/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-14 03:51:49.000000 libfsntfs-20230606/m4/gettext.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-18 13:59:08.000000 libfsntfs-20230606/m4/tests.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libfusn.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-14 03:51:49.000000 libfsntfs-20230606/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-06-06 19:51:00.000000 libfsntfs-20230606/m4/ltoptions.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2019-12-16 19:17:55.000000 libfsntfs-20230606/m4/libfwnt.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2020-09-21 04:08:13.000000 libfsntfs-20230606/m4/lib-ld.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-14 03:51:49.000000 libfsntfs-20230606/m4/lib-link.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2020-11-29 18:18:15.000000 libfsntfs-20230606/m4/libhmac.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-17 03:27:32.000000 libfsntfs-20230606/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-06-06 19:51:00.000000 libfsntfs-20230606/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-14 03:51:49.000000 libfsntfs-20230606/m4/nls.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libclocale.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-03-21 15:40:29.000000 libfsntfs-20230606/m4/libfdata.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-14 03:51:49.000000 libfsntfs-20230606/m4/host-cpu-c-abi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-06-06 19:51:01.000000 libfsntfs-20230606/m4/ltversion.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-02-06 02:34:47.000000 libfsntfs-20230606/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-14 03:51:50.000000 libfsntfs-20230606/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-06-06 19:51:01.000000 libfsntfs-20230606/m4/lt~obsolete.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libcfile.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    27306 2022-12-03 08:47:43.000000 libfsntfs-20230606/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-14 03:51:50.000000 libfsntfs-20230606/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2013-09-14 20:39:31.000000 libfsntfs-20230606/m4/pthread.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-12-13 07:44:48.000000 libfsntfs-20230606/m4/common.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libcerror.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2020-09-21 04:08:13.000000 libfsntfs-20230606/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-06-06 19:51:01.000000 libfsntfs-20230606/m4/ltsugar.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-02-06 02:34:47.000000 libfsntfs-20230606/m4/libfcache.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2019-05-09 05:43:09.000000 libfsntfs-20230606/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-14 03:51:49.000000 libfsntfs-20230606/m4/intlmacosx.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-08-18 07:16:18.000000 libfsntfs-20230606/m4/types.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2020-11-27 18:36:28.000000 libfsntfs-20230606/m4/libbfio.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-06-06 18:54:53.000000 libfsntfs-20230606/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:21.000000 libfsntfs-20230606/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-06-06 19:50:33.000000 libfsntfs-20230606/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31189 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-06-06 19:50:32.000000 libfsntfs-20230606/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31676 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-06-06 19:50:37.000000 libfsntfs-20230606/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-06-06 19:51:00.000000 libfsntfs-20230606/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-06-06 19:51:08.000000 libfsntfs-20230606/compile
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:24.000000 libfsntfs-20230606/pyfsntfs-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2954 2023-06-06 18:54:59.000000 libfsntfs-20230606/pyfsntfs-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77798 2023-06-06 19:51:09.000000 libfsntfs-20230606/pyfsntfs-python2/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-14 03:51:49.000000 libfsntfs-20230606/config.rpath
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-06-06 19:51:09.000000 libfsntfs-20230606/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:24.000000 libfsntfs-20230606/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-14 03:51:50.000000 libfsntfs-20230606/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-14 03:51:50.000000 libfsntfs-20230606/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2010-12-09 10:42:14.000000 libfsntfs-20230606/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-14 03:51:50.000000 libfsntfs-20230606/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2010-12-14 11:01:34.000000 libfsntfs-20230606/po/Makevars.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-09 12:44:04.000000 libfsntfs-20230606/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-14 03:51:50.000000 libfsntfs-20230606/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2010-12-09 10:42:14.000000 libfsntfs-20230606/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1811 2023-06-06 19:51:24.000000 libfsntfs-20230606/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-14 03:51:50.000000 libfsntfs-20230606/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-14 03:51:50.000000 libfsntfs-20230606/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2010-12-09 10:42:13.000000 libfsntfs-20230606/po/boldquot.sed
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:24.000000 libfsntfs-20230606/pyfsntfs-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2954 2023-06-06 18:54:59.000000 libfsntfs-20230606/pyfsntfs-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77798 2023-06-06 19:51:09.000000 libfsntfs-20230606/pyfsntfs-python3/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:23.000000 libfsntfs-20230606/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35029 2023-06-06 19:51:08.000000 libfsntfs-20230606/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2023-06-06 19:50:45.000000 libfsntfs-20230606/libfdata/libfdata_range.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34248 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-06-06 19:50:31.000000 libfsntfs-20230606/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2023-06-06 18:56:13.000000 libfsntfs-20230606/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-06-07 04:06:22.000000 libfsntfs-20230606/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32622 2023-06-06 19:51:08.000000 libfsntfs-20230606/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-06-06 19:50:40.000000 libfsntfs-20230606/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2794 2023-06-06 19:51:24.000000 libfsntfs-20230606/libfsntfs.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8666 2023-06-06 18:54:53.000000 libfsntfs-20230606/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      355 2023-06-07 04:06:26.469284 libfsntfs-20230606/PKG-INFO
```

### Comparing `libfsntfs-20230427/libfcache/libfcache_extern.h` & `libfsntfs-20230606/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_types.h` & `libfsntfs-20230606/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_cache.h` & `libfsntfs-20230606/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_support.h` & `libfsntfs-20230606/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_support.c` & `libfsntfs-20230606/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/Makefile.am` & `libfsntfs-20230606/libfcache/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_libcdata.h` & `libfsntfs-20230606/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_unused.h` & `libfsntfs-20230606/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_libcerror.h` & `libfsntfs-20230606/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_definitions.h` & `libfsntfs-20230606/libfcache/libfcache_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_cache_value.h` & `libfsntfs-20230606/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_cache_value.c` & `libfsntfs-20230606/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/Makefile.in` & `libfsntfs-20230606/libfcache/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_error.c` & `libfsntfs-20230606/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_date_time.c` & `libfsntfs-20230606/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_cache.c` & `libfsntfs-20230606/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_error.h` & `libfsntfs-20230606/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfcache/libfcache_date_time.h` & `libfsntfs-20230606/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/config_msc.h` & `libfsntfs-20230606/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/byte_stream.h` & `libfsntfs-20230606/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/common.h` & `libfsntfs-20230606/common/common.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/system_string.h` & `libfsntfs-20230606/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/types.h` & `libfsntfs-20230606/common/types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/types.h.in` & `libfsntfs-20230606/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/config_winapi.h` & `libfsntfs-20230606/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/memory.h` & `libfsntfs-20230606/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/config.h` & `libfsntfs-20230606/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -610,24 +610,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfsntfs"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfsntfs 20230427"
+#define PACKAGE_STRING "libfsntfs 20230606"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfsntfs"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20230427"
+#define PACKAGE_VERSION "20230606"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -648,15 +648,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20230427"
+#define VERSION "20230606"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfsntfs-20230427/common/narrow_string.h` & `libfsntfs-20230606/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/Makefile.in` & `libfsntfs-20230606/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/file_stream.h` & `libfsntfs-20230606/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/config_borlandc.h` & `libfsntfs-20230606/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/config.h.in` & `libfsntfs-20230606/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/common/wide_string.h` & `libfsntfs-20230606/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_identifier.c` & `libfsntfs-20230606/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_support.c` & `libfsntfs-20230606/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/Makefile.am` & `libfsntfs-20230606/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_support.h` & `libfsntfs-20230606/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_definitions.h` & `libfsntfs-20230606/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_identifier.h` & `libfsntfs-20230606/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_unused.h` & `libfsntfs-20230606/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_error.h` & `libfsntfs-20230606/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_libcerror.h` & `libfsntfs-20230606/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/Makefile.in` & `libfsntfs-20230606/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_error.c` & `libfsntfs-20230606/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_types.h` & `libfsntfs-20230606/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfguid/libfguid_extern.h` & `libfsntfs-20230606/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_root_header.c` & `libfsntfs-20230606/tests/fsntfs_test_index_root_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_unused.h` & `libfsntfs-20230606/tests/fsntfs_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_volume_information_values.c` & `libfsntfs-20230606/tests/fsntfs_test_volume_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libfsntfs.h` & `libfsntfs-20230606/tests/fsntfs_test_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_tools_signal.c` & `libfsntfs-20230606/tests/fsntfs_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_security_descriptor_values.c` & `libfsntfs-20230606/tests/fsntfs_test_security_descriptor_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_library.sh` & `libfsntfs-20230606/tests/test_library.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_buffer_data_handle.c` & `libfsntfs-20230606/tests/fsntfs_test_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_security_descriptor_index_value.c` & `libfsntfs-20230606/tests/fsntfs_test_security_descriptor_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_node.c` & `libfsntfs-20230606/tests/fsntfs_test_index_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_profiler.c` & `libfsntfs-20230606/tests/fsntfs_test_profiler.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_error.c` & `libfsntfs-20230606/tests/fsntfs_test_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compressed_data_handle.c` & `libfsntfs-20230606/tests/fsntfs_test_compressed_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_cluster_block_stream.c` & `libfsntfs-20230606/tests/fsntfs_test_cluster_block_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libcerror.h` & `libfsntfs-20230606/tests/fsntfs_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_memory.c` & `libfsntfs-20230606/tests/fsntfs_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_entry.c` & `libfsntfs-20230606/tests/fsntfs_test_index_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_file_name_attribute.c` & `libfsntfs-20230606/tests/fsntfs_test_file_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_path_hint.c` & `libfsntfs-20230606/tests/fsntfs_test_path_hint.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compressed_block.c` & `libfsntfs-20230606/tests/fsntfs_test_compressed_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_name.c` & `libfsntfs-20230606/tests/fsntfs_test_name.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_entry_vector.c` & `libfsntfs-20230606/tests/fsntfs_test_index_entry_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compressed_block_data_handle.c` & `libfsntfs-20230606/tests/fsntfs_test_compressed_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_python_module.sh` & `libfsntfs-20230606/tests/test_python_module.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_txf_data_values.c` & `libfsntfs-20230606/tests/fsntfs_test_txf_data_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_data_stream.c` & `libfsntfs-20230606/tests/fsntfs_test_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_tools_output.c` & `libfsntfs-20230606/tests/fsntfs_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/Makefile.am` & `libfsntfs-20230606/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_attribute_list_entry.c` & `libfsntfs-20230606/tests/fsntfs_test_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libfdata.h` & `libfsntfs-20230606/tests/fsntfs_test_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_rwlock.h` & `libfsntfs-20230606/tests/fsntfs_test_rwlock.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_tools_info_handle.c` & `libfsntfs-20230606/tests/fsntfs_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_memory.h` & `libfsntfs-20230606/tests/fsntfs_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_rwlock.c` & `libfsntfs-20230606/tests/fsntfs_test_rwlock.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_entry_header.c` & `libfsntfs-20230606/tests/fsntfs_test_index_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_usn_change_journal.c` & `libfsntfs-20230606/tests/fsntfs_test_usn_change_journal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_extent.c` & `libfsntfs-20230606/tests/fsntfs_test_extent.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_support.c` & `libfsntfs-20230606/tests/fsntfs_test_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_attribute.c` & `libfsntfs-20230606/tests/fsntfs_test_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_node_header.c` & `libfsntfs-20230606/tests/fsntfs_test_index_node_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_fixup_values.c` & `libfsntfs-20230606/tests/fsntfs_test_fixup_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft_attribute.c` & `libfsntfs-20230606/tests/fsntfs_test_mft_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_file_system.c` & `libfsntfs-20230606/tests/fsntfs_test_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_getopt.c` & `libfsntfs-20230606/tests/fsntfs_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_cluster_block_vector.c` & `libfsntfs-20230606/tests/fsntfs_test_cluster_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_tools.sh` & `libfsntfs-20230606/tests/test_tools.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_macros.h` & `libfsntfs-20230606/tests/fsntfs_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_standard_information_values.c` & `libfsntfs-20230606/tests/fsntfs_test_standard_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_manpage.sh` & `libfsntfs-20230606/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compression_unit_data_handle.c` & `libfsntfs-20230606/tests/fsntfs_test_compression_unit_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_functions.c` & `libfsntfs-20230606/tests/fsntfs_test_functions.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_volume_name_values.c` & `libfsntfs-20230606/tests/fsntfs_test_volume_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_data_run.c` & `libfsntfs-20230606/tests/fsntfs_test_data_run.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/pyfsntfs_test_volume.py` & `libfsntfs-20230606/tests/pyfsntfs_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_security_descriptor_index.c` & `libfsntfs-20230606/tests/fsntfs_test_security_descriptor_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_runner.sh` & `libfsntfs-20230606/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_volume_information_attribute.c` & `libfsntfs-20230606/tests/fsntfs_test_volume_information_attribute.c`

 * *Files 1% similar despite different names*

```diff
@@ -452,14 +452,31 @@
 	 "attribute",
 	 attribute );
 
 	FSNTFS_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
+	result = libfsntfs_mft_attribute_free(
+	          &mft_attribute,
+	          &error );
+
+	FSNTFS_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FSNTFS_TEST_ASSERT_IS_NULL(
+	 "attribute",
+	 attribute );
+
+	FSNTFS_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
 	result = libfsntfs_io_handle_free(
 	          &io_handle,
 	          &error );
 
 	FSNTFS_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
```

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libcdata.h` & `libfsntfs-20230606/tests/fsntfs_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_directory_entry.c` & `libfsntfs-20230606/tests/fsntfs_test_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libclocale.h` & `libfsntfs-20230606/tests/fsntfs_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_reparse_point_attribute.c` & `libfsntfs-20230606/tests/fsntfs_test_reparse_point_attribute.c`

 * *Files 2% similar despite different names*

```diff
@@ -1085,14 +1085,31 @@
 	 "attribute",
 	 attribute );
 
 	FSNTFS_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
+	result = libfsntfs_mft_attribute_free(
+	          &mft_attribute,
+	          &error );
+
+	FSNTFS_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FSNTFS_TEST_ASSERT_IS_NULL(
+	 "attribute",
+	 attribute );
+
+	FSNTFS_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
 	result = libfsntfs_io_handle_free(
 	          &io_handle,
 	          &error );
 
 	FSNTFS_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
```

### Comparing `libfsntfs-20230427/tests/fsntfs_test_reparse_point_values.c` & `libfsntfs-20230606/tests/fsntfs_test_reparse_point_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compression.c` & `libfsntfs-20230606/tests/fsntfs_test_compression.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/pyfsntfs_test_support.py` & `libfsntfs-20230606/tests/pyfsntfs_test_support.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_volume.c` & `libfsntfs-20230606/tests/fsntfs_test_volume.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_functions.h` & `libfsntfs-20230606/tests/fsntfs_test_functions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft.c` & `libfsntfs-20230606/tests/fsntfs_test_mft.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/Makefile.in` & `libfsntfs-20230606/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libbfio.h` & `libfsntfs-20230606/tests/fsntfs_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libuna.h` & `libfsntfs-20230606/tests/fsntfs_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index.c` & `libfsntfs-20230606/tests/fsntfs_test_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_directory_entries_tree.c` & `libfsntfs-20230606/tests/fsntfs_test_directory_entries_tree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libfcache.h` & `libfsntfs-20230606/tests/fsntfs_test_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_libcnotify.h` & `libfsntfs-20230606/tests/fsntfs_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft_attribute_list_entry.c` & `libfsntfs-20230606/tests/fsntfs_test_mft_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_file_entry.c` & `libfsntfs-20230606/tests/fsntfs_test_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compression_unit_descriptor.c` & `libfsntfs-20230606/tests/fsntfs_test_compression_unit_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_notify.c` & `libfsntfs-20230606/tests/fsntfs_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_index_value.c` & `libfsntfs-20230606/tests/fsntfs_test_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_volume_name_attribute.c` & `libfsntfs-20230606/tests/fsntfs_test_volume_name_attribute.c`

 * *Files 0% similar despite different names*

```diff
@@ -676,14 +676,31 @@
 	 "attribute",
 	 attribute );
 
 	FSNTFS_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
+	result = libfsntfs_mft_attribute_free(
+	          &mft_attribute,
+	          &error );
+
+	FSNTFS_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FSNTFS_TEST_ASSERT_IS_NULL(
+	 "attribute",
+	 attribute );
+
+	FSNTFS_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
 	result = libfsntfs_io_handle_free(
 	          &io_handle,
 	          &error );
 
 	FSNTFS_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
```

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft_entry.c` & `libfsntfs-20230606/tests/fsntfs_test_mft_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_fsntfsinfo_bodyfile.sh` & `libfsntfs-20230606/tests/test_fsntfsinfo_bodyfile.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_file_name_values.c` & `libfsntfs-20230606/tests/fsntfs_test_file_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_logged_utility_stream_values.c` & `libfsntfs-20230606/tests/fsntfs_test_logged_utility_stream_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/test_fsntfsinfo.sh` & `libfsntfs-20230606/tests/test_fsntfsinfo.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_io_handle.c` & `libfsntfs-20230606/tests/fsntfs_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft_entry_header.c` & `libfsntfs-20230606/tests/fsntfs_test_mft_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_object_identifier_values.c` & `libfsntfs-20230606/tests/fsntfs_test_object_identifier_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_cluster_block_data.c` & `libfsntfs-20230606/tests/fsntfs_test_cluster_block_data.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft_metadata_file.c` & `libfsntfs-20230606/tests/fsntfs_test_mft_metadata_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_bitmap_values.c` & `libfsntfs-20230606/tests/fsntfs_test_bitmap_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_cluster_block.c` & `libfsntfs-20230606/tests/fsntfs_test_cluster_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_volume_header.c` & `libfsntfs-20230606/tests/fsntfs_test_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_getopt.h` & `libfsntfs-20230606/tests/fsntfs_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_sds_index_value.c` & `libfsntfs-20230606/tests/fsntfs_test_sds_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_mft_attribute_list.c` & `libfsntfs-20230606/tests/fsntfs_test_mft_attribute_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/tests/fsntfs_test_compressed_block_vector.c` & `libfsntfs-20230606/tests/fsntfs_test_compressed_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_wide_string.h` & `libfsntfs-20230606/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_support.c` & `libfsntfs-20230606/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_locale.h` & `libfsntfs-20230606/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/Makefile.am` & `libfsntfs-20230606/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_locale.c` & `libfsntfs-20230606/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_extern.h` & `libfsntfs-20230606/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_unused.h` & `libfsntfs-20230606/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_support.h` & `libfsntfs-20230606/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_definitions.h` & `libfsntfs-20230606/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_codepage.h` & `libfsntfs-20230606/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_codepage.c` & `libfsntfs-20230606/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/Makefile.in` & `libfsntfs-20230606/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_wide_string.c` & `libfsntfs-20230606/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libclocale/libclocale_libcerror.h` & `libfsntfs-20230606/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/missing` & `libfsntfs-20230606/missing`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/Makefile.am` & `libfsntfs-20230606/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/aclocal.m4` & `libfsntfs-20230606/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_handle.h` & `libfsntfs-20230606/libbfio/libbfio_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libcerror.h` & `libfsntfs-20230606/libbfio/libbfio_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_handle.c` & `libfsntfs-20230606/libbfio/libbfio_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libuna.h` & `libfsntfs-20230606/libbfio/libbfio_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_definitions.h` & `libfsntfs-20230606/libbfio/libbfio_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libclocale.h` & `libfsntfs-20230606/libbfio/libbfio_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_codepage.h` & `libfsntfs-20230606/libbfio/libbfio_codepage.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libcdata.h` & `libfsntfs-20230606/libbfio/libbfio_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_extern.h` & `libfsntfs-20230606/libbfio/libbfio_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_range.c` & `libfsntfs-20230606/libbfio/libbfio_file_range.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_range_io_handle.c` & `libfsntfs-20230606/libbfio/libbfio_file_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/Makefile.am` & `libfsntfs-20230606/libbfio/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_pool.c` & `libfsntfs-20230606/libbfio/libbfio_file_pool.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file.c` & `libfsntfs-20230606/libbfio/libbfio_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_pool.h` & `libfsntfs-20230606/libbfio/libbfio_pool.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_range.h` & `libfsntfs-20230606/libbfio/libbfio_file_range.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_system_string.h` & `libfsntfs-20230606/libbfio/libbfio_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_io_handle.h` & `libfsntfs-20230606/libbfio/libbfio_file_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_memory_range_io_handle.c` & `libfsntfs-20230606/libbfio/libbfio_memory_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file.h` & `libfsntfs-20230606/libbfio/libbfio_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_support.c` & `libfsntfs-20230606/libbfio/libbfio_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_pool.h` & `libfsntfs-20230606/libbfio/libbfio_file_pool.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_memory_range_io_handle.h` & `libfsntfs-20230606/libbfio/libbfio_memory_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_error.h` & `libfsntfs-20230606/libbfio/libbfio_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libcthreads.h` & `libfsntfs-20230606/libbfio/libbfio_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_system_string.c` & `libfsntfs-20230606/libbfio/libbfio_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_memory_range.h` & `libfsntfs-20230606/libbfio/libbfio_memory_range.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_range_io_handle.h` & `libfsntfs-20230606/libbfio/libbfio_file_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_memory_range.c` & `libfsntfs-20230606/libbfio/libbfio_memory_range.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/Makefile.in` & `libfsntfs-20230606/libbfio/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_pool.c` & `libfsntfs-20230606/libbfio/libbfio_pool.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_unused.h` & `libfsntfs-20230606/libbfio/libbfio_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libcpath.h` & `libfsntfs-20230606/libbfio/libbfio_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_libcfile.h` & `libfsntfs-20230606/libbfio/libbfio_libcfile.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_support.h` & `libfsntfs-20230606/libbfio/libbfio_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_file_io_handle.c` & `libfsntfs-20230606/libbfio/libbfio_file_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_error.c` & `libfsntfs-20230606/libbfio/libbfio_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libbfio/libbfio_types.h` & `libfsntfs-20230606/libbfio/libbfio_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/COPYING` & `libfsntfs-20230606/COPYING`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/README` & `libfsntfs-20230606/README`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs.h.in` & `libfsntfs-20230606/include/libfsntfs.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/definitions.h.in` & `libfsntfs-20230606/include/libfsntfs/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/extern.h` & `libfsntfs-20230606/include/libfsntfs/extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/types.h` & `libfsntfs-20230606/include/libfsntfs/types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/features.h.in` & `libfsntfs-20230606/include/libfsntfs/features.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/types.h.in` & `libfsntfs-20230606/include/libfsntfs/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/features.h` & `libfsntfs-20230606/include/libfsntfs/features.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/definitions.h` & `libfsntfs-20230606/include/libfsntfs/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFSNTFS_DEFINITIONS_H )
 #define _LIBFSNTFS_DEFINITIONS_H
 
 #include <libfsntfs/types.h>
 
-#define LIBFSNTFS_VERSION					20230427
+#define LIBFSNTFS_VERSION					20230606
 
 /* The version string
  */
-#define LIBFSNTFS_VERSION_STRING				"20230427"
+#define LIBFSNTFS_VERSION_STRING				"20230606"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSNTFS_ACCESS_FLAGS
```

### Comparing `libfsntfs-20230427/include/libfsntfs/codepage.h` & `libfsntfs-20230606/include/libfsntfs/codepage.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs/error.h` & `libfsntfs-20230606/include/libfsntfs/error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/Makefile.in` & `libfsntfs-20230606/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/include/libfsntfs.h` & `libfsntfs-20230606/include/libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_file_system.h` & `libfsntfs-20230606/fsntfstools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/info_handle.c` & `libfsntfs-20230606/fsntfstools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/digest_hash.h` & `libfsntfs-20230606/fsntfstools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_signal.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_signal.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_file_system.c` & `libfsntfs-20230606/fsntfstools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libcerror.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_getopt.c` & `libfsntfs-20230606/fsntfstools/fsntfstools_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_fuse.c` & `libfsntfs-20230606/fsntfstools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libcpath.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_dokan.h` & `libfsntfs-20230606/fsntfstools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libuna.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfdatetime.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_file_entry.c` & `libfsntfs-20230606/fsntfstools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libclocale.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfcache.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_fuse.h` & `libfsntfs-20230606/fsntfstools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfsmount.c` & `libfsntfs-20230606/fsntfstools/fsntfsmount.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_handle.h` & `libfsntfs-20230606/fsntfstools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/Makefile.am` & `libfsntfs-20230606/fsntfstools/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libhmac.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_handle.c` & `libfsntfs-20230606/fsntfstools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfusn.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfusn.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfsinfo.c` & `libfsntfs-20230606/fsntfstools/fsntfsinfo.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_getopt.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfwnt.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_dokan.c` & `libfsntfs-20230606/fsntfstools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/mount_file_entry.h` & `libfsntfs-20230606/fsntfstools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_i18n.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_i18n.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfguid.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfdata.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_output.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_output.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libbfio.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/info_handle.h` & `libfsntfs-20230606/fsntfstools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/digest_hash.c` & `libfsntfs-20230606/fsntfstools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libfsntfs.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_signal.c` & `libfsntfs-20230606/fsntfstools/fsntfstools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/Makefile.in` & `libfsntfs-20230606/fsntfstools/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_libcnotify.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_output.c` & `libfsntfs-20230606/fsntfstools/fsntfstools_output.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/fsntfstools/fsntfstools_unused.h` & `libfsntfs-20230606/fsntfstools/fsntfstools_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/install-sh` & `libfsntfs-20230606/install-sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/INSTALL` & `libfsntfs-20230606/INSTALL`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/dpkg/copyright` & `libfsntfs-20230606/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/dpkg/rules` & `libfsntfs-20230606/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/dpkg/control` & `libfsntfs-20230606/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_data_handle.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_txf_data_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_txf_data_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_root_header.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_root_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_header.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_bitmap_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_bitmap_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libfwnt.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_profiler.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_profiler.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_secure.h` & `libfsntfs-20230606/libfsntfs/fsntfs_secure.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_object_identifier.h` & `libfsntfs-20230606/libfsntfs/fsntfs_object_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compression.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compression.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_data.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_data.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_mft_attribute.h` & `libfsntfs-20230606/libfsntfs/fsntfs_mft_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_fixup_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_fixup_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_reparse_point.h` & `libfsntfs-20230606/libfsntfs/fsntfs_reparse_point.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_data.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_data.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_name_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_vector.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_txf_data_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_txf_data_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_data_stream.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_standard_information.h` & `libfsntfs-20230606/libfsntfs/fsntfs_standard_information.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_io_handle.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libcnotify.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_notify.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_name.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_name.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libcerror.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_data_handle.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_node.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/Makefile.am` & `libfsntfs-20230606/libfsntfs/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_vector.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_data_stream.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry.c`

 * *Files 1% similar despite different names*

```diff
@@ -2456,15 +2456,15 @@
  */
 int libfsntfs_mft_entry_set_attribute_helper_values(
      libfsntfs_mft_entry_t *mft_entry,
      int attribute_index,
      libfsntfs_mft_attribute_t *attribute,
      libcerror_error_t **error )
 {
-	uint8_t utf8_attribute_name[ 64 ];
+	uint8_t utf8_attribute_name[ 8 ];
 
 	static char *function                                                = "libfsntfs_mft_entry_set_attribute_helper_values";
 	size_t utf8_attribute_name_size                                      = 0;
 	uint32_t attribute_type                                              = 0;
 	int result                                                           = 0;
 
 #if defined( HAVE_DEBUG_OUTPUT )
@@ -2533,18 +2533,25 @@
 			if( mft_entry->file_name_attribute_index == -1 )
 			{
 				mft_entry->file_name_attribute_index = attribute_index;
 			}
 			break;
 
 		case LIBFSNTFS_ATTRIBUTE_TYPE_INDEX_ROOT:
+			/* Only interested in attribute names that would match $I30
+			 */
+			if( ( utf8_attribute_name_size == 0 )
+			 || ( utf8_attribute_name_size > 8 ) )
+			{
+				break;
+			}
 			if( libfsntfs_mft_attribute_get_utf8_name(
 			     attribute,
 			     utf8_attribute_name,
-			     64,
+			     utf8_attribute_name_size,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 				 "%s: unable to retrieve UTF-8 attribute name.",
@@ -2723,17 +2730,16 @@
  * Returns 1 if successful or -1 on error
  */
 int libfsntfs_mft_entry_set_data_attribute_helper_values(
      libfsntfs_mft_entry_t *mft_entry,
      libfsntfs_mft_attribute_t *data_attribute,
      libcerror_error_t **error )
 {
-	uint8_t utf8_attribute_name[ 64 ];
-
 	libfsntfs_mft_attribute_t *existing_data_attribute = NULL;
+	uint8_t *utf8_attribute_name                       = NULL;
 	static char *function                              = "libfsntfs_mft_entry_set_data_attribute_helper_values";
 	size_t utf8_attribute_name_size                    = 0;
 	int attribute_index                                = 0;
 	int entry_index                                    = 0;
 	int result                                         = 0;
 
 	if( mft_entry == NULL )
@@ -2755,15 +2761,15 @@
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve UTF-8 attribute name size.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
 	if( utf8_attribute_name_size <= 1 )
 	{
 		if( libfsntfs_mft_attribute_append_to_chain(
 		     &( mft_entry->data_attribute ),
 		     data_attribute,
 		     error ) != 1 )
@@ -2771,33 +2777,58 @@
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_APPEND_FAILED,
 			 "%s: unable to chain attribute.",
 			 function );
 
-			return( -1 );
+			goto on_error;
 		}
 	}
 	else
 	{
+		if( utf8_attribute_name_size > (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid UTF-8 attribute name size value out of bounds.",
+			 function );
+
+			goto on_error;
+		}
+		utf8_attribute_name = (uint8_t *) memory_allocate(
+		                                   (size_t) utf8_attribute_name_size );
+
+		if( utf8_attribute_name == NULL )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+			 "%s: unable to create UTF-8 attribute name.",
+			 function );
+
+			goto on_error;
+		}
 		if( libfsntfs_mft_attribute_get_utf8_name(
 		     data_attribute,
 		     utf8_attribute_name,
-		     64,
+		     utf8_attribute_name_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve UTF-8 attribute name.",
 			 function );
 
-			return( -1 );
+			goto on_error;
 		}
 		result = libfsntfs_mft_entry_get_data_attribute_by_utf8_name(
 		          mft_entry,
 		          utf8_attribute_name,
 		          utf8_attribute_name_size,
 		          &attribute_index,
 		          &existing_data_attribute,
@@ -2808,15 +2839,15 @@
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve data attribute.",
 			 function );
 
-			return( -1 );
+			goto on_error;
 		}
 		else if( result == 0 )
 		{
 			if( libcdata_array_append_entry(
 			     mft_entry->alternate_data_attributes_array,
 			     &entry_index,
 			     (intptr_t *) data_attribute,
@@ -2825,15 +2856,15 @@
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_APPEND_FAILED,
 				 "%s: unable to append alternate data attribute to array.",
 				 function );
 
-				return( -1 );
+				goto on_error;
 			}
 			existing_data_attribute = data_attribute;
 		}
 		else
 		{
 			if( libfsntfs_mft_attribute_append_to_chain(
 			     &existing_data_attribute,
@@ -2843,15 +2874,15 @@
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_APPEND_FAILED,
 				 "%s: unable to chain alternate data attribute.",
 				 function );
 
-				return( -1 );
+				goto on_error;
 			}
 			if( libcdata_array_set_entry_by_index(
 			     mft_entry->alternate_data_attributes_array,
 			     attribute_index,
 			     (intptr_t *) existing_data_attribute,
 			     error ) != 1 )
 			{
@@ -2859,17 +2890,22 @@
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 				 "%s: unable to append set data attribute: %d in array.",
 				 function,
 				 attribute_index );
 
-				return( -1 );
+				goto on_error;
 			}
 		}
+		memory_free(
+		 utf8_attribute_name );
+
+		utf8_attribute_name = NULL;
+
 		result = libfsntfs_mft_attribute_compare_name_with_utf8_string(
 		          data_attribute,
 		          (uint8_t *) "WofCompressedData",
 		          17,
 		          error );
 
 		if( result == -1 )
@@ -2877,22 +2913,30 @@
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GENERIC,
 			 "%s: unable to compare UTF-8 string with alternative data attribute name.",
 			 function );
 
-			return( -1 );
+			goto on_error;
 		}
 		else if( result == 1 )
 		{
 			mft_entry->wof_compressed_data_attribute = existing_data_attribute;
 		}
 	}
 	return( 1 );
+
+on_error:
+	if( utf8_attribute_name != NULL )
+	{
+		memory_free(
+		 utf8_attribute_name );
+	}
+	return( -1 );
 }
 
 /* Retrieves a data attribute with the specified name
  * Returns 1 if successful, 0 if no attribute was found or -1 on error
  */
 int libfsntfs_mft_entry_get_data_attribute_by_utf8_name(
      libfsntfs_mft_entry_t *mft_entry,
```

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list_entry.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_profiler.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_profiler.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_value.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_support.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_buffer_data_handle.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index_value.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs.c` & `libfsntfs-20230606/libfsntfs/libfsntfs.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_sds_index_value.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_sds_index_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_name.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_name.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libfcache.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_volume_information.h` & `libfsntfs-20230606/libfsntfs/fsntfs_volume_information.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry_header.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_extent.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_extent.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_index_value.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_directory_entry.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_entry.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_header.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_directory_entries_tree.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_directory_entries_tree.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_data_handle.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_name_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_data_run.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_data_run.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_descriptor.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_entry.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_debug.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_debug.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_header.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libfdata.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_attribute.c`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 		 "%s: invalid attribute.",
 		 function );
 
 		return( -1 );
 	}
 	if( *internal_attribute != NULL )
 	{
-		/* The mft_attribute references is freed elsewhere
+		/* The mft_attribute reference is freed elsewhere
 		 */
 #if defined( HAVE_LIBFSNTFS_MULTI_THREAD_SUPPORT )
 		if( libcthreads_read_write_lock_free(
 		     &( ( *internal_attribute )->read_write_lock ),
 		     error ) != 1 )
 		{
 			libcerror_error_set(
```

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_path_hint.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_path_hint.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_directory_entries_tree.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_directory_entries_tree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_data_handle.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_metadata_file.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_metadata_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_vector.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_node_header.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_node_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_vector.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_path_hint.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_path_hint.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_definitions.h.in` & `libfsntfs-20230606/libfsntfs/libfsntfs_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_fixup_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_fixup_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_error.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_data_run.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_data_run.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_entry.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libbfio.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_types.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_descriptor.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_index.h` & `libfsntfs-20230606/libfsntfs/fsntfs_index.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_bitmap_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_bitmap_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_error.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_name_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_volume_header.h` & `libfsntfs-20230606/libfsntfs/fsntfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_header.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libclocale.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_extent.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_extent.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_definitions.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 #if !defined( HAVE_LOCAL_LIBFSNTFS )
 #include <libfsntfs/definitions.h>
 
 /* The definitions in <libfsntfs/definitions.h> are copied here
  * for local use of libfsntfs
  */
 #else
-#define LIBFSNTFS_VERSION						20230427
+#define LIBFSNTFS_VERSION						20230606
 
 /* The version string
  */
-#define LIBFSNTFS_VERSION_STRING					"20230427"
+#define LIBFSNTFS_VERSION_STRING					"20230606"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSNTFS_ACCESS_FLAGS
```

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_buffer_data_handle.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_buffer_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_stream.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libcthreads.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_reparse_point_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_reparse_point_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_metadata_file.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_metadata_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_entry.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_mft_entry.h` & `libfsntfs-20230606/libfsntfs/fsntfs_mft_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_debug.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_debug.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_node.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_node.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_directory_entry.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compressed_block_data_handle.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compressed_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_system.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_support.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libfdatetime.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/Makefile.in` & `libfsntfs-20230606/libfsntfs/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_file_name.h` & `libfsntfs-20230606/libfsntfs/fsntfs_file_name.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_usn_change_journal.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_usn_change_journal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_name_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_logged_utility_stream_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_logged_utility_stream_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_logged_utility_stream_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_logged_utility_stream_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libuna.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_txf_data.h` & `libfsntfs-20230606/libfsntfs/fsntfs_txf_data.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_entry_header.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_entry_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_node_header.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_node_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_extern.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_root_header.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_root_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_notify.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_vector.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_name_values.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_name_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs.rc.in` & `libfsntfs-20230606/libfsntfs/libfsntfs.rc.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute_list_entry.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_logged_utility_stream.h` & `libfsntfs-20230606/libfsntfs/fsntfs_logged_utility_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_standard_information_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_standard_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_system.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_file_entry.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_value.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_unused.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_cluster_block_stream.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_cluster_block_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_mft_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_mft_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_volume_information_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_volume_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_io_handle.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_entry_vector.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_entry_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_security_descriptor_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_security_descriptor_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_attribute_list_attribute.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_attribute_list_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libcdata.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_libfguid.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_values.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_sds_index_value.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_sds_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/fsntfs_mft_attribute_list.h` & `libfsntfs-20230606/libfsntfs/fsntfs_mft_attribute_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_object_identifier_attribute.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_object_identifier_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs.rc` & `libfsntfs-20230606/libfsntfs/libfsntfs.rc`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows New Technology File System (NTFS) format\0"
-      VALUE "FileVersion",		"20230427" "\0"
+      VALUE "FileVersion",		"20230606" "\0"
       VALUE "InternalName",		"libfsntfs.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfsntfs.dll\0"
       VALUE "ProductName",		"libfsntfs\0"
-      VALUE "ProductVersion",		"20230427" "\0"
+      VALUE "ProductVersion",		"20230606" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfsntfs/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compression_unit_data_handle.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_compression_unit_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_compression.c` & `libfsntfs-20230606/libfsntfs/libfsntfs_compression.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_index_entry.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_index_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs/libfsntfs_usn_change_journal.h` & `libfsntfs-20230606/libfsntfs/libfsntfs_usn_change_journal.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_support.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_systemtime.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_error.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/Makefile.am` & `libfsntfs-20230606/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_unused.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_error.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_posix_time.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_fat_date_time.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_types.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_floatingtime.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_hfs_time.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_support.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_extern.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_filetime.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_date_time_values.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_floatingtime.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_libcerror.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/Makefile.in` & `libfsntfs-20230606/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_nsf_timedate.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_date_time_values.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_hfs_time.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_posix_time.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_fat_date_time.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_nsf_timedate.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_definitions.h` & `libfsntfs-20230606/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_systemtime.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdatetime/libfdatetime_filetime.c` & `libfsntfs-20230606/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_file.c` & `libfsntfs-20230606/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_libclocale.h` & `libfsntfs-20230606/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_support.c` & `libfsntfs-20230606/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_support.h` & `libfsntfs-20230606/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_error.c` & `libfsntfs-20230606/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_winapi.c` & `libfsntfs-20230606/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/Makefile.am` & `libfsntfs-20230606/libcfile/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_libcerror.h` & `libfsntfs-20230606/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_unused.h` & `libfsntfs-20230606/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_winapi.h` & `libfsntfs-20230606/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_types.h` & `libfsntfs-20230606/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_extern.h` & `libfsntfs-20230606/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_notify.h` & `libfsntfs-20230606/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_definitions.h` & `libfsntfs-20230606/libcfile/libcfile_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_file.h` & `libfsntfs-20230606/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_error.h` & `libfsntfs-20230606/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_system_string.c` & `libfsntfs-20230606/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/Makefile.in` & `libfsntfs-20230606/libcfile/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_system_string.h` & `libfsntfs-20230606/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_libcnotify.h` & `libfsntfs-20230606/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_libuna.h` & `libfsntfs-20230606/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcfile/libcfile_notify.c` & `libfsntfs-20230606/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_debug.c` & `libfsntfs-20230606/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_bit_stream.c` & `libfsntfs-20230606/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_lznt1.c` & `libfsntfs-20230606/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_libcerror.h` & `libfsntfs-20230606/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_unused.h` & `libfsntfs-20230606/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_support.c` & `libfsntfs-20230606/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_huffman_tree.c` & `libfsntfs-20230606/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/Makefile.am` & `libfsntfs-20230606/libfwnt/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_lzxpress.h` & `libfsntfs-20230606/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_lznt1.h` & `libfsntfs-20230606/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_locale_identifier.c` & `libfsntfs-20230606/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_libcdata.h` & `libfsntfs-20230606/libfwnt/libfwnt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_definitions.h` & `libfsntfs-20230606/libfwnt/libfwnt_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_notify.h` & `libfsntfs-20230606/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_types.h` & `libfsntfs-20230606/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_access_control_list.c` & `libfsntfs-20230606/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_locale_identifier.h` & `libfsntfs-20230606/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_notify.c` & `libfsntfs-20230606/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_extern.h` & `libfsntfs-20230606/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_support.h` & `libfsntfs-20230606/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_security_descriptor.h` & `libfsntfs-20230606/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_libcnotify.h` & `libfsntfs-20230606/libfwnt/libfwnt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_security_identifier.h` & `libfsntfs-20230606/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_access_control_list.h` & `libfsntfs-20230606/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_lzxpress.c` & `libfsntfs-20230606/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_access_control_entry.c` & `libfsntfs-20230606/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_lzx.c` & `libfsntfs-20230606/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_security_descriptor.c` & `libfsntfs-20230606/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_error.h` & `libfsntfs-20230606/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/Makefile.in` & `libfsntfs-20230606/libfwnt/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_security_identifier.c` & `libfsntfs-20230606/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_error.c` & `libfsntfs-20230606/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_lzx.h` & `libfsntfs-20230606/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_huffman_tree.h` & `libfsntfs-20230606/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_bit_stream.h` & `libfsntfs-20230606/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_access_control_entry.h` & `libfsntfs-20230606/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfwnt/libfwnt_debug.h` & `libfsntfs-20230606/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_thread_pool.h` & `libfsntfs-20230606/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_thread_pool.c` & `libfsntfs-20230606/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_repeating_thread.c` & `libfsntfs-20230606/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_error.c` & `libfsntfs-20230606/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/Makefile.am` & `libfsntfs-20230606/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_unused.h` & `libfsntfs-20230606/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_condition.h` & `libfsntfs-20230606/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_definitions.h` & `libfsntfs-20230606/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_thread.h` & `libfsntfs-20230606/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_repeating_thread.h` & `libfsntfs-20230606/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_read_write_lock.c` & `libfsntfs-20230606/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_mutex.h` & `libfsntfs-20230606/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_support.h` & `libfsntfs-20230606/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_thread.c` & `libfsntfs-20230606/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_mutex.c` & `libfsntfs-20230606/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_types.h` & `libfsntfs-20230606/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_lock.h` & `libfsntfs-20230606/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_extern.h` & `libfsntfs-20230606/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_error.h` & `libfsntfs-20230606/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_queue.c` & `libfsntfs-20230606/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_condition.c` & `libfsntfs-20230606/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/Makefile.in` & `libfsntfs-20230606/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_thread_attributes.c` & `libfsntfs-20230606/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_libcerror.h` & `libfsntfs-20230606/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_lock.c` & `libfsntfs-20230606/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_support.c` & `libfsntfs-20230606/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_read_write_lock.h` & `libfsntfs-20230606/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_thread_attributes.h` & `libfsntfs-20230606/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcthreads/libcthreads_queue.h` & `libfsntfs-20230606/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs.pc.in` & `libfsntfs-20230606/libfsntfs.pc.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_data_streams.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_data_streams.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_name_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_name_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_attribute_flags.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_attribute_flags.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_libclocale.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_guid.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_guid.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_object_identifier_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_object_identifier_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/Makefile.am` & `libfsntfs-20230606/pyfsntfs/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_attributes.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_standard_information_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_standard_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_reparse_point_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_reparse_point_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_python.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_python.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_libfsntfs.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_data_stream.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_object_io_handle.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_datetime.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_datetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_security_descriptor_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_security_descriptor_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_libfguid.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entry.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_unused.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_error.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_guid.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_guid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_attributes.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_name_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_file_entries.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_standard_information_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_standard_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute_types.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_name_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_libbfio.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_usn_change_journal.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_usn_change_journal.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_information_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_reparse_point_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_reparse_point_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_object_identifier_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_object_identifier_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entries.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_libcerror.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_integer.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_integer.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/Makefile.in` & `libfsntfs-20230606/pyfsntfs/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_error.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_datetime.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_datetime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_integer.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_integer.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_security_descriptor_attribute.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_security_descriptor_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entries.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_information_attribute.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_entry.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_attribute_flags.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_attribute_flags.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_attribute_types.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_attribute_types.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_volume_file_entries.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_volume_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_usn_change_journal.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_usn_change_journal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_file_object_io_handle.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_data_stream.h` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs/pyfsntfs_data_streams.c` & `libfsntfs-20230606/pyfsntfs/pyfsntfs_data_streams.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/config.sub` & `libfsntfs-20230606/config.sub`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_unused.h` & `libfsntfs-20230606/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_support.c` & `libfsntfs-20230606/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_libclocale.h` & `libfsntfs-20230606/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/Makefile.am` & `libfsntfs-20230606/libcpath/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_error.h` & `libfsntfs-20230606/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_system_string.h` & `libfsntfs-20230606/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_error.c` & `libfsntfs-20230606/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_libcsplit.h` & `libfsntfs-20230606/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_path.h` & `libfsntfs-20230606/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/Makefile.in` & `libfsntfs-20230606/libcpath/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_definitions.h` & `libfsntfs-20230606/libcpath/libcpath_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_libcerror.h` & `libfsntfs-20230606/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_extern.h` & `libfsntfs-20230606/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_path.c` & `libfsntfs-20230606/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_system_string.c` & `libfsntfs-20230606/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_support.h` & `libfsntfs-20230606/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcpath/libcpath_libuna.h` & `libfsntfs-20230606/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/manuals/libfsntfs.3` & `libfsntfs-20230606/manuals/libfsntfs.3`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/manuals/Makefile.in` & `libfsntfs-20230606/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/manuals/fsntfsinfo.1` & `libfsntfs-20230606/manuals/fsntfsinfo.1`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_libuna.h` & `libfsntfs-20230606/libfusn/libfusn_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_error.h` & `libfsntfs-20230606/libfusn/libfusn_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_definitions.h` & `libfsntfs-20230606/libfusn/libfusn_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/fusn_record.h` & `libfsntfs-20230606/libfusn/fusn_record.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_debug.c` & `libfsntfs-20230606/libfusn/libfusn_debug.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/Makefile.am` & `libfsntfs-20230606/libfusn/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_unused.h` & `libfsntfs-20230606/libfusn/libfusn_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_libfdatetime.h` & `libfsntfs-20230606/libfusn/libfusn_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_debug.h` & `libfsntfs-20230606/libfusn/libfusn_debug.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_libcerror.h` & `libfsntfs-20230606/libfusn/libfusn_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_support.h` & `libfsntfs-20230606/libfusn/libfusn_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_record.c` & `libfsntfs-20230606/libfusn/libfusn_record.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_extern.h` & `libfsntfs-20230606/libfusn/libfusn_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_libcnotify.h` & `libfsntfs-20230606/libfusn/libfusn_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_record.h` & `libfsntfs-20230606/libfusn/libfusn_record.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/Makefile.in` & `libfsntfs-20230606/libfusn/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_support.c` & `libfsntfs-20230606/libfusn/libfusn_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_error.c` & `libfsntfs-20230606/libfusn/libfusn_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfusn/libfusn_types.h` & `libfsntfs-20230606/libfusn/libfusn_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfcache/libfcache.vcproj` & `libfsntfs-20230606/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfsmount/fsntfsmount.vcproj` & `libfsntfs-20230606/msvscpp/fsntfsmount/fsntfsmount.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfguid/libfguid.vcproj` & `libfsntfs-20230606/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libclocale/libclocale.vcproj` & `libfsntfs-20230606/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/Makefile.am` & `libfsntfs-20230606/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libbfio/libbfio.vcproj` & `libfsntfs-20230606/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfsntfs.sln` & `libfsntfs-20230606/msvscpp/libfsntfs.sln`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfsntfs/libfsntfs.vcproj` & `libfsntfs-20230606/msvscpp/libfsntfs/libfsntfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfsntfs-20230606/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcfile/libcfile.vcproj` & `libfsntfs-20230606/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfwnt/libfwnt.vcproj` & `libfsntfs-20230606/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcthreads/libcthreads.vcproj` & `libfsntfs-20230606/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/pyfsntfs/pyfsntfs.vcproj` & `libfsntfs-20230606/msvscpp/pyfsntfs/pyfsntfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcpath/libcpath.vcproj` & `libfsntfs-20230606/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfusn/libfusn.vcproj` & `libfsntfs-20230606/msvscpp/libfusn/libfusn.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libhmac/libhmac.vcproj` & `libfsntfs-20230606/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libuna/libuna.vcproj` & `libfsntfs-20230606/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/Makefile.in` & `libfsntfs-20230606/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcerror/libcerror.vcproj` & `libfsntfs-20230606/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcnotify/libcnotify.vcproj` & `libfsntfs-20230606/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfsinfo/fsntfsinfo.vcproj` & `libfsntfs-20230606/msvscpp/fsntfsinfo/fsntfsinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libfdata/libfdata.vcproj` & `libfsntfs-20230606/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcdata/libcdata.vcproj` & `libfsntfs-20230606/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/libcsplit/libcsplit.vcproj` & `libfsntfs-20230606/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj` & `libfsntfs-20230606/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha1_context.h` & `libfsntfs-20230606/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_md5.h` & `libfsntfs-20230606/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha1.c` & `libfsntfs-20230606/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_support.c` & `libfsntfs-20230606/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_definitions.h` & `libfsntfs-20230606/libhmac/libhmac_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/Makefile.am` & `libfsntfs-20230606/libhmac/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_error.c` & `libfsntfs-20230606/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha256.c` & `libfsntfs-20230606/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha512.c` & `libfsntfs-20230606/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha256.h` & `libfsntfs-20230606/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_support.h` & `libfsntfs-20230606/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_md5.c` & `libfsntfs-20230606/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha512_context.c` & `libfsntfs-20230606/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_libcerror.h` & `libfsntfs-20230606/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_extern.h` & `libfsntfs-20230606/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha256_context.h` & `libfsntfs-20230606/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_md5_context.h` & `libfsntfs-20230606/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha224_context.h` & `libfsntfs-20230606/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha224.c` & `libfsntfs-20230606/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha224_context.c` & `libfsntfs-20230606/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/Makefile.in` & `libfsntfs-20230606/libhmac/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_types.h` & `libfsntfs-20230606/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha512.h` & `libfsntfs-20230606/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_unused.h` & `libfsntfs-20230606/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha512_context.h` & `libfsntfs-20230606/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha224.h` & `libfsntfs-20230606/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha1_context.c` & `libfsntfs-20230606/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha1.h` & `libfsntfs-20230606/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_error.h` & `libfsntfs-20230606/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_sha256_context.c` & `libfsntfs-20230606/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_byte_stream.h` & `libfsntfs-20230606/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libhmac/libhmac_md5_context.c` & `libfsntfs-20230606/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/setup.py` & `libfsntfs-20230606/setup.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/config.guess` & `libfsntfs-20230606/config.guess`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/file_entry_fuzzer.cc` & `libfsntfs-20230606/ossfuzz/file_entry_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/Makefile.am` & `libfsntfs-20230606/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/volume_fuzzer.cc` & `libfsntfs-20230606/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/ossfuzz_libfsntfs.h` & `libfsntfs-20230606/ossfuzz/ossfuzz_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/Makefile.in` & `libfsntfs-20230606/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/mft_metadata_file_fuzzer.cc` & `libfsntfs-20230606/ossfuzz/mft_metadata_file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ossfuzz/ossfuzz_libbfio.h` & `libfsntfs-20230606/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/test-driver` & `libfsntfs-20230606/test-driver`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/configure` & `libfsntfs-20230606/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfsntfs 20230427.
+# Generated by GNU Autoconf 2.71 for libfsntfs 20230606.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfsntfs'
 PACKAGE_TARNAME='libfsntfs'
-PACKAGE_VERSION='20230427'
-PACKAGE_STRING='libfsntfs 20230427'
+PACKAGE_VERSION='20230606'
+PACKAGE_STRING='libfsntfs 20230606'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfsntfs.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1739,15 +1739,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfsntfs 20230427 to adapt to many kinds of systems.
+\`configure' configures libfsntfs 20230606 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1810,15 +1810,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfsntfs 20230427:";;
+     short | recursive ) echo "Configuration of libfsntfs 20230606:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2099,15 +2099,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfsntfs configure 20230427
+libfsntfs configure 20230606
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2820,15 +2820,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfsntfs $as_me 20230427, which was
+It was created by libfsntfs $as_me 20230606, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4309,15 +4309,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfsntfs'
- VERSION='20230427'
+ VERSION='20230606'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -62377,15 +62377,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfsntfs $as_me 20230427, which was
+This file was extended by libfsntfs $as_me 20230606, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -62445,15 +62445,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfsntfs config.status 20230427
+libfsntfs config.status 20230606
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfsntfs-20230427/libuna/libuna_url_stream.c` & `libfsntfs-20230606/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_symbol.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_support.c` & `libfsntfs-20230606/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_scsu.h` & `libfsntfs-20230606/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_5.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_2.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1253.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_koi8_u.h` & `libfsntfs-20230606/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1252.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf32_stream.c` & `libfsntfs-20230606/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1257.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_cyrillic.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_thai.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf32_string.c` & `libfsntfs-20230606/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_thai.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_874.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1251.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_libcerror.h` & `libfsntfs-20230606/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_949.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_6.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1256.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_greek.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_russian.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_ukrainian.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_6.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_874.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1251.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1256.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_base16_stream.h` & `libfsntfs-20230606/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_2.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/Makefile.am` & `libfsntfs-20230606/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1257.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1254.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1255.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_unused.h` & `libfsntfs-20230606/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1253.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_unicode_character.h` & `libfsntfs-20230606/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_dingbats.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_scsu.c` & `libfsntfs-20230606/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_byte_stream.c` & `libfsntfs-20230606/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_celtic.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_croatian.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_3.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_15.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_roman.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf32_string.h` & `libfsntfs-20230606/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_koi8_r.c` & `libfsntfs-20230606/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_icelandic.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_936.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_base64_stream.h` & `libfsntfs-20230606/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_celtic.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_950.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf8_string.h` & `libfsntfs-20230606/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_936.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_unicode_character.c` & `libfsntfs-20230606/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf8_string.c` & `libfsntfs-20230606/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_base32_stream.c` & `libfsntfs-20230606/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_950.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_error.h` & `libfsntfs-20230606/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_932.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_turkish.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf8_stream.c` & `libfsntfs-20230606/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_ukrainian.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_koi8_r.h` & `libfsntfs-20230606/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_base16_stream.c` & `libfsntfs-20230606/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1250.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_16.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_croatian.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_gaelic.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf16_stream.h` & `libfsntfs-20230606/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_10.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_centraleurroman.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_932.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf8_stream.h` & `libfsntfs-20230606/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_url_stream.h` & `libfsntfs-20230606/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_farsi.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_949.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_romanian.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_gaelic.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_8.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_types.h` & `libfsntfs-20230606/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_arabic.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1252.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1250.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_russian.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf16_string.c` & `libfsntfs-20230606/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_5.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_extern.h` & `libfsntfs-20230606/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_4.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_byte_stream.h` & `libfsntfs-20230606/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_roman.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf16_string.h` & `libfsntfs-20230606/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_4.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_10.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_icelandic.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/Makefile.in` & `libfsntfs-20230606/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf7_stream.h` & `libfsntfs-20230606/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_symbol.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_base32_stream.h` & `libfsntfs-20230606/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_turkish.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_inuit.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf16_stream.c` & `libfsntfs-20230606/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf7_stream.c` & `libfsntfs-20230606/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_support.h` & `libfsntfs-20230606/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_utf32_stream.h` & `libfsntfs-20230606/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_3.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_greek.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_definitions.h` & `libfsntfs-20230606/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1255.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_14.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_13.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_centraleurroman.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_8.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_9.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1254.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_cyrillic.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_arabic.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1258.c` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_farsi.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_15.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_7.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_dingbats.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_9.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_windows_1258.h` & `libfsntfs-20230606/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_base64_stream.c` & `libfsntfs-20230606/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_romanian.c` & `libfsntfs-20230606/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_error.c` & `libfsntfs-20230606/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_koi8_u.c` & `libfsntfs-20230606/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_13.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_7.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_14.h` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_mac_inuit.h` & `libfsntfs-20230606/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libuna/libuna_codepage_iso_8859_16.c` & `libfsntfs-20230606/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs.spec.in` & `libfsntfs-20230606/libfsntfs.spec.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/Makefile.in` & `libfsntfs-20230606/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ChangeLog` & `libfsntfs-20230606/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libuna.m4` & `libfsntfs-20230606/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfuse.m4` & `libfsntfs-20230606/m4/libfuse.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/gettext.m4` & `libfsntfs-20230606/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/tests.m4` & `libfsntfs-20230606/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfusn.m4` & `libfsntfs-20230606/m4/libfusn.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/lib-prefix.m4` & `libfsntfs-20230606/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/ltoptions.m4` & `libfsntfs-20230606/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfwnt.m4` & `libfsntfs-20230606/m4/libfwnt.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcpath.m4` & `libfsntfs-20230606/m4/libcpath.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/lib-ld.m4` & `libfsntfs-20230606/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcthreads.m4` & `libfsntfs-20230606/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/lib-link.m4` & `libfsntfs-20230606/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libhmac.m4` & `libfsntfs-20230606/m4/libhmac.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/python.m4` & `libfsntfs-20230606/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libtool.m4` & `libfsntfs-20230606/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/nls.m4` & `libfsntfs-20230606/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libclocale.m4` & `libfsntfs-20230606/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfdata.m4` & `libfsntfs-20230606/m4/libfdata.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfdatetime.m4` & `libfsntfs-20230606/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/host-cpu-c-abi.m4` & `libfsntfs-20230606/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcnotify.m4` & `libfsntfs-20230606/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/ltversion.m4` & `libfsntfs-20230606/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcdata.m4` & `libfsntfs-20230606/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/progtest.m4` & `libfsntfs-20230606/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/lt~obsolete.m4` & `libfsntfs-20230606/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcfile.m4` & `libfsntfs-20230606/m4/libcfile.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcrypto.m4` & `libfsntfs-20230606/m4/libcrypto.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/po.m4` & `libfsntfs-20230606/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/pthread.m4` & `libfsntfs-20230606/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/common.m4` & `libfsntfs-20230606/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcerror.m4` & `libfsntfs-20230606/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfguid.m4` & `libfsntfs-20230606/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/iconv.m4` & `libfsntfs-20230606/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/ltsugar.m4` & `libfsntfs-20230606/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libfcache.m4` & `libfsntfs-20230606/m4/libfcache.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libcsplit.m4` & `libfsntfs-20230606/m4/libcsplit.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/intlmacosx.m4` & `libfsntfs-20230606/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/types.m4` & `libfsntfs-20230606/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/m4/libbfio.m4` & `libfsntfs-20230606/m4/libbfio.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/COPYING.LESSER` & `libfsntfs-20230606/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_system.c` & `libfsntfs-20230606/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_error.c` & `libfsntfs-20230606/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_extern.h` & `libfsntfs-20230606/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/Makefile.am` & `libfsntfs-20230606/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_error.h` & `libfsntfs-20230606/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_support.h` & `libfsntfs-20230606/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_types.h` & `libfsntfs-20230606/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_definitions.h` & `libfsntfs-20230606/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_unused.h` & `libfsntfs-20230606/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/Makefile.in` & `libfsntfs-20230606/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_support.c` & `libfsntfs-20230606/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcerror/libcerror_system.h` & `libfsntfs-20230606/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_libcerror.h` & `libfsntfs-20230606/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_unused.h` & `libfsntfs-20230606/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_support.h` & `libfsntfs-20230606/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_support.c` & `libfsntfs-20230606/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/Makefile.am` & `libfsntfs-20230606/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_print.c` & `libfsntfs-20230606/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_verbose.c` & `libfsntfs-20230606/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_stream.h` & `libfsntfs-20230606/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_extern.h` & `libfsntfs-20230606/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_stream.c` & `libfsntfs-20230606/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/Makefile.in` & `libfsntfs-20230606/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_print.h` & `libfsntfs-20230606/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_verbose.h` & `libfsntfs-20230606/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcnotify/libcnotify_definitions.h` & `libfsntfs-20230606/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/ltmain.sh` & `libfsntfs-20230606/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/compile` & `libfsntfs-20230606/compile`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs-python2/Makefile.am` & `libfsntfs-20230606/pyfsntfs-python2/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs-python2/Makefile.in` & `libfsntfs-20230606/pyfsntfs-python2/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/config.rpath` & `libfsntfs-20230606/config.rpath`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/depcomp` & `libfsntfs-20230606/depcomp`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/en@quot.header` & `libfsntfs-20230606/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/Rules-quot` & `libfsntfs-20230606/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/remove-potcdate.sin` & `libfsntfs-20230606/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/Makevars.in` & `libfsntfs-20230606/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/en@boldquot.header` & `libfsntfs-20230606/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/Makevars` & `libfsntfs-20230606/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/insert-header.sin` & `libfsntfs-20230606/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/po/Makefile.in.in` & `libfsntfs-20230606/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs-python3/Makefile.am` & `libfsntfs-20230606/pyfsntfs-python3/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/pyfsntfs-python3/Makefile.in` & `libfsntfs-20230606/pyfsntfs-python3/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_segments_array.h` & `libfsntfs-20230606/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_cache.c` & `libfsntfs-20230606/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_support.c` & `libfsntfs-20230606/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_list_element.c` & `libfsntfs-20230606/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_mapped_range.h` & `libfsntfs-20230606/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_extern.h` & `libfsntfs-20230606/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_list.c` & `libfsntfs-20230606/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_libcdata.h` & `libfsntfs-20230606/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_notify.h` & `libfsntfs-20230606/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_range_list.h` & `libfsntfs-20230606/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/Makefile.am` & `libfsntfs-20230606/libfdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_error.c` & `libfsntfs-20230606/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_list.h` & `libfsntfs-20230606/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_area.h` & `libfsntfs-20230606/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_types.h` & `libfsntfs-20230606/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_area.c` & `libfsntfs-20230606/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_range.h` & `libfsntfs-20230606/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_vector.c` & `libfsntfs-20230606/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_stream.h` & `libfsntfs-20230606/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_vector.h` & `libfsntfs-20230606/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_support.h` & `libfsntfs-20230606/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_libfcache.h` & `libfsntfs-20230606/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_libcerror.h` & `libfsntfs-20230606/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_range_list.c` & `libfsntfs-20230606/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_libcnotify.h` & `libfsntfs-20230606/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_notify.c` & `libfsntfs-20230606/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_list_element.h` & `libfsntfs-20230606/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_unused.h` & `libfsntfs-20230606/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_error.h` & `libfsntfs-20230606/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/Makefile.in` & `libfsntfs-20230606/libfdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_cache.h` & `libfsntfs-20230606/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_stream.c` & `libfsntfs-20230606/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_segments_array.c` & `libfsntfs-20230606/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_mapped_range.c` & `libfsntfs-20230606/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_definitions.h` & `libfsntfs-20230606/libfdata/libfdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfdata/libfdata_range.c` & `libfsntfs-20230606/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_array.c` & `libfsntfs-20230606/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_btree_node.c` & `libfsntfs-20230606/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_tree_node.c` & `libfsntfs-20230606/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_libcthreads.h` & `libfsntfs-20230606/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_range_list_value.h` & `libfsntfs-20230606/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_unused.h` & `libfsntfs-20230606/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_range_list.h` & `libfsntfs-20230606/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/Makefile.am` & `libfsntfs-20230606/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_range_list.c` & `libfsntfs-20230606/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_extern.h` & `libfsntfs-20230606/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_support.c` & `libfsntfs-20230606/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_list_element.h` & `libfsntfs-20230606/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_btree_values_list.c` & `libfsntfs-20230606/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_range_list_value.c` & `libfsntfs-20230606/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_libcerror.h` & `libfsntfs-20230606/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_error.c` & `libfsntfs-20230606/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_error.h` & `libfsntfs-20230606/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_support.h` & `libfsntfs-20230606/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_btree_node.h` & `libfsntfs-20230606/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_list.c` & `libfsntfs-20230606/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_tree_node.h` & `libfsntfs-20230606/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_list.h` & `libfsntfs-20230606/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_types.h` & `libfsntfs-20230606/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_list_element.c` & `libfsntfs-20230606/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/Makefile.in` & `libfsntfs-20230606/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_btree_values_list.h` & `libfsntfs-20230606/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_array.h` & `libfsntfs-20230606/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_btree.h` & `libfsntfs-20230606/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_definitions.h` & `libfsntfs-20230606/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcdata/libcdata_btree.c` & `libfsntfs-20230606/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/acinclude.m4` & `libfsntfs-20230606/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_types.h` & `libfsntfs-20230606/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_wide_string.h` & `libfsntfs-20230606/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_error.h` & `libfsntfs-20230606/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_support.h` & `libfsntfs-20230606/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_narrow_split_string.c` & `libfsntfs-20230606/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_narrow_split_string.h` & `libfsntfs-20230606/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/Makefile.am` & `libfsntfs-20230606/libcsplit/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_wide_split_string.c` & `libfsntfs-20230606/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_narrow_string.h` & `libfsntfs-20230606/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_unused.h` & `libfsntfs-20230606/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_wide_string.c` & `libfsntfs-20230606/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_narrow_string.c` & `libfsntfs-20230606/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/Makefile.in` & `libfsntfs-20230606/libcsplit/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_wide_split_string.h` & `libfsntfs-20230606/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_definitions.h` & `libfsntfs-20230606/libcsplit/libcsplit_definitions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_error.c` & `libfsntfs-20230606/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_support.c` & `libfsntfs-20230606/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_libcerror.h` & `libfsntfs-20230606/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libcsplit/libcsplit_extern.h` & `libfsntfs-20230606/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20230427/libfsntfs.spec` & `libfsntfs-20230606/libfsntfs.spec`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfsntfs
-Version: 20230427
+Version: 20230606
 Release: 1
 Summary: Library to access the Windows New Technology File System (NTFS) format
 Group: System Environment/Libraries
 License: LGPLv3+
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfsntfs
 BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
@@ -97,10 +97,10 @@
 %defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %attr(755,root,root) %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Apr 29 2023 Joachim Metz <joachim.metz@gmail.com> 20230427-1
+* Tue Jun  6 2023 Joachim Metz <joachim.metz@gmail.com> 20230606-1
 - Auto-generated
```

### Comparing `libfsntfs-20230427/configure.ac` & `libfsntfs-20230606/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfsntfs],
- [20230427],
+ [20230606],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfsntfs.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

