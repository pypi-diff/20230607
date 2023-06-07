# Comparing `tmp/sppersist-0.1.9.tar.gz` & `tmp/sppersist-0.2.0.tar.gz`

## Comparing `sppersist-0.1.9.tar` & `sppersist-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.9/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 sppersist-0.1.9/src/spPersist/dp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.9/LICENSE
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sppersist-0.1.9/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sppersist-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/dp.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 sppersist-0.2.0/src/spPersist/ph.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.2.0/LICENSE
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 sppersist-0.2.0/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sppersist-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 sppersist-0.2.0/PKG-INFO
```

### Comparing `sppersist-0.1.9/src/spPersist/dp.py` & `sppersist-0.2.0/src/spPersist/dp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import tarfile, zipfile, os, shutil, requests
+import os, shutil, requests
+import tarfile, zipfile
 from zipfile import ZipFile
-from google.colab import auth
+
 import scanpy as sc
 import pandas as pd
 import anndata
 
 
 
-
 def Visium_FFPE_Mouse_Brain():
   '''
   Returns annotated data object of the Adult Mouse Brain (FFPE) dataset from 
   Visium, 10x Genomics.
   '''
 
   gex = 'Visium_FFPE_Mouse_Brain_filtered_feature_bc_matrix.h5'
@@ -40,24 +40,43 @@
 
   tar = tarfile.open('spatial.tar')
   posfile = tar.getmembers()[3] # 3 is the index of the coordinate file.
   tar.extract(posfile)
   return visium(gex, posfile.name)
 
 
+def Vizgen_V1_S2R1():
+  '''
+  Returns annotated data object of Slice 2 Replicate 1
+  of the MERFISH Mouse Brain Receptor Map datasets from
+  Vizgen.
+  '''
+  return Vizgen_V1(2,1)
+
+
+def Vizgen_V1_S1R3():
+  '''
+  Returns annotated data object of Slice 1 Replicate 3
+  of the MERFISH Mouse Brain Receptor Map datasets from
+  Vizgen.
+  '''
+  return Vizgen_V1(1,3)
+
+
 def Vizgen_V1(slice_num: int, replicate_num: int):
   '''
   Returns annotated data object of the dataset of 
   slice number slice_num and replicate number replicate_num  
   of the MERFISH Mouse Brain Receptor Map datasets from Vizgen.
   '''
 
   if slice_num > 3 or replicate_num >3:
     raise ValueError('Slice '+str(slice_num)+' Replicate '+str(replicate_num)+' does not exist.')
 
+  from google.colab import auth 
   auth.authenticate_user()
 
   # Paths to Data
   base_path = 'gs://public-datasets-vizgen-merfish/datasets/mouse_brain_map/BrainReceptorShowcase/'
 
   dataset_name = 'Slice' + str(slice_num) + '/Replicate' + str(replicate_num) + '/'
   dataset_suffix = '_S' + str(slice_num) + 'R' + str(replicate_num)
@@ -109,15 +128,15 @@
   if 'GSE' in id_num:
     path = 'https://ftp.ncbi.nlm.nih.gov/geo/series/GSE'+id_num[3:6]+'nnn/'+id_num+'/suppl/'
   elif 'zenodo' in id_num:
     record_id = id_num.split('.')[-1]
     r = requests.get(f"https://zenodo.org/api/records/{record_id}") 
     urls = [f['links']['self'] for f in r.json()['files']]
     path = os.path.commonprefix(urls)
-    if not os.path.isdir(path):
+    if os.path.isfile(path):
       path = os.path.dirname(path)
   else:
     raise ValueError(id_num + ' is neither GEO accession or Zenodo doi.')
 
   return path
```

### Comparing `sppersist-0.1.9/LICENSE` & `sppersist-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.9/pyproject.toml` & `sppersist-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
-description = "Spatial analysis package"
+description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

