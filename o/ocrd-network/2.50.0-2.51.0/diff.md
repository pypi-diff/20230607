# Comparing `tmp/ocrd_network-2.50.0.tar.gz` & `tmp/ocrd_network-2.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrd_network-2.50.0.tar", last modified: Mon Apr 24 11:39:59 2023, max compression
+gzip compressed data, was "ocrd_network-2.51.0.tar", last modified: Wed Jun  7 11:27:39 2023, max compression
```

## Comparing `ocrd_network-2.50.0.tar` & `ocrd_network-2.51.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/
--rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)       85 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/README.md
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/ocrd_network/
--rw-rw-r--   0 kba       (1000) kba       (1000)     1824 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3284 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/database.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    13670 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/deployer.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3115 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/deployment_config.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     5209 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/deployment_utils.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/ocrd_network/models/
--rw-rw-r--   0 kba       (1000) kba       (1000)      368 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/models/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2304 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/models/job.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      293 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/models/ocrd_tool.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      976 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/models/workspace.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1285 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/param_validators.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    12949 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/processing_server.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    15391 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/processing_worker.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/
--rw-rw-r--   0 kba       (1000) kba       (1000)      299 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     9224 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/connector.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1098 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/constants.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3252 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/consumer.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4239 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/ocrd_messages.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4149 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/publisher.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2300 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/ocrd_network/utils.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/ocrd_network.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-04-24 11:39:59.000000 ocrd_network-2.50.0/ocrd_network.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)      835 2023-04-24 11:39:59.000000 ocrd_network-2.50.0/ocrd_network.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2023-04-24 11:39:59.000000 ocrd_network-2.50.0/ocrd_network.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       96 2023-04-24 11:39:59.000000 ocrd_network-2.50.0/ocrd_network.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       13 2023-04-24 11:39:59.000000 ocrd_network-2.50.0/ocrd_network.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2023-04-24 11:39:59.450320 ocrd_network-2.50.0/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      789 2023-04-02 14:17:57.000000 ocrd_network-2.50.0/setup.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.596478 ocrd_network-2.51.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-06-07 11:27:39.592478 ocrd_network-2.51.0/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)       85 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.580478 ocrd_network-2.51.0/ocrd_network/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1824 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3284 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/database.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    13670 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/deployer.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3115 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/deployment_config.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     5209 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/deployment_utils.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.588478 ocrd_network-2.51.0/ocrd_network/models/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      368 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2304 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/job.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      293 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/ocrd_tool.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      976 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/workspace.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1285 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/param_validators.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    12949 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/processing_server.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    15391 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/processing_worker.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.592478 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      299 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     9224 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/connector.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1098 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/constants.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3252 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/consumer.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4239 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/ocrd_messages.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4149 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/publisher.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2300 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/utils.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.580478 ocrd_network-2.51.0/ocrd_network.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)      835 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       96 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       13 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2023-06-07 11:27:39.596478 ocrd_network-2.51.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      789 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/setup.py
```

### Comparing `ocrd_network-2.50.0/ocrd_network/__init__.py` & `ocrd_network-2.51.0/ocrd_network/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/database.py` & `ocrd_network-2.51.0/ocrd_network/database.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/deployer.py` & `ocrd_network-2.51.0/ocrd_network/deployer.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/deployment_config.py` & `ocrd_network-2.51.0/ocrd_network/deployment_config.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/deployment_utils.py` & `ocrd_network-2.51.0/ocrd_network/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/models/job.py` & `ocrd_network-2.51.0/ocrd_network/models/job.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/models/workspace.py` & `ocrd_network-2.51.0/ocrd_network/models/workspace.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/param_validators.py` & `ocrd_network-2.51.0/ocrd_network/param_validators.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/processing_server.py` & `ocrd_network-2.51.0/ocrd_network/processing_server.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/processing_worker.py` & `ocrd_network-2.51.0/ocrd_network/processing_worker.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/connector.py` & `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/connector.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/constants.py` & `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/constants.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/consumer.py` & `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/consumer.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/ocrd_messages.py` & `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/ocrd_messages.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/rabbitmq_utils/publisher.py` & `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/publisher.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network/utils.py` & `ocrd_network-2.51.0/ocrd_network/utils.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/ocrd_network.egg-info/SOURCES.txt` & `ocrd_network-2.51.0/ocrd_network.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.50.0/setup.py` & `ocrd_network-2.51.0/setup.py`

 * *Files identical despite different names*

