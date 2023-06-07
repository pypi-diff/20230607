# Comparing `tmp/kedro-prefect-oliver-0.1.7.tar.gz` & `tmp/kedro-prefect-oliver-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-prefect-oliver-0.1.7.tar", last modified: Thu May 18 01:00:32 2023, max compression
+gzip compressed data, was "kedro-prefect-oliver-0.1.8.tar", last modified: Wed Jun  7 20:55:59 2023, max compression
```

## Comparing `kedro-prefect-oliver-0.1.7.tar` & `kedro-prefect-oliver-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 01:00:32.965431 kedro-prefect-oliver-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-18 01:00:15.000000 kedro-prefect-oliver-0.1.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-18 01:00:32.965431 kedro-prefect-oliver-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4582 2023-05-18 01:00:15.000000 kedro-prefect-oliver-0.1.7/README
--rw-rw-rw-   0 root         (0) root         (0)     5684 2023-05-18 01:00:15.000000 kedro-prefect-oliver-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 01:00:32.965431 kedro-prefect-oliver-0.1.7/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 01:00:32.961431 kedro-prefect-oliver-0.1.7/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 01:00:32.961431 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-18 01:00:15.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-05-18 01:00:15.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver/infrastructure.py
--rw-rw-rw-   0 root         (0) root         (0)    14380 2023-05-18 01:00:15.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver/register.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 01:00:32.965431 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-18 01:00:32.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-18 01:00:32.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-18 01:00:32.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-05-18 01:00:32.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-18 01:00:32.000000 kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4582 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/README
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/infrastructure.py
+-rw-rw-rw-   0 root         (0) root         (0)    14741 2023-06-07 20:55:43.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/register.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-07 20:55:59.212405 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-07 20:55:59.000000 kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/top_level.txt
```

### Comparing `kedro-prefect-oliver-0.1.7/LICENSE` & `kedro-prefect-oliver-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.7/PKG-INFO` & `kedro-prefect-oliver-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.7
+Version: 0.1.8
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kedro-prefect-oliver-0.1.7/README` & `kedro-prefect-oliver-0.1.8/README`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.7/pyproject.toml` & `kedro-prefect-oliver-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "kedro-prefect-oliver"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     {name = "Oliver OTL", email = "dev@olivetreeholdings.com"},
 ]
 description = "Kedro-Prefect integration library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver/infrastructure.py` & `kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/infrastructure.py`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver/register.py` & `kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+import json
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union
 
-from kedro.framework.project import pipelines, find_pipelines
-from kedro.framework.session import KedroSession
-from kedro.framework.startup import bootstrap_project
-from kedro.io import DataCatalog, MemoryDataSet
-from kedro.runner import run_node
-from kedro.pipeline.node import Node
+import click
+import pendulum
+import prefect
 from pluggy import PluginManager
-
-from prefect.infrastructure.kubernetes import KubernetesJob
-from prefect.task_runners import SequentialTaskRunner
 from prefect import flow, get_run_logger, task
 from prefect.deployments import Deployment
 from prefect.filesystems import GCS
-import prefect
-
-import pendulum
-import click
-
-from prefect.utilities.hashing import file_hash
+from prefect.infrastructure.kubernetes import KubernetesJob
 from prefect.server.schemas.schedules import (
     CronSchedule,
     IntervalSchedule,
     RRuleSchedule,
 )
+from prefect.task_runners import SequentialTaskRunner
+from prefect.utilities.hashing import file_hash
+
+from kedro.framework.project import find_pipelines, pipelines
+from kedro.framework.session import KedroSession
+from kedro.framework.startup import bootstrap_project
+from kedro.io import DataCatalog, MemoryDataSet
+from kedro.pipeline.node import Node
+from kedro.runner import run_node
 
 
 class KedroInitTask(object):
     """Task to initialize KedroSession"""
 
     def __init__(
         self,
@@ -294,18 +293,20 @@
     anchor_date: str = None,
     rrule_string: str = None,
     cron_string: str = None,
     day_or: bool = True,
     timezone: str = "America/New_York",
     task_retries: int = 0,
     task_retry_delay: int = 0,
+    env_vars: Dict[str, str] = None,
 ) -> None:
     """Deploy a Kedro pipeline as a Prefect flow."""
 
     kedro_pipeline = kedro_pipeline or "__default__"
+    env_vars = env_vars or {}
     # get the dependencies and installs
     requires = None
     if dev:
         with open("src/requirements.lock", encoding="utf-8") as f:
             # Make sure we strip all comments and options (e.g "--extra-index-url")
             # that arise from a modified pip.conf file that configure global options
             # when running kedro build-reqs
@@ -343,17 +344,19 @@
         name="kubernetes-job",
         work_queue_name="kubernetes",
         tags=["kubernetes", "kedro"] + tags or [],
         storage=gcs_block,
         infrastructure=kubernetes_job,
         parameters=parameters,
         infra_overrides={
-            "env": {"EXTRA_PIP_PACKAGES": requires},
+            "env": {**env_vars, **{"EXTRA_PIP_PACKAGES": requires}},
         }
         if requires
+        else {"env": env_vars}
+        if env_vars
         else {},
         schedule=create_prefect_schedule(
             interval, anchor_date, rrule_string, cron_string, day_or, timezone
         ),
     )
     dep_id = deployment.apply()
     print("Deployment ID: {}".format(dep_id))
@@ -416,14 +419,20 @@
 )
 @click.option(
     "--task_retry_delay",
     type=int,
     default=0,
     help="Number of seconds to wait between task retries",
 )
+@click.option(
+    "--env_vars",
+    type=str,
+    default=None,
+    help="A JSON string of environment variables to pass to the Prefect flow",
+)
 def deploy_prefect_flow(
     project: str,
     entrypoint: str,
     bucket: str,
     kedro_package: str,
     kedro_pipeline: str,
     tags: List[str],
@@ -433,14 +442,15 @@
     anchor_date: str,
     rrule: str,
     cron: str,
     day_or: bool,
     timezone: str,
     task_retries: int,
     task_retry_delay: int,
+    env_vars: str,
 ) -> None:
     deploy_flow(
         project,
         entrypoint,
         bucket,
         kedro_package,
         kedro_pipeline,
@@ -451,14 +461,15 @@
         anchor_date,
         rrule,
         cron,
         day_or,
         timezone,
         task_retries,
         task_retry_delay,
+        json.loads(env_vars) if env_vars else None,
     )
 
 
 if __name__ == "__main__":
     print("Deploying Prefect flow...")
     # Standalone mode is false to make the function callable from other scripts
     # Standalone mode is a click parameter
```

### Comparing `kedro-prefect-oliver-0.1.7/src/kedro_prefect_oliver.egg-info/PKG-INFO` & `kedro-prefect-oliver-0.1.8/src/kedro_prefect_oliver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.7
+Version: 0.1.8
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

