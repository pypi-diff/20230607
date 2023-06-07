# Comparing `tmp/pympipool-0.4.0.tar.gz` & `tmp/pympipool-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.4.0.tar", last modified: Thu Jun  1 19:00:01 2023, max compression
+gzip compressed data, was "pympipool-0.4.1.tar", last modified: Wed Jun  7 02:51:41 2023, max compression
```

## Comparing `pympipool-0.4.0.tar` & `pympipool-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-01 18:59:57.000000 pympipool-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 18:59:57.000000 pympipool-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-01 19:00:01.239016 pympipool-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-01 18:59:57.000000 pympipool-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.243016 pympipool-0.4.0/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-01 19:00:01.243016 pympipool-0.4.0/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-01 19:00:01.243016 pympipool-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-01 19:00:00.000000 pympipool-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_futurepool.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-01 18:59:57.000000 pympipool-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.891586 pympipool-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-07 02:51:33.000000 pympipool-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 02:51:33.000000 pympipool-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 02:51:41.891586 pympipool-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-07 02:51:33.000000 pympipool-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.891586 pympipool-0.4.1/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 02:51:41.891586 pympipool-0.4.1/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.887586 pympipool-0.4.1/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.887586 pympipool-0.4.1/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.887586 pympipool-0.4.1/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 02:51:41.891586 pympipool-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 02:51:41.000000 pympipool-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.891586 pympipool-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 02:51:33.000000 pympipool-0.4.1/versioneer.py
```

### Comparing `pympipool-0.4.0/LICENSE` & `pympipool-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/PKG-INFO` & `pympipool-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.4.0
+Version: 0.4.1
 Summary: pympipool - scale functions over multiple compute nodes using mpi4py
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.4.0/README.md` & `pympipool-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/pympipool/__init__.py` & `pympipool-0.4.1/pympipool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,32 +93,39 @@
         if len(hash_to_update) > 0:
             self._interface.send_dict(input_dict={"u": hash_to_update})
             for k, v in self._interface.receive_dict().items():
                 self._future_dict[k].set_result(v)
 
 
 class Worker(Executor):
-    def __init__(self, cores, oversubscribe=False, enable_flux_backend=False):
+    def __init__(
+        self, cores, oversubscribe=False, enable_flux_backend=False, init_function=None
+    ):
         self._future_queue = Queue()
         self._process = Thread(
             target=execute_tasks,
             args=(self._future_queue, cores, oversubscribe, enable_flux_backend),
         )
         self._process.start()
         _cloudpickle_update(ind=2)
+        if init_function is not None:
+            self._future_queue.put({"i": True, "f": init_function, "a": (), "k": {}})
 
     def submit(self, fn, *args, **kwargs):
         f = Future()
         self._future_queue.put({"f": fn, "a": args, "k": kwargs, "l": f})
         return f
 
     def shutdown(self, wait=True, *, cancel_futures=False):
         self._future_queue.put({"c": "close"})
         self._process.join()
 
+    def __len__(self):
+        return self._future_queue.qsize()
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.shutdown()
         return False
```

### Comparing `pympipool-0.4.0/pympipool/executor/mpipool.py` & `pympipool-0.4.1/pympipool/executor/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/pympipool/share/communication.py` & `pympipool-0.4.1/pympipool/share/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/pympipool/share/parallel.py` & `pympipool-0.4.1/pympipool/share/parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import zmq
 from tqdm import tqdm
 
 
 def parse_arguments(argument_lst):
     argument_dict = {
         "total_cores": "--cores-total",
@@ -57,28 +58,25 @@
             lst_parallel,
         )
         return list(tqdm(results, desc="Tasks", total=len(lst_parallel)))[
             ::cores_per_task
         ]
 
 
-def call_funct(input_dict, funct=None):
+def call_funct(input_dict, funct=None, memory=None):
     if funct is None:
 
         def funct(*args, **kwargs):
             return args[0].__call__(*args[1:], **kwargs)
 
