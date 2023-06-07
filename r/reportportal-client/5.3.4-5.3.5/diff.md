# Comparing `tmp/reportportal-client-5.3.4.tar.gz` & `tmp/reportportal-client-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportportal-client-5.3.4.tar", last modified: Wed May 24 12:17:23 2023, max compression
+gzip compressed data, was "reportportal-client-5.3.5.tar", last modified: Wed Jun  7 14:25:32 2023, max compression
```

## Comparing `reportportal-client-5.3.4.tar` & `reportportal-client-5.3.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.734690 reportportal-client-5.3.4/reportportal_client/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.734690 reportportal-client-5.3.4/reportportal_client/_local/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19275 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.738690 reportportal-client-5.3.4/reportportal_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/rp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/rp_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/rp_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/rp_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.738690 reportportal-client-5.3.4/reportportal_client/items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/item_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_base_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.738690 reportportal-client-5.3.4/reportportal_client/items/rp_log_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_log_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_log_items/rp_log_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.738690 reportportal-client-5.3.4/reportportal_client/items/rp_test_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_test_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_test_items/rp_base_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_test_items/rp_child_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/items/rp_test_items/rp_root_test_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/reportportal_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/logs/log_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/reportportal_client/services/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/services/client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/services/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/services/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/reportportal_client/static/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/static/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/static/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/static/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/reportportal_client/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/reportportal_client/steps/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.734690 reportportal-client-5.3.4/reportportal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-24 12:17:23.000000 reportportal-client-5.3.4/reportportal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-24 12:17:23.000000 reportportal-client-5.3.4/reportportal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:17:23.000000 reportportal-client-5.3.4/reportportal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 12:17:23.000000 reportportal-client-5.3.4/reportportal_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 12:17:23.000000 reportportal-client-5.3.4/reportportal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 12:17:23.746690 reportportal-client-5.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:17:23.742690 reportportal-client-5.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/tests/test_client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-24 12:17:18.000000 reportportal-client-5.3.4/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-07 14:25:32.206095 reportportal-client-5.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.194094 reportportal-client-5.3.5/reportportal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21241 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/item_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_base_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/items/rp_log_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_log_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_log_items/rp_log_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_base_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_child_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_root_test_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/logs/log_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/steps/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.194094 reportportal-client-5.3.5/reportportal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 14:25:32.206095 reportportal-client-5.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_statistics.py
```

### Comparing `reportportal-client-5.3.4/CONTRIBUTING.rst` & `reportportal-client-5.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/LICENSE.md` & `reportportal-client-5.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/PKG-INFO` & `reportportal-client-5.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.4
+Version: 5.3.5
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.4
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.5
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -55,21 +55,21 @@
 
 from reportportal_client import RPClient
 from reportportal_client.helpers import timestamp
 
 endpoint = "http://docker.local:8080"
 project = "default"
 # You can get UUID from user profile page in the Report Portal.
