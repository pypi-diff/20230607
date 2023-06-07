# Comparing `tmp/netunicorn-client-0.3.0.tar.gz` & `tmp/netunicorn-client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-client-0.3.0.tar", last modified: Mon May  8 20:50:28 2023, max compression
+gzip compressed data, was "netunicorn-client-0.3.1.tar", last modified: Wed Jun  7 00:22:55 2023, max compression
```

## Comparing `netunicorn-client-0.3.0.tar` & `netunicorn-client-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/
--rw-rw-r--   0 kell      (1000) kell      (1000)      494 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      831 2023-05-08 20:43:11.000000 netunicorn-client-0.3.0/pyproject.toml
--rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/setup.cfg
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/netunicorn/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/netunicorn/client/
--rw-rw-r--   0 kell      (1000) kell      (1000)       68 2023-04-12 23:54:04.000000 netunicorn-client-0.3.0/src/netunicorn/client/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     4847 2023-04-11 08:27:07.000000 netunicorn-client-0.3.0/src/netunicorn/client/base.py
--rw-rw-r--   0 kell      (1000) kell      (1000)    10592 2023-04-24 15:52:34.000000 netunicorn-client-0.3.0/src/netunicorn/client/remote.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/
--rw-rw-r--   0 kell      (1000) kell      (1000)      494 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      334 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/SOURCES.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)        1 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/dependency_links.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       52 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/requires.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       11 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.554805 netunicorn-client-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-07 00:22:55.554805 netunicorn-client-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-07 00:22:41.000000 netunicorn-client-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:22:55.554805 netunicorn-client-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.550805 netunicorn-client-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.550805 netunicorn-client-0.3.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.550805 netunicorn-client-0.3.1/src/netunicorn/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 00:22:41.000000 netunicorn-client-0.3.1/src/netunicorn/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-07 00:22:41.000000 netunicorn-client-0.3.1/src/netunicorn/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-07 00:22:41.000000 netunicorn-client-0.3.1/src/netunicorn/client/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.554805 netunicorn-client-0.3.1/src/netunicorn_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-07 00:22:55.000000 netunicorn-client-0.3.1/src/netunicorn_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-07 00:22:55.000000 netunicorn-client-0.3.1/src/netunicorn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:22:55.000000 netunicorn-client-0.3.1/src/netunicorn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 00:22:55.000000 netunicorn-client-0.3.1/src/netunicorn_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:22:55.000000 netunicorn-client-0.3.1/src/netunicorn_client.egg-info/top_level.txt
```

### Comparing `netunicorn-client-0.3.0/pyproject.toml` & `netunicorn-client-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-client"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn client module"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "netunicorn-base >= 0.3.0",
+    "netunicorn-base >= 0.3.3",
     "cloudpickle",
     "requests",
     "returns",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `netunicorn-client-0.3.0/src/netunicorn/client/base.py` & `netunicorn-client-0.3.1/src/netunicorn/client/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,161 @@
+"""
+Base class for netunicorn clients implementations.
+"""
+
 from abc import ABC, abstractmethod
 from typing import Dict, Iterable, Optional
 
-from netunicorn.base.experiment import Experiment, ExperimentExecutionInformation
+from netunicorn.base import Experiment, ExperimentExecutionInformation, FlagValues
 from netunicorn.base.nodes import Nodes
 
 
 class BaseClient(ABC):
+    """
+    Base class for netunicorn client implementations.
+    """
+
     @abstractmethod
     def get_nodes(self) -> Nodes:
         """
-        This method returns description of available nodes in the system.
+        Return nodes currently available to the current user.
+
         :return: Nodes object with available nodes
         """
         pass
 
     @abstractmethod
     def get_experiments(self) -> Dict[str, ExperimentExecutionInformation]:
         """
-        This method returns information about all experiments that belong to the user.
-        :return: dictionary of experiment-name: ExperimentExecutionInformation
+        Get information about all experiments that belong to the current user.
+
+        :return: dictionary of {experiment-name: experiment information}
         """
         pass
 
     @abstractmethod
     def delete_experiment(self, experiment_name: str) -> None:
         """
-        This method deletes experiment from the system or raise the exception if something's wrong.
+        Delete experiment from the system (to release experiment name).
+
         :param experiment_name: name of the experiment to delete
         """
         pass
 
     @abstractmethod
     def healthcheck(self) -> bool:
         """
-        This method checks if the system is alive.
-        :return: True if server is alive, raises exception otherwise
+        Check if the current netunicorn instance is healthy.
+
+        :return: True if core service is healthy
         """
         pass
 
     @abstractmethod
     def prepare_experiment(
         self,
         experiment: Experiment,
         experiment_id: str,
         deployment_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
         """
-        Prepares an Experiment. Server will start compiling and distributing the environment among nodes.
-        You can check status of preparation by calling 'get_experiment_status' function and checking if it's in
-        "READY" status.
-        You need to provide a per-user unique experiment name.
-        This method is network-failure-safe: subsequent calls with the same network name
-        will not create additional deployment processes.
+        | Prepare an Experiment. Server will start compiling and distributing the environment among nodes.
+        | You can check status of preparation by calling 'get_experiment_status' function and checking if it's in "READY" status.
+        | You need to provide a per-user unique experiment name.
+        | This method is network-failure-safe: subsequent calls with the same network name will not create additional deployment processes.
+
         :param experiment: experiment to prepare
         :param experiment_id: user-wide unique experiment name
-        :param deployment_context: deployment context for connectors (see connectors documentation)
-        Format: {connector_name: {key: value}, ...}
+        :param deployment_context: deployment context for connectors specific for each connector,
+            format: {connector_name: {key: value}, ...}
         :return: the same experiment_id if everything's correct
         """
         pass
 
     @abstractmethod
     def start_execution(
         self,
         experiment_id: str,
         execution_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
         """
-        Starts execution of prepared experiment.
-        You can check status and results of an experiment by calling 'get_experiment_status' function and checking if it's in
-        "FINISHED" status.
-        You need to provide an experiment_id of prepared experiment to start.
-        This method is network-failure-safe: subsequent calls with the same experiment id
-        will not create additional start process.
+        | Start execution of prepared experiment.
+        | You can check status and results of an experiment by calling 'get_experiment_status' function and checking if it's in "FINISHED" status.
+        | You need to provide an experiment_id of prepared experiment to start.
+        | This method is network-failure-safe - subsequent calls with the same experiment id will not create additional start process.
+
         :param experiment_id: prepared experiment id
-        :param execution_context: execution context for connectors (see connectors documentation)
-        Format: {connector_name: {key: value}, ...}
+        :param execution_context: execution context for connectors specific for each connector,
+            format: {connector_name: {key: value}, ...}
         :return: the same experiment_id if execution already in progress or finished
         """
         pass
 
     @abstractmethod
     def get_experiment_status(
         self, experiment_id: str
     ) -> ExperimentExecutionInformation:
         """
-        Returns status and results of experiment.
-        If experiment preparation succeed, you can explore map to see what nodes are prepared for deployment.
-        If experiment finished, you can explore results of the experiment
+        | Return status and results of experiment.
+        | If experiment preparation succeed, you can explore map to see what nodes are prepared for deployment.
+        | If experiment finished, you can explore results of the experiment
+
         :param experiment_id: id of the experiment returned by 'prepare_experiment' function
         :return: current status of the experiment, optionally experiment definition, optionally experiment results
         """
         pass
 
     @abstractmethod
     def cancel_experiment(
         self,
         experiment_id: str,
         cancellation_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
         """
-        Cancels experiment execution.
+        Cancel experiment execution.
+
         :param experiment_id: id of the experiment
-        :param cancellation_context: cancellation context for connectors (see connectors documentation)
-        Format: {connector_name: {key: value}, ...}
+        :param cancellation_context: cancellation context for connectors specific for each connector,
+            format: {connector_name: {key: value}, ...}
         :return: the same experiment_id if everything's correct
         """
         pass
 
     @abstractmethod
     def cancel_executors(
         self,
         executors: Iterable[str],
         cancellation_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
         """
-        Cancels particular executors.
+        Cancel particular executors.
+
         :param executors: list of executors to cancel
-        :param cancellation_context: cancellation context for connectors (see connectors documentation)
-        Format: {connector_name: {key: value}, ...}
+        :param cancellation_context: cancellation context for connectors specific for each connector,
+            format: {connector_name: {key: value}, ...}
         :return: the same experiment_id if everything's correct
         """
         pass
+
+    @abstractmethod
+    def get_flag_values(self, experiment_id: str, flag_name: str) -> FlagValues:
+        """
+        Get flag values for a particular flag of the experiment.
+
+        :param experiment_id: id of the experiment
+        :param flag_name: name of the flag
+        :return: flag values (string, int, or both)
+        """
+        pass
+
+    @abstractmethod
+    def set_flag_values(
+        self, experiment_id: str, flag_name: str, flag_values: FlagValues
+    ) -> None:
+        """
+        Set flag values for a particular flag of the experiment.
+
+        :param experiment_id: id of the experiment
+        :param flag_name: name of the flag
+        :param flag_values: flag values (string, int, or both)
+        """
+        pass
```

