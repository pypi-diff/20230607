# Comparing `tmp/pylammpsmpi-0.1.0.tar.gz` & `tmp/pylammpsmpi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpsmpi-0.1.0.tar", last modified: Wed Mar  1 12:50:53 2023, max compression
+gzip compressed data, was "pylammpsmpi-0.1.1.tar", last modified: Wed Jun  7 15:18:09 2023, max compression
```

## Comparing `pylammpsmpi-0.1.0.tar` & `pylammpsmpi-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/pylammpsmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/pylammpsmpi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/lammps_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:53.915368 pylammpsmpi-0.1.0/pylammpsmpi/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/mpi/lmpmpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/pylammpsmpi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/pylammpsmpi/utils/lammps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:53.915368 pylammpsmpi-0.1.0/pylammpsmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-01 12:50:53.000000 pylammpsmpi-0.1.0/pylammpsmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-01 12:50:53.000000 pylammpsmpi-0.1.0/pylammpsmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 12:50:53.000000 pylammpsmpi-0.1.0/pylammpsmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-01 12:50:53.000000 pylammpsmpi-0.1.0/pylammpsmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-01 12:50:53.000000 pylammpsmpi-0.1.0/pylammpsmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-01 12:50:53.000000 pylammpsmpi-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:50:53.919368 pylammpsmpi-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/tests/test_pylammpsmpi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/tests/test_pylammpsmpi_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-01 12:50:50.000000 pylammpsmpi-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/lammps_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/mpi/lmpmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/utils/lammps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.116839 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 15:18:08.000000 pylammpsmpi-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/tests/test_pylammpsmpi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/tests/test_pylammpsmpi_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/versioneer.py
```

### Comparing `pylammpsmpi-0.1.0/LICENSE` & `pylammpsmpi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.0/PKG-INFO` & `pylammpsmpi-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.1.0/README.md` & `pylammpsmpi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.0/pylammpsmpi/lammps_wrapper.py` & `pylammpsmpi-0.1.1/pylammpsmpi/lammps_wrapper.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.0/pylammpsmpi/mpi/lmpmpi.py` & `pylammpsmpi-0.1.1/pylammpsmpi/mpi/lmpmpi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from ctypes import c_double, c_int
 from mpi4py import MPI
 import numpy as np
-import pickle
+import cloudpickle
 import sys
 import zmq
 from lammps import lammps
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
@@ -38,22 +38,16 @@
     "torque": {"type": 3, "gtype": 1, "dim": 3},
     "radius": {"type": 2, "gtype": 1, "dim": 1},
     "image": {"type": 2, "gtype": 0, "dim": 3},
     # we can add more quantities as needed
     # taken directly from atom.cpp -> extract()
 }
 
-# Lammps executable
-args = ["-screen", "none"]
-if len(sys.argv) > 3:
-    args.extend(sys.argv[3:])
-job = lammps(cmdargs=args)
 
-
-def extract_compute(funct_args):
+def extract_compute(job, funct_args):
     def convert_data(val, type, length, width):
         data = []
         if type == 2:
             for i in range(length):
                 dummy = []
                 for j in range(width):
                     dummy.append(val[i][j])
@@ -84,50 +78,50 @@
         if MPI.COMM_WORLD.rank == 0:
             length = job.get_natoms()
             return convert_data(val=val, type=type, length=length, width=width)
     else:  # Todo
         raise ValueError("Local style is currently not supported")
 
 