-    if "a" in input_dict.keys() and "k" in input_dict.keys():
-        return funct(input_dict["f"], *input_dict["a"], **input_dict["k"])
-    elif "a" in input_dict.keys():
-        return funct(input_dict["f"], *input_dict["a"])
-    elif "k" in input_dict.keys():
-        return funct(input_dict["f"], **input_dict["k"])
-    else:
-        raise ValueError("Neither *args nor *kwargs are defined.")
+    funct_args = inspect.getfullargspec(input_dict["f"]).args
+    if memory is not None:
+        input_dict["k"].update({k: v for k, v in memory.items() if k in funct_args})
+
+    return funct(input_dict["f"], *input_dict["a"], **input_dict["k"])
 
 
 def parse_socket_communication(executor, input_dict, future_dict, cores_per_task):
     if "c" in input_dict.keys() and input_dict["c"] == "close":
         # If close "c" is communicated the process is shutdown.
         return "exit"
     elif "f" in input_dict.keys() and "l" in input_dict.keys():
@@ -91,16 +89,18 @@
                 lst=input_dict["l"],
                 cores_per_task=cores_per_task,
             )
         except Exception as error:
             return {"e": error, "et": str(type(error))}
         else:
             return {"r": output}
-    elif "f" in input_dict.keys() and (
-        "a" in input_dict.keys() or "k" in input_dict.keys()
+    elif (
+        "f" in input_dict.keys()
+        and "a" in input_dict.keys()
+        and "k" in input_dict.keys()
     ):
         # If a function "f" and either arguments "a" or keyword arguments "k" are
         # communicated pympipool uses submit() to asynchronously apply the function
         # on the arguments and or keyword arguments.
         future = call_funct(input_dict=input_dict, funct=executor.submit)
         future_hash = hash(future)
         future_dict[future_hash] = future
```

### Comparing `pympipool-0.4.0/pympipool/share/serial.py` & `pympipool-0.4.1/pympipool/share/serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,8 +89,15 @@
         task_dict = future_queue.get()
         if "c" in task_dict.keys() and task_dict["c"] == "close":
             interface.shutdown(wait=True)
             break
         elif "f" in task_dict.keys() and "l" in task_dict.keys():
             f = task_dict.pop("l")
             if f.set_running_or_notify_cancel():
-                f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+                if cores == 1:
+                    f.set_result(
+                        interface.send_and_receive_dict(input_dict=task_dict)[0]
+                    )
+                else:
+                    f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+        elif "f" in task_dict.keys() and "i" in task_dict.keys():
+            interface.send_dict(input_dict=task_dict)
```

### Comparing `pympipool-0.4.0/pympipool.egg-info/PKG-INFO` & `pympipool-0.4.1/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.4.0
+Version: 0.4.1
 Summary: pympipool - scale functions over multiple compute nodes using mpi4py
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.4.0/pympipool.egg-info/SOURCES.txt` & `pympipool-0.4.1/pympipool.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 pympipool/share/__init__.py
 pympipool/share/communication.py
 pympipool/share/parallel.py
 pympipool/share/serial.py
 tests/test_communicator_split.py
 tests/test_executor.py
 tests/test_future.py
-tests/test_futurepool.py
 tests/test_interface.py
 tests/test_parse.py
 tests/test_pool.py
 tests/test_task.py
+tests/test_worker.py
+tests/test_worker_memory.py
 tests/test_zmq.py
```

### Comparing `pympipool-0.4.0/setup.py` & `pympipool-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/tests/test_communicator_split.py` & `pympipool-0.4.1/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/tests/test_executor.py` & `pympipool-0.4.1/tests/test_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,27 +72,27 @@
         self.assertEqual(output["et"], "<class 'TypeError'>")
 
     def test_parse_socket_communication_submit_args(self):
         future_dict = {}
         with ThreadPoolExecutor(max_workers=1) as executor:
             output = parse_socket_communication(
                 executor=executor,
-                input_dict={"f": sum, "a": [[1, 1]]},
+                input_dict={"f": sum, "a": [[1, 1]], "k":{}},
                 future_dict=future_dict,
                 cores_per_task=1
             )
         future = future_dict[output['r']]
         self.assertEqual(future.result(), 2)
 
     def test_parse_socket_communication_submit_kwargs(self):
         future_dict = {}
         with ThreadPoolExecutor(max_workers=1) as executor:
             output = parse_socket_communication(
                 executor=executor,
-                input_dict={"f": function_multi_args, "k": {"a": 1, "b": 2}},
+                input_dict={"f": function_multi_args, "a":(), "k": {"a": 1, "b": 2}},
                 future_dict=future_dict,
                 cores_per_task=1
             )
         future = future_dict[output['r']]
         self.assertEqual(future.result(), 3)
 
     def test_parse_socket_communication_submit_both(self):
@@ -108,15 +108,15 @@
         self.assertEqual(future.result(), 3)
 
     def test_parse_socket_communication_update(self):
         future_dict = {}
         with ThreadPoolExecutor(max_workers=1) as executor:
             output = parse_socket_communication(
                 executor=executor,
-                input_dict={"f": sum, "a": [[1, 1]]},
+                input_dict={"f": sum, "a": [[1, 1]], "k": {}},
                 future_dict=future_dict,
                 cores_per_task=1
             )
             future_hash = output["r"]
             result = parse_socket_communication(
                 executor=executor,
                 input_dict={"u": [future_hash]},
@@ -124,9 +124,10 @@
                 cores_per_task=1
             )
         self.assertEqual(result, {"r": {future_hash: 2}})
 
     def test_funct_call_default(self):
         self.assertEqual(call_funct(input_dict={
             "f": sum,
-            "a": [[1, 2, 3]]
+            "a": [[1, 2, 3]],
+            "k": {}
         }), 6)
```

### Comparing `pympipool-0.4.0/tests/test_future.py` & `pympipool-0.4.1/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/tests/test_futurepool.py` & `pympipool-0.4.1/tests/test_worker.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,27 +18,31 @@
     return i, size, rank
 
 
 class TestFuturePool(unittest.TestCase):
     def test_pool_serial(self):
         with Worker(cores=1) as p:
             output = p.submit(calc, i=2)
+            self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
-        self.assertTrue(output.done())
+            self.assertTrue(output.done())
+            self.assertEqual(len(p), 0)
         self.assertEqual(output.result(), np.array(4))
 
     def test_pool_serial_multi_core(self):
         with Worker(cores=2) as p:
             output = p.submit(mpi_funct, i=2)
+            self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
-        self.assertTrue(output.done())
+            self.assertTrue(output.done())
+            self.assertEqual(len(p), 0)
         self.assertEqual(output.result(), [(2, 2, 0), (2, 2, 1)])
 
     def test_execute_task(self):
         f = Future()
         q = Queue()
         q.put({"f": calc, 'a': (), "k": {"i": 2}, "l": f})
         q.put({"c": "close"})
@@ -46,7 +50,21 @@
         execute_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array(4))
