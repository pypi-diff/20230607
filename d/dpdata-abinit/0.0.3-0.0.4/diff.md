# Comparing `tmp/dpdata_abinit-0.0.3.tar.gz` & `tmp/dpdata_abinit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpdata_abinit-0.0.3.tar", last modified: Wed Jun  7 14:12:53 2023, max compression
+gzip compressed data, was "dpdata_abinit-0.0.4.tar", last modified: Wed Jun  7 14:57:12 2023, max compression
```

## Comparing `dpdata_abinit-0.0.3.tar` & `dpdata_abinit-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-07 14:12:53.545428 dpdata_abinit-0.0.3/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    26526 2023-02-10 09:40:53.000000 dpdata_abinit-0.0.3/LICENSE
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      857 2023-06-07 14:12:53.545428 dpdata_abinit-0.0.3/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      694 2023-05-29 10:30:29.000000 dpdata_abinit-0.0.3/README.md
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-07 14:12:53.541428 dpdata_abinit-0.0.3/dpdata_abinit/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2558 2023-06-07 14:12:10.000000 dpdata_abinit-0.0.3/dpdata_abinit/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      296 2023-05-29 10:18:48.000000 dpdata_abinit-0.0.3/dpdata_abinit/abihist.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2213 2023-06-07 14:11:35.000000 dpdata_abinit-0.0.3/dpdata_abinit/histnc.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-07 14:12:53.545428 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      857 2023-06-07 14:12:53.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      382 2023-06-07 14:12:53.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/SOURCES.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2023-06-07 14:12:53.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/dependency_links.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       55 2023-06-07 14:12:53.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/entry_points.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       23 2023-06-07 14:12:53.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/requires.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       14 2023-06-07 14:12:53.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/top_level.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2023-02-10 10:22:55.000000 dpdata_abinit-0.0.3/dpdata_abinit.egg-info/zip-safe
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      358 2023-06-07 14:12:50.000000 dpdata_abinit-0.0.3/pyproject.toml
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      159 2023-06-07 14:12:53.545428 dpdata_abinit-0.0.3/setup.cfg
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       92 2023-05-29 10:28:07.000000 dpdata_abinit-0.0.3/setup.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-07 14:57:12.431019 dpdata_abinit-0.0.4/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    26526 2023-02-10 09:40:53.000000 dpdata_abinit-0.0.4/LICENSE
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      857 2023-06-07 14:57:12.431019 dpdata_abinit-0.0.4/PKG-INFO
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      694 2023-05-29 10:30:29.000000 dpdata_abinit-0.0.4/README.md
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-07 14:57:12.431019 dpdata_abinit-0.0.4/dpdata_abinit/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2558 2023-06-07 14:54:42.000000 dpdata_abinit-0.0.4/dpdata_abinit/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      296 2023-05-29 10:18:48.000000 dpdata_abinit-0.0.4/dpdata_abinit/abihist.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2213 2023-06-07 14:11:35.000000 dpdata_abinit-0.0.4/dpdata_abinit/histnc.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-07 14:57:12.431019 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      857 2023-06-07 14:57:12.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/PKG-INFO
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      382 2023-06-07 14:57:12.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2023-06-07 14:57:12.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       55 2023-06-07 14:57:12.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/entry_points.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       23 2023-06-07 14:57:12.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/requires.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       14 2023-06-07 14:57:12.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/top_level.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2023-02-10 10:22:55.000000 dpdata_abinit-0.0.4/dpdata_abinit.egg-info/zip-safe
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      358 2023-06-07 14:54:57.000000 dpdata_abinit-0.0.4/pyproject.toml
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      159 2023-06-07 14:57:12.435019 dpdata_abinit-0.0.4/setup.cfg
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       92 2023-05-29 10:28:07.000000 dpdata_abinit-0.0.4/setup.py
```

### Comparing `dpdata_abinit-0.0.3/LICENSE` & `dpdata_abinit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdata_abinit-0.0.3/PKG-INFO` & `dpdata_abinit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdata_abinit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dpdata plugin of ABINIT hist file
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dpdata_abinit
 Abinit plugin for dpdata
```

### Comparing `dpdata_abinit-0.0.3/README.md` & `dpdata_abinit-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dpdata_abinit-0.0.3/dpdata_abinit/__init__.py` & `dpdata_abinit-0.0.4/dpdata_abinit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     # stress tensor in GPa
     system['virials'] =   hist.reader.read_cart_stress_tensors()[0]
 
     for s in structures:
         atoms=s.to_ase_atoms()
         system['cells'].append(atoms.get_cell().array)
         system['coords'].append(atoms.get_positions())
-        #system['forces'].append(atoms.arrays["cartesian_forces"])
-        system['forces'].append(atoms.arrays.cartesian_forces.flatten())
+        system['forces'].append(atoms.arrays["cartesian_forces"])
+        #system['forces'].append(atoms.arrays.cartesian_forces.flatten())
 
 
 
     system['cells'] = np.array(system['cells'])
     system['coords'] = np.array(system['coords'])
     system['energies'] = np.array(system['energies'])
     system['forces'] = np.array(system['forces'])
```

### Comparing `dpdata_abinit-0.0.3/dpdata_abinit/histnc.py` & `dpdata_abinit-0.0.4/dpdata_abinit/histnc.py`

 * *Files identical despite different names*

### Comparing `dpdata_abinit-0.0.3/dpdata_abinit.egg-info/PKG-INFO` & `dpdata_abinit-0.0.4/dpdata_abinit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdata-abinit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dpdata plugin of ABINIT hist file
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dpdata_abinit
 Abinit plugin for dpdata
```