-def get_version(funct_args):
+def get_version(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.version()
 
 
-def get_file(funct_args):
+def get_file(job, funct_args):
     job.file(*funct_args)
     return 1
 
 
-def commands_list(funct_args):
+def commands_list(job, funct_args):
     job.commands_list(*funct_args)
     return 1
 
 
-def commands_string(funct_args):
+def commands_string(job, funct_args):
     job.commands_string(*funct_args)
     return 1
 
 
-def extract_setting(funct_args):
+def extract_setting(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.extract_setting(*funct_args)
 
 
-def extract_global(funct_args):
+def extract_global(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.extract_global(*funct_args)
 
 
-def extract_box(funct_args):
+def extract_box(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.extract_box(*funct_args)
 
 
-def extract_atom(funct_args):
+def extract_atom(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         # extract atoms return an internal data type
         # this has to be reformatted
         name = str(funct_args[0])
         if not name in atom_properties.keys():
             return []
 
@@ -149,20 +143,20 @@
                 data.append(dummy)
         else:
             data = [val[x] for x in range(int(natoms))]
 
         return np.array(data)
 
 
-def extract_fix(funct_args):
+def extract_fix(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.extract_fix(*funct_args)
 
 
-def extract_variable(funct_args):
+def extract_variable(job, funct_args):
     # in the args - if the third one,
     # which is the type is 1 - a lammps array is returned
     if funct_args[2] == 1:
         data = _gather_data_from_all_processors(
             data=job.numpy.extract_variable(*funct_args)
         )
         if MPI.COMM_WORLD.rank == 0:
@@ -173,29 +167,29 @@
             try:
                 data = job.extract_variable(*funct_args)
             except ValueError:
                 return []
             return data
 
 
-def get_natoms(funct_args):
+def get_natoms(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.get_natoms()
 
 
-def set_variable(funct_args):
+def set_variable(job, funct_args):
     return job.set_variable(*funct_args)
 
 
-def reset_box(funct_args):
+def reset_box(job, funct_args):
     job.reset_box(*funct_args)
     return 1
 
 
-def gather_atoms(funct_args):
+def gather_atoms(job, funct_args):
     # extract atoms return an internal data type
     # this has to be reformatted
     name = str(funct_args[0])
     if name not in atom_properties.keys():
         return []
 
     # this block prevents error when trying to access values
@@ -213,15 +207,15 @@
     if dim > 1:
         data = [val[x : x + dim] for x in range(0, len(val), dim)]
     else:
         data = list(val)
     return np.array(data)
 
 
-def gather_atoms_concat(funct_args):
+def gather_atoms_concat(job, funct_args):
     # extract atoms return an internal data type
     # this has to be reformatted
     name = str(funct_args[0])
     if not name in atom_properties.keys():
         return []
 
     # this block prevents error when trying to access values
@@ -239,15 +233,15 @@
     if dim > 1:
         data = [val[x : x + dim] for x in range(0, len(val), dim)]
     else:
         data = list(val)
     return np.array(data)
 
 
-def gather_atoms_subset(funct_args):
+def gather_atoms_subset(job, funct_args):
     # convert to ctypes
     name = str(funct_args[0])
     lenids = int(funct_args[1])
     ids = funct_args[2]
 
     # prep ids
     cids = (lenids * c_int)()
@@ -276,103 +270,84 @@
     if dim > 1:
         data = [val[x : x + dim] for x in range(0, len(val), dim)]
     else:
         data = list(val)
     return np.array(data)
 
 
-def create_atoms(funct_args):
-    # we have to process the input items
-    # args are natoms, ids, type, x, v, image, shrinkexceed
-    natoms = funct_args[0]
-    ids = funct_args[1]
-    type = funct_args[2]
-    x = funct_args[3]
-    v = funct_args[4]
-    image = funct_args[5]
-    shrinkexceed = funct_args[6]
-
-    id_lmp = (c_int * natoms)()
-    id_lmp[:] = ids
-
-    type_lmp = (c_int * natoms)()
-    type_lmp[:] = type
-
-    image_lmp = (c_int * natoms)()
-    image_lmp[:] = image
-
-    args = [natoms, id_lmp, type_lmp, x, v, image_lmp, shrinkexceed]
-    job.create_atoms(*args)
+def create_atoms(job, funct_args):
+    job.create_atoms(*funct_args)
     return 1
 
 
-def has_exceptions(funct_args):
+def has_exceptions(job, funct_args):
     return job.has_exceptions
 
 
-def has_gzip_support(funct_args):
+def has_gzip_support(job, funct_args):
     return job.has_gzip_support
 
 
-def has_png_support(funct_args):
+def has_png_support(job, funct_args):
     return job.has_png_support
 
 
-def has_jpeg_support(funct_args):
+def has_jpeg_support(job, funct_args):
     return job.has_jpeg_support
 
 
-def has_ffmpeg_support(funct_args):
+def has_ffmpeg_support(job, funct_args):
     return job.has_ffmpeg_support
 
 
-def installed_packages(funct_args):
+def installed_packages(job, funct_args):
     return job.installed_packages
 
 
-def set_fix_external_callback(funct_args):
+def set_fix_external_callback(job, funct_args):
     job.set_fix_external_callback(*funct_args)
+    return 1
 
 
-def get_neighlist(funct_args):
+def get_neighlist(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.get_neighlist(*funct_args)
 
 
-def find_pair_neighlist(funct_args):
+def find_pair_neighlist(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.find_pair_neighlist(*funct_args)
 
 
-def find_fix_neighlist(funct_args):
+def find_fix_neighlist(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.find_fix_neighlist(*funct_args)
 
 
-def find_compute_neighlist(funct_args):
+def find_compute_neighlist(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.find_compute_neighlist(*funct_args)
 
 
-def get_neighlist_size(funct_args):
+def get_neighlist_size(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.get_neighlist_size(*funct_args)
 
 
-def get_neighlist_element_neighbors(funct_args):
+def get_neighlist_element_neighbors(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return job.get_neighlist_element_neighbors(*funct_args)
 
 
-def get_thermo(funct_args):
+def get_thermo(job, funct_args):
     if MPI.COMM_WORLD.rank == 0:
         return np.array(job.get_thermo(*funct_args))
 
 
-def scatter_atoms(funct_args):
+def scatter_atoms(job, funct_args):
     name = str(funct_args[0])
     py_vector = funct_args[1]
     # now see if its an integer or double type- but before flatten
     py_vector = np.array(py_vector).flatten()
 
     if atom_properties[name]["gtype"] == 0:
         c_vector = (len(py_vector) * c_int)(*py_vector)
@@ -381,15 +356,15 @@
 
     job.scatter_atoms(
         name, atom_properties[name]["gtype"], atom_properties[name]["dim"], c_vector
     )
     return 1
 
 
-def scatter_atoms_subset(funct_args):
+def scatter_atoms_subset(job, funct_args):
     name = str(funct_args[0])
     lenids = int(funct_args[2])
     ids = funct_args[3]
 
     # prep ids
     cids = (lenids * c_int)()
     for i in range(lenids):
@@ -411,15 +386,15 @@
         lenids,
         cids,
         c_vector,
     )
     return 1
 
 
-def command(funct_args):
+def command(job, funct_args):
     job.command(funct_args)
     return 1
 
 
 def select_cmd(argument):
     """
     Select a lammps command
@@ -479,30 +454,43 @@
         data = []
         for vl in data_gather:
             for v in vl:
                 data.append(v)
         return data
 
 
-if __name__ == "__main__":
+def _run_lammps_mpi(argument_lst):
     if MPI.COMM_WORLD.rank == 0:
         context = zmq.Context()
         socket = context.socket(zmq.PAIR)
-        argument_lst = sys.argv
         port_selected = argument_lst[argument_lst.index("--zmqport") + 1]
         socket.connect("tcp://localhost:" + port_selected)
+    else:
+        context, socket = None, None
+    # Lammps executable
+    args = ["-screen", "none"]
+    if len(argument_lst) > 3:
+        args.extend(argument_lst[3:])
+    job = lammps(cmdargs=args)
     while True:
         if MPI.COMM_WORLD.rank == 0:
-            input_dict = pickle.loads(socket.recv())
+            input_dict = cloudpickle.loads(socket.recv())
             # with open('process.txt', 'a') as file:
             #     print('Input:', input_dict, file=file)
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
         if input_dict["c"] == "close":
+            if MPI.COMM_WORLD.rank == 0:
+                socket.close()
+                context.term()
             job.close()
             break
-        output = select_cmd(input_dict["c"])(input_dict["d"])
+        output = select_cmd(input_dict["c"])(job=job, funct_args=input_dict["d"])
         if MPI.COMM_WORLD.rank == 0 and output is not None:
             # with open('process.txt', 'a') as file:
             #     print('Output:', output, file=file)
-            socket.send(pickle.dumps(output))
+            socket.send(cloudpickle.dumps({"r": output}))
+
+
+if __name__ == "__main__":
+    _run_lammps_mpi(argument_lst=sys.argv)
```

### Comparing `pylammpsmpi-0.1.0/pylammpsmpi/utils/commands.py` & `pylammpsmpi-0.1.1/pylammpsmpi/utils/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "get_neighlist_size",
     "get_neighlist_element_neighbors",
     "command",
     "gather_atoms",
     "scatter_atoms",
     "get_thermo",
     "extract_compute",
+    "create_atoms",
 ]
 
 prop_list = [
     "version",
     "natoms",
     "has_exceptions",
     "has_gzip_support",
```

### Comparing `pylammpsmpi-0.1.0/pylammpsmpi/utils/lammps.py` & `pylammpsmpi-0.1.1/pylammpsmpi/utils/lammps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
-import pickle
-import subprocess
-import zmq
+from pympipool import SocketInterface
 
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -22,45 +20,42 @@
 
 class LammpsBase:
     def __init__(
         self, cores=8, oversubscribe=False, working_directory=".", cmdargs=None
     ):
         self.cores = cores
         self.working_directory = working_directory
+        self._interface = SocketInterface()
         self._process = None
         self._oversubscribe = oversubscribe
         self._cmdargs = cmdargs
-        self._socket = None
 
     def start_process(self):
+        port_selected = self._interface.bind_to_random_port()
         executable = os.path.join(
             os.path.dirname(os.path.abspath(__file__)), "../mpi", "lmpmpi.py"
         )
-        context = zmq.Context()
-        self._socket = context.socket(zmq.PAIR)
-        port_selected = self._socket.bind_to_random_port("tcp://*")
         cmds = ["mpiexec"]
         if self._oversubscribe:
             cmds += ["--oversubscribe"]
         cmds += [
             "-n",
             str(self.cores),
             "python",
             executable,
             "--zmqport",
             str(port_selected),
         ]
         if self._cmdargs is not None:
             cmds.extend(self._cmdargs)
-        self._process = subprocess.Popen(
-            cmds,
-            stdout=subprocess.PIPE,
-            stderr=None,
-            stdin=subprocess.PIPE,
-            cwd=self.working_directory,
+        self._interface.bootup(command_lst=cmds, cwd=self.working_directory)
+
+    def _send_and_receive_dict(self, command, data=None):
+        return self._interface.send_and_receive_dict(
+            input_dict={"c": command, "d": data}
         )
 
     def _send(self, command, data=None):
         """
         Send a command to the Lammps Library executable
 
         Parameters
@@ -71,31 +66,30 @@
         data: optional, default None
             data to be sent to the command
 
         Returns
         -------
         None
         """
-        self._socket.send(pickle.dumps({"c": command, "d": data}))
+        self._interface.send_dict({"c": command, "d": data})
 
     def _receive(self):
         """
         Receive data from the Lammps library
 
         Parameters
         ----------
         None
 
         Returns
         -------
         data : string
             data from the command
         """
-        output = pickle.loads(self._socket.recv())
-        return output
+        return self._interface.receive_dict()
 
     @property
     def version(self):
         """
         Get the version of lammps
 
         Parameters
@@ -103,16 +97,15 @@
         None
 
         Returns
         -------
         version: string
             version string of lammps
         """
-        self._send(command="get_version", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="get_version", data=[])
 
     def file(self, inputfile):
         """
         Read script from an input file
 
         Parameters
         ----------
@@ -121,21 +114,19 @@
 
         Returns
         -------
         None
         """
         if not os.path.exists(inputfile):
             raise FileNotFoundError("Input file does not exist")
-        self._send(command="get_file", data=[inputfile])
-        _ = self._receive()
+        _ = self._send_and_receive_dict(command="get_file", data=[inputfile])
 
     # TODO
     def extract_setting(self, *args):
-        self._send(command="extract_setting", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_setting", data=list(args))
 
     def extract_global(self, name):
         """
         Extract value of global simulation parameters
 
         Parameters
         ----------
@@ -155,16 +146,15 @@
         Also global constants defined by units can be accessed-
         "boltz", "hplanck", "mvv2e", "ftm2v", "mv2d",
         "nktv2p", "qqr2e", "qe2f", "vxmu2f", "xxt2kmu",
         "dielectric", "qqr2e", "e_mass", "hhmrr2e",
         "mvh2r", "angstrom", "femtosecond", "qelectron"
 
         """
-        self._send(command="extract_global", data=[name])
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_global", data=[name])
 
     def extract_box(self):
         """
         Get the simulation box
 
         Parameters
         ----------
@@ -174,16 +164,15 @@
         -------
         box : list
             of the form `[boxlo,boxhi,xy,yz,xz,periodicity,box_change]` where
             `boxlo` and `boxhi` are lower and upper bounds of the box in three dimensions,
             `xy, yz, xz` are the box tilts, `periodicity` is an array which shows if
             the box is periodic in three dimensions.
         """
-        self._send(command="extract_box", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_box", data=[])
 
     def extract_atom(self, name):
         """
         Extract a property of the atoms
 
         Parameters
         ----------
@@ -202,16 +191,15 @@
         This method only gathers information from the current processor.
         Rest of the values would be zero.
 
         See Also
         --------
         scatter_atoms
         """
-        self._send(command="extract_atom", data=list([name]))
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_atom", data=list([name]))
 
     def extract_fix(self, *args):
         """
         Extract a fix value
 
         Parameters
         ----------
@@ -235,17 +223,15 @@
             index to select fix output
 
         Returns
         -------
         value
             Fix data corresponding to the requested dimensions
         """
-
-        self._send(command="extract_fix", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_fix", data=list(args))
 
     def extract_variable(self, *args):
         """
         Extract the value of a variable
 
         Parameters
         ----------
@@ -265,16 +251,15 @@
             value of variable depending on the requested dimension
 
         Notes
         -----
         Currently only returns the information provided on a single processor
 
         """
-        self._send(command="extract_variable", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_variable", data=list(args))
 
     @property
     def natoms(self):
         return self.get_natoms()
 
     def get_natoms(self):
         """
@@ -285,17 +270,15 @@
         None
 
         Returns
         -------
         natoms : int
             number of atoms
         """
-
-        self._send(command="get_natoms", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="get_natoms", data=[])
 
     def set_variable(self, *args):
         """
         Set the value of a string style variable
 
         Parameters
         ----------
@@ -306,16 +289,15 @@
             value of the variable
 
         Returns
         -------
         flag : int
             0 if successfull, -1 otherwise
         """
-        self._send(command="set_variable", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(command="set_variable", data=list(args))
 
     def reset_box(self, *args):
         """
         Reset the simulation box
 
         Parameters
         ----------
@@ -324,16 +306,15 @@
 
         boxhi: array of floats
             upper bound of box in three dimensions
 
         xy, yz, xz : floats
             box tilts
         """
-        self._send(command="reset_box", data=list(args))
-        _ = self._receive()
+        _ = self._send_and_receive_dict(command="reset_box", data=list(args))
 
     def generate_atoms(
         self, ids=None, type=None, x=None, v=None, image=None, shrinkexceed=False
     ):
         """
         Create atoms on all procs
 
@@ -363,23 +344,24 @@
         None
 
         """
         self.create_atoms(
             ids=ids, type=type, x=x, v=v, image=image, shrinkexceed=shrinkexceed
         )
 
-    def create_atoms(
-        self, ids=None, type=None, x=None, v=None, image=None, shrinkexceed=False
-    ):
+    def create_atoms(self, n, id, type, x, v=None, image=None, shrinkexceed=False):
         """
         Create atoms on all procs
 
         Parameters
         ----------
-        ids : list of ints, optional
+        n : int
+            number of atoms
+
+        id : list of ints, optional
             ids of N atoms that need to be created
             if not specified, ids from 1 to N are assigned
 
         type : list of atom types, optional
             type of N atoms, if not specied, all atoms are assigned as type 1
 
         x: list of positions
@@ -397,71 +379,57 @@
         Returns
         -------
         None
 
         """
 
         if x is not None:
-            natoms = len(x)
-            if type is None:
-                type = [1] * natoms
-            if ids is None:
-                ids = list(range(1, natoms + 1))
-            if image is None:
-                image = [0] * natoms
-
-            funct_args = [natoms, ids, type, x, v, image, shrinkexceed]
-            self._send(command="create_atoms", data=funct_args)
-            _ = self._receive()
+            funct_args = [n, id, type, x, v, image, shrinkexceed]
+            _ = self._send_and_receive_dict(command="create_atoms", data=funct_args)
         else:
             raise TypeError("Value of x cannot be None")
 
     @property
     def has_exceptions(self):
         """Return whether the LAMMPS shared library was compiled with C++ exceptions handling enabled"""
-        self._send(command="has_exceptions", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="has_exceptions", data=[])
 
     @property
     def has_gzip_support(self):
-        self._send(command="has_gzip_support", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="has_gzip_support", data=[])
 
     @property
     def has_png_support(self):
-        self._send(command="has_png_support", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="has_png_support", data=[])
 
     @property
     def has_jpeg_support(self):
-        self._send(command="has_jpeg_support", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="has_jpeg_support", data=[])
 
     @property
     def has_ffmpeg_support(self):
-        self._send(command="has_ffmpeg_support", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="has_ffmpeg_support", data=[])
 
     @property
     def installed_packages(self):
-        self._send(command="get_installed_packages", data=[])
-        return self._receive()
+        return self._send_and_receive_dict(command="get_installed_packages", data=[])
 
     def set_fix_external_callback(self, *args):
-        self._send(command="set_fix_external_callback", data=list(args))
+        _ = self._send_and_receive_dict(
+            command="set_fix_external_callback", data=list(args)
+        )
 
     def get_neighlist(self, *args):
         """Returns an instance of :class:`NeighList` which wraps access to the neighbor list with the given index
         :param idx: index of neighbor list
         :type  idx: int
         :return: an instance of :class:`NeighList` wrapping access to neighbor list data
         :rtype:  NeighList
         """
-        self._send(command="get_neighlist", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(command="get_neighlist", data=list(args))
 
     def find_pair_neighlist(self, *args):
         """Find neighbor list index of pair style neighbor list
         Try finding pair instance that matches style. If exact is set, the pair must
         match style exactly. If exact is 0, style must only be contained. If pair is
         of style pair/hybrid, style is instead matched the nsub-th hybrid sub-style.
         Once the pair instance has been identified, multiple neighbor list requests
@@ -475,54 +443,59 @@
         :param nsub:  match nsub-th hybrid sub-style, defaults to 0
         :type  nsub:  int, optional
         :param request:   index of neighbor list request, in case there are more than one, defaults to 0
         :type  request:   int, optional
         :return: neighbor list index if found, otherwise -1
         :rtype:  int
         """
-        self._send(command="find_pair_neighlist", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(
+            command="find_pair_neighlist", data=list(args)
+        )
 
     def find_fix_neighlist(self, *args):
         """Find neighbor list index of fix neighbor list
         :param fixid: name of fix
         :type  fixid: string
         :param request:   index of neighbor list request, in case there are more than one, defaults to 0
         :type  request:   int, optional
         :return: neighbor list index if found, otherwise -1
         :rtype:  int
         """
-        self._send(command="find_fix_neighlist", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(
+            command="find_fix_neighlist", data=list(args)
+        )
 
     def find_compute_neighlist(self, *args):
         """Find neighbor list index of compute neighbor list
         :param computeid: name of compute
         :type  computeid: string
         :param request:   index of neighbor list request, in case there are more than one, defaults to 0
         :type  request:   int, optional
         :return: neighbor list index if found, otherwise -1
         :rtype:  int
         """
-        self._send(command="find_compute_neighlist", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(
+            command="find_compute_neighlist", data=list(args)
+        )
 
     def get_neighlist_size(self, *args):
         """Return the number of elements in neighbor list with the given index
         :param idx: neighbor list index
         :type  idx: int
         :return: number of elements in neighbor list with index idx
         :rtype:  int
         """
-        self._send(command="get_neighlist_size", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(
+            command="get_neighlist_size", data=list(args)
+        )
 
     def get_neighlist_element_neighbors(self, *args):
-        self._send(command="get_neighlist_element_neighbors", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(
+            command="get_neighlist_element_neighbors", data=list(args)
+        )
 
     def command(self, cmd):
         """
         Send a command to the lammps object
 
         Parameters
         ----------
@@ -531,23 +504,20 @@
 
         Returns
         -------
         None
         """
         if isinstance(cmd, list):
             for c in cmd:
-                self._send(command="command", data=c)
-                _ = self._receive()
+                _ = self._send_and_receive_dict(command="command", data=c)
         elif len(cmd.split("\n")) > 1:
             for c in cmd.split("\n"):
-                self._send(command="command", data=c)
-                _ = self._receive()
+                _ = self._send_and_receive_dict(command="command", data=c)
         else:
-            self._send(command="command", data=cmd)
-            _ = self._receive()
+            _ = self._send_and_receive_dict(command="command", data=cmd)
 
     def gather_atoms(self, *args, concat=False, ids=None):
         """
         Gather atom properties
 
         Parameters
         ----------
@@ -574,42 +544,41 @@
         This method gathers information from all processors.
 
         See Also
         --------
         extract_atoms
         """
         if concat:
-            self._send(command="gather_atoms_concat", data=list(args))
+            return self._send_and_receive_dict(
+                command="gather_atoms_concat", data=list(args)
+            )
         elif ids is not None:
             lenids = len(ids)
             args = list(args)
             args.append(len(ids))
             args.append(ids)
-            self._send(command="gather_atoms_subset", data=args)
+            return self._send_and_receive_dict(command="gather_atoms_subset", data=args)
         else:
-            self._send(command="gather_atoms", data=list(args))
-        return self._receive()
+            return self._send_and_receive_dict(command="gather_atoms", data=list(args))
 
     def scatter_atoms(self, *args, ids=None):
         """
         Scatter atoms for the lammps library
 
         Args:
             *args:
         """
         if ids is not None:
             lenids = len(ids)
             args = list(args)
             args.append(len(ids))
             args.append(ids)
-            self._send(command="scatter_atoms_subset", data=args)
-            _ = self._receive()
+            _ = self._send_and_receive_dict(command="scatter_atoms_subset", data=args)
         else:
-            self._send(command="scatter_atoms", data=list(args))
-            _ = self._receive()
+            _ = self._send_and_receive_dict(command="scatter_atoms", data=list(args))
 
     def get_thermo(self, *args):
         """
         Return current value of thermo keyword
 
         Parameters
         ----------
@@ -618,16 +587,15 @@
 
         Returns
         -------
         val
             value of the thermo keyword
 
         """
-        self._send(command="get_thermo", data=list(args))
-        return self._receive()
+        return self._send_and_receive_dict(command="get_thermo", data=list(args))
 
     # TODO
     def extract_compute(self, id, style, type, length=0, width=0):
         """
         Extract compute value from the lammps library
 
         Parameters
@@ -655,34 +623,27 @@
         Returns
         -------
         val
             data computed by the fix depending on the chosen inputs
 
         """
         args = [id, style, type, length, width]
-        self._send(command="extract_compute", data=args)
-        return self._receive()
+        return self._send_and_receive_dict(command="extract_compute", data=args)
 
     def close(self):
         """
         Close the current lammps object
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
         """
-        self._send(command="close")
-        try:
-            self._process.kill()
-        except AttributeError:
-            pass
-        self._process = None
-        self._socket = None
+        self._interface.shutdown(wait=True)
 
     # TODO
     def __del__(self):
         if self._process is not None:
             self.close()
```

### Comparing `pylammpsmpi-0.1.0/pylammpsmpi.egg-info/PKG-INFO` & `pylammpsmpi-0.1.1/pylammpsmpi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.1.0/pylammpsmpi.egg-info/SOURCES.txt` & `pylammpsmpi-0.1.1/pylammpsmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.0/setup.py` & `pylammpsmpi-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,11 +22,11 @@
                  'Programming Language :: Python :: 3.10',
                  'Programming Language :: Python :: 3.11'
                 ],
 
     keywords='lammps, mpi4py',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        'mpi4py>=3.1.4', "pyzmq>=25.0.0"
+        "cloudpickle>=2.2.1", "mpi4py>=3.1.4", "pympipool>=0.4.2", "pyzmq>=25.1.0",
     ],
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pylammpsmpi-0.1.0/tests/test_pylammpsmpi_cluster.py` & `pylammpsmpi-0.1.1/tests/test_pylammpsmpi_cluster.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.0/tests/test_pylammpsmpi_local.py` & `pylammpsmpi-0.1.1/tests/test_pylammpsmpi_local.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.0/versioneer.py` & `pylammpsmpi-0.1.1/versioneer.py`

 * *Files identical despite different names*

