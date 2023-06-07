# Comparing `tmp/gridworks-0.2.5.tar.gz` & `tmp/gridworks-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.5.tar", max compression
+gzip compressed data, was "gridworks-0.2.6.tar", max compression
```

## Comparing `gridworks-0.2.5.tar` & `gridworks-0.2.6.tar`

### file list

```diff
@@ -1,55 +1,58 @@
--rw-r--r--   0        0        0     1065 2023-06-07 14:02:46.338172 gridworks-0.2.5/LICENSE
--rw-r--r--   0        0        0     5778 2023-06-07 14:02:46.338172 gridworks-0.2.5/README.md
--rw-r--r--   0        0        0     2446 2023-06-07 14:02:58.782388 gridworks-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      249 2023-06-07 14:02:58.782388 gridworks-0.2.5/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/__main__.py
--rw-r--r--   0        0        0    47777 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2016 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0    23522 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/base_g_node.py
--rw-r--r--   0        0        0     6726 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6405 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0     5011 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/g_node_strategy.py
--rw-r--r--   0        0        0      694 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1214 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2547 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     2734 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/errors.py
--rw-r--r--   0        0        0     4187 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/message.py
--rw-r--r--   0        0        0    17029 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     1476 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    20321 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/types/base_g_node_gt.py
--rw-r--r--   0        0        0    24525 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-06-07 14:02:46.410173 gridworks-0.2.5/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0        0 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     5788 2023-06-07 14:02:46.414173 gridworks-0.2.5/src/gridworks/utils.py
--rw-r--r--   0        0        0     7273 1970-01-01 00:00:00.000000 gridworks-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-07 14:24:50.545067 gridworks-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5778 2023-06-07 14:24:50.545067 gridworks-0.2.6/README.md
+-rw-r--r--   0        0        0     2552 2023-06-07 14:25:03.549213 gridworks-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    47777 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6726 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6405 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0     5011 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/g_node_strategy.py
+-rw-r--r--   0        0        0      694 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1214 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2547 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     2734 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/errors.py
+-rw-r--r--   0        0        0     4187 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/utils.py
+-rw-r--r--   0        0        0      543 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks_test/__init__.py
+-rw-r--r--   0        0        0     2634 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks_test/stub_actors.py
+-rw-r--r--   0        0        0     2936 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks_test/wait.py
+-rw-r--r--   0        0        0     7269 1970-01-01 00:00:00.000000 gridworks-0.2.6/PKG-INFO
```

### Comparing `gridworks-0.2.5/LICENSE` & `gridworks-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/README.md` & `gridworks-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/pyproject.toml` & `gridworks-0.2.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.5"
+version = "0.2.6"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
+packages = [
+    { include = "gridworks", from = "src" },
+    { include = "gridworks_test", from = "src" },
+]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4.0"
```

### Comparing `gridworks-0.2.5/src/gridworks/actor_base.py` & `gridworks-0.2.6/src/gridworks/actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/algo_utils.py` & `gridworks-0.2.6/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/api_utils.py` & `gridworks-0.2.6/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/base_api_types.py` & `gridworks-0.2.6/src/gridworks/base_api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/base_g_node.py` & `gridworks-0.2.6/src/gridworks/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.6/src/gridworks/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.6/src/gridworks/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/g_node_strategy.py` & `gridworks-0.2.6/src/gridworks/data_classes/g_node_strategy.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.6/src/gridworks/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.6/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.6/src/gridworks/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.6/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/__init__.py` & `gridworks-0.2.6/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.6/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.6/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.6/src/gridworks/enums/g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.6/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/gni_status.py` & `gridworks-0.2.6/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.6/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.6/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.6/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/message_category.py` & `gridworks-0.2.6/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.6/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.6/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/strategy_name.py` & `gridworks-0.2.6/src/gridworks/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.6/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/enums/universe_type.py` & `gridworks-0.2.6/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/gw_config.py` & `gridworks-0.2.6/src/gridworks/gw_config.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/message.py` & `gridworks-0.2.6/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/property_format.py` & `gridworks-0.2.6/src/gridworks/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/rest_api.py` & `gridworks-0.2.6/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/__init__.py` & `gridworks-0.2.6/src/gridworks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/base_g_node_gt.py` & `gridworks-0.2.6/src/gridworks/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.6/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.6/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.6/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.6/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.6/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/ready.py` & `gridworks-0.2.6/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.6/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/super_starter.py` & `gridworks-0.2.6/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.6/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/src/gridworks/utils.py` & `gridworks-0.2.6/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.5/PKG-INFO` & `gridworks-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.5
+Version: 0.2.6
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocache[redis,memcached] (>=0.11.1,<0.12.0)
 Requires-Dist: aioredis (==1.3.1)
 Requires-Dist: beaker-pyteal (>=0.4.0,<0.5.0)
```

