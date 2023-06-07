# Comparing `tmp/kartograf-0.0.6.tar.gz` & `tmp/kartograf-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kartograf-0.0.6.tar", last modified: Fri May  5 21:47:16 2023, max compression
+gzip compressed data, was "kartograf-0.5.1.tar", last modified: Wed Jun  7 21:06:30 2023, max compression
```

## Comparing `kartograf-0.0.6.tar` & `kartograf-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,45 @@
-drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/
--rw-r--r--   0 bries     (1000) bries     (1000)     1073 2023-02-03 06:44:21.000000 kartograf-0.0.6/LICENSE
--rw-r--r--   0 bries     (1000) bries     (1000)     3268 2023-05-05 21:47:16.739968 kartograf-0.0.6/PKG-INFO
--rw-r--r--   0 bries     (1000) bries     (1000)     2648 2023-05-05 20:51:44.000000 kartograf-0.0.6/README.md
--rw-r--r--   0 bries     (1000) bries     (1000)     1366 2023-05-05 16:51:56.000000 kartograf-0.0.6/pyproject.toml
--rw-r--r--   0 bries     (1000) bries     (1000)       38 2023-05-05 21:47:16.739968 kartograf-0.0.6/setup.cfg
-drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/
-drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/kartograf/
--rw-r--r--   0 bries     (1000) bries     (1000)      239 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/__init__.py
--rw-r--r--   0 bries     (1000) bries     (1000)       22 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf/_version.py
--rw-r--r--   0 bries     (1000) bries     (1000)     2348 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/atom_align.py
--rw-r--r--   0 bries     (1000) bries     (1000)    21050 2023-05-05 21:44:58.000000 kartograf-0.0.6/src/kartograf/atom_mapper.py
--rw-r--r--   0 bries     (1000) bries     (1000)    13007 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/atom_mapping_scorer.py
-drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/kartograf/tests/
--rw-r--r--   0 bries     (1000) bries     (1000)        0 2023-04-06 16:28:36.000000 kartograf-0.0.6/src/kartograf/tests/__init__.py
--rw-r--r--   0 bries     (1000) bries     (1000)     2605 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/tests/conf.py
--rw-r--r--   0 bries     (1000) bries     (1000)      652 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/tests/test_atom_align.py
--rw-r--r--   0 bries     (1000) bries     (1000)     3842 2023-04-07 22:20:12.000000 kartograf-0.0.6/src/kartograf/tests/test_atom_mapper.py
--rw-r--r--   0 bries     (1000) bries     (1000)     3105 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/tests/test_atom_mapping_scorer.py
-drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/kartograf.egg-info/
--rw-r--r--   0 bries     (1000) bries     (1000)     3268 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/PKG-INFO
--rw-r--r--   0 bries     (1000) bries     (1000)      549 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/SOURCES.txt
--rw-r--r--   0 bries     (1000) bries     (1000)        1 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/dependency_links.txt
--rw-r--r--   0 bries     (1000) bries     (1000)       23 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/requires.txt
--rw-r--r--   0 bries     (1000) bries     (1000)       10 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/top_level.txt
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.781697 kartograf-0.5.1/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1073 2023-02-02 13:06:04.000000 kartograf-0.5.1/LICENSE
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3268 2023-06-07 21:06:30.780690 kartograf-0.5.1/PKG-INFO
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2576 2023-06-05 14:08:55.000000 kartograf-0.5.1/README.md
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1316 2023-06-05 14:08:55.000000 kartograf-0.5.1/pyproject.toml
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       38 2023-06-07 21:06:30.782673 kartograf-0.5.1/setup.cfg
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.560423 kartograf-0.5.1/src/
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.619744 kartograf-0.5.1/src/kartograf/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      257 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/__init__.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3650 2023-04-28 14:06:23.000000 kartograf-0.5.1/src/kartograf/_old_dev.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       22 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf/_version.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2255 2023-04-28 14:59:10.000000 kartograf-0.5.1/src/kartograf/atom_align.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)    27089 2023-06-07 19:51:48.000000 kartograf-0.5.1/src/kartograf/atom_mapper.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)    17110 2023-06-07 20:38:42.000000 kartograf-0.5.1/src/kartograf/atom_mapping_scoring.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.673667 kartograf-0.5.1/src/kartograf/dev/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 13:51:44.000000 kartograf-0.5.1/src/kartograf/dev/__init__.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      667 2023-05-08 08:50:41.000000 kartograf-0.5.1/src/kartograf/dev/stylez.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.696674 kartograf-0.5.1/src/kartograf/dev/visualisation/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 07:56:19.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/__init__.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.719703 kartograf-0.5.1/src/kartograf/dev/visualisation/approachPics/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 08:08:32.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/approachPics/__init__.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     6339 2023-06-07 08:04:40.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/approachPics/vis_approach.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.737695 kartograf-0.5.1/src/kartograf/dev/visualisation/benzenePics/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 08:08:10.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/benzenePics/__init__.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     9309 2023-05-03 08:01:11.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/benzenePics/vis_metrics.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      571 2023-04-28 08:01:29.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/pymol_utils.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1824 2023-06-07 08:25:12.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/single.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.760656 kartograf-0.5.1/src/kartograf/filters/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      212 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/filters/__init__.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1435 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/filters/element_change.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2723 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/filters/ring_changes.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.776698 kartograf-0.5.1/src/kartograf/tests/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-13 13:43:13.000000 kartograf-0.5.1/src/kartograf/tests/__init__.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2574 2023-06-07 20:00:46.000000 kartograf-0.5.1/src/kartograf/tests/conf.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      630 2023-04-28 15:03:26.000000 kartograf-0.5.1/src/kartograf/tests/test_atom_align.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     5193 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_atom_mapper.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3008 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_atom_mapping_scorer.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1232 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_element_filters.py
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2137 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_ring_filters.py
+drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.667712 kartograf-0.5.1/src/kartograf.egg-info/
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3268 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/PKG-INFO
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1197 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/SOURCES.txt
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        1 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/dependency_links.txt
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       23 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/requires.txt
+-rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       10 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/top_level.txt
```

### Comparing `kartograf-0.0.6/LICENSE` & `kartograf-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kartograf-0.0.6/PKG-INFO` & `kartograf-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kartograf
-Version: 0.0.6
+Version: 0.5.1
 Summary: Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)
 Author-email: Benjamin Ries <benjamin-ries@outlook.com>, David Swenson <dwhswenson@gmail.com>, Irfan Alibay <irfan.alibay@gmail.com>, Mike Henry <mike.henry@choderalab.org>, Richard J Gowers <richardjgowers@gmail.com>
 Project-URL: Homepage, https://github.com/OpenFreeEnergy/kartograf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `kartograf-0.0.6/README.md` & `kartograf-0.5.1/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-
