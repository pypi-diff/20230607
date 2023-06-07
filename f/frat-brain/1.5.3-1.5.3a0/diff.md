# Comparing `tmp/frat_brain-1.5.3.tar.gz` & `tmp/frat_brain-1.5.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.5.3.tar", max compression
+gzip compressed data, was "frat_brain-1.5.3a0.tar", max compression
```

## Comparing `frat_brain-1.5.3.tar` & `frat_brain-1.5.3a0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.3/LICENSE
--rw-r--r--   0        0        0     3354 2023-06-07 15:46:02.204928 frat_brain-1.5.3/README.md
--rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.3/fRAT/.DS_Store
--rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.3/fRAT/HOUSE/__init__.py
--rw-r--r--   0        0        0      539 2023-05-17 16:08:32.624385 frat_brain-1.5.3/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6154 2023-05-18 10:54:31.552312 frat_brain-1.5.3/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
--rw-r--r--   0        0        0     1732 2023-05-18 10:54:31.593176 frat_brain-1.5.3/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
--rw-r--r--   0        0        0     3402 2023-05-17 16:08:32.709491 frat_brain-1.5.3/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
--rw-r--r--   0        0        0     2339 2023-05-18 10:54:31.598566 frat_brain-1.5.3/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
--rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.3/fRAT/HOUSE/add_motion.py
--rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.3/fRAT/HOUSE/add_noise.py
--rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.3/fRAT/HOUSE/handler.py
--rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.3/fRAT/HOUSE/separate_noise_volumes.py
--rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.3/fRAT/__main__.py
--rw-r--r--   0        0        0       82 2023-06-07 16:11:40.286032 frat_brain-1.5.3/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.3/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.3/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4473 2023-05-25 16:05:08.824208 frat_brain-1.5.3/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.3/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.3/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17991 2023-05-25 15:58:53.843682 frat_brain-1.5.3/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.3/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.3/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.3/fRAT/nogui.py
--rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.3/fRAT/utils/.DS_Store
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.3/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.3/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.3/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.3/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.3/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17651 2023-05-17 16:08:16.861001 frat_brain-1.5.3/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.3/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.3/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.3/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.3/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0     9315 2023-05-17 16:16:18.839737 frat_brain-1.5.3/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5726 2023-05-17 16:08:29.826539 frat_brain-1.5.3/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    15290 2023-05-18 10:45:31.348301 frat_brain-1.5.3/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.3/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.3/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.3/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.3/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.3/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.3/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.3/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.3/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.3/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.3/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    13137 2023-05-17 16:16:14.911516 frat_brain-1.5.3/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.3/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    19312 2023-05-18 10:45:29.419506 frat_brain-1.5.3/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-06-07 16:09:14.641346 frat_brain-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     6306 1970-01-01 00:00:00.000000 frat_brain-1.5.3/setup.py
--rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 frat_brain-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.3a0/LICENSE
+-rw-r--r--   0        0        0     3354 2023-06-07 15:46:02.204928 frat_brain-1.5.3a0/README.md
+-rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.3a0/fRAT/.DS_Store
+-rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.3a0/fRAT/HOUSE/__init__.py
+-rw-r--r--   0        0        0      539 2023-05-17 16:08:32.624385 frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6154 2023-05-18 10:54:31.552312 frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
+-rw-r--r--   0        0        0     1732 2023-05-18 10:54:31.593176 frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
+-rw-r--r--   0        0        0     3402 2023-05-17 16:08:32.709491 frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
+-rw-r--r--   0        0        0     2339 2023-05-18 10:54:31.598566 frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
+-rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.3a0/fRAT/HOUSE/add_motion.py
+-rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.3a0/fRAT/HOUSE/add_noise.py
+-rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.3a0/fRAT/HOUSE/handler.py
+-rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.3a0/fRAT/HOUSE/separate_noise_volumes.py
+-rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.3a0/fRAT/__main__.py
+-rw-r--r--   0        0        0      211 2023-06-07 15:45:49.585255 frat_brain-1.5.3a0/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.3a0/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.3a0/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4473 2023-05-25 16:05:08.824208 frat_brain-1.5.3a0/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.3a0/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.3a0/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-25 15:58:53.843682 frat_brain-1.5.3a0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.3a0/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.3a0/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.3a0/fRAT/nogui.py
+-rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.3a0/fRAT/utils/.DS_Store
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.3a0/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.3a0/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.3a0/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.3a0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.3a0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17651 2023-05-17 16:08:16.861001 frat_brain-1.5.3a0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.3a0/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.3a0/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.3a0/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.3a0/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0     9315 2023-05-17 16:16:18.839737 frat_brain-1.5.3a0/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5726 2023-05-17 16:08:29.826539 frat_brain-1.5.3a0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    15290 2023-05-18 10:45:31.348301 frat_brain-1.5.3a0/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.3a0/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.3a0/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.3a0/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.3a0/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.3a0/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.3a0/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.3a0/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.3a0/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.3a0/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.3a0/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    13137 2023-05-17 16:16:14.911516 frat_brain-1.5.3a0/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.3a0/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    19312 2023-05-18 10:45:29.419506 frat_brain-1.5.3a0/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2421 2023-06-07 15:46:10.556485 frat_brain-1.5.3a0/pyproject.toml
+-rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 frat_brain-1.5.3a0/setup.py
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 frat_brain-1.5.3a0/PKG-INFO
```

### Comparing `frat_brain-1.5.3/LICENSE` & `frat_brain-1.5.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/README.md` & `frat_brain-1.5.3a0/README.md`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/.DS_Store` & `frat_brain-1.5.3a0/fRAT/.DS_Store`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/add_motion.py` & `frat_brain-1.5.3a0/fRAT/HOUSE/add_motion.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/add_noise.py` & `frat_brain-1.5.3a0/fRAT/HOUSE/add_noise.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/handler.py` & `frat_brain-1.5.3a0/fRAT/HOUSE/handler.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/HOUSE/separate_noise_volumes.py` & `frat_brain-1.5.3a0/fRAT/HOUSE/separate_noise_volumes.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/__main__.py` & `frat_brain-1.5.3a0/fRAT/__main__.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.5.3a0/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.5.3a0/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.5.3a0/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.5.3a0/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.5.3a0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.5.3a0/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/images/fRAT.gif` & `frat_brain-1.5.3a0/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/nogui.py` & `frat_brain-1.5.3a0/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/.DS_Store` & `frat_brain-1.5.3a0/fRAT/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.5.3a0/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/analysis.py` & `frat_brain-1.5.3a0/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/bootstrap.css` & `frat_brain-1.5.3a0/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/dash_report.py` & `frat_brain-1.5.3a0/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/directory_comparison.py` & `frat_brain-1.5.3a0/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.5.3a0/fRAT/utils/fRAT_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/figures.py` & `frat_brain-1.5.3a0/fRAT/utils/figures.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/html_report.py` & `frat_brain-1.5.3a0/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/printResults.py` & `frat_brain-1.5.3a0/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/statistics.py` & `frat_brain-1.5.3a0/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/statmap.py` & `frat_brain-1.5.3a0/fRAT/utils/statmap.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.5.3a0/fRAT/utils/statmap_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/fRAT/utils/utils.py` & `frat_brain-1.5.3a0/fRAT/utils/utils.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.3/pyproject.toml` & `frat_brain-1.5.3a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.5.3"
+version = "1.5.3a0"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
+include = ["pyproject.toml"]
 
 [tool.poetry.scripts]
 fRAT = 'fRAT.__main__:start_gui'
 
 [tool.poetry.dependencies]
 python = "~3.10"
 altgraph = "0.17.2"
```

### Comparing `frat_brain-1.5.3/setup.py` & `frat_brain-1.5.3a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.5.3',
+    'version': '1.5.3a0',
     'description': 'Application for ROI fMRI data analysis.',
     'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Citation\n\n**When using fRAT, please include the following citation:**\n\nHowley, E., Francis, S., & Schluppeck, D. (2023). fRAT: an interactive, Python-based tool for region-of-interest summaries of functional imaging data. Journal of Open Source Software, 8(85), 5200. https://doi.org/10.21105/joss.05200\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
```

### Comparing `frat_brain-1.5.3/PKG-INFO` & `frat_brain-1.5.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.5.3
+Version: 1.5.3a0
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

