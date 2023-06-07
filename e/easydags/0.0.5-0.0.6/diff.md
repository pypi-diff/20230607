# Comparing `tmp/easydags-0.0.5.tar.gz` & `tmp/easydags-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.5.tar", last modified: Wed Jun  7 00:26:51 2023, max compression
+gzip compressed data, was "easydags-0.0.6.tar", last modified: Wed Jun  7 19:36:53 2023, max compression
```

## Comparing `easydags-0.0.5.tar` & `easydags-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 00:26:51.653168 easydags-0.0.5/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.5/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)    14279 2023-06-07 00:26:51.652916 easydags-0.0.5/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)    14084 2023-06-07 00:22:08.000000 easydags-0.0.5/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 00:26:51.651593 easydags-0.0.5/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.5/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.5/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    20098 2023-06-06 23:52:21.000000 easydags-0.0.5/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.5/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    11304 2023-06-06 21:34:44.000000 easydags-0.0.5/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.5/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 00:26:51.652606 easydags-0.0.5/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)    14279 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-07 00:26:51.000000 easydags-0.0.5/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.0.5/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-07 00:26:51.653232 easydags-0.0.5/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-07 00:26:09.000000 easydags-0.0.5/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 19:36:53.906931 easydags-0.0.6/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.6/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    14949 2023-06-07 19:36:53.906738 easydags-0.0.6/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    14754 2023-06-07 19:26:58.000000 easydags-0.0.6/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 19:36:53.905883 easydags-0.0.6/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.6/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.6/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    20355 2023-06-07 19:17:32.000000 easydags-0.0.6/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.6/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    11304 2023-06-06 21:34:44.000000 easydags-0.0.6/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.6/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 19:36:53.906576 easydags-0.0.6/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    14949 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.0.6/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-07 19:36:53.906970 easydags-0.0.6/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-07 19:36:44.000000 easydags-0.0.6/setup.py
```

### Comparing `easydags-0.0.5/LICENSE` & `easydags-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.5/PKG-INFO` & `easydags-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -280,14 +280,50 @@
 4. On each node you can click/hover to check this info:
     - Started at
     - End at
     - Execution time
     - Log of error in case of an error
 
 
+If you do not need or do not want the html output you can set the argument draw as false in the DAG inicialization 
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+
+
+
+nodes.append( ExecNode(id_= 'f0',
+              exec_function = example0
+              ) )  
+
+
+def example1():
+    print('beginning 1')
+    print('end 1')
+
+nodes.append( ExecNode(id_= 'f1',
+              exec_function = example1 ,
+              depends_on_soft= ['f0']
+              ) )   
+
+dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
+
+dag.execute()
+```
+
+
 ![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
```

### Comparing `easydags-0.0.5/README.md` & `easydags-0.0.6/easydags.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: easydags
+Version: 0.0.6
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
@@ -271,14 +280,50 @@
 4. On each node you can click/hover to check this info:
     - Started at
     - End at
     - Execution time
     - Log of error in case of an error
 
 
+If you do not need or do not want the html output you can set the argument draw as false in the DAG inicialization 
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+
+
+
+nodes.append( ExecNode(id_= 'f0',
+              exec_function = example0
+              ) )  
+
+
+def example1():
+    print('beginning 1')
+    print('end 1')
+
+nodes.append( ExecNode(id_= 'f1',
+              exec_function = example1 ,
+              depends_on_soft= ['f0']
+              ) )   
+
+dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
+
+dag.execute()
+```
+
+
 ![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
@@ -459,8 +504,8 @@
 Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
 
 1. Activate the conda envioronment
 2. Run a python script with your dag
 
 After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-You will need to to make the bash and python script executables with chmod +x {file}
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.5/easydags/dag.py` & `easydags-0.0.6/easydags/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,29 +167,33 @@
 
     def __init__(
         self,
         exec_nodes: List[ExecNode],
         name: str = 'DAG',
         max_concurrency: int = 1,
         debug: bool = True,
-        error_type_fatal: bool = True
+        error_type_fatal: bool = True,
+        draw: bool = True
     ):
         """
         Args:
             exec_nodes: all the ExecNodes
             max_concurrency: the maximal number of threads running in parallel
             name: Name of the dag, will be usefull for creating the html output
             degub: weather or not you want degub messages
+            error_type_fatal: weather or not you want the whole process to fail if at least one node fails
+            draw: Set false if you do not want the html output
 
         """
         self.graph_ids = DiGraphEx()
     
         self.name = name
 
         self.debug = debug
+        self.draw = draw
 
         self.error_type_fatal = error_type_fatal
         # since ExecNodes are modified they must be copied
         self.exec_nodes = exec_nodes
 
         self.max_concurrency = int(max_concurrency)
         assert max_concurrency >= 1, "Invalid maximum number of threads! Must be a positive integer"
@@ -396,15 +400,15 @@
             "physics": {
                 "enabled": false
             }
         }
         ''')
 
 
-        g.show('nx.html')
+        #g.show('nx.html')
         
 
         import re 
         html_str = re.sub(r'<center>.+?<\/h1>\s+<\/center>', '', g.html, 1, re.DOTALL)
         h = open(f'{self.name}_states_run.html','w')
         h.write(html_str)
         h.close()
@@ -532,16 +536,17 @@
                 futures[exec_node.id] = exec_future
 
                 # 5.2 wait for the sequential node to finish
                 # TODO: not sure this code ever runs
                 if exec_node.is_sequential:
                     wait(futures.values(), return_when=ALL_COMPLETED)
         self.node_dict = node_dict
-
-        self._draw()
+        
+        if self.draw:
+            self._draw()
 
         states = [node_dict[x].result['state'] for x in node_dict]
 
         if (min(states)!=1) and (self.error_type_fatal):
             raise ValueError('DAG did not finished as expected')
 
         return self
```

### Comparing `easydags-0.0.5/easydags/node.py` & `easydags-0.0.6/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.5/easydags/ops.py` & `easydags-0.0.6/easydags/ops.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.5/easydags.egg-info/PKG-INFO` & `easydags-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: easydags
-Version: 0.0.5
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
@@ -280,14 +271,50 @@
 4. On each node you can click/hover to check this info:
     - Started at
     - End at
     - Execution time
     - Log of error in case of an error
 
 
+If you do not need or do not want the html output you can set the argument draw as false in the DAG inicialization 
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+
+
+
+nodes.append( ExecNode(id_= 'f0',
+              exec_function = example0
+              ) )  
+
+
+def example1():
+    print('beginning 1')
+    print('end 1')
+
+nodes.append( ExecNode(id_= 'f1',
+              exec_function = example1 ,
+              depends_on_soft= ['f0']
+              ) )   
+
+dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
+
+dag.execute()
+```
+
+
 ![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
@@ -468,8 +495,8 @@
 Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
 
 1. Activate the conda envioronment
 2. Run a python script with your dag
 
 After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-You will need to to make the bash and python script executables with chmod +x {file}
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.5/setup.py` & `easydags-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.0.5',      # Start with a small number and increase it with every change you make
+  version = '0.0.6',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
```

