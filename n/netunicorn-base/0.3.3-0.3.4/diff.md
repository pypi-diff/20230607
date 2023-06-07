# Comparing `tmp/netunicorn-base-0.3.3.tar.gz` & `tmp/netunicorn-base-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-base-0.3.3.tar", last modified: Sun May 14 23:15:39 2023, max compression
+gzip compressed data, was "netunicorn-base-0.3.4.tar", last modified: Wed Jun  7 00:22:59 2023, max compression
```

## Comparing `netunicorn-base-0.3.3.tar` & `netunicorn-base-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/base/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/environment_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/director/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.912385 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/director/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:27.000000 netunicorn-base-0.3.3/src/netunicorn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:15:39.916385 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 23:15:39.000000 netunicorn-base-0.3.3/src/netunicorn_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.607789 netunicorn-base-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:22:59.607789 netunicorn-base-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.599789 netunicorn-base-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.599789 netunicorn-base-0.3.4/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.599789 netunicorn-base-0.3.4/src/netunicorn/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/environment_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.595789 netunicorn-base-0.3.4/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/src/netunicorn/director/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/director/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-base-0.3.4/src/netunicorn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:59.603789 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:22:59.000000 netunicorn-base-0.3.4/src/netunicorn_base.egg-info/top_level.txt
```

### Comparing `netunicorn-base-0.3.3/pyproject.toml` & `netunicorn-base-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-base"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn base module"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-base-0.3.3/src/netunicorn/base/deployment.py` & `netunicorn-base-0.3.4/src/netunicorn/base/deployment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,104 @@
+"""
+Single deployment of pipeline on node.
+"""
 from __future__ import annotations
 
 from base64 import b64decode
 from copy import deepcopy
-from typing import Optional
+from typing import List, Optional, cast
 
 import netunicorn.base.environment_definitions
 
 from .nodes import Node
 from .pipeline import Pipeline
-from .task import TaskDispatcher
+from .task import Task, TaskDispatcher
 from .types import DeploymentRepresentation
 from .utils import SerializedPipelineType
 
 try:
     import cloudpickle  # it's needed only on client side, but this module is also imported on engine side
     import netunicorn.library
 
     cloudpickle.register_pickle_by_value(netunicorn.library)
 except ImportError:
     pass
 
 
 class Deployment:
+    """
+    Single deployment of pipeline on node.
+
+    :param node: Node to deploy pipeline on
+    :param pipeline: Pipeline to deploy
+    :param keep_alive_timeout_minutes: time to wait for executor update before timeout
+    :param cleanup: whether to remove artifacts (e.g., Docker image and containers) after execution
+    """
+
     def __init__(
         self,
         node: Node,
         pipeline: Pipeline,
         keep_alive_timeout_minutes: int = 10,
         cleanup: bool = True,
     ):
-        self.node = node
-        self.prepared = False
-        self.executor_id = ""
+        self.node: Node = node
+        """
+        Node to deploy pipeline on
+        """
+
+        self.prepared: bool = False
+        """
+        if False, deployment is not prepared yet or failed during preparation
+        """
+
+        self.executor_id: str = ""
+        """
+        ID of executor on node
+        """
+
         self.error: Optional[Exception] = None
+        """
+        if deployment failed, this field contains error
+        """
+
         self.pipeline: SerializedPipelineType = b""
-        self.environment_definition = deepcopy(pipeline.environment_definition)
-        self.keep_alive_timeout_minutes = keep_alive_timeout_minutes
-        self.cleanup = cleanup
+        """
+        Serialized Pipeline to be deployed
+        """
+
+        self.environment_definition: netunicorn.base.environment_definitions.EnvironmentDefinition = deepcopy(
+            pipeline.environment_definition
+        )
+        """
+        Environment definition to use for deployment
+        """
+
+        self.keep_alive_timeout_minutes: int = keep_alive_timeout_minutes
+        """
+        time to wait for executor update before timeout
+        """
+
+        self.cleanup: bool = cleanup
+        """
+        if True, corresponding artifacts (Docker image and containers) will be removed after execution
+        """
 
         self._validate_deployment(node, pipeline)
 
         pipeline = deepcopy(pipeline)
 
         for i, element in enumerate(pipeline.tasks):
             pipeline.tasks[i] = [
                 x.dispatch(node) if isinstance(x, TaskDispatcher) else x
                 for x in element
             ]