-<p align="center">
-    <img src="docs/_static/img/Kartograf_logo_boxed_dark_transp.png" id="gh-dark-mode-only"  width=35%/>
-    <!-- <img src="img/Kartograf_logo_boxed_light_transp.png" id="gh-light-mode-only"  width=20%/> -->
-</p>
-
-Kartograf: A 3D Atom Graph Mapper
-==================================
-
-[//]: # (Badges)
-[![Logo](https://img.shields.io/badge/OSMF-OpenFreeEnergy-%23002f4a)](https://openfree.energy/)
-[![build](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml/badge.svg)](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml)
-[![coverage](https://codecov.io/gh/OpenFreeEnergy/kartograf/branch/main/graph/badge.svg)](https://codecov.io/gh/OpenFreeEnergy/kartograf)
-[![Documentation Status](https://readthedocs.org/projects/kartograf/badge/?version=latest)](https://kartograf.readthedocs.io/en/latest/?badge=latest)
-
-[![Pip Install](https://img.shields.io/badge/pip%20install-kartograf-d9c4b1)](https://pypi.org/project/kartograf/)
-[![Conda Install](https://img.shields.io/badge/Conda%20install---c%20conda--forge%20kartograf-009384)](https://anaconda.org/conda-forge/kartograf)
-
-
-Kartograf offers a geometric atom mapper approach, that allows to map a given set of ligand coordinates. (can be used for hybrid topology  RBFE calculations)
-This package can be used standalone, or from the OpenFE environment.
-
-**More will be here soon!**
-
-## Usage
-```python3
-from rdkit import Chem
-from kartograf.atom_align import align_mol_shape
-from kartograf import KartografAtomMapper, SmallMoleculeComponent
-
-#Preprocessing from Smiles - Here you can add your Input!
-# Generate Data: START
-smiles = ["c1ccccc1", "c1ccccc1(CO)"]
-rdmols = [Chem.MolFromSmiles(s) for s in smiles]
-rdmols = [Chem.AddHs(m, addCoords=True) for m in rdmols]
-[Chem.rdDistGeom.EmbedMolecule(m, useRandomCoords=False, randomSeed = 0) for m in rdmols]
-# Generate Data: END
-
-# Build Small Molecule Components
-molA, molB = [SmallMoleculeComponent.from_rdkit(m) for m in rdmols]
-
-# Align the mols first - this might not needed, depends on input.
-a_molB = align_mol_shape(molB, ref_mol=molA)
-
-
-# Build Kartograf Atom Mapper
-mapper = KartografAtomMapper(atom_map_hydrogens=True)
-
-# Get Mapping
-kartograf_mapping = next(mapper.suggest_mappings(molA, a_molB))
-
-kartograf_mapping
-```
-![](docs/_static/img/alignment_benz_ol.png)
-
-## Installation
-you can install Kartograf via the package manager of your choice:
-
-```shell
-pip install kartograf
-```
-
-```shell
-conda install -c conda-forge kartograf
-```
-
-Or use Kartograf from the OpenFE Environment (soon).
-
-## References
-
-
-
+
+<p align="center">
+    <img src="docs/_static/img/Kartograf_logo_boxed_dark_transp.png" id="gh-dark-mode-only"  width=35%/>
+    <!-- <img src="img/Kartograf_logo_boxed_light_transp.png" id="gh-light-mode-only"  width=20%/> -->
+</p>
+
+Kartograf: A 3D Atom Graph Mapper
+==================================
+
+[//]: # (Badges)
+[![Logo](https://img.shields.io/badge/OSMF-OpenFreeEnergy-%23002f4a)](https://openfree.energy/)
+[![build](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml/badge.svg)](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml)
+[![coverage](https://codecov.io/gh/OpenFreeEnergy/kartograf/branch/main/graph/badge.svg)](https://codecov.io/gh/OpenFreeEnergy/kartograf)
+[![Documentation Status](https://readthedocs.org/projects/kartograf/badge/?version=latest)](https://kartograf.readthedocs.io/en/latest/?badge=latest)
+
+[![Pip Install](https://img.shields.io/badge/pip%20install-kartograf-d9c4b1)](https://pypi.org/project/kartograf/)
+[![Conda Install](https://img.shields.io/badge/Conda%20install---c%20conda--forge%20kartograf-009384)](https://anaconda.org/conda-forge/kartograf)
+
+
+Kartograf offers a geometric atom mapper approach, that allows to map a given set of ligand coordinates. (can be used for hybrid topology  RBFE calculations)
+This package can be used standalone, or from the OpenFE environment.
+
+**More will be here soon!**
+
+## Usage
+```python3
+from rdkit import Chem
+from kartograf.atom_align import align_mol_shape
+from kartograf import KartografAtomMapper, SmallMoleculeComponent
+
+#Preprocessing from Smiles - Here you can add your Input!
+# Generate Data: START
+smiles = ["c1ccccc1", "c1ccccc1(CO)"]
+rdmols = [Chem.MolFromSmiles(s) for s in smiles]
+rdmols = [Chem.AddHs(m, addCoords=True) for m in rdmols]
+[Chem.rdDistGeom.EmbedMolecule(m, useRandomCoords=False, randomSeed = 0) for m in rdmols]
+# Generate Data: END
+
+# Build Small Molecule Components
+molA, molB = [SmallMoleculeComponent.from_rdkit(m) for m in rdmols]
+
+# Align the mols first - this might not needed, depends on input.
+a_molB = align_mol_shape(molB, ref_mol=molA)
+
+
+# Build Kartograf Atom Mapper
+mapper = KartografAtomMapper(atom_map_hydrogens=True)
+
+# Get Mapping
+kartograf_mapping = next(mapper.suggest_mappings(molA, a_molB))
+
+kartograf_mapping
+```
+![](docs/_static/img/alignment_benz_ol.png)
+
+## Installation
+you can install Kartograf via the package manager of your choice:
+
+```shell
+pip install kartograf
+```
+
+```shell
+conda install -c conda-forge kartograf
+```
+
+Or use Kartograf from the OpenFE Environment (soon).
+
+## References
+
+
+
```

### Comparing `kartograf-0.0.6/pyproject.toml` & `kartograf-0.5.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-[build-system]
-requires=[
-	"setuptools>=61.0",
-	"versioningit",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "kartograf"
-dynamic = ["version"]
-authors=[
-    {name="Benjamin Ries", email="benjamin-ries@outlook.com"},
-    {name="David Swenson", email="dwhswenson@gmail.com"},
-    {name="Irfan Alibay", email="irfan.alibay@gmail.com"},
-    {name="Mike Henry", email="mike.henry@choderalab.org"},
-    {name="Richard J Gowers", email="richardjgowers@gmail.com"},
-]
-dependencies = [
-  'rdkit',
-  'scipy',
-  'numpy',
-  'gufe',
-]
-description="Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)"
-readme="README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/OpenFreeEnergy/kartograf"
-
-[tool.versioningit]
-default-version = "1+unknown"
-
-[tool.versioningit.format]
-distance = "{base_version}+{distance}.{vcs}{rev}"
-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
-distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
-
-[tool.versioningit.vcs]
-method = "git" 
-match = ["*"]
-default-tag = "0.0.0"
-
-[tool.versioningit.write]
-file = "src/kartograf/_version.py"
+[build-system]
+requires=[
+	"setuptools>=61.0",
+	"versioningit",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "kartograf"
+dynamic = ["version"]
+authors=[
+    {name="Benjamin Ries", email="benjamin-ries@outlook.com"},
+    {name="David Swenson", email="dwhswenson@gmail.com"},
+    {name="Irfan Alibay", email="irfan.alibay@gmail.com"},
+    {name="Mike Henry", email="mike.henry@choderalab.org"},
+    {name="Richard J Gowers", email="richardjgowers@gmail.com"},
+]
+dependencies = [
+  'rdkit',
+  'scipy',
+  'numpy',
+  'gufe',
+]
+description="Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)"
+readme="README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/OpenFreeEnergy/kartograf"
+
+[tool.versioningit]
+default-version = "1+unknown"
+
+[tool.versioningit.format]
+distance = "{base_version}+{distance}.{vcs}{rev}"
+dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
+distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
+
+[tool.versioningit.vcs]
+method = "git" 
+match = ["*"]
+default-tag = "0.0.0"
+
+[tool.versioningit.write]
+file = "src/kartograf/_version.py"
```

### Comparing `kartograf-0.0.6/src/kartograf/atom_align.py` & `kartograf-0.5.1/src/kartograf/atom_align.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from copy import deepcopy
-
-from rdkit import Chem
-from rdkit.Chem import AllChem
-from rdkit.Chem import rdFMCS
-from rdkit.Chem import rdMolAlign
-
-from gufe import SmallMoleculeComponent
-
-import logging
-
-log = logging.getLogger(__name__)
-
-
-def align_mol_sceletons(
-    mol: SmallMoleculeComponent,
-    ref_mol: SmallMoleculeComponent,
-) -> SmallMoleculeComponent:
-    """
-        WORK IN PROGRESS!
-        This i a Wrapper for rdkit - MCS align
-        Aligns very simply molecule to the reference molecule, based on the shared MCS.
-
-    Parameters
-    ----------
-    mol : SmallMoleculeComponent
-        molecule to be aligned to molA (will be moved)
-    ref_mol : SmallMoleculeComponent
-        molecule with the reference_positions.
-
-    Returns
-    -------
-    SmallMoleculeComponent
-        return an aligned copy of molB
-    """
-    mol = deepcopy(mol)
-
-    mol1b = ref_mol._rdkit
-    mol2b = mol._rdkit
-
-    # MCS
-    p = rdFMCS.MCSParameters()
-    p.AtomTyper = rdFMCS.AtomCompare.CompareAny
-
-    res = rdFMCS.FindMCS([mol1b, mol2b], p)
-
-    # convert match to mapping
-    q = Chem.MolFromSmarts(res.smartsString)
-    logging.debug(q)
-
-    m1_idx = mol1b.GetSubstructMatch(q)
-    m2_idx = mol2b.GetSubstructMatch(q)
-    logging.debug(m1_idx, m2_idx)
-
-    idx_mappings = list(zip(m2_idx, m1_idx))
-
-    rms = AllChem.AlignMol(
-        prbMol=mol2b,
-        refMol=mol1b,
-        atomMap=idx_mappings,
-    )
-    logging.debug(rms)
-
-    mol._rdkit = mol2b
-    return mol
-
-def align_mol_shape(mol:SmallMoleculeComponent, ref_mol:SmallMoleculeComponent)->Chem.Mol:
-    """
-        WORK IN PROGRESS!
-        This i a Wrapper for rdkit / OPEN3DAlign
-        Aligns shape based two SmallMoleculeComponents.
-
-    Parameters
-    ----------
-    mol : SmallMoleculeComponent
-        molecule to be aligned to molA (will be moved)
-    ref_mol : SmallMoleculeComponent
-        molecule with the reference_positions.
-
-    Returns
-    -------
-    SmallMoleculeComponent
-        return an aligned copy of molB
-    """
-    mol = deepcopy(mol)
-
-    mol1b = ref_mol._rdkit
-    mol2b = mol._rdkit
-    pyO3A = rdMolAlign.GetO3A(prbMol=mol2b, refMol=mol1b,)
-    score = pyO3A.Align()
-    logging.debug("alignment score: "+str(score))
-
-    mol._rdkit = mol2b
+from copy import deepcopy
+
+from rdkit import Chem
+from rdkit.Chem import AllChem
+from rdkit.Chem import rdFMCS
+from rdkit.Chem import rdMolAlign
+
+from gufe import SmallMoleculeComponent
+
+import logging
+
+log = logging.getLogger(__name__)
+
+
+def align_mol_sceletons(
+    mol: SmallMoleculeComponent,
+    ref_mol: SmallMoleculeComponent,
+) -> SmallMoleculeComponent:
+    """
+        WORK IN PROGRESS!
+        This i a Wrapper for rdkit - MCS align
+        Aligns very simply molecule to the reference molecule, based on the shared MCS.
+
+    Parameters
+    ----------
+    mol : SmallMoleculeComponent
+        molecule to be aligned to molA (will be moved)
+    ref_mol : SmallMoleculeComponent
+        molecule with the reference_positions.
+
+    Returns
+    -------
+    SmallMoleculeComponent
+        return an aligned copy of molB
+    """
+    mol = deepcopy(mol)
+
+    mol1b = ref_mol._rdkit
+    mol2b = mol._rdkit
+
+    # MCS
+    p = rdFMCS.MCSParameters()
+    p.AtomTyper = rdFMCS.AtomCompare.CompareAny
+
+    res = rdFMCS.FindMCS([mol1b, mol2b], p)
+
+    # convert match to mapping
+    q = Chem.MolFromSmarts(res.smartsString)
+    logging.debug(q)
+
+    m1_idx = mol1b.GetSubstructMatch(q)
+    m2_idx = mol2b.GetSubstructMatch(q)
+    logging.debug(m1_idx, m2_idx)
+
+    idx_mappings = list(zip(m2_idx, m1_idx))
+
+    rms = AllChem.AlignMol(
+        prbMol=mol2b,
+        refMol=mol1b,
+        atomMap=idx_mappings,
+    )
+    logging.debug(rms)
+
+    mol._rdkit = mol2b
+    return mol
+
+def align_mol_shape(mol:SmallMoleculeComponent, ref_mol:SmallMoleculeComponent)->Chem.Mol:
+    """
+        WORK IN PROGRESS!
+        This i a Wrapper for rdkit / OPEN3DAlign
+        Aligns shape based two SmallMoleculeComponents.
+
+    Parameters
+    ----------
+    mol : SmallMoleculeComponent
+        molecule to be aligned to molA (will be moved)
+    ref_mol : SmallMoleculeComponent
+        molecule with the reference_positions.
+
+    Returns
+    -------
+    SmallMoleculeComponent
+        return an aligned copy of molB
+    """
+    mol = deepcopy(mol)
+
+    mol1b = ref_mol._rdkit
+    mol2b = mol._rdkit
+    pyO3A = rdMolAlign.GetO3A(prbMol=mol2b, refMol=mol1b,)
+    score = pyO3A.Align()
+    logging.debug("alignment score: "+str(score))
+
+    mol._rdkit = mol2b
     return mol
```

### Comparing `kartograf-0.0.6/src/kartograf/tests/conf.py` & `kartograf-0.5.1/src/kartograf/tests/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,14 @@
     return naphtalene_benzene_mols()
 
 
 @pytest.fixture(scope="session")
 def naphtalene_benzene_mapping():
     mols = naphtalene_benzene_mols()
     expected_mapping = {
-        6: 11,
-        9: 6,
         10: 7,
         11: 8,
         12: 9,
         13: 10,
         0: 0,
         1: 1,
         2: 2,
```

### Comparing `kartograf-0.0.6/src/kartograf/tests/test_atom_align.py` & `kartograf-0.5.1/src/kartograf/tests/test_atom_align.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# This code is part of OpenFE and is licensed under the MIT license.
-# For details, see https://github.com/OpenFreeEnergy/kartograf
-
-import pytest
-
-from kartograf.atom_align import align_mol_sceletons, align_mol_shape
-
-from .conf import stereco_chem_molecules
-
-
-def test_stereo_align_mcs(stereco_chem_molecules):
-    """
-    Currently a smoke test
-    """
-    molA, molB = stereco_chem_molecules
-    aligned_molA = align_mol_sceletons(molA, molB)
-
-def test_stereo_align_shape(stereco_chem_molecules):
-    """
-    Currently a smoke test
-    """
-    molA, molB = stereco_chem_molecules
+# This code is part of OpenFE and is licensed under the MIT license.
+# For details, see https://github.com/OpenFreeEnergy/kartograf
+
+import pytest
+
+from kartograf.atom_align import align_mol_sceletons, align_mol_shape
+
+from .conf import stereco_chem_molecules
+
+
+def test_stereo_align_mcs(stereco_chem_molecules):
+    """
+    Currently a smoke test
+    """
+    molA, molB = stereco_chem_molecules
+    aligned_molA = align_mol_sceletons(molA, molB)
+
+def test_stereo_align_shape(stereco_chem_molecules):
+    """
+    Currently a smoke test
+    """
+    molA, molB = stereco_chem_molecules
     aligned_molA = align_mol_shape(molA, molB)
```

### Comparing `kartograf-0.0.6/src/kartograf/tests/test_atom_mapper.py` & `kartograf-0.5.1/src/kartograf/tests/test_atom_mapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .conf import (
     naphtalene_benzene_molecules,
     naphtalene_benzene_mapping,
     stereco_chem_molecules,
     stereo_chem_mapping,
 )
-
+from copy import deepcopy
 
 def check_mapping_vs_expected(mapping, expected_mapping):
     assert len(expected_mapping) == len(mapping.componentA_to_componentB)
 
     diff = []
     for exp_k, exp_v in expected_mapping.items():
         if exp_k not in mapping.componentA_to_componentB:
@@ -86,15 +86,15 @@
     Test mapping of naphtalene to benzene without H-atoms added as additional filter.
     """
     expected_mapping = {10: 7, 11: 8, 12: 9, 13: 10, 0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5}
     geom_mapper = KartografAtomMapper(
         atom_max_distance=0.95,
         atom_map_hydrogens=True,
         map_hydrogens_on_hydrogens_only=False,
-        _additional_mapping_filter_functions=[filter_atoms_h_only_h_mapped],
+        additional_mapping_filter_functions=[filter_atoms_h_only_h_mapped],
     )
 
     geom_mapping = next(
         geom_mapper.suggest_mappings(
             naphtalene_benzene_molecules[0],
             naphtalene_benzene_molecules[1],
         )
@@ -115,7 +115,50 @@
         geom_mapper.suggest_mappings(
             stereco_chem_molecules[0],
             stereco_chem_molecules[1],
         )
     )
 
     check_mapping_vs_expected(geom_mapping, expected_mapping)
+
+
+def test_to_From_dict():
+    mapper = KartografAtomMapper()
+    d1 = mapper._to_dict()
+    mapper2 = KartografAtomMapper._from_dict(d1)
+    d2 = mapper2._to_dict()
+
+    for key, val1 in d1.items():
+        val2 = d2[key]
+
+        if(val1 != val2):
+            raise ValueError("they need to be identical.")
+
+    mapper2.atom_max_distance = 10
+    d3 = mapper2._to_dict()
+    print(d3)
+    for key, val1 in d1.items():
+        val2 = d3[key]
+
+        if(val1 != val2 and key != "atom_max_distance"):
+            raise ValueError("they need to be identical.")
+        if(key == "atom_max_distance" and val1 == val2 ):
+            raise ValueError("they must not be identical.")
+
+
+def test_filter_property():
+    mapper = KartografAtomMapper(map_hydrogens_on_hydrogens_only=False)
+    first_filters = deepcopy(mapper._filter_funcs)
+
+    mapper.map_hydrogens_on_hydrogens_only = True
+    second_filters = deepcopy(mapper._filter_funcs)
+
+    mapper.map_hydrogens_on_hydrogens_only = False
+    third_filters = deepcopy(mapper._filter_funcs)
+
+    assert len(first_filters) == len(third_filters)
+    assert len(first_filters) == len(second_filters)-1
+
+    assert filter_atoms_h_only_h_mapped in second_filters
+    assert filter_atoms_h_only_h_mapped not in first_filters
+    assert filter_atoms_h_only_h_mapped not in first_filters
+
```

### Comparing `kartograf-0.0.6/src/kartograf/tests/test_atom_mapping_scorer.py` & `kartograf-0.5.1/src/kartograf/tests/test_atom_mapping_scorer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pytest
-from kartograf.atom_mapping_scorer import (
-    MappingRMSDScorer,
-    _MappingShapeDistanceScorer,
-    MappingShapeMismatchScorer,
-    MappingShapeOverlapScorer,
-    MappingVolumeRatioScorer,
-    MappingRatioMappedAtomsScorer,
-    DefaultKartografScorer
-)
-
-from .conf import stereo_chem_mapping, benzene_benzene_mapping, benzene_benzene_empty_mapping
-
-
-def test_score_mappings_rmsd(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingRMSDScorer()
-    score = scorer.get_rmsd(stereo_chem_mapping)
-    print(score)
-
-
-def test_score_norm_mapping_rmsd(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingRMSDScorer()
-    score = scorer.get_rmsd_p(stereo_chem_mapping)
-    print(score)
-
-def test_score_mapping_volume_ratio(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingVolumeRatioScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-
-def test_score_shape_dist(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = _MappingShapeDistanceScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-def test_score_shape_overlap(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingShapeOverlapScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-def test_score_shape_mismatch(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingShapeMismatchScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-
-@pytest.mark.parametrize("scorer_class", [ MappingRMSDScorer,
-    _MappingShapeDistanceScorer,
-    MappingShapeMismatchScorer,
-    MappingShapeOverlapScorer,
-    MappingVolumeRatioScorer,
-    MappingRatioMappedAtomsScorer,
-    DefaultKartografScorer])
-def test_scorer_identical_molecules(scorer_class, benzene_benzene_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = scorer_class()
-    score = scorer(benzene_benzene_mapping)
-
-    assert isinstance(score, float)
-    assert score == 0, "Score of identical Molecule should be 0"
-
-
-@pytest.mark.parametrize("scorer_class, exp", [(MappingRMSDScorer, 0),
-                                               (_MappingShapeDistanceScorer, 1),
-                                               (MappingShapeMismatchScorer,1),
-                                               (MappingShapeOverlapScorer, 1),
-                                               (MappingVolumeRatioScorer, 1),
-                                               (MappingRatioMappedAtomsScorer,1),
-                                               (DefaultKartografScorer,1)])
-def test_scorer_empty_mapping(scorer_class, exp:float, benzene_benzene_empty_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = scorer_class()
-    score = scorer(benzene_benzene_empty_mapping)
-
-    assert isinstance(score, float)
+import pytest
+from kartograf.atom_mapping_scoring import (
+    MappingRMSDScorer,
+    _MappingShapeDistanceScorer,
+    MappingShapeMismatchScorer,
+    MappingShapeOverlapScorer,
+    MappingVolumeRatioScorer,
+    MappingRatioMappedAtomsScorer,
+    DefaultKartografScorer
+)
+
+from .conf import stereo_chem_mapping, benzene_benzene_mapping, benzene_benzene_empty_mapping
+
+
+def test_score_mappings_rmsd(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingRMSDScorer()
+    score = scorer.get_rmsd(stereo_chem_mapping)
+    print(score)
+
+
+def test_score_norm_mapping_rmsd(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingRMSDScorer()
+    score = scorer.get_rmsd_p(stereo_chem_mapping)
+    print(score)
+
+def test_score_mapping_volume_ratio(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingVolumeRatioScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+
+def test_score_shape_dist(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = _MappingShapeDistanceScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+def test_score_shape_overlap(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingShapeOverlapScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+def test_score_shape_mismatch(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingShapeMismatchScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+
+@pytest.mark.parametrize("scorer_class", [ MappingRMSDScorer,
+    _MappingShapeDistanceScorer,
+    MappingShapeMismatchScorer,
+    MappingShapeOverlapScorer,
+    MappingVolumeRatioScorer,
+    MappingRatioMappedAtomsScorer,
+    DefaultKartografScorer])
+def test_scorer_identical_molecules(scorer_class, benzene_benzene_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = scorer_class()
+    score = scorer(benzene_benzene_mapping)
+
+    assert isinstance(score, float)
+    assert score == 0, "Score of identical Molecule should be 0"
+
+
+@pytest.mark.parametrize("scorer_class, exp", [(MappingRMSDScorer, 0),
+                                               (_MappingShapeDistanceScorer, 1),
+                                               (MappingShapeMismatchScorer,1),
+                                               (MappingShapeOverlapScorer, 1),
+                                               (MappingVolumeRatioScorer, 1),
+                                               (MappingRatioMappedAtomsScorer,1),
+                                               (DefaultKartografScorer,1)])
+def test_scorer_empty_mapping(scorer_class, exp:float, benzene_benzene_empty_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = scorer_class()
+    score = scorer(benzene_benzene_empty_mapping)
+
+    assert isinstance(score, float)
     assert score == exp, "Score of non-Mapping should be "+str(exp)+" for "+str(scorer_class.__name__)+" but is: "+str(score)
```

### Comparing `kartograf-0.0.6/src/kartograf.egg-info/PKG-INFO` & `kartograf-0.5.1/src/kartograf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kartograf
-Version: 0.0.6
+Version: 0.5.1
 Summary: Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)
 Author-email: Benjamin Ries <benjamin-ries@outlook.com>, David Swenson <dwhswenson@gmail.com>, Irfan Alibay <irfan.alibay@gmail.com>, Mike Henry <mike.henry@choderalab.org>, Richard J Gowers <richardjgowers@gmail.com>
 Project-URL: Homepage, https://github.com/OpenFreeEnergy/kartograf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