+
+    def test_execute_task_parallel(self):
+        f = Future()
+        q = Queue()
+        q.put({"f": calc, 'a': (), "k": {"i": 2}, "l": f})
+        q.put({"c": "close"})
+        _cloudpickle_update(ind=1)
+        execute_tasks(
+            future_queue=q,
+            cores=2,
+            oversubscribe=False,
+            enable_flux_backend=False
+        )
+        self.assertEqual(f.result(), [np.array(4), np.array(4)])
```

### Comparing `pympipool-0.4.0/tests/test_interface.py` & `pympipool-0.4.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/tests/test_parse.py` & `pympipool-0.4.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/tests/test_pool.py` & `pympipool-0.4.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/tests/test_task.py` & `pympipool-0.4.1/tests/test_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     def test_mpi(self):
         with Pool(cores=2, enable_mpi4py_backend=False) as p:
             output = p.apply(mpi_funct, 2)
         self.assertEqual(output, [(2, 2, 0), (2, 2, 1)])
 
     def test_mpi_multiple(self):
         with Pool(cores=2, enable_mpi4py_backend=False) as p:
-            p._interface.send_dict(input_dict={"f": mpi_funct, "a": [2]})
-            p._interface.send_dict(input_dict={"f": mpi_funct, "a": [2]})
-            p._interface.send_dict(input_dict={"f": mpi_funct, "a": [2]})
+            p._interface.send_dict(input_dict={"f": mpi_funct, "a": [2], "k": {}})
+            p._interface.send_dict(input_dict={"f": mpi_funct, "a": [2], "k": {}})
+            p._interface.send_dict(input_dict={"f": mpi_funct, "a": [2], "k": {}})
             output = [
                 p._interface.receive_dict(),
                 p._interface.receive_dict(),
                 p._interface.receive_dict(),
             ]
         self.assertEqual(output, [
             [(2, 2, 0), (2, 2, 1)],
```

### Comparing `pympipool-0.4.0/tests/test_zmq.py` & `pympipool-0.4.1/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.0/versioneer.py` & `pympipool-0.4.1/versioneer.py`

 * *Files identical despite different names*