-            for x in pipeline.tasks[i]:
-                # now it's only Tasks
-                self.environment_definition.commands.extend(x.requirements)  # type: ignore
+            tasks_list: List[Task] = cast(List[Task], pipeline.tasks[i])
+            for x in tasks_list:
+                self.environment_definition.commands.extend(x.requirements)
 
         self.pipeline = cloudpickle.dumps(pipeline)
 
     @staticmethod
     def _validate_deployment(node: Node, pipeline: Pipeline) -> None:
         if type(pipeline.environment_definition) not in node.available_environments:
             raise ValueError(
@@ -77,14 +122,20 @@
             "cleanup": self.cleanup,
             "environment_definition": self.environment_definition.__json__(),
             "environment_definition_type": self.environment_definition.__class__.__name__,
         }
 
     @classmethod
     def from_json(cls, data: DeploymentRepresentation) -> Deployment:
+        """
+        Create Deployment from JSON representation
+
+        :param data: JSON representation of Deployment
+        :return: Deserialized Deployment
+        """
         instance = cls.__new__(cls)
 
         instance.node = Node.from_json(data["node"])
         instance.prepared = data["prepared"]
         instance.executor_id = data["executor_id"]
         instance.error = Exception(data["error"]) if data["error"] else None
         instance.pipeline = b64decode(data["pipeline"])
```

### Comparing `netunicorn-base-0.3.3/src/netunicorn/base/nodes.py` & `netunicorn-base-0.3.4/src/netunicorn/base/nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,114 @@
+"""
+Abstractions for nodes representation.
+"""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
-from itertools import chain, cycle
-from typing import Callable, Dict, Iterator, List, Sequence, Set, Union
-from uuid import uuid4
+from itertools import chain, count, cycle
+from typing import Callable, Dict, Iterable, Iterator, List, Sequence, Set, Union, cast
 
-import netunicorn
+import netunicorn.base
 
 from .architecture import Architecture
 from .environment_definitions import _available_environment_definitions
 from .types import NodeProperty, NodeRepresentation, NodesRepresentation
 
 
 class Node:
+    """
+    Represents a single node in a pool of nodes.
+
+    :param name: name of the node
+    :param properties: custom properties of the node
+    :param architecture: node architecture
+    """
+
     def __init__(
         self,
         name: str,
         properties: Dict[str, NodeProperty],
         architecture: Architecture = Architecture.UNKNOWN,
     ):
-        self.name = name
-        self.properties = properties
+        self.name: str = name
+        """
+        Node name.
+        """
+
+        self.properties: Dict[str, NodeProperty] = properties
+        """
+        Node properties. Could be used to store custom information about the node.
+        """
+
         self.additional_properties: Dict[str, NodeProperty] = {}
-        self.architecture = architecture
+        """
+        Additional node properties, often used for internal purposes and not to be exposed to the user.
+        """
+
+        self.architecture: Architecture = architecture
+        """
+        Node architecture.
+        """
+
         self.available_environments: Set[type] = self._infer_environments()
+        """
+        Supported environments for the node (see :py:mod:`netunicorn.base.environment_definitions`).
+        """
 
     def _infer_environments(self) -> Set[type]:
         result = set()
         # noinspection PyBroadException
         try:
             environments = self.properties.get(
                 "netunicorn-environments", _available_environment_definitions.keys()
             )
             if hasattr(environments, "__iter__"):
-                for environment_name in environments:  # type: ignore
+                for environment_name in cast(Iterable[str], environments):
                     if environment_name in _available_environment_definitions:
                         result.add(_available_environment_definitions[environment_name])
         except Exception:
             return set(_available_environment_definitions.values())
         return result
 
     def __getitem__(self, item: str) -> NodeProperty:
+        """
+        Returns a node property by name.
+
+        :param item: name of the property
+        :return: property value
+        """
         return self.properties.get(item, None)
 
     def __iter__(self) -> Iterator[NodeProperty]:
         raise TypeError("Node is not iterable")
 
     def __setitem__(self, key: str, value: NodeProperty) -> None:
