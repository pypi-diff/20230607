# Comparing `tmp/pynamer-2.1.2.tar.gz` & `tmp/pynamer-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.1.2.tar", last modified: Tue Jun  6 20:46:26 2023, max compression
+gzip compressed data, was "pynamer-2.1.3.tar", last modified: Wed Jun  7 13:48:00 2023, max compression
```

## Comparing `pynamer-2.1.2.tar` & `pynamer-2.1.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:46:26.148704 pynamer-2.1.2/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.2/AUTHORS.md
--rw-rw-rw-   0        0        0    10638 2023-06-06 20:46:11.000000 pynamer-2.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.2/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    19277 2023-06-06 20:46:26.148704 pynamer-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    17613 2023-06-06 20:06:46.000000 pynamer-2.1.2/README.md
--rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1954 2023-06-06 20:46:26.152713 pynamer-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:46:25.861188 pynamer-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 20:46:25.968178 pynamer-2.1.2/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.2/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-06 20:46:11.000000 pynamer-2.1.2/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.2/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2354 2023-06-04 10:27:28.000000 pynamer-2.1.2/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      823 2023-06-04 16:16:48.000000 pynamer-2.1.2/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:46:25.982185 pynamer-2.1.2/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.2/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7623 2023-06-06 14:49:53.000000 pynamer-2.1.2/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.2/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.2/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.2/src/pynamer/utils.py
--rw-rw-rw-   0        0        0    10643 2023-06-06 14:04:47.000000 pynamer-2.1.2/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:46:25.979177 pynamer-2.1.2/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    19277 2023-06-06 20:46:25.000000 pynamer-2.1.2/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-06-06 20:46:25.000000 pynamer-2.1.2/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:46:25.000000 pynamer-2.1.2/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 20:46:25.000000 pynamer-2.1.2/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       90 2023-06-06 20:46:25.000000 pynamer-2.1.2/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 20:46:25.000000 pynamer-2.1.2/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 20:46:26.145702 pynamer-2.1.2/tests/
--rw-rw-rw-   0        0        0     2063 2023-06-04 10:27:28.000000 pynamer-2.1.2/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.2/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.2/tests/test_get_homepage.py
--rw-rw-rw-   0        0        0     1927 2023-06-06 13:17:15.000000 pynamer-2.1.2/tests/test_github_meta.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.2/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.2/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.2/tests/test_utils_search_json.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.2/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.2/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:48:00.688069 pynamer-2.1.3/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.3/AUTHORS.md
+-rw-rw-rw-   0        0        0    10806 2023-06-07 13:47:48.000000 pynamer-2.1.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    19277 2023-06-07 13:48:00.689068 pynamer-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17613 2023-06-06 20:06:46.000000 pynamer-2.1.3/README.md
+-rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1991 2023-06-07 13:48:00.693066 pynamer-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:48:00.545068 pynamer-2.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 13:48:00.597079 pynamer-2.1.3/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.3/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-07 13:47:48.000000 pynamer-2.1.3/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.3/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2354 2023-06-04 10:27:28.000000 pynamer-2.1.3/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      823 2023-06-04 16:16:48.000000 pynamer-2.1.3/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:48:00.614089 pynamer-2.1.3/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.3/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7701 2023-06-07 10:30:39.000000 pynamer-2.1.3/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.3/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.3/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.3/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    10901 2023-06-07 11:32:19.000000 pynamer-2.1.3/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:48:00.610067 pynamer-2.1.3/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    19277 2023-06-07 13:48:00.000000 pynamer-2.1.3/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-06-07 13:48:00.000000 pynamer-2.1.3/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:48:00.000000 pynamer-2.1.3/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-07 13:48:00.000000 pynamer-2.1.3/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2023-06-07 13:48:00.000000 pynamer-2.1.3/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 13:48:00.000000 pynamer-2.1.3/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 13:48:00.684076 pynamer-2.1.3/tests/
+-rw-rw-rw-   0        0        0     2063 2023-06-04 10:27:28.000000 pynamer-2.1.3/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.3/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.3/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2822 2023-06-07 13:04:42.000000 pynamer-2.1.3/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.3/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.3/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     1927 2023-06-06 13:17:15.000000 pynamer-2.1.3/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.3/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.3/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.3/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.3/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.3/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.3/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.3/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.3/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.3/tests/test_write_output_file.py
```

### Comparing `pynamer-2.1.2/CHANGELOG.md` & `pynamer-2.1.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.3 (2023-06-07)
+### Fix
+* Regex for package names ([`756c6ff`](https://github.com/Stephen-RA-King/pynamer/commit/756c6ff297ca872ae3805df0ce25064cd4e518a2))
+
 ## v2.1.2 (2023-06-06)
 ### Documentation
 * Update documentation ([`cf7ea92`](https://github.com/Stephen-RA-King/pynamer/commit/cf7ea92cb25354a2e7378d5fe44e24293ecf43dd))
 
 ## v2.1.1 (2023-06-06)
 ### Fix
 * Missing dependencies ([`cd5027f`](https://github.com/Stephen-RA-King/pynamer/commit/cd5027fe5bbd95694658448b25ce5702f1fca986))
```

### Comparing `pynamer-2.1.2/LICENSE` & `pynamer-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/PKG-INFO` & `pynamer-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.2
+Version: 2.1.3
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-2.1.2/README.md` & `pynamer-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/pyproject.toml` & `pynamer-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/setup.cfg` & `pynamer-2.1.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -36,88 +36,90 @@
 00000230: 616d 6572 0d0a 646f 776e 6c6f 6164 5f75  amer..download_u
 00000240: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
 00000250: 6875 622e 636f 6d2f 5374 6570 6865 6e2d  hub.com/Stephen-
 00000260: 5241 2d4b 696e 672f 7079 6e61 6d65 722f  RA-King/pynamer/
 00000270: 6172 6368 6976 652f 7265 6673 2f68 6561  archive/refs/hea
 00000280: 6473 2f6d 6169 6e2e 7a69 700d 0a6c 6963  ds/main.zip..lic
 00000290: 656e 7365 203d 204d 4954 0d0a 6c69 6365  ense = MIT..lice
-000002a0: 6e73 655f 6669 6c65 203d 204c 4943 454e  nse_file = LICEN
-000002b0: 5345 0d0a 636c 6173 7369 6669 6572 7320  SE..classifiers 
-000002c0: 3d20 0d0a 0944 6576 656c 6f70 6d65 6e74  = ...Development
-000002d0: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
-000002e0: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
-000002f0: 0d0a 0945 6e76 6972 6f6e 6d65 6e74 203a  ...Environment :
-00000300: 3a20 436f 6e73 6f6c 650d 0a09 496e 7465  : Console...Inte
-00000310: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000320: 2044 6576 656c 6f70 6572 730d 0a09 4c69   Developers...Li
-00000330: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000340: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000350: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
-00000360: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000370: 6465 7065 6e64 656e 740d 0a09 4e61 7475  dependent...Natu
-00000380: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
-00000390: 456e 676c 6973 680d 0a09 5072 6f67 7261  English...Progra
-000003a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000003b0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-000003c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003e0: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
-000003f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000400: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000410: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
-00000420: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000430: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
-00000440: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000450: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000460: 2033 2e31 310d 0a0d 0a5b 6f70 7469 6f6e   3.11....[option
-00000470: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000480: 3d20 0d0a 093d 7372 630d 0a70 6163 6b61  = ...=src..packa
-00000490: 6765 7320 3d20 6669 6e64 3a0d 0a70 726f  ges = find:..pro
-000004a0: 6a65 6374 5f75 726c 7320 3d20 0d0a 696e  ject_urls = ..in
-000004b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-000004c0: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
-000004d0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000004e0: 2e39 0d0a 696e 7374 616c 6c5f 7265 7175  .9..install_requ
-000004f0: 6972 6573 203d 200d 0a09 6273 340d 0a09  ires = ...bs4...
-00000500: 6275 696c 640d 0a09 636f 6c6f 7261 6d61  build...colorama
-00000510: 0d0a 096a 696e 6a61 320d 0a09 7061 636b  ...jinja2...pack
-00000520: 6167 696e 670d 0a09 7079 7468 6f6e 2d64  aging...python-d
-00000530: 6174 6575 7469 6c0d 0a09 7079 7961 6d6c  ateutil...pyyaml
-00000540: 0d0a 0972 6571 7565 7374 730d 0a09 7269  ...requests...ri
-00000550: 6368 0d0a 0974 7164 6d0d 0a09 7477 696e  ch...tqdm...twin
-00000560: 650d 0a09 7768 6565 6c0d 0a0d 0a5b 6f70  e...wheel....[op
-00000570: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000580: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000590: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
-000005a0: 636b 6167 655f 6461 7461 5d0d 0a70 796e  ckage_data]..pyn
-000005b0: 616d 6572 203d 200d 0a09 5245 4144 4d45  amer = ...README
-000005c0: 2e6d 640d 0a09 636f 6e66 6967 2e70 790d  .md...config.py.
-000005d0: 0a09 7072 6f6a 6563 745f 6e61 6d65 0d0a  ..project_name..
-000005e0: 0970 726f 6a65 6374 5f6e 616d 652f 5f5f  .project_name/__
-000005f0: 696e 6974 5f5f 2e70 790d 0a09 7365 7475  init__.py...setu
-00000600: 702e 7478 740d 0a09 7365 7475 705f 6261  p.txt...setup_ba
-00000610: 7365 2e74 7874 0d0a 0975 7469 6c73 2e70  se.txt...utils.p
-00000620: 790d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  y....[options.en
-00000630: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-00000640: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-00000650: 0a09 7079 6e61 6d65 7220 3d20 7079 6e61  ..pynamer = pyna
-00000660: 6d65 722e 7079 6e61 6d65 723a 6d61 696e  mer.pynamer:main
-00000670: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 646f  ....[flake8]..do
-00000680: 6373 7472 696e 672d 636f 6e76 656e 7469  cstring-conventi
-00000690: 6f6e 203d 206e 756d 7079 0d0a 6d61 782d  on = numpy..max-
-000006a0: 636f 6d70 6c65 7869 7479 203d 2031 380d  complexity = 18.
-000006b0: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
-000006c0: 203d 2038 380d 0a73 656c 6563 7420 3d20   = 88..select = 
-000006d0: 422c 2042 392c 2043 2c20 442c 2045 2c20  B, B9, C, D, E, 
-000006e0: 462c 204e 2c20 570d 0a65 7863 6c75 6465  F, N, W..exclude
-000006f0: 203d 2074 6573 7473 2f2a 2c2e 746f 782f   = tests/*,.tox/
-00000700: 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f 2a2c  *,.nox/*,docs/*,
-00000710: 2e67 6974 2f2a 2c2e 6769 7468 7562 2f2a  .git/*,.github/*
-00000720: 0d0a 6967 6e6f 7265 203d 200d 0a09 4532  ..ignore = ...E2
-00000730: 3033 2c0d 0a09 5735 3033 2c0d 0a70 6572  03,...W503,..per
-00000740: 2d66 696c 652d 6967 6e6f 7265 7320 3d20  -file-ignores = 
-00000750: 0d0a 0970 796e 616d 6572 2e70 793a 4339  ...pynamer.py:C9
-00000760: 3031 0d0a 0962 7569 6c64 6572 2e70 793a  01...builder.py:
-00000770: 4339 3031 0d0a 0d0a 5b65 6767 5f69 6e66  C901....[egg_inf
-00000780: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000790: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000007a0: 0d0a                                     ..
+000002a0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
+000002b0: 4e53 450d 0a64 6f63 756d 656e 7461 7469  NSE..documentati
+000002c0: 6f6e 203d 2068 7474 7073 3a2f 2f70 796e  on = https://pyn
+000002d0: 616d 6572 2e72 6561 6474 6865 646f 6373  amer.readthedocs
+000002e0: 2e69 6f2f 656e 2f6c 6174 6573 742f 0d0a  .io/en/latest/..
+000002f0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000300: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
+00000310: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+00000320: 6374 696f 6e2f 5374 6162 6c65 0d0a 0945  ction/Stable...E
+00000330: 6e76 6972 6f6e 6d65 6e74 203a 3a20 436f  nvironment :: Co
+00000340: 6e73 6f6c 650d 0a09 496e 7465 6e64 6564  nsole...Intended
+00000350: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000360: 656c 6f70 6572 730d 0a09 4c69 6365 6e73  elopers...Licens
+00000370: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000380: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000390: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000003a0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000003b0: 6e64 656e 740d 0a09 4e61 7475 7261 6c20  ndent...Natural 
+000003c0: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
+000003d0: 6973 680d 0a09 5072 6f67 7261 6d6d 696e  ish...Programmin
+000003e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003f0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+00000400: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000410: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+00000420: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
+00000430: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000440: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000450: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000460: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000470: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+00000480: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000490: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000004a0: 310d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  1....[options]..
+000004b0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000004c0: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
+000004d0: 3d20 6669 6e64 3a0d 0a70 726f 6a65 6374  = find:..project
+000004e0: 5f75 726c 7320 3d20 0d0a 696e 636c 7564  _urls = ..includ
+000004f0: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+00000500: 2054 7275 650d 0a70 7974 686f 6e5f 7265   True..python_re
+00000510: 7175 6972 6573 203d 203e 3d33 2e39 0d0a  quires = >=3.9..
+00000520: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000530: 203d 200d 0a09 6273 340d 0a09 6275 696c   = ...bs4...buil
+00000540: 640d 0a09 636f 6c6f 7261 6d61 0d0a 096a  d...colorama...j
+00000550: 696e 6a61 320d 0a09 7061 636b 6167 696e  inja2...packagin
+00000560: 670d 0a09 7079 7468 6f6e 2d64 6174 6575  g...python-dateu
+00000570: 7469 6c0d 0a09 7079 7961 6d6c 0d0a 0972  til...pyyaml...r
+00000580: 6571 7565 7374 730d 0a09 7269 6368 0d0a  equests...rich..
+00000590: 0974 7164 6d0d 0a09 7477 696e 650d 0a09  .tqdm...twine...
+000005a0: 7768 6565 6c0d 0a0d 0a5b 6f70 7469 6f6e  wheel....[option
+000005b0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000005c0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+000005d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000005e0: 655f 6461 7461 5d0d 0a70 796e 616d 6572  e_data]..pynamer
+000005f0: 203d 200d 0a09 5245 4144 4d45 2e6d 640d   = ...README.md.
+00000600: 0a09 7072 6f6a 6563 745f 6e61 6d65 0d0a  ..project_name..
+00000610: 0970 726f 6a65 6374 5f6e 616d 652f 5f5f  .project_name/__
+00000620: 696e 6974 5f5f 2e70 790d 0a09 7365 7475  init__.py...setu
+00000630: 702e 7478 740d 0a09 7365 7475 705f 6261  p.txt...setup_ba
+00000640: 7365 2e74 7874 0d0a 0d0a 5b6f 7074 696f  se.txt....[optio
+00000650: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
+00000660: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
+00000670: 7320 3d20 0d0a 0970 796e 616d 6572 203d  s = ...pynamer =
+00000680: 2070 796e 616d 6572 2e70 796e 616d 6572   pynamer.pynamer
+00000690: 3a6d 6169 6e0d 0a0d 0a5b 666c 616b 6538  :main....[flake8
+000006a0: 5d0d 0a64 6f63 7374 7269 6e67 2d63 6f6e  ]..docstring-con
+000006b0: 7665 6e74 696f 6e20 3d20 6e75 6d70 790d  vention = numpy.
+000006c0: 0a6d 6178 2d63 6f6d 706c 6578 6974 7920  .max-complexity 
+000006d0: 3d20 3138 0d0a 6d61 782d 6c69 6e65 2d6c  = 18..max-line-l
+000006e0: 656e 6774 6820 3d20 3838 0d0a 7365 6c65  ength = 88..sele
+000006f0: 6374 203d 2042 2c20 4239 2c20 432c 2044  ct = B, B9, C, D
+00000700: 2c20 452c 2046 2c20 4e2c 2057 0d0a 6578  , E, F, N, W..ex
+00000710: 636c 7564 6520 3d20 7465 7374 732f 2a2c  clude = tests/*,
+00000720: 2e74 6f78 2f2a 2c2e 6e6f 782f 2a2c 646f  .tox/*,.nox/*,do
+00000730: 6373 2f2a 2c2e 6769 742f 2a2c 2e67 6974  cs/*,.git/*,.git
+00000740: 6875 622f 2a0d 0a69 676e 6f72 6520 3d20  hub/*..ignore = 
+00000750: 0d0a 0945 3230 332c 0d0a 0957 3530 332c  ...E203,...W503,
+00000760: 0d0a 7065 722d 6669 6c65 2d69 676e 6f72  ..per-file-ignor
+00000770: 6573 203d 200d 0a09 7079 6e61 6d65 722e  es = ...pynamer.
+00000780: 7079 3a43 3930 310d 0a09 6275 696c 6465  py:C901...builde
+00000790: 722e 7079 3a43 3930 310d 0a0d 0a5b 6567  r.py:C901....[eg
+000007a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000007b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000007c0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `pynamer-2.1.2/src/pynamer/__init__.py` & `pynamer-2.1.3/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.1.2"
+__version__ = "2.1.3"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.1.2/src/pynamer/builder.py` & `pynamer-2.1.3/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/src/pynamer/cli.py` & `pynamer-2.1.3/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/src/pynamer/config.py` & `pynamer-2.1.3/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/src/pynamer/pynamer.py` & `pynamer-2.1.3/src/pynamer/pynamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         logger.debug("project_list = %s", project_list)
     project_list.sort()
 
     # Main loop
     for new_project in project_list:
         if not _is_valid_package_name(new_project):
             _feedback(f"{new_project} is not a valid package name", "error")
+            _feedback("refer to PEP508 & PEP423 for more details", "warning")
             continue
 
         test_table = Table(title=f"Test Results for {new_project}", show_lines=True)
         test_table.add_column("No.", style="bold yellow")
         test_table.add_column("Test", style="bold cyan")
         test_table.add_column("Result")
         test_table.add_column("Details", style="bold cyan")
```

### Comparing `pynamer-2.1.2/src/pynamer/utils.py` & `pynamer-2.1.3/src/pynamer/utils.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/src/pynamer/validators.py` & `pynamer-2.1.3/src/pynamer/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Args:
         project_name:   the name of the project to test.
 
     Returns:
         True:           If the name passes the basic check
         False:          If the name fails the basic check
     """
-    pattern = r"^[a-z][_\-a-z0-9]*$"
+    pattern = re.compile("^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.I)
     if re.match(pattern, project_name) is not None:
         return True
     else:
         return False
 
 
 def _get_homepage(project_json: dict, project_name: str) -> tuple[str, str]:
@@ -268,15 +268,18 @@
     table.add_column("FINAL ANALYSIS", style="bold cyan")
     if pattern == [0, 1, 0]:
         table.add_row("[red]NOT AVAILABLE![/red]\n")
         table.add_row(
             "A Gotcha!, whereby the package is not found even with PyPI's own search"
             " facility.\n"
             "It can only be found by searching the simple index which is not available "
-            "through the interface"
+            "through the web interface.\n\n"
+            "The most likely cause is an abandoned or deleted project by the owner.\n\n"
+            "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
+            "to name transfer"
         )
     elif pattern == [1, 1, 0]:
         table.add_row("[red]NOT AVAILABLE![/red]\n")
         table.add_row(
             "A Gotcha!, whereby the package is not found even with PyPI's own search"
             " facility.\n"
             "However if appears in the simple index and can be displayed by simply"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pynamer-2.1.2/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.3/src/pynamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.2
+Version: 2.1.3
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-2.1.2/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.3/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_args.py` & `pynamer-2.1.3/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_build_dist.py` & `pynamer-2.1.3/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_cleanup.py` & `pynamer-2.1.3/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_create_setup_file.py` & `pynamer-2.1.3/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_defaults.py` & `pynamer-2.1.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_delete_director.py` & `pynamer-2.1.3/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_feedback.py` & `pynamer-2.1.3/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_final_analysis.py` & `pynamer-2.1.3/tests/test_final_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,86 @@
-#!/usr/bin/env python3
-# Core Library modules
-from pathlib import Path
-
-# Third party modules
-from rich.console import Console
-from rich.table import Table
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_final_analysis_010(capsys):
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    table.add_row("[red]NOT AVAILABLE![/red]\n")
-    table.add_row(
-        "A Gotcha!, whereby the package is not found even with PyPI's own search"
-        " facility.\n"
-        "It can only be found by searching the simple index which is not available "
-        "through the interface"
-    )
-    console = Console()
-    console.print(table)
-    captured_expected = capsys.readouterr()
-
-    pynamer._final_analysis([0, 1, 0])
-    captured_actual = capsys.readouterr()
-
-    assert captured_actual.out.strip() == captured_expected.out.strip()
-
-
-def test_final_analysis_110(capsys):
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    table.add_row("[red]NOT AVAILABLE![/red]\n")
-    table.add_row(
-        "A Gotcha!, whereby the package is not found even with PyPI's own search"
-        " facility.\n"
-        "However if appears in the simple index and can be displayed by simply"
-        " browsing "
-        "to the projects URL"
-    )
-    console = Console()
-    console.print(table)
-    captured_expected = capsys.readouterr()
-
-    pynamer._final_analysis([1, 1, 0])
-    captured_actual = capsys.readouterr()
-
-    assert captured_actual.out.strip() == captured_expected.out.strip()
-
-
-def test_final_analysis_001(capsys):
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    table.add_row("[red]NOT AVAILABLE![/red]\n")
-    table.add_row("The package name was found in at least one place")
-    console = Console()
-    console.print(table)
-    captured_expected = capsys.readouterr()
-
-    pynamer._final_analysis([0, 0, 1])
-    captured_actual = capsys.readouterr()
-
-    assert captured_actual.out.strip() == captured_expected.out.strip()
-
-
-def test_final_analysis_000(capsys):
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    table.add_row("[green]AVAILABLE![/green]\n")
-    table.add_row("The package name was not found in any part of PyPI")
-    console = Console()
-    console.print(table)
-    captured_expected = capsys.readouterr()
-
-    pynamer._final_analysis([0, 0, 0])
-    captured_actual = capsys.readouterr()
-
-    assert captured_actual.out.strip() == captured_expected.out.strip()
+#!/usr/bin/env python3
+# Core Library modules
+from pathlib import Path
+
+# Third party modules
+from rich.console import Console
+from rich.table import Table
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_final_analysis_010(capsys):
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    table.add_row("[red]NOT AVAILABLE![/red]\n")
+    table.add_row(
+        "A Gotcha!, whereby the package is not found even with PyPI's own search"
+        " facility.\n"
+        "It can only be found by searching the simple index which is not available "
+        "through the web interface.\n\n"
+        "The most likely cause is an abandoned or deleted project by the owner.\n\n"
+        "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
+        "to name transfer"
+    )
+    console = Console()
+    console.print(table)
+    captured_expected = capsys.readouterr()
+
+    pynamer._final_analysis([0, 1, 0])
+    captured_actual = capsys.readouterr()
+
+    assert captured_actual.out.strip() == captured_expected.out.strip()
+
+
+def test_final_analysis_110(capsys):
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    table.add_row("[red]NOT AVAILABLE![/red]\n")
+    table.add_row(
+        "A Gotcha!, whereby the package is not found even with PyPI's own search"
+        " facility.\n"
+        "However if appears in the simple index and can be displayed by simply"
+        " browsing "
+        "to the projects URL"
+    )
+    console = Console()
+    console.print(table)
+    captured_expected = capsys.readouterr()
+
+    pynamer._final_analysis([1, 1, 0])
+    captured_actual = capsys.readouterr()
+
+    assert captured_actual.out.strip() == captured_expected.out.strip()
+
+
+def test_final_analysis_001(capsys):
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    table.add_row("[red]NOT AVAILABLE![/red]\n")
+    table.add_row("The package name was found in at least one place")
+    console = Console()
+    console.print(table)
+    captured_expected = capsys.readouterr()
+
+    pynamer._final_analysis([0, 0, 1])
+    captured_actual = capsys.readouterr()
+
+    assert captured_actual.out.strip() == captured_expected.out.strip()
+
+
+def test_final_analysis_000(capsys):
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    table.add_row("[green]AVAILABLE![/green]\n")
+    table.add_row("The package name was not found in any part of PyPI")
+    console = Console()
+    console.print(table)
+    captured_expected = capsys.readouterr()
+
+    pynamer._final_analysis([0, 0, 0])
+    captured_actual = capsys.readouterr()
+
+    assert captured_actual.out.strip() == captured_expected.out.strip()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pynamer-2.1.2/tests/test_find_pypirc_file.py` & `pynamer-2.1.3/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_generate_pypi_index.py` & `pynamer-2.1.3/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_get_homepage.py` & `pynamer-2.1.3/tests/test_get_homepage.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_github_meta.py` & `pynamer-2.1.3/tests/test_github_meta.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_ping_json.py` & `pynamer-2.1.3/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_ping_project.py` & `pynamer-2.1.3/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_process_input_file.py` & `pynamer-2.1.3/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_pypi_search.py` & `pynamer-2.1.3/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_pypi_search_index.py` & `pynamer-2.1.3/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_rename_project_dir.py` & `pynamer-2.1.3/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_upload_dist.py` & `pynamer-2.1.3/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_utils_search_json.py` & `pynamer-2.1.3/tests/test_utils_search_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_utils_version.py` & `pynamer-2.1.3/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.2/tests/test_write_output_file.py` & `pynamer-2.1.3/tests/test_write_output_file.py`

 * *Files identical despite different names*