### Comparing `netunicorn-client-0.3.0/src/netunicorn/client/remote.py` & `netunicorn-client-0.3.1/src/netunicorn/client/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Default remote client for netunicorn.
+"""
 import json
 import warnings
 from typing import Dict, Iterable, Optional
 from urllib.parse import quote_plus
 
 import requests as req
 from netunicorn.base.experiment import Experiment, ExperimentExecutionInformation
@@ -13,43 +16,64 @@
 )
 from netunicorn.base.utils import UnicornEncoder
 
 from .base import BaseClient
 
 
 class RemoteClientException(Exception):
+    """
+    Generic exception for remote client.
+    """
+
     pass
 
 
 class RemoteClient(BaseClient):
+    """
+    Remote client for Unicorn.
+
+    :param endpoint: netunicorn endpoint
+    :param login: netunicorn login
+    :param password: netunicorn password
+    :param authentication_context: authentication context for connectors
+    """
+
     def __init__(
         self,
         endpoint: str,
         login: str,
         password: str,
         authentication_context: Optional[Dict[str, Dict[str, str]]] = None,
     ):
-        """
-        Remote client for Unicorn.
-        :param endpoint: Unicorn installation endpoint.
-        :param login: Unicorn installation login.
-        :param password: Unicorn installation password.
-        :param authentication_context: Authentication context for connectors.
-        E.g., if a connector A requires users to provide additional security token, it could be specified here.
-        Format: {connector_name: {key: value}}
-        """
         if endpoint.endswith("/"):
             endpoint = endpoint[:-1]
         self.endpoint = endpoint
+        """
+        netunicorn installation endpoint.
+        """
+
         self.login = login
+        """
+        netunicorn installation login.
+        """
+
         self.password = password
+        """
+        netunicorn installation password.
+        """
+
         self.authentication_context = authentication_context or {}
+        """
+        Authentication context for connectors.
+            E.g., if a connector A requires users to provide additional security token, it could be specified here.
+            Format: {connector_name: {key: value}}
+        """
 
     @staticmethod
-    def quote_plus_and_warn(string: str) -> str:
+    def _quote_plus_and_warn(string: str) -> str:
         result = quote_plus(string)
         if result != string:
             warnings.warn(
                 f"String {string} was encoded to {result}. "
                 f"Consider using only alphanumeric characters and underscores."
             )
 
@@ -81,15 +105,15 @@
 
         raise RemoteClientException(
             f"Failed to get node pool. "
             f"Status code: {result.status_code}, content: {result.content.decode('utf-8')}"
         )
 
     def delete_experiment(self, experiment_name: str) -> None:
-        experiment_name = self.quote_plus_and_warn(experiment_name)
+        experiment_name = self._quote_plus_and_warn(experiment_name)
         result_data = req.delete(
             f"{self.endpoint}/api/v1/experiment/{experiment_name}",
             auth=(self.login, self.password),
             headers={
                 "netunicorn-authentication-context": json.dumps(
                     self.authentication_context
                 )
@@ -130,15 +154,15 @@
         deployment_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
         if deployment_context is not None:
             if experiment.deployment_context is None:
                 experiment.deployment_context = {}
             experiment.deployment_context.update(deployment_context)
 
-        experiment_id = self.quote_plus_and_warn(experiment_id)
+        experiment_id = self._quote_plus_and_warn(experiment_id)
         data = json.dumps(experiment, cls=UnicornEncoder)
         result = req.post(
             f"{self.endpoint}/api/v1/experiment/{experiment_id}/prepare",
             auth=(self.login, self.password),
             data=data,
             headers={
                 "Content-Type": "application/json",
@@ -156,15 +180,15 @@
         )
 
     def start_execution(
         self,
         experiment_id: str,
         execution_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
-        experiment_id = self.quote_plus_and_warn(experiment_id)
+        experiment_id = self._quote_plus_and_warn(experiment_id)
         result = req.post(
             f"{self.endpoint}/api/v1/experiment/{experiment_id}/start",
             auth=(self.login, self.password),
             json=execution_context,
             headers={
                 "netunicorn-authentication-context": json.dumps(
                     self.authentication_context
@@ -178,15 +202,15 @@
             "Failed to start experiment execution. "
             f"Status code: {result.status_code}, content: {result.content.decode('utf-8')}"
         )
 
     def get_experiment_status(
         self, experiment_id: str
     ) -> ExperimentExecutionInformation:
-        experiment_id = self.quote_plus_and_warn(experiment_id)
+        experiment_id = self._quote_plus_and_warn(experiment_id)
         result_data = req.get(
             f"{self.endpoint}/api/v1/experiment/{experiment_id}",
             auth=(self.login, self.password),
             headers={
                 "netunicorn-authentication-context": json.dumps(
                     self.authentication_context
                 )
@@ -202,15 +226,15 @@
         return ExperimentExecutionInformation.from_json(result)
 
     def cancel_experiment(
         self,
         experiment_id: str,
         cancellation_context: Optional[Dict[str, Dict[str, str]]] = None,
     ) -> str:
-        experiment_id = self.quote_plus_and_warn(experiment_id)
+        experiment_id = self._quote_plus_and_warn(experiment_id)
         result = req.post(
             f"{self.endpoint}/api/v1/experiment/{experiment_id}/cancel",
             auth=(self.login, self.password),
             json=cancellation_context,
             headers={
                 "netunicorn-authentication-context": json.dumps(
                     self.authentication_context
@@ -248,16 +272,16 @@
 
         raise RemoteClientException(
             "Failed to cancel provided executors. "
             f"Status code: {result.status_code}, content: {result.content.decode('utf-8')}"
         )
 
     def get_flag_values(self, experiment_id: str, flag_name: str) -> FlagValues:
-        experiment_id = self.quote_plus_and_warn(experiment_id)
-        flag_name = self.quote_plus_and_warn(flag_name)
+        experiment_id = self._quote_plus_and_warn(experiment_id)
+        flag_name = self._quote_plus_and_warn(flag_name)
         result_data = req.get(
             f"{self.endpoint}/api/v1/experiment/{experiment_id}/flag/{flag_name}",
             auth=(self.login, self.password),
         )
         if result_data.status_code >= 400:
             raise RemoteClientException(
                 "Failed to get flag value. "
@@ -265,16 +289,16 @@
             )
 
         return FlagValues(**(result_data.json()))
 
     def set_flag_values(
         self, experiment_id: str, flag_name: str, flag_values: FlagValues
     ) -> None:
-        experiment_id = self.quote_plus_and_warn(experiment_id)
-        flag_name = self.quote_plus_and_warn(flag_name)
+        experiment_id = self._quote_plus_and_warn(experiment_id)
+        flag_name = self._quote_plus_and_warn(flag_name)
         if flag_values.int_value is None and flag_values.text_value is None:
             raise RemoteClientException(
                 "One of int_value or text_value must be provided."
             )
 
         result_data = req.post(
             f"{self.endpoint}/api/v1/experiment/{experiment_id}/flag/{flag_name}",
```

