# Comparing `tmp/pympipool-0.4.1.tar.gz` & `tmp/pympipool-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.4.1.tar", last modified: Wed Jun  7 02:51:41 2023, max compression
+gzip compressed data, was "pympipool-0.4.2.tar", last modified: Wed Jun  7 05:16:59 2023, max compression
```

## Comparing `pympipool-0.4.1.tar` & `pympipool-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.891586 pympipool-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-07 02:51:33.000000 pympipool-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 02:51:33.000000 pympipool-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 02:51:41.891586 pympipool-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-07 02:51:33.000000 pympipool-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.891586 pympipool-0.4.1/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 02:51:41.891586 pympipool-0.4.1/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.887586 pympipool-0.4.1/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.887586 pympipool-0.4.1/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-07 02:51:33.000000 pympipool-0.4.1/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.887586 pympipool-0.4.1/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 02:51:41.000000 pympipool-0.4.1/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 02:51:41.891586 pympipool-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 02:51:41.000000 pympipool-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:51:41.891586 pympipool-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 02:51:33.000000 pympipool-0.4.1/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 02:51:33.000000 pympipool-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.527638 pympipool-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-07 05:16:56.000000 pympipool-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 05:16:56.000000 pympipool-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 05:16:59.527638 pympipool-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-07 05:16:56.000000 pympipool-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.527638 pympipool-0.4.2/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 05:16:59.527638 pympipool-0.4.2/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.523638 pympipool-0.4.2/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.523638 pympipool-0.4.2/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.523638 pympipool-0.4.2/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 05:16:59.527638 pympipool-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 05:16:59.000000 pympipool-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.527638 pympipool-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 05:16:56.000000 pympipool-0.4.2/versioneer.py
```

### Comparing `pympipool-0.4.1/LICENSE` & `pympipool-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/PKG-INFO` & `pympipool-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.4.1
+Version: 0.4.2
 Summary: pympipool - scale functions over multiple compute nodes using mpi4py
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.4.1/README.md` & `pympipool-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/pympipool/__init__.py` & `pympipool-0.4.2/pympipool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,26 +38,28 @@
     def __init__(
         self,
         cores=1,
         cores_per_task=1,
         oversubscribe=False,
         enable_flux_backend=False,
         enable_mpi4py_backend=True,
+        cwd=None,
     ):
         self._future_dict = {}
         self._interface = SocketInterface()
         self._interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=self._interface.bind_to_random_port(),
                 cores=cores,
                 cores_per_task=cores_per_task,
                 oversubscribe=oversubscribe,
                 enable_flux_backend=enable_flux_backend,
                 enable_mpi4py_backend=enable_mpi4py_backend,
-            )
+            ),
+            cwd=cwd,
         )
         _cloudpickle_update(ind=2)
 
     def map(self, fn, iterables, timeout=None, chunksize=1):
         """
         Map a given function on a list of attributes.
 
@@ -94,20 +96,25 @@
             self._interface.send_dict(input_dict={"u": hash_to_update})
             for k, v in self._interface.receive_dict().items():
                 self._future_dict[k].set_result(v)
 
 
 class Worker(Executor):
     def __init__(
-        self, cores, oversubscribe=False, enable_flux_backend=False, init_function=None
+        self,
+        cores,
+        oversubscribe=False,
+        enable_flux_backend=False,
+        init_function=None,
+        cwd=None,
     ):
         self._future_queue = Queue()
         self._process = Thread(
             target=execute_tasks,
-            args=(self._future_queue, cores, oversubscribe, enable_flux_backend),
+            args=(self._future_queue, cores, oversubscribe, enable_flux_backend, cwd),
         )
         self._process.start()
         _cloudpickle_update(ind=2)
         if init_function is not None:
             self._future_queue.put({"i": True, "f": init_function, "a": (), "k": {}})
 
     def submit(self, fn, *args, **kwargs):
```

### Comparing `pympipool-0.4.1/pympipool/executor/mpiexec.py` & `pympipool-0.4.2/pympipool/executor/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/pympipool/executor/mpipool.py` & `pympipool-0.4.2/pympipool/executor/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/pympipool/share/communication.py` & `pympipool-0.4.2/pympipool/share/communication.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,20 +24,21 @@
     def send_and_receive_dict(self, input_dict):
         self.send_dict(input_dict=input_dict)
         return self.receive_dict()
 
     def bind_to_random_port(self):
         return self._socket.bind_to_random_port("tcp://*")
 
-    def bootup(self, command_lst):
+    def bootup(self, command_lst, cwd=None):
         self._process = subprocess.Popen(
             args=command_lst,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             stdin=subprocess.PIPE,
+            cwd=cwd,
         )
 
     def shutdown(self, wait=True):
         if self._process is not None and self._process.poll() is None:
             self.send_dict(input_dict={"c": "close"})
             self._process_close(wait=wait)
         if self._socket is not None:
```

### Comparing `pympipool-0.4.1/pympipool/share/parallel.py` & `pympipool-0.4.2/pympipool/share/parallel.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/pympipool/share/serial.py` & `pympipool-0.4.2/pympipool/share/serial.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,25 +69,26 @@
         oversubscribe=oversubscribe,
         enable_flux_backend=enable_flux_backend,
         enable_mpi4py_backend=enable_mpi4py_backend,
     )
     return command_lst
 
 
-def execute_tasks(future_queue, cores, oversubscribe, enable_flux_backend):
+def execute_tasks(future_queue, cores, oversubscribe, enable_flux_backend, cwd=None):
     interface = SocketInterface()
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
             cores_per_task=1,
             oversubscribe=oversubscribe,
             enable_flux_backend=enable_flux_backend,
             enable_mpi4py_backend=False,
-        )
+        ),
+        cwd=cwd,
     )
     while True:
         task_dict = future_queue.get()
         if "c" in task_dict.keys() and task_dict["c"] == "close":
             interface.shutdown(wait=True)
             break
         elif "f" in task_dict.keys() and "l" in task_dict.keys():
```

### Comparing `pympipool-0.4.1/pympipool.egg-info/PKG-INFO` & `pympipool-0.4.2/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.4.1
+Version: 0.4.2
 Summary: pympipool - scale functions over multiple compute nodes using mpi4py
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.4.1/pympipool.egg-info/SOURCES.txt` & `pympipool-0.4.2/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/setup.py` & `pympipool-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_communicator_split.py` & `pympipool-0.4.2/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_executor.py` & `pympipool-0.4.2/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_future.py` & `pympipool-0.4.2/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_interface.py` & `pympipool-0.4.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_parse.py` & `pympipool-0.4.2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_pool.py` & `pympipool-0.4.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_task.py` & `pympipool-0.4.2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_worker.py` & `pympipool-0.4.2/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_worker_memory.py` & `pympipool-0.4.2/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/tests/test_zmq.py` & `pympipool-0.4.2/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.1/versioneer.py` & `pympipool-0.4.2/versioneer.py`

 * *Files identical despite different names*

