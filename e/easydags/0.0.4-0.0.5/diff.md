# Comparing `tmp/easydags-0.0.4.tar.gz` & `tmp/easydags-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.4.tar", last modified: Tue Jun  6 15:18:26 2023, max compression
+gzip compressed data, was "easydags-0.0.5.tar", last modified: Wed Jun  7 00:26:51 2023, max compression
```

## Comparing `easydags-0.0.4.tar` & `easydags-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 15:18:26.257042 easydags-0.0.4/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.4/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)    12166 2023-06-06 15:18:26.256843 easydags-0.0.4/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)    11971 2023-06-06 14:56:55.000000 easydags-0.0.4/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 15:18:26.255995 easydags-0.0.4/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.4/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.4/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.4/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.4/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.4/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.4/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 15:18:26.256686 easydags-0.0.4/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)    12166 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 15:18:26.000000 easydags-0.0.4/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      104 2023-06-06 07:55:47.000000 easydags-0.0.4/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-06 15:18:26.257084 easydags-0.0.4/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-06 15:18:12.000000 easydags-0.0.4/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 00:26:51.653168 easydags-0.0.5/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.5/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    14279 2023-06-07 00:26:51.652916 easydags-0.0.5/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    14084 2023-06-07 00:22:08.000000 easydags-0.0.5/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 00:26:51.651593 easydags-0.0.5/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.5/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.5/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    20098 2023-06-06 23:52:21.000000 easydags-0.0.5/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.5/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    11304 2023-06-06 21:34:44.000000 easydags-0.0.5/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.5/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 00:26:51.652606 easydags-0.0.5/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    14279 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.0.5/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-07 00:26:51.653232 easydags-0.0.5/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-07 00:26:09.000000 easydags-0.0.5/setup.py
```

### Comparing `easydags-0.0.4/LICENSE` & `easydags-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.4/PKG-INFO` & `easydags-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -69,15 +69,15 @@
 This library will help you get through all those challenges if you use it wisely; I really hope that this helps someone with a real-world problem. 
 
 
 ## Why do we need DAGs
 
 This is a tricky question... after all, all your processes might be ok. But I will try to explain the main reason with one example:
 
-![Motivation](resource_readme/concurrence_imp.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrence_imp.png)
               
 
 Unless you are using DAGs, there is a high possibility that you are following the lineal DAG.. but thats inefficient; there is a high possibility that you have a lot of processes that can run in parallel thats why DAGs are so useful; they do not only give us one execution order, they also help us realize which task can be parallelized... and of course, this library implements that using threads (we can define the maximum number of threads with the parameter max_concurrency in the DAG constructor)
 
 
 
 
@@ -254,15 +254,15 @@
 
 dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
 
 dag.execute()
 ```
 Please note that we can check the logs to verify that model 1 and model ran in parallel
 
-![Motivation](resource_readme/concurrence_check.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrent_check.png)
 
 
 
 #### Checking the HTML output
 
 One of the coolest features of Airflow is that once you have built your DAG, you can see it on their UI and check the status of the latest run!
 
@@ -273,32 +273,54 @@
 
 1. The current structure
 2. Datetime of last execution 
 3. States of each node:
     - Green: ok
     - Red: It failed
     - Gray: Did not run because one of their dependencies failed
+4. On each node you can click/hover to check this info:
+    - Started at
+    - End at
+    - Execution time
+    - Log of error in case of an error
 
 
-![Motivation](resource_readme/html_output.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
-#### One last cool feature: The number of trials
+#### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
 ```python
 
 node = ExecNode(id_= 'id',
               exec_function = your_function,
               n_trials= 3 # set number of trials
               )
 ```
 
 
+#### Handling the errors in the dag
+
+When you call the execute method on a DAG object it will always run all the possible nodes... that means that if B depends on A and A fails we wont run A!.
+
+When that happens we create the "gray" state in the html output but the execute method will raise an exception by default to alert that there was an error... in case you do not need that alert you can simply modify the DAG creation with one additional parameter called error_type_fatal and setting it as False (this is True by default)
+
+```python
+dag = DAG(nodes,name = 'gray example',
+              max_concurrency=3, 
+              debug = False,
+              error_type_fatal= False)
+
+dag.execute() # if there is an error we wont raise an exception because error_type_fatal= False 
+```
+
+
+
 ## Deploying your DAGs
 
 #### Deploying on serverless (GCP example)
 
 Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
 
 ```python 