-token = "1adf271d-505f-44a8-ad71-0afbdf8c83bd"
+api_key = "1adf271d-505f-44a8-ad71-0afbdf8c83bd"
 launch_name = "Test launch"
 launch_doc = "Testing logging with attachment."
 
 
 client = RPClient(endpoint=endpoint, project=project,
-                  token=token)
+                  api_key=api_key)
 
 # Start log upload thread
 client.start()
 
 # Start launch.
 launch = client.start_launch(name=launch_name,
                              start_time=timestamp(),
```

### Comparing `reportportal-client-5.3.4/README.md` & `reportportal-client-5.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 
 from reportportal_client import RPClient
 from reportportal_client.helpers import timestamp
 
 endpoint = "http://docker.local:8080"
 project = "default"
 # You can get UUID from user profile page in the Report Portal.
-token = "1adf271d-505f-44a8-ad71-0afbdf8c83bd"
+api_key = "1adf271d-505f-44a8-ad71-0afbdf8c83bd"
 launch_name = "Test launch"
 launch_doc = "Testing logging with attachment."
 
 
 client = RPClient(endpoint=endpoint, project=project,
-                  token=token)
+                  api_key=api_key)
 
 # Start log upload thread
 client.start()
 
 # Start launch.
 launch = client.start_launch(name=launch_name,
                              start_time=timestamp(),
```

### Comparing `reportportal-client-5.3.4/reportportal_client/__init__.py` & `reportportal-client-5.3.5/reportportal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/_local/__init__.py` & `reportportal-client-5.3.5/reportportal_client/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/client.py` & `reportportal-client-5.3.5/reportportal_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 import logging
+import warnings
 from os import getenv
 
 import requests
 from requests.adapters import HTTPAdapter, Retry, DEFAULT_RETRIES
 
 from ._local import set_current
 from .core.rp_requests import (
@@ -47,30 +48,30 @@
     NOTICE: the class is not thread-safe, use new class instance for every new
     thread to avoid request/response messing and other issues.
     """
 
     def __init__(self,
                  endpoint,
                  project,
-                 token,
+                 api_key=None,
                  log_batch_size=20,
                  is_skipped_an_issue=True,
                  verify_ssl=True,
                  retries=None,
                  max_pool_size=50,
                  launch_id=None,
                  http_timeout=(10, 10),
                  log_batch_payload_size=MAX_LOG_BATCH_PAYLOAD_SIZE,
                  mode='DEFAULT',
-                 **_):
+                 **kwargs):
         """Initialize required attributes.
 
         :param endpoint:               Endpoint of the report portal service
         :param project:                Project name to report to
-        :param token:                  Authorization token
+        :param api_key:                Authorization API key
         :param log_batch_size:         Option to set the maximum number of
                                        logs that can be processed in one batch
         :param is_skipped_an_issue:    Option to mark skipped tests as not
                                        'To Investigate' items on the server
                                        side
         :param verify_ssl:             Option to skip ssl verification
         :param max_pool_size:          Option to set the maximum number of
@@ -92,41 +93,70 @@
             self.endpoint, 'api/{}'.format(self.api_v1), self.project)
         self.base_url_v2 = uri_join(
             self.endpoint, 'api/{}'.format(self.api_v2), self.project)
         self.is_skipped_an_issue = is_skipped_an_issue
         self.launch_id = launch_id
         self.log_batch_size = log_batch_size
         self.log_batch_payload_size = log_batch_payload_size
-        self.token = token
         self.verify_ssl = verify_ssl
         self.retries = retries
         self.max_pool_size = max_pool_size
         self.http_timeout = http_timeout
-        self.session = requests.Session()
         self.step_reporter = StepReporter(self)
         self._item_stack = []
         self.mode = mode
         self._skip_analytics = getenv('AGENT_NO_ANALYTICS')
 
+        self.api_key = api_key
+        if not self.api_key:
+            if 'token' in kwargs:
+                warnings.warn(
+                    message="Argument `token` is deprecated since 5.3.5 and "
+                            "will be subject for removing in the next major "
+                            "version. Use `api_key` argument instead.",
+                    category=DeprecationWarning,
+                    stacklevel=2
+                )
+                self.api_key = kwargs['token']
+
+            if not self.api_key:
+                warnings.warn(
+                    message="Argument `api_key` is `None` or empty string, "
+                            "that's not supposed to happen because Report "
+                            "Portal is usually requires an authorization key. "
+                            "Please check your code.",
+                    category=RuntimeWarning,
+                    stacklevel=2
+                )
+
+        self.__init_session()
+        self.__init_log_manager()
+
+    def __init_session(self):
         retry_strategy = Retry(
-            total=retries,
+            total=self.retries,
             backoff_factor=0.1,
             status_forcelist=[429, 500, 502, 503, 504]
-        ) if retries else DEFAULT_RETRIES
-        self.session.mount('https://', HTTPAdapter(
-            max_retries=retry_strategy, pool_maxsize=max_pool_size))
+        ) if self.retries else DEFAULT_RETRIES
+        session = requests.Session()
+        session.mount('https://', HTTPAdapter(
+            max_retries=retry_strategy, pool_maxsize=self.max_pool_size))
         # noinspection HttpUrlsUsage
-        self.session.mount('http://', HTTPAdapter(
-            max_retries=retry_strategy, pool_maxsize=max_pool_size))
-        self.session.headers['Authorization'] = 'bearer {0}'.format(self.token)
+        session.mount('http://', HTTPAdapter(
+            max_retries=retry_strategy, pool_maxsize=self.max_pool_size))
+        if self.api_key:
+            session.headers['Authorization'] = 'Bearer {0}'.format(
+                self.api_key)
+        self.session = session
 