+        """
+        Sets a node property.
+
+        :param key: name of the property
+        :param value: property value
+        """
         self.properties[key] = value
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
 
     def __eq__(self, other: object) -> bool:
+        """
+        Checks if two nodes are equal.
+
+        :param other: other node
+        :return: True if the nodes have all parameters equal, False otherwise
+        """
         return (
             isinstance(other, Node)
             and self.name == other.name
             and self.properties == other.properties
             and self.additional_properties == other.additional_properties
             and self.architecture == other.architecture
         )
@@ -71,112 +119,155 @@
             "properties": self.properties,
             "additional_properties": self.additional_properties,
             "architecture": self.architecture.value,
         }
 
     @classmethod
     def from_json(cls, data: NodeRepresentation) -> Node:
+        """
+        Returns an instance of the object from a JSON representation.
+
+        :param data: JSON representation of the object
+        :return: instance of the object
+        """
         instance = cls(
             data["name"], data["properties"], Architecture(data["architecture"])
         )
         instance.additional_properties = data["additional_properties"]
         return instance
 
 
 class Nodes(ABC):
     """
-    Represents a pool of nodes.
+    A base class that represents a pool of nodes. Not to be used directly, but to be inherited from.
     """
 
     @abstractmethod
     def __json__(self) -> NodesRepresentation:
         """
         Returns a JSON representation of the object.
         """
         pass
 
     @staticmethod
     def dispatch_and_deserialize(data: NodesRepresentation) -> Nodes:
+        """
+        Deserializes a JSON representation of the object and returns an instance of the object.
+
+        :param data: JSON representation of the object
+        :return: instance of the object
+        """
+
         cls: Nodes = getattr(netunicorn.base.nodes, data["node_pool_type"])
         return cls.from_json(data["node_pool_data"])
 
     @classmethod
     @abstractmethod
     def from_json(
         cls, data: List[Union[NodeRepresentation, NodesRepresentation]]
     ) -> Nodes:
         """
-        Accepts a JSON representation of the object (from "node_pool_data") and returns an instance of the object.
+        Class-specific implementation of deserialization from JSON.
+
+        :param data: JSON representation of the object
+        :return: instance of the object
         """
         pass
 
     @abstractmethod
     def __str__(self) -> str:
-        """
-        Returns a string representation of the object.
-        """
         pass
 
     @abstractmethod
     def __len__(self) -> int:
         pass
 
     @abstractmethod
     def __getitem__(self, item: int) -> Union[Node, Nodes]:
         pass
 
     @abstractmethod
     def filter(self, function: Callable[[Node], bool]) -> Nodes:
         """
-        Returns a pool of nodes that match the given filter.
+        Returns a pool of nodes that match the given filter function.
+
+        :param function: filter function returning True if the node should be included in the result
+        :return: pool of nodes
         """
         pass
 
     @abstractmethod
     def take(self, count: int) -> Sequence[Node]:
         """
-        Returns a sequence of nodes consisting of the first n nodes.
+        Returns a sequence of nodes consisting of the first `count` nodes.
+
+        :param count: number of nodes to take
+        :return: sequence of nodes
         """
         pass
 
     @abstractmethod
     def skip(self, count: int) -> Nodes:
         """
-        Returns a pool of nodes consisting of the nodes after the first n nodes.
+        Returns a pool of nodes consisting of the nodes after the first 'count' nodes.
+
+        :param count: number of nodes to skip
+        :return: pool of nodes
         """
         pass
 
     @abstractmethod
     def set_property(self, name: str, value: NodeProperty) -> Nodes:
+        """
+        Sets a property for all nodes in the pool.
+
+        :param name: name of the property
+        :param value: property value
+        :return: self
+        """
         pass
 
 
 class CountableNodePool(Nodes):
     """
-    Represents a typical pool of nodes.
+    Represents a pool of nodes that contains a fixed number of nodes.
+
+    :param nodes: list of nodes
     """
 
     def __init__(self, nodes: List[Union[Node, Nodes]]):
         self.nodes = nodes
