# Comparing `tmp/netunicorn-director-infrastructure-0.3.0.tar.gz` & `tmp/netunicorn-director-infrastructure-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-director-infrastructure-0.3.0.tar", last modified: Wed May 10 08:32:56 2023, max compression
+gzip compressed data, was "netunicorn-director-infrastructure-0.3.1.tar", last modified: Wed Jun  7 00:23:00 2023, max compression
```

## Comparing `netunicorn-director-infrastructure-0.3.0.tar` & `netunicorn-director-infrastructure-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.010753 netunicorn-director-infrastructure-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.010753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.010753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/simple_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/simple_rest_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.813907 netunicorn-director-infrastructure-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.813907 netunicorn-director-infrastructure-0.3.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.813907 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/rest/simple_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-07 00:22:45.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:00.817908 netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-07 00:23:00.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 00:23:00.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:23:00.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 00:23:00.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 00:23:00.000000 netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/top_level.txt
```

### Comparing `netunicorn-director-infrastructure-0.3.0/LICENSE` & `netunicorn-director-infrastructure-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-director-infrastructure-0.3.0/PKG-INFO` & `netunicorn-director-infrastructure-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-director-infrastructure
-Version: 0.3.0
+Version: 0.3.1
 Summary: netunicorn infrastructure module
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-director-infrastructure-0.3.0/pyproject.toml` & `netunicorn-director-infrastructure-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-director-infrastructure"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn infrastructure module"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/dummy.py` & `netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/connectors/dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,7 +97,18 @@
     ) -> dict[str, Result[Optional[str], str]]:
         self.logger.info(
             f"Stop executors called with {username=}, {requests_list=}, {cancellation_context=},"
             f" {authentication_context=}, {args=}, {kwargs=}"
         )
         self.logger.info("Returning dummy stop executors results")
         return {request["executor_id"]: Success(None) for request in requests_list}