+    def __init_log_manager(self):
         self._log_manager = LogManager(
             self.endpoint, self.session, self.api_v2, self.launch_id,
-            self.project, max_entry_number=log_batch_size,
-            max_payload_size=log_batch_payload_size,
+            self.project, max_entry_number=self.log_batch_size,
+            max_payload_size=self.log_batch_payload_size,
             verify_ssl=self.verify_ssl)
 
     def finish_launch(self,
                       end_time,
                       status=None,
                       attributes=None,
                       **kwargs):
@@ -270,15 +300,15 @@
 
     def get_project_settings(self):
         """Get project settings.
 
         :return: HTTP response in dictionary
         """
         url = uri_join(self.base_url_v1, 'settings')
-        response = HttpRequest(self.session.get, url=url, json={},
+        response = HttpRequest(self.session.get, url=url,
                                verify_ssl=self.verify_ssl).make()
         return response.json if response else None
 
     def log(self, time, message, level=None, attachment=None, item_id=None):
         """Send log message to the Report Portal.
 
         :param time:       Time in UTC
@@ -459,22 +489,46 @@
 
         :returns: Cloned client object
         :rtype: RPClient
         """
         cloned = RPClient(
             endpoint=self.endpoint,
             project=self.project,
-            token=self.token,
+            api_key=self.api_key,
             log_batch_size=self.log_batch_size,
             is_skipped_an_issue=self.is_skipped_an_issue,
             verify_ssl=self.verify_ssl,
             retries=self.retries,
             max_pool_size=self.max_pool_size,
             launch_id=self.launch_id,
             http_timeout=self.http_timeout,
             log_batch_payload_size=self.log_batch_payload_size,
             mode=self.mode
         )
         current_item = self.current_item()
         if current_item:
             cloned._item_stack.append(current_item)
         return cloned
+
+    def __getstate__(self):
+        """Control object pickling and return object fields as Dictionary.
+
+        :returns: object state dictionary
+        :rtype: dict
+        """
+        state = self.__dict__.copy()
+        # Don't pickle 'session' field, since it contains unpickling 'socket'
+        del state['session']
+        # Don't pickle '_log_manager' field, since it uses 'session' field
+        del state['_log_manager']
+        return state
+
+    def __setstate__(self, state):
+        """Control object pickling, receives object state as Dictionary.
+
+        :param dict state: object state dictionary
+        """
+        self.__dict__.update(state)
+        # Restore 'session' field
+        self.__init_session()
+        # Restore '_log_manager' field
+        self.__init_log_manager()
```

### Comparing `reportportal-client-5.3.4/reportportal_client/client.pyi` & `reportportal-client-5.3.5/reportportal_client/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,55 +3,57 @@
 from requests import Session
 
 from reportportal_client.core.rp_issues import Issue as Issue
 from reportportal_client.logs.log_manager import LogManager as LogManager
 from reportportal_client.steps import StepReporter
 
 
-def current() -> RPClient: ...
-
-
 class RPClient:
     _log_manager: LogManager = ...
     api_v1: Text = ...
     api_v2: Text = ...
     base_url_v1: Text = ...
     base_url_v2: Text = ...
     endpoint: Text = ...
     is_skipped_an_issue: bool = ...
     launch_id: Text = ...
     log_batch_size: int = ...
     log_batch_payload_size: int = ...
     project: Text = ...
-    token: Text = ...
+    api_key: Text = ...
     verify_ssl: bool = ...
     retries: int = ...
     max_pool_size: int = ...
     http_timeout: Union[float, Tuple[float, float]] = ...
     session: Session = ...
     step_reporter: StepReporter = ...
     mode: str = ...
     _skip_analytics: Text = ...
     _item_stack: List[Text] = ...
 
     def __init__(
             self,
             endpoint: Text,
-            project: Text, token: Text,
+            project: Text,
+            api_key: Text,
             log_batch_size: int = ...,
             is_skipped_an_issue: bool = ...,
             verify_ssl: bool = ...,
             retries: int = ...,
             max_pool_size: int = ...,
             launch_id: Text = ...,
             http_timeout: Union[float, Tuple[float, float]] = ...,
             log_batch_payload_size: int = ...,
             mode: str = ...
     ) -> None: ...
 
+    def __init_session(self) -> None: ...
+
+    def __init_log_manager(self) -> None: ...
+
     def finish_launch(self,
                       end_time: Text,
                       status: Text = ...,
                       attributes: Optional[Union[List, Dict]] = ...,
                       **kwargs: Any) -> Dict: ...
 
     def finish_test_item(self,
@@ -105,10 +107,10 @@
 
     def update_test_item(self, item_uuid: Text,
                          attributes: Optional[Union[List, Dict]],
                          description: Optional[Text]) -> Text: ...
 
     def current_item(self) -> Text: ...
 
-    def start(self) -> None : ...
+    def start(self) -> None: ...
 
     def clone(self) -> RPClient: ...
```

### Comparing `reportportal-client-5.3.4/reportportal_client/core/__init__.py` & `reportportal-client-5.3.5/reportportal_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/core/rp_file.py` & `reportportal-client-5.3.5/reportportal_client/core/rp_file.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/core/rp_issues.py` & `reportportal-client-5.3.5/reportportal_client/core/rp_issues.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/core/rp_requests.py` & `reportportal-client-5.3.5/reportportal_client/core/rp_requests.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/core/rp_responses.py` & `reportportal-client-5.3.5/reportportal_client/core/rp_responses.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/core/test_manager.py` & `reportportal-client-5.3.5/reportportal_client/core/test_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/core/worker.py` & `reportportal-client-5.3.5/reportportal_client/core/worker.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/errors.py` & `reportportal-client-5.3.5/reportportal_client/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/helpers.py` & `reportportal-client-5.3.5/reportportal_client/helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/helpers.pyi` & `reportportal-client-5.3.5/reportportal_client/helpers.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/__init__.py` & `reportportal-client-5.3.5/reportportal_client/items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/item_weight.py` & `reportportal-client-5.3.5/reportportal_client/items/item_weight.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_base_item.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_base_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_log_items/__init__.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_log_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_log_items/rp_log_item.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_log_items/rp_log_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_test_items/__init__.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_test_items/rp_base_test_item.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_base_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_test_items/rp_child_test_item.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_child_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/items/rp_test_items/rp_root_test_item.py` & `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_root_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/logs/__init__.py` & `reportportal-client-5.3.5/reportportal_client/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/logs/log_manager.py` & `reportportal-client-5.3.5/reportportal_client/logs/log_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/services/__init__.py` & `reportportal-client-5.3.5/reportportal_client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/services/client_id.py` & `reportportal-client-5.3.5/reportportal_client/services/client_id.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/services/constants.py` & `reportportal-client-5.3.5/reportportal_client/services/constants.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/services/statistics.py` & `reportportal-client-5.3.5/reportportal_client/services/statistics.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/static/__init__.py` & `reportportal-client-5.3.5/reportportal_client/static/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/static/abstract.py` & `reportportal-client-5.3.5/reportportal_client/static/abstract.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/static/defines.py` & `reportportal-client-5.3.5/reportportal_client/static/defines.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/static/errors.py` & `reportportal-client-5.3.5/reportportal_client/static/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/steps/__init__.py` & `reportportal-client-5.3.5/reportportal_client/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client/steps/__init__.pyi` & `reportportal-client-5.3.5/reportportal_client/steps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/reportportal_client.egg-info/PKG-INFO` & `reportportal-client-5.3.5/reportportal_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.4
+Version: 5.3.5
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.4
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.5
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -55,21 +55,21 @@
 
 from reportportal_client import RPClient
 from reportportal_client.helpers import timestamp
 
 endpoint = "http://docker.local:8080"
 project = "default"
 # You can get UUID from user profile page in the Report Portal.
-token = "1adf271d-505f-44a8-ad71-0afbdf8c83bd"
+api_key = "1adf271d-505f-44a8-ad71-0afbdf8c83bd"
 launch_name = "Test launch"
 launch_doc = "Testing logging with attachment."
 
 
 client = RPClient(endpoint=endpoint, project=project,
-                  token=token)
+                  api_key=api_key)
 
 # Start log upload thread
 client.start()
 
 # Start launch.
 launch = client.start_launch(name=launch_name,
                              start_time=timestamp(),
```

### Comparing `reportportal-client-5.3.4/reportportal_client.egg-info/SOURCES.txt` & `reportportal-client-5.3.5/reportportal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/setup.py` & `reportportal-client-5.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config for setup package client Python."""
 
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '5.3.4'
+__version__ = '5.3.5'
 
 TYPE_STUBS = ['*.pyi']
 
 
 def read_file(fname):
     """Read the given file.
```

### Comparing `reportportal-client-5.3.4/tests/test_client.py` & `reportportal-client-5.3.5/tests/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,48 +121,78 @@
     assert rp_client.get_launch_ui_url() == expected_url
 
 
 @mock.patch('reportportal_client.client.getenv')
 @mock.patch('reportportal_client.client.send_event')
 def test_skip_statistics(send_event, getenv):
     getenv.return_value = '1'
-    client = RPClient('http://endpoint', 'project', 'token')
+    client = RPClient('http://endpoint', 'project', 'api_key')
     client.session = mock.Mock()
     client.start_launch('Test Launch', timestamp())
     assert mock.call('start_launch', None, None) not in send_event.mock_calls
 
 
 @mock.patch('reportportal_client.client.getenv')
 @mock.patch('reportportal_client.client.send_event')
 def test_statistics(send_event, getenv):
     getenv.return_value = ''
-    client = RPClient('http://endpoint', 'project', 'token')
+    client = RPClient('http://endpoint', 'project', 'api_key')
     client.session = mock.Mock()
     client.start_launch('Test Launch', timestamp())
     assert mock.call('start_launch', None, None) in send_event.mock_calls
 
 
 def test_clone():
-    args = ['http://endpoint', 'project', 'token']
-    kwargs = {'log_batch_size': 30, 'is_skipped_an_issue': False,
-              'verify_ssl': False, 'retries': 5,
+    args = ['http://endpoint', 'project']
+    kwargs = {'api_key': 'api_key', 'log_batch_size': 30,
+              'is_skipped_an_issue': False, 'verify_ssl': False, 'retries': 5,
               'max_pool_size': 30, 'launch_id': 'test-123',
               'http_timeout': (30, 30),
               'log_batch_payload_size': 1000000, 'mode': 'DEBUG'}
     client = RPClient(*args, **kwargs)
     client._item_stack.append('test-321')
     client._item_stack.append('test-322')
     cloned = client.clone()
     assert cloned is not None and client is not cloned
-    assert cloned.endpoint == args[0] and cloned.project == args[
-        1] and cloned.token == args[2]
-    assert cloned.log_batch_size == kwargs[
-        'log_batch_size'] and cloned.is_skipped_an_issue == kwargs[
+    assert cloned.endpoint == args[0] and cloned.project == args[1]
+    assert cloned.api_key == kwargs[
+        'api_key'] and cloned.log_batch_size == kwargs[
+               'log_batch_size'] and cloned.is_skipped_an_issue == kwargs[
                'is_skipped_an_issue'] and cloned.verify_ssl == kwargs[
                'verify_ssl'] and cloned.retries == kwargs[
                'retries'] and cloned.max_pool_size == kwargs[
                'max_pool_size'] and cloned.launch_id == kwargs[
                'launch_id'] and cloned.http_timeout == kwargs[
                'http_timeout'] and cloned.log_batch_payload_size == kwargs[
                'log_batch_payload_size'] and cloned.mode == kwargs['mode']
     assert len(cloned._item_stack) == 1 \
            and client.current_item() == cloned.current_item()
+
+
+@mock.patch('reportportal_client.client.warnings.warn')
+def test_deprecated_token_argument(warn):
+    api_key = 'api_key'
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      token=api_key)
+
+    assert warn.call_count == 1
+    assert client.api_key == api_key
+
+
+@mock.patch('reportportal_client.client.warnings.warn')
+def test_api_key_argument(warn):
+    api_key = 'api_key'
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      api_key=api_key)
+
+    assert warn.call_count == 0
+    assert client.api_key == api_key
+
+
+@mock.patch('reportportal_client.client.warnings.warn')
+def test_empty_api_key_argument(warn):
+    api_key = ''
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      api_key=api_key)
+
+    assert warn.call_count == 1
+    assert client.api_key == api_key
```

### Comparing `reportportal-client-5.3.4/tests/test_client_id.py` & `reportportal-client-5.3.5/tests/test_client_id.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/tests/test_helpers.py` & `reportportal-client-5.3.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.4/tests/test_statistics.py` & `reportportal-client-5.3.5/tests/test_statistics.py`

 * *Files identical despite different names*