+        """
+        Nodes in the pool.
+        """
 
     def __json__(self) -> NodesRepresentation:
         return {
             "node_pool_type": self.__class__.__name__,
             "node_pool_data": [x.__json__() for x in self.nodes],
         }
 
     @classmethod
     def from_json(
         cls, data: List[Union[NodeRepresentation, NodesRepresentation]]
     ) -> CountableNodePool:
+        """
+        Returns an instance of the object from a JSON representation.
+
+        :param data: JSON representation of the object
+        :return: instance of the object
+        """
         nodes: List[Union[Node, Nodes]] = []
         for element in data:
             if "node_pool_type" in element:
                 # we know this is a NodesRepresentation
-                nodes.append(Nodes.dispatch_and_deserialize(element))  # type: ignore
+                nodes_representation_element = cast(NodesRepresentation, element)
+                nodes.append(
+                    Nodes.dispatch_and_deserialize(nodes_representation_element)
+                )
             else:
                 nodes.append(Node.from_json(element))
         return cls(nodes)
 
     def __str__(self) -> str:
         return str(self.nodes)
 
@@ -188,14 +279,20 @@
 
     def __setitem__(
         self, key: int, value: Union[Node, CountableNodePool, UncountableNodePool]
     ) -> None:
         self.nodes[key] = value
 
     def pop(self, index: int) -> Union[Node, Nodes]:
+        """
+        Removes and returns the node at the given index.
+
+        :param index: index of the node to remove
+        :return: popped node
+        """
         return self.nodes.pop(index)
 
     def __repr__(self) -> str:
         return str(self.nodes)
 
     def filter(self, function: Callable[[Node], bool]) -> CountableNodePool:
         nodes: List[Union[Node, Nodes]] = []
@@ -207,15 +304,18 @@
                 filtered_nodes = node.filter(function)
                 if len(filtered_nodes) > 0:
                     nodes.append(filtered_nodes)
         return CountableNodePool(nodes)
 
     def take(self, count: int) -> Sequence[Node]:
         iterator: Iterator[Node] = chain.from_iterable(
-            [x] if isinstance(x, Node) else x for x in self.nodes  # type: ignore
+            cast(
+                Iterable[Iterable[Node]],
+                ([x] if isinstance(x, Node) else x for x in self.nodes),
+            )
         )
         nodes = []
         for _ in range(count):
             try:
                 nodes.append(next(iterator))
             except StopIteration:
                 break
@@ -237,33 +337,52 @@
             else:
                 node.set_property(name, value)
         return self
 
 
 class UncountableNodePool(Nodes):
     """
-    Represents a pool of nodes that is not countable (e.g., dynamic pools of cloud providers).
-    In the current implementation cannot have Nodes as elements.
+    | Represents a pool of nodes that is not countable (i.e., contains possibly infinite amount of nodes, e.g. cloud provider).
+    | In the current implementation cannot have Nodes as elements.
+
+    :param node_template: list of nodes that will be used as a template for generating new nodes
     """
 
     def __init__(self, node_template: List[Node]):
         self._node_template = node_template
+        """
+        Node template used for generating new nodes.
+        """
+
         self._nodes = cycle(node_template)
+        """
+        An iterator over the node template.
+        """
+
+        self._counter = count(start=1, step=1)
+        """
+        Node name counter.
+        """
 
     def __str__(self) -> str:
         return str(
             f"<Uncountable node pool with next node template: {self._node_template}>"
         )
 
     def __repr__(self) -> str:
         return str(self)
 
     def __next__(self) -> Node:
+        """
+        Generate and returns the next node in the pool.
+
+        :return: next node
+        """
         node = deepcopy(next(self._nodes))
-        node.name += uuid4().hex
+        node.name += str(next(self._counter))
         return node
 
     def __getitem__(self, key: int) -> Node:
         return self._node_template[key]
 
     def __setitem__(self, key: int, value: Node) -> None:
         self._node_template[key] = value