@@ -424,9 +446,30 @@
 
     return {"message": "Updated!"}
 
 @app.get("/ready")
 async def ready():
     return {"ready"}
 
-
 ```
+
+Then you can deploy your API on Cloud Run and schedule your DAGs with cloud scheduler (calling desired enpoint on the cloud run service).
+
+For ease of reading the example i added the complete dag definition and execution in the same file... but in reality you can import the definition and execution from a module.
+
+You can test this on your local machine following this steps:
+
+1. Install uvicorn and fastapi (you can do it with pip)
+2. Run the app with "uvicorn api_example:app --reload"
+3. Go to http://127.0.0.1:8000/dag1 or http://127.0.0.1:8000/dag2 and check the logs
+
+
+#### Deploying on serverless (GCP example)
+
+Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
+
+1. Activate the conda envioronment
+2. Run a python script with your dag
+
+After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
+
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.4/README.md` & `easydags-0.0.5/easydags.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: easydags
+Version: 0.0.5
+Summary: Dags made easy
+Author: Mateo Graciano
+Author-email: magralo@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
 
 ## Easy install using pypi
 You can easily install this in a separate conda envioronment with the following:
@@ -60,15 +69,15 @@
 This library will help you get through all those challenges if you use it wisely; I really hope that this helps someone with a real-world problem. 
 
 
 ## Why do we need DAGs
 
 This is a tricky question... after all, all your processes might be ok. But I will try to explain the main reason with one example:
 
-![Motivation](resource_readme/concurrence_imp.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrence_imp.png)
               
 
 Unless you are using DAGs, there is a high possibility that you are following the lineal DAG.. but thats inefficient; there is a high possibility that you have a lot of processes that can run in parallel thats why DAGs are so useful; they do not only give us one execution order, they also help us realize which task can be parallelized... and of course, this library implements that using threads (we can define the maximum number of threads with the parameter max_concurrency in the DAG constructor)
 
 
 
 
@@ -245,15 +254,15 @@
 
 dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
 
 dag.execute()
 ```
 Please note that we can check the logs to verify that model 1 and model ran in parallel
 
-![Motivation](resource_readme/concurrence_check.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrent_check.png)
 
 
 
 #### Checking the HTML output
 
 One of the coolest features of Airflow is that once you have built your DAG, you can see it on their UI and check the status of the latest run!
 
@@ -264,32 +273,54 @@
 
 1. The current structure
 2. Datetime of last execution 
 3. States of each node:
     - Green: ok
     - Red: It failed
     - Gray: Did not run because one of their dependencies failed