+
+    async def cleanup(
+        self,
+        experiment_id: str,
+        deployments: list[Deployment],
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        self.logger.info(
+            f"Cleanup called with {experiment_id=}, {deployments=}, {args=}, {kwargs=}"
+        )
```

### Comparing `netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/simple_rest_server.py` & `netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,145 +1,169 @@
 import json
-from typing import Dict, List, Literal, Optional, TypeAlias, TypedDict, Union
+from typing import Annotated, Any, Optional
 
 import uvicorn
-from fastapi import FastAPI, Header, HTTPException
-from fastapi.openapi.models import Response
-from netunicorn.base.deployment import Deployment
-from netunicorn.base.nodes import CountableNodePool, Node
-from netunicorn.base.types import DeploymentRepresentation, NodeRepresentation
+from fastapi import BackgroundTasks, FastAPI, Header, HTTPException
+from fastapi.responses import Response
 from netunicorn.base.utils import UnicornEncoder
-from pydantic import BaseModel
-
-OperationContext: TypeAlias = Optional[str]
-
-
-class StopExecutorRequest(TypedDict):
-    executor_id: str
-    node_name: str
-
-
-class ResultData(TypedDict):
-    type: Literal["success", "failure"]
-    data: Optional[str]
-
+from netunicorn.director.base.types import (
+    ConnectorContext,
+    ExecutorsCancellationRequest,
+)
+
+from .kernel import (
+    deploy,
+    execute,
+    get_nodes,
+    health,
+    initialize,
+    parse_config,
+    shutdown,
+    stop_execution,
+    stop_executors,
+)
 
 app = FastAPI()
+config: dict[str, Any]
 
 
-class HealthResponse(BaseModel):
-    status: str
-
-
-class Results(BaseModel):
-    __root__: Dict[str, Optional[str]]
-
-
-# using original types from netunicorn.base.types introduce recursion during type inference from pydantic
-class NodesRepresentation(BaseModel):
-    node_pool_type: str
-    node_pool_data: List[Union[NodeRepresentation, "NodesRepresentation"]]
-
-
-async def parse_context(json_str: Optional[str]) -> Optional[dict[str, str]]:
+async def parse_context(json_str: Optional[str]) -> ConnectorContext:
     if not json_str or json_str == "null":
         return None
     try:
         return json.loads(json_str)  # type: ignore
     except json.JSONDecodeError as e:
         raise HTTPException(
             status_code=400,
             detail=f"Couldn't parse the context: {e}",
         )
 
 
-@app.post("/initialize", status_code=204)
-async def init() -> None:
-    return None
-
+@app.get("/health")
+async def health_handler() -> Response:
+    code, result = await health()
+    return Response(
+        status_code=code,
+        content=json.dumps(result, cls=UnicornEncoder),
+        media_type="application/json",
+    )
+
+
+@app.on_event("startup")
+async def startup_handler() -> None:
+    await initialize(config)
+
+
+@app.on_event("shutdown")
+async def shutdown_handler() -> None:
+    await shutdown()
 
-@app.get("/health", status_code=200, responses={500: {"model": HealthResponse}})
-async def health() -> HealthResponse:
-    return HealthResponse(status="OK")
 
-
-@app.post("/shutdown", status_code=204)
-async def shutdown() -> None:
-    return None
+@app.get("/nodes/{username}", status_code=200)
+async def get_nodes_handler(
+    username: str,
+    netunicorn_auth_context: Annotated[Optional[str], Header()] = None,
+) -> Response:
+    parsed_netunicorn_auth_context = await parse_context(netunicorn_auth_context)
+    code, result = await get_nodes(username, parsed_netunicorn_auth_context)
+    return Response(
+        status_code=code,
+        content=json.dumps(result, cls=UnicornEncoder),
+        media_type="application/json",
+    )
 
 
-@app.post("/deploy/{username}/{experiment_id}", status_code=200)
-async def deploy(
+@app.post("/deployment/{username}/{experiment_id}", status_code=200)
+async def deployment_handler(
     username: str,
     experiment_id: str,
-    deployments_data: List[DeploymentRepresentation],
-    netunicorn_auth_context: OperationContext = Header(default=None),
-    netunicorn_deployment_context: OperationContext = Header(default=None),
-) -> Dict[str, ResultData]:
-    _ = await parse_context(netunicorn_auth_context)
-    _ = await parse_context(netunicorn_deployment_context)
-    deployments = [Deployment.from_json(x) for x in deployments_data]
-    return {
-        x.executor_id: {
-            "type": "success",
-            "data": "something",
-        }
-        for x in deployments
-    }
+    background_tasks: BackgroundTasks,
+    netunicorn_auth_context: Annotated[Optional[str], Header()] = None,
+) -> Response:
+    parsed_netunicorn_auth_context = await parse_context(netunicorn_auth_context)
+    code, result = await deploy(
+        username, experiment_id, background_tasks, parsed_netunicorn_auth_context
+    )
+    return Response(
+        status_code=code,
+        content=json.dumps(result, cls=UnicornEncoder),
+        media_type="application/json",
+    )
 
 
-@app.post("/execute/{username}/{experiment_id}", status_code=200)
-async def execute(
+@app.post("/execution/{username}/{experiment_id}")
+async def execution_handler(
     username: str,
     experiment_id: str,
-    deployments_data: List[DeploymentRepresentation],
-    netunicorn_auth_context: OperationContext = Header(default=None),
-    netunicorn_execution_context: OperationContext = Header(default=None),
-) -> Dict[str, ResultData]:
-    _ = await parse_context(netunicorn_auth_context)
-    _ = await parse_context(netunicorn_execution_context)
-    deployments = [Deployment.from_json(x) for x in deployments_data]
-    return {
-        x.executor_id: {
-            "type": "success",
-            "data": "something",
-        }
-        for x in deployments
-    }
+    background_tasks: BackgroundTasks,
+    execution_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_auth_context: Annotated[Optional[str], Header()] = None,
+) -> Response:
+    parsed_netunicorn_auth_context = await parse_context(netunicorn_auth_context)
+    code, result = await execute(
+        username,
+        experiment_id,
+        background_tasks,
+        execution_context,
+        parsed_netunicorn_auth_context,
+    )
+    return Response(
+        status_code=code,
+        content=json.dumps(result, cls=UnicornEncoder),
+        media_type="application/json",
+    )
 
 
-@app.post("/stop_executors/{username}", status_code=200)
-async def stop_executors(
+@app.delete("/execution/{username}/{experiment_id}")
+async def stop_execution_handler(
     username: str,
-    requests_list: List[StopExecutorRequest],
-    netunicorn_auth_context: OperationContext = Header(default=None),
-    netunicorn_cancellation_context: OperationContext = Header(default=None),
-) -> Dict[str, ResultData]:
-    _ = await parse_context(netunicorn_auth_context)
-    _ = await parse_context(netunicorn_cancellation_context)
-    return {
-        x["executor_id"]: {
-            "type": "success",
-            "data": "something",
-        }
-        for x in requests_list
-    }
+    experiment_id: str,
+    background_tasks: BackgroundTasks,
+    cancellation_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_auth_context: Annotated[Optional[str], Header()] = None,
+) -> Response:
+    parsed_netunicorn_auth_context = await parse_context(netunicorn_auth_context)
+    code, result = await stop_execution(
+        username,
+        experiment_id,
+        background_tasks,
+        cancellation_context,
+        parsed_netunicorn_auth_context,
+    )
+    return Response(
+        status_code=code,
+        content=json.dumps(result, cls=UnicornEncoder),
+        media_type="application/json",
+    )
 
 
-@app.get("/nodes/{username}", status_code=200)
-async def return_nodes(
+@app.delete("/executors/{username}")
+async def stop_executors_handler(
     username: str,
-    netunicorn_auth_context: OperationContext = Header(default=None),
-) -> NodesRepresentation:
-    _ = await parse_context(netunicorn_auth_context)
-    dummy_nodes = [
-        Node(name="node1", properties={"a": 1}),
-        Node(name="node2", properties={"b": 2}),
-    ]
-    dummy_node_pool = CountableNodePool(nodes=dummy_nodes)  # type: ignore
-
-    # or use json.dumps(x, cls=UnicornEncoder)
-    json_str = json.dumps(dummy_node_pool, cls=UnicornEncoder)
-    return Response(media_type="application/json", content=json_str)  # type: ignore
-
-
-uvicorn.run(app)
+    cancellation_request: ExecutorsCancellationRequest,
+    background_tasks: BackgroundTasks,
+    netunicorn_auth_context: Annotated[Optional[str], Header()] = None,
+) -> Response:
+    parsed_netunicorn_auth_context = await parse_context(netunicorn_auth_context)
+    code, result = await stop_executors(
+        username,
+        cancellation_request["executors"],
+        background_tasks,
+        cancellation_request.get("cancellation_context", None),
+        parsed_netunicorn_auth_context,
+    )
+    return Response(
+        status_code=code,
+        content=json.dumps(result, cls=UnicornEncoder),
+        media_type="application/json",
+    )
+
+
+def main(filepath: str) -> None:
+    global config
+    config = parse_config(filepath)
+    uvicorn.run(
+        app,
+        host=config["netunicorn.infrastructure.host"],
+        port=config["netunicorn.infrastructure.port"],
+        log_level=config["netunicorn.infrastructure.log.level"],
+    )
```

### Comparing `netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/kernel.py` & `netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/kernel.py`

 * *Files identical despite different names*

### Comparing `netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/tasks.py` & `netunicorn-director-infrastructure-0.3.1/src/netunicorn/director/infrastructure/tasks.py`

 * *Files identical despite different names*

### Comparing `netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/PKG-INFO` & `netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-director-infrastructure
-Version: 0.3.0
+Version: 0.3.1
 Summary: netunicorn infrastructure module
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt` & `netunicorn-director-infrastructure-0.3.1/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,13 +6,12 @@
 src/netunicorn/director/infrastructure/kernel.py
 src/netunicorn/director/infrastructure/server.py
 src/netunicorn/director/infrastructure/tasks.py
 src/netunicorn/director/infrastructure/connectors/__init__.py
 src/netunicorn/director/infrastructure/connectors/dummy.py
 src/netunicorn/director/infrastructure/connectors/rest/__init__.py
 src/netunicorn/director/infrastructure/connectors/rest/simple_rest.py
-src/netunicorn/director/infrastructure/connectors/rest/simple_rest_server.py
 src/netunicorn_director_infrastructure.egg-info/PKG-INFO
 src/netunicorn_director_infrastructure.egg-info/SOURCES.txt
 src/netunicorn_director_infrastructure.egg-info/dependency_links.txt
 src/netunicorn_director_infrastructure.egg-info/requires.txt
 src/netunicorn_director_infrastructure.egg-info/top_level.txt
```