@@ -296,13 +415,14 @@
     def from_json(
         cls, data: List[Union[NodeRepresentation, NodesRepresentation]]
     ) -> UncountableNodePool:
         for x in data:
             if "node_pool_type" in x:
                 raise ValueError("UncountableNodePool cannot have Nodes as elements.")
         # now we have only NodeRepresentation in the list
-        return cls([Node.from_json(x) for x in data])  # type: ignore
+        node_representation_data = cast(List[NodeRepresentation], data)
+        return cls([Node.from_json(x) for x in node_representation_data])
 
     def set_property(self, name: str, value: NodeProperty) -> UncountableNodePool:
         for node in self._node_template:
             node.properties[name] = value
         return self
```

### Comparing `netunicorn-base-0.3.3/src/netunicorn/base/pipeline.py` & `netunicorn-base-0.3.4/src/netunicorn/base/pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Abstrcations for Pipeline representation.
+"""
+
 from __future__ import annotations
 
 import uuid
 from copy import deepcopy
 from typing import Collection, List, Optional, Set, Union
 from warnings import warn
 
@@ -14,41 +18,66 @@
 class Pipeline:
     """
     Pipeline is a class that takes a tuple of Tasks and executes them in order.
     Each element in the tuple should be either a Task or a tuple of Tasks.
     Pipeline will execute elements in order and return the combined result of all tasks.
     If element is a tuple of tasks, these tasks would be executed in parallel.
 
-    The result of pipeline execution would be one of the following:
-    - Success: if all tasks succeed, then Success is returned
-    - Failure: if any task fails, then Failure is returned
-
-    Returning object will always contain a Result object for each task executed.
-    If early_stopping is set to True, then any task after first failed wouldn't be executed.
+    | The result of pipeline execution would be one of the following:
+    | - Success: if all tasks succeed, then Success is returned
+    | - Failure: if any task fails, then Failure is returned
+
+    | Returning object will always contain a Result object for each task executed.
+    | If early_stopping is set to True, then any task after first failed wouldn't be executed.
+
+    :param tasks: tasks (ordered by stages) to be executed
+    :param early_stopping: whether to stop executing tasks after first failure
+    :param report_results: whether executor should connect core services to report pipeline results in the end
+    :param environment_definition: environment definition for the pipeline
     """
 
     def __init__(
         self,
         tasks: Collection[PipelineElement] = (),
         early_stopping: bool = True,
         report_results: bool = True,
         environment_definition: Optional[EnvironmentDefinition] = None,
     ):
+        self.name: str = str(uuid.uuid4())
         """
-        Initialize Pipeline with a tuple of Tasks or TaskDispatchers and early_stopping flag.
-        :param tasks: a tuple of tasks to be executed
-        :param early_stopping: whether to stop executing tasks after first failure
-        :param report_results: whether executor should connect director services to report pipeline results after exec
+        Pipeline name.
         """
-        self.name = str(uuid.uuid4())
+
         self.task_names: Set[str] = set()
-        self.early_stopping = early_stopping
+        """
+        Task names in the pipeline, used for dictionary of results.
+        """
+
+        self.early_stopping: bool = early_stopping
+        """
+        Whether to stop executing tasks after first failure.
+        """
+
         self.tasks: List[List[TaskElement]] = []
-        self.report_results = report_results
-        self.environment_definition = environment_definition or DockerImage()
+        """
+        Tasks stages to be executed.
+        """
+
+        self.report_results: bool = report_results
+        """
+        Whether executor should connect core services to report pipeline results in the end.
+        """
+
+        self.environment_definition: EnvironmentDefinition = (
+            environment_definition or DockerImage()
+        )
+        """
+        Environment definition for the pipeline.
+        """
+
         for element in tasks:
             self.then(element)
 
     @staticmethod
     def __element_to_stage(element: PipelineElement) -> List[TaskElement]:
         if not isinstance(element, Collection):
             element = [element]
@@ -63,26 +92,28 @@
                     f"Task with name {task.name} already exists in the current pipeline {self.__str__()}. "
                     "Please, note that execution results of these tasks could be mixed or overwritten."
                 )
             self.task_names.add(task.name)
 
     def then(self, element: PipelineElement) -> Pipeline:
         """