+4. On each node you can click/hover to check this info:
+    - Started at
+    - End at
+    - Execution time
+    - Log of error in case of an error
 
 
-![Motivation](resource_readme/html_output.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
-#### One last cool feature: The number of trials
+#### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
 ```python
 
 node = ExecNode(id_= 'id',
               exec_function = your_function,
               n_trials= 3 # set number of trials
               )
 ```
 
 
+#### Handling the errors in the dag
+
+When you call the execute method on a DAG object it will always run all the possible nodes... that means that if B depends on A and A fails we wont run A!.
+
+When that happens we create the "gray" state in the html output but the execute method will raise an exception by default to alert that there was an error... in case you do not need that alert you can simply modify the DAG creation with one additional parameter called error_type_fatal and setting it as False (this is True by default)
+
+```python
+dag = DAG(nodes,name = 'gray example',
+              max_concurrency=3, 
+              debug = False,
+              error_type_fatal= False)
+
+dag.execute() # if there is an error we wont raise an exception because error_type_fatal= False 
+```
+
+
+
 ## Deploying your DAGs
 
 #### Deploying on serverless (GCP example)
 
 Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
 
 ```python 
@@ -415,9 +446,30 @@
 
     return {"message": "Updated!"}
 
 @app.get("/ready")
 async def ready():
     return {"ready"}
 
+```
+
+Then you can deploy your API on Cloud Run and schedule your DAGs with cloud scheduler (calling desired enpoint on the cloud run service).
+
+For ease of reading the example i added the complete dag definition and execution in the same file... but in reality you can import the definition and execution from a module.
+
+You can test this on your local machine following this steps:
+
+1. Install uvicorn and fastapi (you can do it with pip)
+2. Run the app with "uvicorn api_example:app --reload"
+3. Go to http://127.0.0.1:8000/dag1 or http://127.0.0.1:8000/dag2 and check the logs
+
+
+#### Deploying on serverless (GCP example)
+
+Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
+
+1. Activate the conda envioronment
+2. Run a python script with your dag
+
+After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-```
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.4/easydags/dag.py` & `easydags-0.0.5/easydags/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from networkx import find_cycle
 from networkx.exception import NetworkXNoCycle, NetworkXUnfeasible
 
 import traceback
 
 from .errors import ErrorStrategy
 from .node import ExecNode
-
+from datetime import datetime
 
 # todo remove dependency on DiGraph!
 class DiGraphEx(nx.DiGraph):
     """
     Extends the DiGraph with some methods
     """
 
@@ -166,31 +166,32 @@
     """
 
     def __init__(
         self,
         exec_nodes: List[ExecNode],
         name: str = 'DAG',
         max_concurrency: int = 1,
-        debug: bool = True
+        debug: bool = True,
+        error_type_fatal: bool = True
     ):
         """
         Args:
             exec_nodes: all the ExecNodes
             max_concurrency: the maximal number of threads running in parallel
-            logger: the inferfwk logger name
-            behavior: specify the behavior if an ExecNode raises an Error. Three option are currently supported:
-                1. DAG.STRICT: stop the execution of all the DAG
-                2. DAG.ALL_CHILDREN: do not execute all children ExecNodes, and continue execution of the DAG
-                2. DAG.PERMISSIVE: continue execution of the DAG and ignore the error
+            name: Name of the dag, will be usefull for creating the html output
+            degub: weather or not you want degub messages
+
         """
         self.graph_ids = DiGraphEx()
     
         self.name = name
 
         self.debug = debug
+
+        self.error_type_fatal = error_type_fatal
         # since ExecNodes are modified they must be copied
         self.exec_nodes = exec_nodes
 
         self.max_concurrency = int(max_concurrency)
         assert max_concurrency >= 1, "Invalid maximum number of threads! Must be a positive integer"
 
         # variables necessary for DAG construction
@@ -283,15 +284,15 @@
 
                 # trim the graph from its leaf nodes
                 graph_ids.remove_node(leaf_id)
 
             # assign the new leaf nodes
             leaf_ids = graph_ids.leaf_nodes()
 
-    def __draw(self,name='Graph', k: float = 0.8, display: bool = True, t: int = 3) -> None:
+    def _draw(self,name='Graph', k: float = 0.8, display: bool = True, t: int = 3) -> None:
         """
         Draws the Networkx directed graph.
         Args:
             k: parameter for the layout of the graph, the higher, the further the nodes apart
             display: display the layout created
             t: time to display in seconds
         """
@@ -327,15 +328,20 @@
 
         titles = []
         color_map = [] 
         
         for f in  list(pos.keys()):
             state = aux[f].result['state']
             m = aux[f].result['message']
+            initial = aux[f].result['initial_time']
+            final = aux[f].result['final_time']
+            duration = aux[f].result['duration']
             title = f'''id: {f}
+                        started at: {initial} and finished at {final}
+                        exec_time: {duration}
                         state: {state}
                         message: {m}'''
             titles.append(title)
             
             if state == 0  :
                 color_map.append('grey')
             if state == 1  :
@@ -514,78 +520,41 @@
                             f"Wait for the end of a node in {running}"
                         )
                     done_, running = wait(running, return_when=FIRST_COMPLETED)
                     # go to step 6
                     continue
 
                 # 5.1 submit the exec node to the executor
-                exec_future = executor.submit(exec_node.execute, node_dict=node_dict, debug = self.debug)
+                exec_future = executor.submit(exec_node.execute, 
+                                              node_dict=node_dict, 
+                                              debug = self.debug,
+                                              initial_time = datetime.now().strftime("%Y-%m-%d, %H:%M:%S"))
                 running.add(exec_future)
                 futures[exec_node.id] = exec_future
 
                 # 5.2 wait for the sequential node to finish
                 # TODO: not sure this code ever runs
                 if exec_node.is_sequential:
                     wait(futures.values(), return_when=ALL_COMPLETED)
         self.node_dict = node_dict
 
-        self.__draw()
+        self._draw()
 
         states = [node_dict[x].result['state'] for x in node_dict]
 
-        if min(states)!=1:
+        if (min(states)!=1) and (self.error_type_fatal):
             raise ValueError('DAG did not finished as expected')
 
         return self
 
-    def safe_execute(
-        self, leaves_ids: Optional[List[Union[Hashable, ExecNode]]] = None
-    ) -> Dict[Hashable, Any]:
-        """
-        Execute the ExecNodes in topological order without priority in for loop manner for debugging purposes
-        """
-        # 1. create the subgraph to be executed
-        graph = subgraph(self.graph_ids, leaves_ids)
 
-        # 2. deep copy the node_dict to store the results in each node
-        node_dict = deepcopy(self.node_dict)
-        for node_id in graph.topological_sort():
-            node_dict[node_id].execute(node_dict)
-
-        return node_dict
 
     def handle_exception(self, graph: DiGraphEx, fut: "Future[Any]", id_: Hashable) -> None:
         """
-        checks if futures have produced exceptions, and handles them
-        according to the specified behavior
-        Args:
-            graph: the graph
-            fut: the future
-            id_: the identification of the ExecNode
-
-        Returns:
+        This simply raise an error if any
 
         """
 
-        if self.behavior == ErrorStrategy.strict:
-            # will raise the first encountered exception if there's one
-            # no simpler way to check for exception, and not supported by flake8
-            _res = fut.result()  # noqa: F841
-
-        else:
-            try:
-                _res = fut.result()  # noqa: F841
-
-            except Exception:
-                logger.exception(f"The feature {id_} encountered the following error:")
-
-                if self.behavior == ErrorStrategy.permissive:
-                    logger.warning("Ignoring exception as the behavior is set to permissive")
-
-                elif self.behavior == ErrorStrategy.all_children:
-                    # remove all its children. Current node will be removed directly afterwards
-                    successors = list(graph.successors(id_))
-                    for children_ids in successors:
-                        graph.remove_recursively(children_ids)
 
-                else:
-                    raise NotImplementedError(f"Unknown behavior name: {self.behavior}")
+        _res = fut.result()  # noqa: F841
+
+
```

### Comparing `easydags-0.0.4/easydags/node.py` & `easydags-0.0.5/easydags/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .config import Cfg
 
 # TODO: replace exec_nodes with dict
 # a temporary variable used to pass in exec_nodes to the DAG during building
 exec_nodes: List["ExecNode"] = []
 exec_nodes_lock = Lock()
-
+from datetime import datetime
 
 class ExecNode:
     """
     This class is the base executable node of the Directed Acyclic Execution Graph
     """
     def __init__(
         self,
@@ -78,23 +78,27 @@
         return f"{self.__class__.__name__} {self.id} ~ | <{hex(id(self))}>"
 
     @property
     def computed_dependencies(self) -> bool:
         return isinstance(self.depends_on, list)
 
     # this is breaking change however
-    def execute(self, node_dict: Dict[Hashable, "ExecNode"], debug: bool = True) -> Optional[Dict[str, Any]]:
+    def execute(self, 
+                node_dict: Dict[Hashable, "ExecNode"], 
+                debug: bool = True,
+                initial_time: str = datetime.now().strftime("%Y-%m-%d, %H:%M:%S")) -> Optional[Dict[str, Any]]:
         """
         Execute the ExecNode directly or according to an execution graph.
         Args:
             node_dict (Dict[Hashable, ExecNode]): A shared dictionary containing the other ExecNodes in the DAG;
                                                 the key is the id of the ExecNode.
 
         Returns: the result of the execution of the current ExecNode
         """
+        logger.info(f"Start executing {self.id} at {initial_time}")
         # 1. fabricate the arguments for this ExecNode
         if debug:
             logger.debug(f"Start executing {self.id} with task {self.exec_function}")
 
         kwargs = {
             node_dict[dep_hash].argument_name: node_dict[dep_hash].result['result']
             for dep_hash in self.depends_on_hard
@@ -155,21 +159,26 @@
                     result['message'] = msg
                     logger.info(msg)
                 i+=1
 
         
             
 
+        result['initial_time'] = initial_time
+        final = datetime.now().strftime("%Y-%m-%d, %H:%M:%S")
+        result['final_time'] = final
+        result['duration'] = (datetime.strptime(initial_time,"%Y-%m-%d, %H:%M:%S")-datetime.strptime(final,"%Y-%m-%d, %H:%M:%S")).total_seconds()
+        result['duration'] = str(-int(result['duration']))+ ' sec'
 
         self.result = result
 
         # 3. useless return value
         if debug:
             logger.debug(f"Finished executing {self.id} with task {self.exec_function}")
-        return self.result
+        return result
 
 
 
 class PreComputedExecNode(ExecNode):
     # todo must change this because two functions in the same DAG can use the same argument name for two constants!
     def __init__(self, func: Callable[..., Any], argument_name: str, value: Any):
         super().__init__(
```

### Comparing `easydags-0.0.4/easydags/ops.py` & `easydags-0.0.5/easydags/ops.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.4/easydags.egg-info/PKG-INFO` & `easydags-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: easydags
-Version: 0.0.4
-Summary: Dags made easy
-Author: Mateo Graciano
-Author-email: magralo@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
 
 ## Easy install using pypi
 You can easily install this in a separate conda envioronment with the following:
@@ -69,15 +60,15 @@
 This library will help you get through all those challenges if you use it wisely; I really hope that this helps someone with a real-world problem. 
 
 
 ## Why do we need DAGs
 
 This is a tricky question... after all, all your processes might be ok. But I will try to explain the main reason with one example:
 
-![Motivation](resource_readme/concurrence_imp.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrence_imp.png)
               
 
 Unless you are using DAGs, there is a high possibility that you are following the lineal DAG.. but thats inefficient; there is a high possibility that you have a lot of processes that can run in parallel thats why DAGs are so useful; they do not only give us one execution order, they also help us realize which task can be parallelized... and of course, this library implements that using threads (we can define the maximum number of threads with the parameter max_concurrency in the DAG constructor)
 
 
 
 
@@ -254,15 +245,15 @@
 
 dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
 
 dag.execute()
 ```
 Please note that we can check the logs to verify that model 1 and model ran in parallel
 
-![Motivation](resource_readme/concurrence_check.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrent_check.png)
 
 
 
 #### Checking the HTML output
 
 One of the coolest features of Airflow is that once you have built your DAG, you can see it on their UI and check the status of the latest run!
 
@@ -273,32 +264,54 @@
 
 1. The current structure
 2. Datetime of last execution 
 3. States of each node:
     - Green: ok
     - Red: It failed
     - Gray: Did not run because one of their dependencies failed
+4. On each node you can click/hover to check this info:
+    - Started at
+    - End at
+    - Execution time
+    - Log of error in case of an error
 
 
-![Motivation](resource_readme/html_output.png)
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
-#### One last cool feature: The number of trials
+#### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
 ```python
 
 node = ExecNode(id_= 'id',
               exec_function = your_function,
               n_trials= 3 # set number of trials
               )
 ```
 
 
+#### Handling the errors in the dag
+
+When you call the execute method on a DAG object it will always run all the possible nodes... that means that if B depends on A and A fails we wont run A!.
+
+When that happens we create the "gray" state in the html output but the execute method will raise an exception by default to alert that there was an error... in case you do not need that alert you can simply modify the DAG creation with one additional parameter called error_type_fatal and setting it as False (this is True by default)
+
+```python
+dag = DAG(nodes,name = 'gray example',
+              max_concurrency=3, 
+              debug = False,
+              error_type_fatal= False)
+
+dag.execute() # if there is an error we wont raise an exception because error_type_fatal= False 
+```
+
+
+
 ## Deploying your DAGs
 
 #### Deploying on serverless (GCP example)
 
 Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
 
 ```python 
@@ -424,9 +437,30 @@
 
     return {"message": "Updated!"}
 
 @app.get("/ready")
 async def ready():
     return {"ready"}
 
-
 ```
+
+Then you can deploy your API on Cloud Run and schedule your DAGs with cloud scheduler (calling desired enpoint on the cloud run service).
+
+For ease of reading the example i added the complete dag definition and execution in the same file... but in reality you can import the definition and execution from a module.
+
+You can test this on your local machine following this steps:
+
+1. Install uvicorn and fastapi (you can do it with pip)
+2. Run the app with "uvicorn api_example:app --reload"
+3. Go to http://127.0.0.1:8000/dag1 or http://127.0.0.1:8000/dag2 and check the logs
+
+
+#### Deploying on serverless (GCP example)
+
+Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
+
+1. Activate the conda envioronment
+2. Run a python script with your dag
+
+After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
+
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.4/setup.py` & `easydags-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.0.4',      # Start with a small number and increase it with every change you make
+  version = '0.0.5',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
```

