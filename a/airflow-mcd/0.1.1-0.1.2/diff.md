# Comparing `tmp/airflow_mcd-0.1.1.tar.gz` & `tmp/airflow_mcd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.1.tar", last modified: Mon May 29 14:17:18 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.2.tar", last modified: Wed Jun  7 15:57:22 2023, max compression
```

## Comparing `airflow_mcd-0.1.1.tar` & `airflow_mcd-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     6655 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     6669 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     4695 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/operators/circuit_breaker_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12943 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/operators/test_circuit_breaker_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.670499 airflow_mcd-0.1.2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.670499 airflow_mcd-0.1.2/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.670499 airflow_mcd-0.1.2/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.670499 airflow_mcd-0.1.2/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     6967 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     4759 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.670499 airflow_mcd-0.1.2/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/airflow_mcd/operators/circuit_breaker_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.670499 airflow_mcd-0.1.2/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-07 15:57:22.000000 airflow_mcd-0.1.2/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-06-07 15:57:22.000000 airflow_mcd-0.1.2/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 15:57:22.000000 airflow_mcd-0.1.2/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-07 15:57:22.000000 airflow_mcd-0.1.2/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-07 15:57:22.000000 airflow_mcd-0.1.2/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12943 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:57:22.674499 airflow_mcd-0.1.2/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-06-07 15:56:17.000000 airflow_mcd-0.1.2/tests/operators/test_circuit_breaker_op.py
```

### Comparing `airflow_mcd-0.1.1/.circleci/config.yml` & `airflow_mcd-0.1.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/.gitignore` & `airflow_mcd-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/LICENSE` & `airflow_mcd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/Makefile` & `airflow_mcd-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/PKG-INFO` & `airflow_mcd-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.1/README-dev.md` & `airflow_mcd-0.1.2/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/README.md` & `airflow_mcd-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.2/airflow_mcd/callbacks/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import logging
 
 from dataclasses import dataclass, field
 from typing import Optional, List, Dict
 
 from dataclasses_json import dataclass_json
+from pycarlo.common.retries import ExponentialBackoff
 from pycarlo.core import Session, Client, Mutation
 from pycarlo.lib.schema import GenericScalar
 from sgqlc.types import Variable, non_null
 
 from airflow_mcd.hooks import SessionHook
 
 
@@ -140,16 +141,17 @@
     Client class used to send Airflow related events to Monte Carlo.
     """
 
     _UPLOAD_AIRFLOW_DAG_RESULT_OPERATION = "upload_airflow_dag_result"
     _UPLOAD_AIRFLOW_TASK_RESULT_OPERATION = "upload_airflow_task_result"
     _UPLOAD_AIRFLOW_SLA_MISSES_OPERATION = "upload_airflow_sla_misses"
 
-    def __init__(self, mcd_session_conn_id: str):
+    def __init__(self, mcd_session_conn_id: str, call_timeout: int):
         self.mcd_session_conn_id = mcd_session_conn_id
+        self.mcd_call_timeout = call_timeout
 
     def upload_dag_result(self, result: DagResult):
         payload = {
             'dag_id': result.dag_id,
             'run_id': result.run_id,
             'success': result.success,
             'reason': result.reason,
@@ -195,15 +197,20 @@
     def _upload_result(self, operation_name: str, operation_parameters: Dict, payload_value: Dict):
         try:
             mc_client = Client(self._get_session())
 
             query = Mutation(payload=non_null(GenericScalar))
             attr = getattr(query, operation_name)
             attr(**operation_parameters)
-            mc_client(query=query, variables={'payload': payload_value})
+            mc_client(
+                query=query,
+                variables={'payload': payload_value},
+                retry_backoff=ExponentialBackoff(0, 0),  # disable retries
+                timeout_in_seconds=self.mcd_call_timeout,
+            )
         except Exception as exc:
             logger.exception(f'Failed to upload information to MC: {exc}')
 
     def _get_session(self) -> Session:
         return SessionHook(mcd_session_conn_id=self.mcd_session_conn_id).get_conn()
 
     @staticmethod
```

### Comparing `airflow_mcd-0.1.1/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.2/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.2/airflow_mcd/callbacks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from airflow_mcd.callbacks.client import DagResult, DagTaskResult, AirflowEventsClient, DagTaskInstanceResult, \
     SlaMissesResult, TaskSlaMiss
 from typing import Dict, List, Any, Optional
 
 
 logger = logging.getLogger(__name__)
 
+_DEFAULT_CALL_TIMEOUT = 10
+
 
 class AirflowEventsClientUtils:
     @classmethod
     def mcd_post_dag_result(
             cls,
             context: Dict,
             success: bool,
@@ -96,15 +98,15 @@
             outlets=cls._get_lineage_list(ti, 'outlets'),
         )
 
     @classmethod
     def _get_events_client(cls, dag: DAG) -> AirflowEventsClient:
         dag_params = dag.params or {}
         mcd_session_conn_id = dag_params.get('mcd_session_conn_id', 'mcd_default_session')
-        return AirflowEventsClient(mcd_session_conn_id=mcd_session_conn_id)
+        return AirflowEventsClient(mcd_session_conn_id=mcd_session_conn_id, call_timeout=_DEFAULT_CALL_TIMEOUT)
 
     @classmethod
     def _get_next_retry_datetime(cls, ti: TaskInstance) -> Optional[str]:
         if not hasattr(ti, 'task') or not ti.end_date:
             return None
         return ti.next_retry_datetime().isoformat()
```

### Comparing `airflow_mcd-0.1.1/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.2/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.2/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.2/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.1.2/airflow_mcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.1/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.2/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.2/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/setup.py` & `airflow_mcd-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.2/tests/callbacks/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.2/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/tests/operators/test_base_op.py` & `airflow_mcd-0.1.2/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.1/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.2/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