-        Add a task or list of tasks to the end of the pipeline.
+        Add a task or list of tasks as a separate stage to the end of the pipeline.
+
         :param element: a task or tuple of tasks to be added
         :return: self
         """
         element = self.__element_to_stage(element)
         self.__check_tasks_names(element)
         self.tasks.append(element)
         return self
 
     def copy(self) -> Pipeline:
         """
         Return a copy of the pipeline.
+
         :return: a copy of the pipeline
         """
         return Pipeline(deepcopy(self.tasks), self.early_stopping)
 
     def __str__(self) -> str:
         return f"Pipeline({self.name}): {self.tasks}"
```

### Comparing `netunicorn-base-0.3.3/src/netunicorn/base/task.py` & `netunicorn-base-0.3.4/src/netunicorn/base/task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Abstractions for tasks representation.
+"""
+
 from __future__ import annotations
 
 import copy
 import uuid
 from abc import ABC, abstractmethod
 from typing import Any, List, Optional, Union
 
@@ -13,105 +17,123 @@
 # Keep classes for export
 Success = Success
 Failure = Failure
 
 
 class Task(ABC):
     """
-    This is a base class for all tasks. All new task classes should inherit from this class.
-    The task instance should encapsulate all the logic and data needed to execute the task.
-    Task entrypoint is the run() method.
-    Task class can have requirements - commands to be executed to change environment to support this task.
-    These requirements would be executed with OS shell during environment setup.
-    Each task is to be implemented for a specific architecture, platform, or combination (like Linux + arm64).
-    TaskDispatcher can be used for selecting a specific task for the given architecture, platform, or combination.
-
-    Task always returns a Result object.
-    - If the task's `run` method returns Result object by itself, you'll receive this Result object
-    - If the task's `run` method returns any other object, you'll receive a Success with returned_value encapsulated
-    - If the task's `run` method fires an exception, you'll receive a Failure with the exception encapsulated
+    | This is a base class for all tasks. All new task classes should inherit from this class.
+    | The task instance should encapsulate all the logic and data needed to execute the task.
+    | Task entrypoint is the run() method.
+    | Task class can have requirements - commands to be executed to change environment to support this task.
+    | These requirements would be executed with OS shell during environment setup.
+    | Each task is to be implemented for a specific architecture, platform, or combination (like Linux + arm64).
+    | TaskDispatcher can be used for selecting a specific task for the given architecture, platform, or combination.
+
+    | Task always returns a Result object.
+    | - If the task's `run` method returns Result object by itself, you'll receive this Result object
+    | - If the task's `run` method returns any other object, you'll receive a Success with returned_value encapsulated
+    | - If the task's `run` method fires an exception, you'll receive a Failure with the exception encapsulated
+
+    | When creating your own tasks, please, do not forget to call `super().__init__(*args, **kwargs)` in your implementation
+        to properly initialize the base class.
+
+    :param name: Name of the task. If not provided, a random UUID will be used.
     """
 
-    # Task installation requirements
     requirements: List[str] = []
+    """
+    A list of commands to be executed to change environment to support this task.
+    """
 
-    # this variable would be overwritten before task start with results of previous tasks
-    # format: {task_name: [Result, Result, ...]}
     previous_steps: PipelineResult = {}
+    r"""
+    Stores results of previous steps with task name as a key and list of results as a value.
+        Several results could be stored for each task if it was executed several times.
+    """
 
     def __init__(self, name: Optional[str] = None) -> None:
-        """
-        This is a constructor for the task. Any variables (state) that `run` method should use should be provided here.
-        Please, do not forget to call `super().__init__()` in your implementation.
-        """
-        self.name = name or str(uuid.uuid4())  # Each task should have a name
+        self.name = name or str(uuid.uuid4())
         self.requirements = copy.deepcopy(self.requirements)
 
     def __call__(self) -> Any:
+        """
+        This method is called when you call the task instance as a function. It's a shortcut for `run` method.
+
+        :return: Result of the execution
+        """
         return self.run()
 
     def __repr__(self) -> str:
         type_ = type(self)
         module = type_.__module__
         qualname = type_.__qualname__
         return f"<{module}.{qualname} with name {self.name}>"
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def add_requirement(self, command: str) -> Task:
         """
-        This method adds a requirement to the local requirements of the task.
-        :param command:
-        :return:
-        """
-        self.requirements = copy.deepcopy(
-            self.requirements
-        )  # make it instance-specific
+        | This method adds a requirement to the requirements of the instance of the task.
+        | Please, note that the requirement would be added to the instance, not to all instances of the class.
+        | Use it to provide additional requirements that should be executed only once despite the number of instances.
+
+        :param command: Command to be executed to change environment to support this task.
+        :return: self
+        """
+        self.requirements = copy.deepcopy(self.requirements)
         self.requirements.append(command)
         return self
 
     @abstractmethod
     def run(self) -> Any:
         """
-        ## This method is to be overridden by your implementation. ##
-        This is the entrypoint for the task.
-        This method should never have any arguments except `self`. Any arguments that task would use for execution
-        should be provided to the constructor and used later by this method.
-        This method will always return a Result object. If this method doesn't return a Result object,
-        it will be encapsulated into a Result object.
+        | ## This method is to be overridden by your implementation. ##
+        | This is the entrypoint for the task.
+        | This method should never have any arguments except `self`. Any arguments that task would use for execution
+            should be provided to the constructor and used later by this method.
+        | This method will always return a Result object. If this method doesn't return a Result object,
+            it will be encapsulated into a Result object.
+
         :return: Result of the execution
         """
         raise NotImplementedError
 
 
 class TaskDispatcher(ABC):
     """
-    This class is a wrapper for several tasks that are designed to implement the same functionality
-    but depend on node attributes. Most often you either want to use a specific
-    implementation for a specific architecture (e.g., different Tasks for Windows and Linux),
-    or instantiate a task with some specific parameters for a specific node (e.g., node-specific IP address).
-    You should implement your own TaskDispatcher class and override the dispatch method.
+    | This class is a wrapper for several tasks that are designed to implement the same functionality
+        but depend on node attributes. Most often you either want to use a specific
+        implementation for a specific architecture (e.g., different Tasks for Windows and Linux),
+        or instantiate a task with some specific parameters for a specific node (e.g., node-specific IP address).
+    | You should implement your own TaskDispatcher class and override the dispatch method.
+    |
+    | You also should provide and use any variables (state) that `run` method would use in the constructor of this class
+        and pass them to the constructor of the task implementation.
+    |
+    | Dispatching is done by calling the dispatch method that you should implement.
 
-    Dispatching is done by calling the dispatch method that you should implement.
+    :param name: Name of the task. If not provided, a random UUID will be used.
     """
 
     def __init__(self, name: Optional[str] = None) -> None:
+        self.name = name or str(uuid.uuid4())
         """
-        This is a constructor for the TaskDispatcher. Any variables (state) that `run` method of
-        task implementations should use should be provided here.
-        Please, do not forget to call `super().__init__()` in your implementation.
+        Name of the task.
         """
-        self.name = name or str(uuid.uuid4())  # Each task should have a name
 
     @abstractmethod
     def dispatch(self, node: Node) -> Task:
         """
-        This method takes a node and should return and instance of the task that is designed to be executed on this node.
-        The instance could depend on the node information (such as architecture, platform, properties, etc).
-        :param node: Node object
-        :return: Task object
+        | This method takes a node and should return and instance of the task that is designed to be executed on this node.
+        | The instance could depend on the node information (such as architecture, platform, properties, etc).
+        |
+        | Do not forget to pass all arguments and variables to the constructor of the task implementation.
+
+        :param node: Node instance
+        :return: Task instance selected based on the node information
         """
         raise NotImplementedError
 
 
 TaskElement = Union[Task, TaskDispatcher]
```

### Comparing `netunicorn-base-0.3.3/src/netunicorn/director/base/connectors/protocol.py` & `netunicorn-base-0.3.4/src/netunicorn/director/base/connectors/protocol.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.3/src/netunicorn/director/base/resources.py` & `netunicorn-base-0.3.4/src/netunicorn/director/base/resources.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.3/src/netunicorn_base.egg-info/SOURCES.txt` & `netunicorn-base-0.3.4/src/netunicorn_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

