# Comparing `tmp/deeprankcore-1.0.0.tar.gz` & `tmp/deeprankcore-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeprankcore-1.0.0.tar", last modified: Mon Oct 24 10:12:37 2022, max compression
+gzip compressed data, was "deeprankcore-2.0.0.tar", last modified: Wed Jun  7 10:46:56 2023, max compression
```

## Comparing `deeprankcore-1.0.0.tar` & `deeprankcore-2.0.0.tar`

### file list

```diff
@@ -1,111 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14274 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13415 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore/
--rw-r--r--   0 runner    (1001) docker     (121)    19143 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (121)    28392 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/Trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8942 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/alignmentNet.py
--rw-r--r--   0 runner    (1001) docker     (121)     7541 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/community_pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore/domain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore/domain/features/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/features/edgefeats.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/features/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/features/nodefeats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore/domain/forcefield/
--rw-r--r--   0 runner    (1001) docker     (121)     4428 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/forcefield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/forcefield/patch.top
--rw-r--r--   0 runner    (1001) docker     (121)    10664 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/forcefield/protein-allhdg5-4_new.param
--rw-r--r--   0 runner    (1001) docker     (121)    33428 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/forcefield/protein-allhdg5-5_new.top
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/forcefield/residue-classes
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/domain/targettypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore/feature/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/amino_acid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/atom.py
--rw-r--r--   0 runner    (1001) docker     (121)    10370 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/atomic_contact.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/biopython.py
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/bsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/pssm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/feature/sasa.py
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/foutnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     4122 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/ginet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/ginet_nocluster.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore/h5x/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/h5x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/h5x/baseimport.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      302 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/h5x/h5x.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/h5x/h5x_menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/make_uml.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/deeprankcore/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8308 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/amino_acid.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/contact.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/deeprankcore/models/forcefield/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/forcefield/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/forcefield/residue.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/forcefield/top.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/forcefield/vanderwaals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7285 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     8074 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    10947 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/pair.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/pssm.py
--rw-r--r--   0 runner    (1001) docker     (121)    20832 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     7316 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/models/variant.py
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/naive_gnn.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2230 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/sGAT.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/deeprankcore/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/BSA.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/BioWrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/CustomizeGraph.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/deeprankcore/tools/forcefield/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/forcefield/param.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/forcefield/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/forcefield/residue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/forcefield/top.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/hdf5_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)    13464 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/pdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/pssm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/pssm_3dcons_to_deeprank.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/score.py
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/tools/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.997711 deeprankcore-1.0.0/deeprankcore/uml/
--rw-r--r--   0 runner    (1001) docker     (121)   171529 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/classes_npl.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13828 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.DataSet.HDF5DataSet.svg
--rw-r--r--   0 runner    (1001) docker     (121)    58698 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.NeuralNet.NeuralNet.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8502 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.amino_acid.AminoAcid.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12802 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.contact.AtomicContact.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13372 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.contact.ResidueContact.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9638 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.graph.Edge.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11233 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.graph.Node.svg
--rw-r--r--   0 runner    (1001) docker     (121)    48009 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.grid.Grid.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5157 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.query.ProteinProteinInterfaceAtomicQuery.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.query.ProteinProteinInterfaceResidueQuery.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8796 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.structure.Chain.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.structure.Residue.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10498 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.models.variant.SingleResidueVariant.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7755 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.preprocess.PreProcessor.svg
--rw-r--r--   0 runner    (1001) docker     (121)    22668 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.preprocess._PreProcess.svg
--rw-r--r--   0 runner    (1001) docker     (121)    16346 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/deeprank_gnn.tools.BSA.BSA.svg
--rw-r--r--   0 runner    (1001) docker     (121)    81371 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/deeprankcore/uml/packages_npl.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 10:12:36.993711 deeprankcore-1.0.0/deeprankcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14274 2022-10-24 10:12:36.000000 deeprankcore-1.0.0/deeprankcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2022-10-24 10:12:36.000000 deeprankcore-1.0.0/deeprankcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 10:12:36.000000 deeprankcore-1.0.0/deeprankcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 10:11:56.000000 deeprankcore-1.0.0/deeprankcore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-24 10:12:36.000000 deeprankcore-1.0.0/deeprankcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-24 10:12:36.000000 deeprankcore-1.0.0/deeprankcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-10-24 10:12:37.001711 deeprankcore-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-24 10:05:31.000000 deeprankcore-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.112803 deeprankcore-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-06-07 10:46:56.112803 deeprankcore-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.088803 deeprankcore-2.0.0/deeprankcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45819 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.092803 deeprankcore-2.0.0/deeprankcore/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/aminoacid_summary.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/aminoacidlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/edgestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.096803 deeprankcore-2.0.0/deeprankcore/domain/forcefield/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/forcefield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/forcefield/patch.top
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/forcefield/protein-allhdg5-4_new.param
+-rw-r--r--   0 runner    (1001) docker     (123)    33428 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/forcefield/protein-allhdg5-5_new.top
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/forcefield/residue-classes
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/gridstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/losstypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/nodestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/domain/targetstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.096803 deeprankcore-2.0.0/deeprankcore/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/conservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/secondary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/features/surfacearea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.100803 deeprankcore-2.0.0/deeprankcore/molstruct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/aminoacid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/residue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/molstruct/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.100803 deeprankcore-2.0.0/deeprankcore/neuralnets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.100803 deeprankcore-2.0.0/deeprankcore/neuralnets/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/cnn/model3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.104803 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/alignmentnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/foutnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/ginet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/ginet_nocluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/naive_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/sgat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33948 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.104803 deeprankcore-2.0.0/deeprankcore/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/classdiagrams.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/plotgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.104803 deeprankcore-2.0.0/deeprankcore/tools/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/visualization/baseimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/visualization/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/visualization/h5x_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/tools/visualization/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43363 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.108803 deeprankcore-2.0.0/deeprankcore/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/buildgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/community_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.112803 deeprankcore-2.0.0/deeprankcore/utils/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/parsing/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/parsing/pssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/parsing/residue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/parsing/top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/parsing/vdwparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/deeprankcore/utils/pssmdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.088803 deeprankcore-2.0.0/deeprankcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-06-07 10:46:56.000000 deeprankcore-2.0.0/deeprankcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-07 10:46:56.000000 deeprankcore-2.0.0/deeprankcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:46:56.000000 deeprankcore-2.0.0/deeprankcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:46:24.000000 deeprankcore-2.0.0/deeprankcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-07 10:46:56.000000 deeprankcore-2.0.0/deeprankcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 10:46:56.000000 deeprankcore-2.0.0/deeprankcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-07 10:46:56.112803 deeprankcore-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:46:56.112803 deeprankcore-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    41742 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/tests/test_querycollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/tests/test_set_lossfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-07 10:42:36.000000 deeprankcore-2.0.0/tests/test_trainer.py
```

### Comparing `deeprankcore-1.0.0/LICENSE` & `deeprankcore-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deeprankcore-1.0.0/PKG-INFO` & `deeprankcore-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deeprankcore
-Version: 1.0.0
-Summary: deeprank-core allows to train graph neural networks to classify protein-protein interface with a greater flexibility for the user.
+Version: 2.0.0
+Summary: deeprankcore allows to train graph neural networks to classify protein-protein interface with a greater flexibility for the user.
 Home-page: https://github.com/DeepRank/deeprank-core
 Project-URL: Bug Tracker, https://github.com/DeepRank/deeprank-core/issues
 Keywords: graph neural network,protein-protein interface,pytorch
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -15,354 +15,323 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: publishing
 License-File: LICENSE
 
-# Deeprank-Core
+# DeeprankCore
 
 | Badges | |
 |:----:|----|
 | **fairness** |  [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6403/badge)](https://bestpractices.coreinfrastructure.org/projects/6403) |
 | **package** |  [![PyPI version](https://badge.fury.io/py/deeprankcore.svg)](https://badge.fury.io/py/deeprankcore) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f3f98b2d1883493ead50e3acaa23f2cc)](https://app.codacy.com/gh/DeepRank/deeprank-core?utm_source=github.com&utm_medium=referral&utm_content=DeepRank/deeprank-core&utm_campaign=Badge_Grade) |
 | **docs** | [![Documentation Status](https://readthedocs.org/projects/deeprankcore/badge/?version=latest)](https://deeprankcore.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/450496579.svg)](https://zenodo.org/badge/latestdoi/450496579) |
 | **tests** | [![Build Status](https://github.com/DeepRank/deeprank-core/actions/workflows/build.yml/badge.svg)](https://github.com/DeepRank/deeprank-core/actions) ![Linting status](https://github.com/DeepRank/deeprank-core/actions/workflows/linting.yml/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/DeepRank/deeprank-core/badge.svg?branch=main)](https://coveralls.io/github/DeepRank/deeprank-core?branch=main) |
-| **license** |  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  |
+| **license** |  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/license/apache-2-0/)  |
 
 
 ## Overview
 
 ![alt-text](./deeprankcore.png)
 
-Deeprank-Core is a deep learning framework for data mining Protein-Protein Interactions (PPIs) using Graph Neural Networks. 
 
-Deeprank-Core contains useful APIs for pre-processing PPIs data, computing features and targets, as well as training and testing GNN models.
+DeeprankCore is a Deep Learning (DL) framework for data mining Protein-Protein Interactions (PPIs) using either Graph Neural Networks (GNNs) or Convolutional Neural Networks (CNNs). It is an improved and unified version of the previously developed [deeprank](https://github.com/DeepRank/deeprank) and [Deeprank-GNN](https://github.com/DeepRank/Deeprank-GNN).
 
-#### Features:
+DeeprankCore contains useful APIs for pre-processing PPI data, computing features and targets, as well as training and testing GNN and CNN models.
+
+Main features:
 - Predefined atom-level and residue-level PPI feature types
   - e.g. atomic density, vdw energy, residue contacts, PSSM, etc.
 - Predefined target type
   - e.g. binary class, CAPRI categories, DockQ, RMSD, FNAT, etc.
 - Flexible definition of both new features and targets
-- Graphs feature mapping
+- Graphs and grids feature mapping
 - Efficient data storage in HDF5 format
-- Support both classification and regression (based on PyTorch and PyTorch Geometric)
+- Support both classification and regression (based on [PyTorch](https://pytorch.org/) and [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/))
 
-Deeprank-Core documentation can be found here : https://deeprankcore.rtfd.io/.
+DeeprankCore extensive documentation can be found [here](https://deeprankcore.rtfd.io/).
 
 ## Table of contents
 
-- [Deeprank-Core](#deeprank-core)
+- [DeeprankCore](#deeprankcore)
   - [Overview](#overview)
-      - [Features:](#features)
   - [Table of contents](#table-of-contents)
   - [Installation](#installation)
     - [Dependencies](#dependencies)
-    - [Deeprank-core Package](#deeprank-core-package)
+    - [Deeprank-Core Package](#deeprank-core-package)
   - [Documentation](#documentation)
-  - [Getting Started](#getting-started)
-    - [Data generation](#data-generation)
-    - [Data exploration](#data-exploration)
-    - [Dataset(s)](#datasets)
+  - [Quick start](#quick-start)
+    - [Data mapping](#data-mapping)
+    - [Datasets](#datasets)
+      - [GraphDataset](#graphdataset)
+      - [GridDataset](#griddataset)
     - [Training](#training)
-      - [Custom GNN](#custom-gnn)
   - [h5x support](#h5x-support)
-  - [For the developers](#for-the-developers)
-    - [Software release](#software-release)
+  - [Package development](#package-development)
 
 ## Installation
 
 ### Dependencies
 
-Before installing deeprank-core you need to install:
+Before installing deeprankcore you need to install:
 
  * [reduce](https://github.com/rlabduke/reduce): follow the instructions in the README of the reduce repository.
     * **How to build it without sudo privileges on a Linux machine**. After having run `make` in the reduce/ root directory, go to reduce/reduce_src/Makefile and modify `/usr/local/` to a folder in your home directory, such as `/home/user_name/apps`. Note that such a folder needs to be added to the PATH in the `.bashrc` file. Then run `make install` from reduce/. 
  * [msms](https://ssbio.readthedocs.io/en/latest/instructions/msms.html): `conda install -c bioconda msms`. *For MacOS with M1 chip users*: you can follow [these instructions](https://ssbio.readthedocs.io/en/latest/instructions/msms.html).
- * [pytorch](https://pytorch.org/): `conda install pytorch -c pytorch`. Note that by default the CPU version of pytorch will be installed, but you can also customize that installation following the instructions on pytorch website.
+ * [DSSP 4](https://swift.cmbi.umcn.nl/gv/dssp/): 
+    * on ubuntu 22.04 or newer: `sudo apt-get install dssp`
+    * on older versions of ubuntu or on mac, or lacking sudo sudo priviliges: install from [here](https://github.com/pdb-redo/dssp), following the instructions listed.
+   * CPU only: `conda install pytorch==2.0.0 torchvision==0.15.0 torchaudio==2.0.0 cpuonly -c pytorch`
+   * if using GPU: `conda install pytorch==2.0.0 torchvision==0.15.0 torchaudio==2.0.0 pytorch-cuda=11.7 -c pytorch -c nvidia`
+ * [pytorch-geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html): `conda install pyg -c pyg`
+ * [Dependencies for pytorch geometric from wheels](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#installation-from-wheels): `pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html`. 
+    - Here, `${TORCH}` and `${CUDA}` should be replaced by the pytorch and CUDA versions installed. You can find these using:
+      - `python -c "import torch; print(torch.__version__)"` and
+      - `python -c "import torch; print(torch.version.cuda)"`
+    - For example: `https://data.pyg.org/whl/torch-2.0.0+cpu.html`
+ * Only if you have a MacOS with M1 chip, additional steps are needed:
+    * `conda install pytables`
+    * See [this](https://stackoverflow.com/questions/30145751/python3-cant-find-and-import-pyqt5) solution to install PyQt5 or run `conda install pyqt`
 
-### Deeprank-core Package
+### Deeprank-Core Package
 
-Once the dependencies installed, you can install the latest release of deeprank-core using the PyPi package manager:
+Once the dependencies installed, you can install the latest release of deeprankcore using the PyPi package manager:
 
 ```
 pip install deeprankcore
 ```
 
 You can get all the new developments by cloning the repo and installing the code with
 
 ```
 git clone https://github.com/DeepRank/deeprank-core
 cd deeprank-core
 pip install -e ./
 ```
 
- * For MacOS with M1 chip users only: see [this](https://stackoverflow.com/questions/30145751/python3-cant-find-and-import-pyqt5) solution if you run into problems with PyQt5 during deeprank-core installation.
-
 ## Documentation
 
-The documentation can be found [here](https://deeprankcore.rtfd.io/).
+More extensive and detailed documentation can be found [here](https://deeprankcore.rtfd.io/).
 
-## Getting Started
+## Quick start
 
-### Data generation
+### Data mapping
 
-The process of generating graphs takes as input `.pdb` files representing protein-protein structural complexes and the correspondent Position-Specific Scoring Matrices (PSSMs) in the form of `.pssm` files. Query objects describe how the graphs should be built.
+For each protein-protein complex, a query can be created and added to the `QueryCollection` object, to be processed later on. Different types of queries exist, based on the molecular resolution needed:
+- In a `ProteinProteinInterfaceResidueQuery` each node represents one amino acid residue
+- In a `ProteinProteinInterfaceAtomicQuery` each node represents one atom within the amino acid residues.
+A query takes as inputs:
+- a `.pdb` file, representing the protein-protein structural complex
+- the ids of the two chains composing the complex, and 
+- the correspondent Position-Specific Scoring Matrices (PSSMs), in the form of `.pssm` files.
 
 ```python
-from deeprankcore.preprocess import preprocess
-from deeprankcore.models.query import ProteinProteinInterfaceResidueQuery
-from deeprankcore.feature import bsa, pssm, amino_acid, biopython
+from deeprankcore.query import QueryCollection, ProteinProteinInterfaceResidueQuery
 
-feature_modules = [bsa, pssm, biopython, atomic_contact]
-
-queries = []
+queries = QueryCollection()
 
 # Append data points
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_1w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_1w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 0
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_2w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_2w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 1
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_3w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_3w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 0
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
 
-# Generate graphs and save them in hdf5 files
-# The default creates a number of hdf5 files equals to the cpu cores available
-# See deeprankcore.preprocess.preprocess for more details
-output_paths = preprocess(feature_modules, queries, "<output_folder>/<prefix_for_outputs>")
-
 ```
 
-The user is free to implement his/her own query class. Each implementation requires the `build_graph` method to be present.
+The user is free to implement a custom query class. Each implementation requires the `build` method to be present.
 
+The queries can then be processed into 3D-graphs only or both 3D-graphs and 3D-grids, depending on which kind of network will be used later for training. 
 
-### Data exploration
+```python
+from deeprankcore.features import components, conservation, contact, exposure, irc, surfacearea
+from deeprankcore.utils.grid import GridSettings, MapMethod
 
-As representative example, the following is the hdf5 structure generated by the previous phase for `1ATN_1w.pdb`, so for one single graph:
+feature_modules = [components, conservation, contact, exposure, irc, surfacearea]
 
-```bash
-└── ppi-1ATN_1w:A-B
-    ├── edge_features
-    │   ├── _index
-    │   ├── _name
-    │   ├── covalent
-    │   ├── distance
-    │   ├── electrostatic
-    │   ├── same_chain
-    │   ├── vanderwaals
-    ├── node_features
-    │   ├── _chain_id
-    │   ├── _name
-    │   ├── _position
-    │   ├── bsa
-    │   ├── hse
-    │   ├── info_content
-    │   ├── res_depth
-    │   ├── pssm
-    └── target_values
-        └── binary
+# Save data into 3D-graphs only
+hdf5_paths = queries.process(
+    "<output_folder>/<prefix_for_outputs>",
+    feature_modules = feature_modules)
 
+# Save data into 3D-graphs and 3D-grids
+hdf5_paths = queries.process(
+    "<output_folder>/<prefix_for_outputs>",
+    feature_modules = feature_modules,
+    grid_settings = GridSettings(
+        # the number of points on the x, y, z edges of the cube
+        points_counts = [20, 20, 20],
+        # x, y, z sizes of the box in Å
+        sizes = [1.0, 1.0, 1.0]),
+    grid_map_method = MapMethod.GAUSSIAN)
 ```
 
-This graph represents the interface between two proteins contained in the `.pdb` file at the residue level. Each graph generated by deeprank-core has the above structure (apart from the features and the target that are specified by the user). 
-
-It is always a good practice to first explore the data, and then make decision about splitting them in training, test and validation sets. For this purpose, users can either use [HDF5View](https://www.hdfgroup.org/downloads/hdfview/), a visual tool written in Java for browsing and editing HDF5 files, or Python packages such as [h5py](https://docs.h5py.org/en/stable/). Few examples for the latter:
+### Datasets
 
-```python
-import h5py
-from deeprankcore.domain.features import groups
+Data can be split in sets implementing custom splits according to the specific application. Assuming that the training, validation and testing ids have been chosen (keys of the HDF5 file/s), then the `DeeprankDataset` objects can be defined.
 
-with h5py.File("<hdf5_path.hdf5>", "r") as hdf5:
+#### GraphDataset
 
-    # List of all graphs in hdf5, each graph representing a ppi
-    ids = list(hdf5.keys())
+For training GNNs the user can create a `GraphDataset` instance:
 
-    # List of all node features
-    node_features = list(hdf5[ids[0]]["node_features"]) 
-    # List of all edge features
-    edge_features = list(hdf5[ids[0]]["edge_features"])
-    # List of all edge targets
-    targets = list(hdf5[ids[0]]["target_values"])
-
-    # BSA feature for ids[0], numpy.ndarray
-    node_feat_polarity = hdf5[ids[0]]["node_features"]["bsa"][:] 
-     # Electrostatic feature for ids[0], numpy.ndarray
-    edge_feat_electrostatic = hdf5[ids[0]]["edge_features"]["electrostatic"][:]
-```
-
-### Dataset(s)
-
-Data can be split in sets implementing custom splits according to the specific application. Utility splitting functions are currently under development.
+```python
+from deeprankcore.dataset import GraphDataset
 
-Assuming that the training, validation and testing ids have been chosen (keys of the hdf5 file), then the corresponding graphs can be saved in hdf5 files containing only references (external links) to the original one. For example:
+node_features = ["bsa", "res_depth", "hse", "info_content", "pssm"]
+edge_features = ["distance"]
+target = "binary"
 
-```python
-from deeprankcore.DataSet import save_hdf5_keys
+# Creating GraphDataset objects
+dataset_train = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = train_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
+)
+dataset_val = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = valid_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
 
-save_hdf5_keys("<original_hdf5_path.hdf5>", train_ids, "<train_hdf5_path.hdf5>")
-save_hdf5_keys("<original_hdf5_path.hdf5>", valid_ids, "<val_hdf5_path.hdf5>")
-save_hdf5_keys("<original_hdf5_path.hdf5>", test_ids, "<test_hdf5_path.hdf5>")
+)
+dataset_test = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = test_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
+)
 ```
 
-Now the HDF5DataSet objects can be defined:
+#### GridDataset
+
+For training CNNs the user can create a `GridDataset` instance:
 
 ```python
-from deeprankcore.DataSet import HDF5DataSet
+from deeprankcore.dataset import GridDataset
 
-node_features = ["bsa", "res_depth", "hse", "info_content", "pssm"]
-edge_features = ["distance"]
+features = ["bsa", "res_depth", "hse", "info_content", "pssm", "distance"]
+target = "binary"
 
-# Creating HDF5DataSet objects
-dataset_train = HDF5DataSet(
-    hdf5_path = "<train_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+# Creating GraphDataset objects
+dataset_train = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = train_ids, 
+    features = features,
+    target = target
 )
-dataset_val = HDF5DataSet(
-    hdf5_path = "<val_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+dataset_val = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = valid_ids, 
+    features = features,
+    target = target
 
 )
-dataset_test = HDF5DataSet(
-    hdf5_path = "<test_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+dataset_test = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = test_ids, 
+    features = features,
+    target = target
 )
 ```
 
 ### Training
 
-Let's define a Trainer instance, using for example of the already existing GNNs, GINet:
+Let's define a `Trainer` instance, using for example of the already existing `GINet`. Because `GINet` is a GNN, it requires a dataset instance of type `GraphDataset`.
 
 ```python
-from deeprankcore.Trainer import Trainer
-from deeprankcore.ginet import GINet
-from deeprankcore.models.metrics import OutputExporter, ScatterPlotExporter
-
-metrics_output_directory = "./metrics"
-metrics_exporters = [OutputExporter(metrics_output_directory)]
+from deeprankcore.trainer import Trainer
+from deeprankcore.neuralnets.gnn.naive_gnn import NaiveNetwork
 
 trainer = Trainer(
+    NaiveNetwork,
     dataset_train,
     dataset_val,
-    dataset_test,
-    GINet,
-    batch_size = 64,
-    metrics_exporters = metrics_exporters
+    dataset_test
 )
 
 ```
 
-Optimizer (`torch.optim.Adam` by default) and loss function can be defined by using dedicated functions:
+The same can be done using a CNN, for example `CnnClassification`. Here a dataset instance of type `GridDataset` is required.
 
 ```python
-import torch
-
-trainer.configure_optimizers(torch.optim.Adamax, lr = 0.001, weight_decay = 1e-04)
+from deeprankcore.trainer import Trainer
+from deeprankcore.neuralnets.cnn.model3d import CnnClassification
 
+trainer = Trainer(
+    CnnClassification,
+    dataset_train,
+    dataset_val,
+    dataset_test
+)
 ```
 
-Then the Trainer can be trained and tested, and the model can be saved:
+By default, the `Trainer` class creates the folder `./output` for storing predictions information collected later on during training and testing. `HDF5OutputExporter` is the exporter used by default, but the user can specify any other implemented exporter or implement a custom one.
 
-```python
-trainer.train(nepoch = 50, validate = True)
-trainer.test()
-trainer.save_model(filename = "<output_model_path.pth.tar>")
+Optimizer (`torch.optim.Adam` by default) and loss function can be defined by using dedicated functions:
 
-```
+```python
+import torch
 
+trainer.configure_optimizers(torch.optim.Adamax, lr = 0.001, weight_decay = 1e-04)
 
-#### Custom GNN
+```
 
-It is also possible to define new network architectures:
+Then the `Trainer` can be trained and tested; the best model in terms of validation loss is saved by default, and the user can modify so or indicate where to save it using the `train()` method parameter `filename`.
 
 ```python
-import torch 
-
-def normalized_cut_2d(edge_index, pos):
-    row, col = edge_index
-    edge_attr = torch.norm(pos[row] - pos[col], p=2, dim=1)
-    return normalized_cut(edge_index, edge_attr, num_nodes=pos.size(0))
-
-class CustomNet(torch.nn.Module):
-    def __init__(self):
-        super(Net, self).__init__()
-        self.conv1 = SplineConv(d.num_features, 32, dim=2, kernel_size=5)
-        self.conv2 = SplineConv(32, 64, dim=2, kernel_size=5)
-        self.fc1 = torch.nn.Linear(64, 128)
-        self.fc2 = torch.nn.Linear(128, 1)
-
-    def forward(self, data):
-        data.x = F.elu(self.conv1(data.x, data.edge_index, data.edge_attr))
-        weight = normalized_cut_2d(data.edge_index, data.pos)
-        cluster = graclus(data.edge_index, weight)
-        data = max_pool(cluster, data)
-
-        data.x = F.elu(self.conv2(data.x, data.edge_index, data.edge_attr))
-        weight = normalized_cut_2d(data.edge_index, data.pos)
-        cluster = graclus(data.edge_index, weight)
-        x, batch = max_pool_x(cluster, data.x, data.batch)
-
-        x = scatter_mean(x, batch, dim=0)
-        x = F.elu(self.fc1(x))
-        x = F.dropout(x, training=self.training)
-        return F.log_softmax(self.fc2(x), dim=1)
-
-trainer = Trainer(
-    dataset_train,
-    dataset_val,
-    dataset_test,
-    CustomNet,
+trainer.train(
+    nepoch = 50,
     batch_size = 64,
-    metrics_exporters = metrics_exporters
-)
-
-trainer.train(nepoch=50)
+    validate = True,
+    filename = "<my_folder/model.pth.tar>")
+trainer.test()
 
 ```
 
 ## h5x support
 
-After installing  `h5xplorer`  (https://github.com/DeepRank/h5xplorer), you can execute the python file `deeprankcore/h5x/h5x.py` to explorer the connection graph used by deeprank-core. The context menu (right click on the name of the structure) allows to automatically plot the graphs using `plotly` as shown below.
-
-![alt-text](./h5_deeprankcore.png)
-
-## For the developers
+After installing  `h5xplorer`  (https://github.com/DeepRank/h5xplorer), you can execute the python file `deeprankcore/h5x/h5x.py` to explorer the connection graph used by deeprankcore. The context menu (right click on the name of the structure) allows to automatically plot the graphs using `plotly`.
 
-### Software release
+## Package development
 
-Before creating a new package release, make sure to have updated all version strings in the source code. An easy way to do it is to run `bump2version [part]` from command line after having installed [bump2version](https://pypi.org/project/bump2version/) on your local environment. Instead of `[part]`, type the part of the version to increase, e.g. minor. The settings in `.bumpversion.cfg` will take care of updating all the files containing version strings. 
+- Branching
+  - When creating a new branch, please use the following convention: `<issue_number>_<description>_<author_name>`.
+- Pull Requests
+  - When creating a pull request, please use the following convention: `<type>: <description>`. Example _types_ are `fix:`, `feat:`, `build:`, `chore:`, `ci:`, `docs:`, `style:`, `refactor:`, `perf:`, `test:`, and others based on the [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines).
+- Software release
+  - Before creating a new package release, make sure to have updated all version strings in the source code. An easy way to do it is to run `bump2version [part]` from command line after having installed [bump2version](https://pypi.org/project/bump2version/) on your local environment. Instead of `[part]`, type the part of the version to increase, e.g. minor. The settings in `.bumpversion.cfg` will take care of updating all the files containing version strings.
```

### Comparing `deeprankcore-1.0.0/README.md` & `deeprankcore-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,347 +1,316 @@
-# Deeprank-Core
+# DeeprankCore
 
 | Badges | |
 |:----:|----|
 | **fairness** |  [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6403/badge)](https://bestpractices.coreinfrastructure.org/projects/6403) |
 | **package** |  [![PyPI version](https://badge.fury.io/py/deeprankcore.svg)](https://badge.fury.io/py/deeprankcore) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f3f98b2d1883493ead50e3acaa23f2cc)](https://app.codacy.com/gh/DeepRank/deeprank-core?utm_source=github.com&utm_medium=referral&utm_content=DeepRank/deeprank-core&utm_campaign=Badge_Grade) |
 | **docs** | [![Documentation Status](https://readthedocs.org/projects/deeprankcore/badge/?version=latest)](https://deeprankcore.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/450496579.svg)](https://zenodo.org/badge/latestdoi/450496579) |
 | **tests** | [![Build Status](https://github.com/DeepRank/deeprank-core/actions/workflows/build.yml/badge.svg)](https://github.com/DeepRank/deeprank-core/actions) ![Linting status](https://github.com/DeepRank/deeprank-core/actions/workflows/linting.yml/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/DeepRank/deeprank-core/badge.svg?branch=main)](https://coveralls.io/github/DeepRank/deeprank-core?branch=main) |
-| **license** |  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  |
+| **license** |  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/license/apache-2-0/)  |
 
 
 ## Overview
 
 ![alt-text](./deeprankcore.png)
 
-Deeprank-Core is a deep learning framework for data mining Protein-Protein Interactions (PPIs) using Graph Neural Networks. 
 
-Deeprank-Core contains useful APIs for pre-processing PPIs data, computing features and targets, as well as training and testing GNN models.
+DeeprankCore is a Deep Learning (DL) framework for data mining Protein-Protein Interactions (PPIs) using either Graph Neural Networks (GNNs) or Convolutional Neural Networks (CNNs). It is an improved and unified version of the previously developed [deeprank](https://github.com/DeepRank/deeprank) and [Deeprank-GNN](https://github.com/DeepRank/Deeprank-GNN).
 
-#### Features:
+DeeprankCore contains useful APIs for pre-processing PPI data, computing features and targets, as well as training and testing GNN and CNN models.
+
+Main features:
 - Predefined atom-level and residue-level PPI feature types
   - e.g. atomic density, vdw energy, residue contacts, PSSM, etc.
 - Predefined target type
   - e.g. binary class, CAPRI categories, DockQ, RMSD, FNAT, etc.
 - Flexible definition of both new features and targets
-- Graphs feature mapping
+- Graphs and grids feature mapping
 - Efficient data storage in HDF5 format
-- Support both classification and regression (based on PyTorch and PyTorch Geometric)
+- Support both classification and regression (based on [PyTorch](https://pytorch.org/) and [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/))
 
-Deeprank-Core documentation can be found here : https://deeprankcore.rtfd.io/.
+DeeprankCore extensive documentation can be found [here](https://deeprankcore.rtfd.io/).
 
 ## Table of contents
 
-- [Deeprank-Core](#deeprank-core)
+- [DeeprankCore](#deeprankcore)
   - [Overview](#overview)
-      - [Features:](#features)
   - [Table of contents](#table-of-contents)
   - [Installation](#installation)
     - [Dependencies](#dependencies)
-    - [Deeprank-core Package](#deeprank-core-package)
+    - [Deeprank-Core Package](#deeprank-core-package)
   - [Documentation](#documentation)
-  - [Getting Started](#getting-started)
-    - [Data generation](#data-generation)
-    - [Data exploration](#data-exploration)
-    - [Dataset(s)](#datasets)
+  - [Quick start](#quick-start)
+    - [Data mapping](#data-mapping)
+    - [Datasets](#datasets)
+      - [GraphDataset](#graphdataset)
+      - [GridDataset](#griddataset)
     - [Training](#training)
-      - [Custom GNN](#custom-gnn)
   - [h5x support](#h5x-support)
-  - [For the developers](#for-the-developers)
-    - [Software release](#software-release)
+  - [Package development](#package-development)
 
 ## Installation
 
 ### Dependencies
 
-Before installing deeprank-core you need to install:
+Before installing deeprankcore you need to install:
 
  * [reduce](https://github.com/rlabduke/reduce): follow the instructions in the README of the reduce repository.
     * **How to build it without sudo privileges on a Linux machine**. After having run `make` in the reduce/ root directory, go to reduce/reduce_src/Makefile and modify `/usr/local/` to a folder in your home directory, such as `/home/user_name/apps`. Note that such a folder needs to be added to the PATH in the `.bashrc` file. Then run `make install` from reduce/. 
  * [msms](https://ssbio.readthedocs.io/en/latest/instructions/msms.html): `conda install -c bioconda msms`. *For MacOS with M1 chip users*: you can follow [these instructions](https://ssbio.readthedocs.io/en/latest/instructions/msms.html).
- * [pytorch](https://pytorch.org/): `conda install pytorch -c pytorch`. Note that by default the CPU version of pytorch will be installed, but you can also customize that installation following the instructions on pytorch website.
+ * [DSSP 4](https://swift.cmbi.umcn.nl/gv/dssp/): 
+    * on ubuntu 22.04 or newer: `sudo apt-get install dssp`
+    * on older versions of ubuntu or on mac, or lacking sudo sudo priviliges: install from [here](https://github.com/pdb-redo/dssp), following the instructions listed.
+   * CPU only: `conda install pytorch==2.0.0 torchvision==0.15.0 torchaudio==2.0.0 cpuonly -c pytorch`
+   * if using GPU: `conda install pytorch==2.0.0 torchvision==0.15.0 torchaudio==2.0.0 pytorch-cuda=11.7 -c pytorch -c nvidia`
+ * [pytorch-geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html): `conda install pyg -c pyg`
+ * [Dependencies for pytorch geometric from wheels](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#installation-from-wheels): `pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html`. 
+    - Here, `${TORCH}` and `${CUDA}` should be replaced by the pytorch and CUDA versions installed. You can find these using:
+      - `python -c "import torch; print(torch.__version__)"` and
+      - `python -c "import torch; print(torch.version.cuda)"`
+    - For example: `https://data.pyg.org/whl/torch-2.0.0+cpu.html`
+ * Only if you have a MacOS with M1 chip, additional steps are needed:
+    * `conda install pytables`
+    * See [this](https://stackoverflow.com/questions/30145751/python3-cant-find-and-import-pyqt5) solution to install PyQt5 or run `conda install pyqt`
 
-### Deeprank-core Package
+### Deeprank-Core Package
 
-Once the dependencies installed, you can install the latest release of deeprank-core using the PyPi package manager:
+Once the dependencies installed, you can install the latest release of deeprankcore using the PyPi package manager:
 
 ```
 pip install deeprankcore
 ```
 
 You can get all the new developments by cloning the repo and installing the code with
 
 ```
 git clone https://github.com/DeepRank/deeprank-core
 cd deeprank-core
 pip install -e ./
 ```
 
- * For MacOS with M1 chip users only: see [this](https://stackoverflow.com/questions/30145751/python3-cant-find-and-import-pyqt5) solution if you run into problems with PyQt5 during deeprank-core installation.
-
 ## Documentation
 
-The documentation can be found [here](https://deeprankcore.rtfd.io/).
+More extensive and detailed documentation can be found [here](https://deeprankcore.rtfd.io/).
 
-## Getting Started
+## Quick start
 
-### Data generation
+### Data mapping
 
-The process of generating graphs takes as input `.pdb` files representing protein-protein structural complexes and the correspondent Position-Specific Scoring Matrices (PSSMs) in the form of `.pssm` files. Query objects describe how the graphs should be built.
+For each protein-protein complex, a query can be created and added to the `QueryCollection` object, to be processed later on. Different types of queries exist, based on the molecular resolution needed:
+- In a `ProteinProteinInterfaceResidueQuery` each node represents one amino acid residue
+- In a `ProteinProteinInterfaceAtomicQuery` each node represents one atom within the amino acid residues.
+A query takes as inputs:
+- a `.pdb` file, representing the protein-protein structural complex
+- the ids of the two chains composing the complex, and 
+- the correspondent Position-Specific Scoring Matrices (PSSMs), in the form of `.pssm` files.
 
 ```python
-from deeprankcore.preprocess import preprocess
-from deeprankcore.models.query import ProteinProteinInterfaceResidueQuery
-from deeprankcore.feature import bsa, pssm, amino_acid, biopython
+from deeprankcore.query import QueryCollection, ProteinProteinInterfaceResidueQuery
 
-feature_modules = [bsa, pssm, biopython, atomic_contact]
-
-queries = []
+queries = QueryCollection()
 
 # Append data points
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_1w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_1w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 0
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_2w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_2w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 1
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_3w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_3w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 0
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
 
-# Generate graphs and save them in hdf5 files
-# The default creates a number of hdf5 files equals to the cpu cores available
-# See deeprankcore.preprocess.preprocess for more details
-output_paths = preprocess(feature_modules, queries, "<output_folder>/<prefix_for_outputs>")
-
 ```
 
-The user is free to implement his/her own query class. Each implementation requires the `build_graph` method to be present.
+The user is free to implement a custom query class. Each implementation requires the `build` method to be present.
 
+The queries can then be processed into 3D-graphs only or both 3D-graphs and 3D-grids, depending on which kind of network will be used later for training. 
 
-### Data exploration
+```python
+from deeprankcore.features import components, conservation, contact, exposure, irc, surfacearea
+from deeprankcore.utils.grid import GridSettings, MapMethod
 
-As representative example, the following is the hdf5 structure generated by the previous phase for `1ATN_1w.pdb`, so for one single graph:
+feature_modules = [components, conservation, contact, exposure, irc, surfacearea]
 
-```bash
-└── ppi-1ATN_1w:A-B
-    ├── edge_features
-    │   ├── _index
-    │   ├── _name
-    │   ├── covalent
-    │   ├── distance
-    │   ├── electrostatic
-    │   ├── same_chain
-    │   ├── vanderwaals
-    ├── node_features
-    │   ├── _chain_id
-    │   ├── _name
-    │   ├── _position
-    │   ├── bsa
-    │   ├── hse
-    │   ├── info_content
-    │   ├── res_depth
-    │   ├── pssm
-    └── target_values
-        └── binary
+# Save data into 3D-graphs only
+hdf5_paths = queries.process(
+    "<output_folder>/<prefix_for_outputs>",
+    feature_modules = feature_modules)
 
+# Save data into 3D-graphs and 3D-grids
+hdf5_paths = queries.process(
+    "<output_folder>/<prefix_for_outputs>",
+    feature_modules = feature_modules,
+    grid_settings = GridSettings(
+        # the number of points on the x, y, z edges of the cube
+        points_counts = [20, 20, 20],
+        # x, y, z sizes of the box in Å
+        sizes = [1.0, 1.0, 1.0]),
+    grid_map_method = MapMethod.GAUSSIAN)
 ```
 
-This graph represents the interface between two proteins contained in the `.pdb` file at the residue level. Each graph generated by deeprank-core has the above structure (apart from the features and the target that are specified by the user). 
-
-It is always a good practice to first explore the data, and then make decision about splitting them in training, test and validation sets. For this purpose, users can either use [HDF5View](https://www.hdfgroup.org/downloads/hdfview/), a visual tool written in Java for browsing and editing HDF5 files, or Python packages such as [h5py](https://docs.h5py.org/en/stable/). Few examples for the latter:
+### Datasets
 
-```python
-import h5py
-from deeprankcore.domain.features import groups
+Data can be split in sets implementing custom splits according to the specific application. Assuming that the training, validation and testing ids have been chosen (keys of the HDF5 file/s), then the `DeeprankDataset` objects can be defined.
 
-with h5py.File("<hdf5_path.hdf5>", "r") as hdf5:
+#### GraphDataset
 
-    # List of all graphs in hdf5, each graph representing a ppi
-    ids = list(hdf5.keys())
+For training GNNs the user can create a `GraphDataset` instance:
 
-    # List of all node features
-    node_features = list(hdf5[ids[0]]["node_features"]) 
-    # List of all edge features
-    edge_features = list(hdf5[ids[0]]["edge_features"])
-    # List of all edge targets
-    targets = list(hdf5[ids[0]]["target_values"])
-
-    # BSA feature for ids[0], numpy.ndarray
-    node_feat_polarity = hdf5[ids[0]]["node_features"]["bsa"][:] 
-     # Electrostatic feature for ids[0], numpy.ndarray
-    edge_feat_electrostatic = hdf5[ids[0]]["edge_features"]["electrostatic"][:]
-```
-
-### Dataset(s)
-
-Data can be split in sets implementing custom splits according to the specific application. Utility splitting functions are currently under development.
+```python
+from deeprankcore.dataset import GraphDataset
 
-Assuming that the training, validation and testing ids have been chosen (keys of the hdf5 file), then the corresponding graphs can be saved in hdf5 files containing only references (external links) to the original one. For example:
+node_features = ["bsa", "res_depth", "hse", "info_content", "pssm"]
+edge_features = ["distance"]
+target = "binary"
 
-```python
-from deeprankcore.DataSet import save_hdf5_keys
+# Creating GraphDataset objects
+dataset_train = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = train_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
+)
+dataset_val = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = valid_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
 
-save_hdf5_keys("<original_hdf5_path.hdf5>", train_ids, "<train_hdf5_path.hdf5>")
-save_hdf5_keys("<original_hdf5_path.hdf5>", valid_ids, "<val_hdf5_path.hdf5>")
-save_hdf5_keys("<original_hdf5_path.hdf5>", test_ids, "<test_hdf5_path.hdf5>")
+)
+dataset_test = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = test_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
+)
 ```
 
-Now the HDF5DataSet objects can be defined:
+#### GridDataset
+
+For training CNNs the user can create a `GridDataset` instance:
 
 ```python
-from deeprankcore.DataSet import HDF5DataSet
+from deeprankcore.dataset import GridDataset
 
-node_features = ["bsa", "res_depth", "hse", "info_content", "pssm"]
-edge_features = ["distance"]
+features = ["bsa", "res_depth", "hse", "info_content", "pssm", "distance"]
+target = "binary"
 
-# Creating HDF5DataSet objects
-dataset_train = HDF5DataSet(
-    hdf5_path = "<train_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+# Creating GraphDataset objects
+dataset_train = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = train_ids, 
+    features = features,
+    target = target
 )
-dataset_val = HDF5DataSet(
-    hdf5_path = "<val_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+dataset_val = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = valid_ids, 
+    features = features,
+    target = target
 
 )
-dataset_test = HDF5DataSet(
-    hdf5_path = "<test_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+dataset_test = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = test_ids, 
+    features = features,
+    target = target
 )
 ```
 
 ### Training
 
-Let's define a Trainer instance, using for example of the already existing GNNs, GINet:
+Let's define a `Trainer` instance, using for example of the already existing `GINet`. Because `GINet` is a GNN, it requires a dataset instance of type `GraphDataset`.
 
 ```python
-from deeprankcore.Trainer import Trainer
-from deeprankcore.ginet import GINet
-from deeprankcore.models.metrics import OutputExporter, ScatterPlotExporter
-
-metrics_output_directory = "./metrics"
-metrics_exporters = [OutputExporter(metrics_output_directory)]
+from deeprankcore.trainer import Trainer
+from deeprankcore.neuralnets.gnn.naive_gnn import NaiveNetwork
 
 trainer = Trainer(
+    NaiveNetwork,
     dataset_train,
     dataset_val,
-    dataset_test,
-    GINet,
-    batch_size = 64,
-    metrics_exporters = metrics_exporters
+    dataset_test
 )
 
 ```
 
-Optimizer (`torch.optim.Adam` by default) and loss function can be defined by using dedicated functions:
+The same can be done using a CNN, for example `CnnClassification`. Here a dataset instance of type `GridDataset` is required.
 
 ```python
-import torch
-
-trainer.configure_optimizers(torch.optim.Adamax, lr = 0.001, weight_decay = 1e-04)
+from deeprankcore.trainer import Trainer
+from deeprankcore.neuralnets.cnn.model3d import CnnClassification
 
+trainer = Trainer(
+    CnnClassification,
+    dataset_train,
+    dataset_val,
+    dataset_test
+)
 ```
 
-Then the Trainer can be trained and tested, and the model can be saved:
+By default, the `Trainer` class creates the folder `./output` for storing predictions information collected later on during training and testing. `HDF5OutputExporter` is the exporter used by default, but the user can specify any other implemented exporter or implement a custom one.
 
-```python
-trainer.train(nepoch = 50, validate = True)
-trainer.test()
-trainer.save_model(filename = "<output_model_path.pth.tar>")
+Optimizer (`torch.optim.Adam` by default) and loss function can be defined by using dedicated functions:
 
-```
+```python
+import torch
 
+trainer.configure_optimizers(torch.optim.Adamax, lr = 0.001, weight_decay = 1e-04)
 
-#### Custom GNN
+```
 
-It is also possible to define new network architectures:
+Then the `Trainer` can be trained and tested; the best model in terms of validation loss is saved by default, and the user can modify so or indicate where to save it using the `train()` method parameter `filename`.
 
 ```python
-import torch 
-
-def normalized_cut_2d(edge_index, pos):
-    row, col = edge_index
-    edge_attr = torch.norm(pos[row] - pos[col], p=2, dim=1)
-    return normalized_cut(edge_index, edge_attr, num_nodes=pos.size(0))
-
-class CustomNet(torch.nn.Module):
-    def __init__(self):
-        super(Net, self).__init__()
-        self.conv1 = SplineConv(d.num_features, 32, dim=2, kernel_size=5)
-        self.conv2 = SplineConv(32, 64, dim=2, kernel_size=5)
-        self.fc1 = torch.nn.Linear(64, 128)
-        self.fc2 = torch.nn.Linear(128, 1)
-
-    def forward(self, data):
-        data.x = F.elu(self.conv1(data.x, data.edge_index, data.edge_attr))
-        weight = normalized_cut_2d(data.edge_index, data.pos)
-        cluster = graclus(data.edge_index, weight)
-        data = max_pool(cluster, data)
-
-        data.x = F.elu(self.conv2(data.x, data.edge_index, data.edge_attr))
-        weight = normalized_cut_2d(data.edge_index, data.pos)
-        cluster = graclus(data.edge_index, weight)
-        x, batch = max_pool_x(cluster, data.x, data.batch)
-
-        x = scatter_mean(x, batch, dim=0)
-        x = F.elu(self.fc1(x))
-        x = F.dropout(x, training=self.training)
-        return F.log_softmax(self.fc2(x), dim=1)
-
-trainer = Trainer(
-    dataset_train,
-    dataset_val,
-    dataset_test,
-    CustomNet,
+trainer.train(
+    nepoch = 50,
     batch_size = 64,
-    metrics_exporters = metrics_exporters
-)
-
-trainer.train(nepoch=50)
+    validate = True,
+    filename = "<my_folder/model.pth.tar>")
+trainer.test()
 
 ```
 
 ## h5x support
 
-After installing  `h5xplorer`  (https://github.com/DeepRank/h5xplorer), you can execute the python file `deeprankcore/h5x/h5x.py` to explorer the connection graph used by deeprank-core. The context menu (right click on the name of the structure) allows to automatically plot the graphs using `plotly` as shown below.
-
-![alt-text](./h5_deeprankcore.png)
-
-## For the developers
+After installing  `h5xplorer`  (https://github.com/DeepRank/h5xplorer), you can execute the python file `deeprankcore/h5x/h5x.py` to explorer the connection graph used by deeprankcore. The context menu (right click on the name of the structure) allows to automatically plot the graphs using `plotly`.
 
-### Software release
+## Package development
 
-Before creating a new package release, make sure to have updated all version strings in the source code. An easy way to do it is to run `bump2version [part]` from command line after having installed [bump2version](https://pypi.org/project/bump2version/) on your local environment. Instead of `[part]`, type the part of the version to increase, e.g. minor. The settings in `.bumpversion.cfg` will take care of updating all the files containing version strings. 
+- Branching
+  - When creating a new branch, please use the following convention: `<issue_number>_<description>_<author_name>`.
+- Pull Requests
+  - When creating a pull request, please use the following convention: `<type>: <description>`. Example _types_ are `fix:`, `feat:`, `build:`, `chore:`, `ci:`, `docs:`, `style:`, `refactor:`, `perf:`, `test:`, and others based on the [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines).
+- Software release
+  - Before creating a new package release, make sure to have updated all version strings in the source code. An easy way to do it is to run `bump2version [part]` from command line after having installed [bump2version](https://pypi.org/project/bump2version/) on your local environment. Instead of `[part]`, type the part of the version to increase, e.g. minor. The settings in `.bumpversion.cfg` will take care of updating all the files containing version strings.
```

### Comparing `deeprankcore-1.0.0/deeprankcore/alignmentNet.py` & `deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/alignmentnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import torch
 from torch import nn
 
 __author__ = "Daniel-Tobias Rademaker"
 
-####################################################
-#                 Single GNN-layer                 #
-####################################################
-
-
-class GNN_layer(nn.Module):
+class GNNLayer(nn.Module):
     def __init__( # pylint: disable=too-many-arguments
         self,
         nmb_edge_projection,
         nmb_hidden_attr,
         nmb_output_features,
         message_vector_length,
         nmb_mlp_neurons,
@@ -107,17 +102,14 @@
     def output(self, hidden_features, get_attention=True):
         output = self.output_mlp(hidden_features)
         if get_attention:
             return output, self.attention_mlp(hidden_features)
         return output
 
 
-################################################################
-#                      GNN super class                         #
-################################################################
 class SuperGNN(nn.Module):
     def __init__( # pylint: disable=too-many-arguments
         self,
         nmb_edge_attr,
         nmb_node_attr,
         nmb_hidden_attr,
         nmb_mlp_neurons,
@@ -148,15 +140,15 @@
             act_fn,
             nn.Linear(nmb_mlp_neurons, nmb_hidden_attr),
             act_fn,
         )
 
         self.modlist = nn.ModuleList(
             [
-                GNN_layer(
+                GNNLayer(
                     nmb_edge_projection,
                     nmb_hidden_attr,
                     nmb_output_features,
                     message_vector_length,
                     nmb_mlp_neurons,
                     is_last_layer=(gnn_layer == (nmb_gnn_layers - 1)),
                 )
@@ -168,33 +160,28 @@
     def preprocess(self, edge_attr, node_attr):
         edge_attr = self.preproc_edge_mlp(edge_attr)
         hidden_features = self.preproc_node_mlp(node_attr)
         return edge_attr, hidden_features
 
     # Runs data through layers and return output. Potentially, attention can
     # also be returned
-    def runThroughNetwork(
+    def run_through_network(
         self, edges, edge_attr, node_attr, with_output_attention=False
     ):
         edge_attr, node_attr = self.preprocess(edge_attr, node_attr)
         for layer in self.modlist:
             node_attr = layer.update_nodes(edges, edge_attr, node_attr)
         if with_output_attention:
             representations, attention = self.modlist[-1].output(node_attr, True)
             return representations, attention
         representations = self.modlist[-1].output(node_attr, True)
         return representations
 
 
-######################
-# The alignment GNN  #
-######################
-
-
-class Alignment_GNN(SuperGNN):
+class AlignmentGNN(SuperGNN):
     def __init__( # pylint: disable=too-many-arguments
         self,
         nmb_edge_attr,
         nmb_node_attr,
         nmb_output_features,
         nmb_hidden_attr,
         message_vector_length,
@@ -213,41 +200,9 @@
             nmb_output_features,
             message_vector_length,
             act_fn,
         )
 
     # Run over all layers, and return the ouput vectors
     def forward(self, edges, edge_attr, node_attr):
-        representations = self.runThroughNetwork(edges, edge_attr, node_attr)
+        representations = self.run_through_network(edges, edge_attr, node_attr)
         return representations
-
-
-if __name__ == "__main__":
-    #####################################
-    #   Example of initializing a gnn   #
-    #####################################
-
-    ##############################
-    #         CONSTANTS          #
-    ##############################
-    MESSAGE_VECTOR_LENGTH = 32
-    NMB_HIDDED_ATTRIBUTES = 32
-    NMB_EDGE_PROJECTION = 32
-    NMB_OUPUT_FEATURES = 32
-    NMB_MLP_NEURONS = 32
-    NMB_GNN_LAYERS = 5
-    NODE_RADIUS = 15
-    ##############################
-
-    NMB_EDGE_ATTIBUTES = 4
-    NMB_NODE_ATTRIBUTES = 3 + 21
-
-    gnn = Alignment_GNN(
-        nmb_edge_attr=NMB_EDGE_ATTIBUTES,
-        nmb_node_attr=NMB_NODE_ATTRIBUTES,
-        nmb_output_features=NMB_OUPUT_FEATURES,
-        nmb_gnn_layers=NMB_GNN_LAYERS,
-        message_vector_length=MESSAGE_VECTOR_LENGTH,
-        nmb_mlp_neurons=NMB_MLP_NEURONS,
-        nmb_hidden_attr=NMB_HIDDED_ATTRIBUTES,
-        nmb_edge_projection=NMB_EDGE_PROJECTION,
-    )
```

### Comparing `deeprankcore-1.0.0/deeprankcore/community_pooling.py` & `deeprankcore-2.0.0/deeprankcore/utils/community_pooling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import warnings
 
 import community
 import markov_clustering as mc
+import matplotlib.pyplot as plt
 import networkx as nx
+import numpy as np
 import torch
-
-from torch_scatter import scatter_max, scatter_mean
-from torch_geometric.nn.pool.pool import pool_edge, pool_batch
-from torch_geometric.nn.pool.consecutive import consecutive_cluster
 from torch_geometric.data import Batch, Data
-import matplotlib.pyplot as plt
-
-
-import numpy as np
+from torch_geometric.nn.pool.consecutive import consecutive_cluster
+from torch_geometric.nn.pool.pool import pool_batch, pool_edge
+from torch_scatter import scatter_max, scatter_mean
 
 
 def plot_graph(graph, cluster):
 
     pos = nx.spring_layout(graph, iterations=200)
     nx.draw(graph, pos, node_color=cluster)
     plt.show()
@@ -27,23 +24,23 @@
     nbatch = torch.max(batch) + 1
     for ib in range(1, nbatch):
         cluster[batch == ib] += torch.max(cluster[batch == ib - 1]) + 1
     return cluster
 
 
 def community_detection_per_batch( # pylint: disable=too-many-locals
-    edge_index, batch, num_nodes, edge_attr=None, method="mcl"
+    edge_index, batch, num_nodes: int, edge_attr=None, method: str = "mcl"
 ):
-    """Detects clusters of nodes based on the edge attributes (distances)
+    """Detects clusters of nodes based on the edge attributes (distances).
 
     Args:
-        edge_index (Tensor): Edge index
-        num_nodes (int): Number of nodes
+        edge_index (Tensor): Edge index.
+        num_nodes (int): Number of nodes.
         edge_attr (Tensor, optional): Edge attributes. Defaults to None.
-        method (str, optional): method. Defaults to 'mcl'.
+        method (str, optional): Method. Defaults to "mcl".
 
     Raises:
         ValueError: Requires a valid clustering method ('mcl' or 'louvain')
 
     Returns:
         cluster Tensor
     """
@@ -58,17 +55,17 @@
         else:
             g.add_edge(i, j, weight=edge_attr[iedge])
 
     num_batch = max(batch) + 1
     all_index = range(num_nodes)
     cluster, ncluster = [], 0
 
-    for iB in range(num_batch):
+    for ib in range(num_batch):
 
-        index = torch.tensor(all_index)[batch == iB].tolist()
+        index = torch.tensor(all_index)[batch == ib].tolist()
         subg = g.subgraph(index)
 
         # detect the communities using Louvain method
         if method == "louvain":
             c = community.best_partition(subg)
             cluster += [v + ncluster for k, v in c.items()]
             ncluster = max(cluster)
@@ -89,30 +86,29 @@
         else:
             raise ValueError(f"Clustering method {method} not supported")
     # return
     device = edge_index.device
     return torch.tensor(cluster).to(device)
 
 
-def community_detection(edge_index, num_nodes, edge_attr=None, method="mcl"): # pylint: disable=too-many-locals
-    """Detects clusters of nodes based on the edge attributes (distances)
+def community_detection(edge_index, num_nodes: int, edge_attr=None, method: str = "mcl"): # pylint: disable=too-many-locals
+    """Detects clusters of nodes based on the edge attributes (distances).
 
     Args:
-        edge_index (Tensor): Edge index
-        num_nodes (int): Number of nodes
+        edge_index (Tensor): Edge index.
+        num_nodes (int): Number of nodes.
         edge_attr (Tensor, optional): Edge attributes. Defaults to None.
-        method (str, optional): method. Defaults to 'mcl'.
+        method (str, optional): Method. Defaults to "mcl".
 
     Raises:
         ValueError: Requires a valid clustering method ('mcl' or 'louvain')
 
     Returns:
         cluster Tensor
 
-
     Examples:
 
         >>> import torch
         >>> from torch_geometric.data import Data, Batch
         >>> edge_index = torch.tensor([[0, 1, 1, 2, 3, 4, 4, 5],
         >>>                            [1, 0, 2, 1, 4, 3, 5, 4]], dtype=torch.long)
         >>> x = torch.tensor([[0], [1], [2], [3], [4], [5]],
@@ -155,29 +151,29 @@
 
         return torch.tensor(index).to(device)
 
     raise ValueError(f"Clustering method {method} not supported")
 
 
 def community_pooling(cluster, data):
-    """Pools features and edges of all cluster members
+    """Pools features and edges of all cluster members.
 
     All cluster members are pooled into a single node that is assigned:
     - the max cluster value for each feature
     - the average cluster nodes position
 
     Args:
-        cluster ([type]): clusters
-        data ([type]): features tensor
+        cluster: Clusters.
+        data: Features tensor.
 
     Returns:
         pooled features tensor
 
-
-    Example:
+    Examples:
+    
         >>> import torch
         >>> from torch_geometric.data import Data, Batch
         >>> edge_index = torch.tensor([[0, 1, 1, 2, 3, 4, 4, 5],
         >>>                            [1, 0, 2, 1, 4, 3, 5, 4]], dtype=torch.long)
         >>> x = torch.tensor([[0], [1], [2], [3], [4], [5]],
         >>>                  dtype=torch.float)
         >>> data = Data(x=x, edge_index=edge_index)
@@ -186,15 +182,15 @@
         >>> batch = Batch().from_data_list([data, data])
         >>> cluster = community_detection(batch.edge_index, batch.num_nodes)
         >>> new_batch = community_pooling(cluster, batch)
     """
 
     # determine what the batches has as attributes
     has_internal_edges = hasattr(data, "internal_edge_index")
-    has_pos2D = hasattr(data, "pos2D")
+    has_pos2d = hasattr(data, "pos2d")
     has_pos = hasattr(data, "pos")
     has_cluster = hasattr(data, "cluster0")
 
     if has_internal_edges:
         warnings.warn(
             """Internal edges are not supported anymore.
             You should probably prepare the hdf5 file with
@@ -208,16 +204,16 @@
 
     # pool the edges
     edge_index, edge_attr = pool_edge(cluster, data.edge_index, data.edge_attr)
 
     # pool the pos
     if has_pos:
         pos = scatter_mean(data.pos, cluster, dim=0)
-    if has_pos2D:
-        pos2D = scatter_mean(data.pos2D, cluster, dim=0)
+    if has_pos2d:
+        pos2d = scatter_mean(data.pos2d, cluster, dim=0)
 
     if has_cluster:
         c0, c1 = data.cluster0, data.cluster1
 
     # pool batch
     if hasattr(data, "batch"):
         batch = None if data.batch is None else pool_batch(perm, data.batch)
@@ -228,15 +224,15 @@
         if has_cluster:
             data.cluster0 = c0
             data.cluster1 = c1
 
     else:
         data = Data(x=x, edge_index=edge_index, edge_attr=edge_attr, pos=pos)
 
-        if has_pos2D:
-            data.pos2D = pos2D
+        if has_pos2d:
+            data.pos2d = pos2d
 
         if has_cluster:
             data.cluster0 = c0
             data.cluster1 = c1
 
     return data
```

### Comparing `deeprankcore-1.0.0/deeprankcore/domain/forcefield/__init__.py` & `deeprankcore-2.0.0/deeprankcore/utils/parsing/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,20 @@
-import os
 import logging
-import numpy
-from deeprankcore.models.structure import Atom, Residue
-from deeprankcore.models.forcefield.patch import PatchActionType
-from deeprankcore.tools.forcefield.top import TopParser
-from deeprankcore.tools.forcefield.patch import PatchParser
-from deeprankcore.tools.forcefield.residue import ResidueClassParser
-from deeprankcore.tools.forcefield.param import ParamParser
-from deeprankcore.models.error import UnknownAtomError
-
-logging.getLogger(__name__)
-
-
-_forcefield_directory_path = os.path.dirname(os.path.abspath(__file__))
-
+import os
 
-VANDERWAALS_DISTANCE_OFF = 20.0
-VANDERWAALS_DISTANCE_ON = 1.0
+from deeprankcore.molstruct.atom import Atom
+from deeprankcore.molstruct.residue import Residue
+from deeprankcore.utils.parsing.patch import PatchActionType, PatchParser
+from deeprankcore.utils.parsing.residue import ResidueClassParser
+from deeprankcore.utils.parsing.top import TopParser
+from deeprankcore.utils.parsing.vdwparam import ParamParser, VanderwaalsParam
 
-SQUARED_VANDERWAALS_DISTANCE_OFF = numpy.square(VANDERWAALS_DISTANCE_OFF)
-SQUARED_VANDERWAALS_DISTANCE_ON = numpy.square(VANDERWAALS_DISTANCE_ON)
+_log = logging.getLogger(__name__)
 
-EPSILON0 = 1.0
-COULOMB_CONSTANT = 332.0636
-MAX_COVALENT_DISTANCE = 2.1
+_forcefield_directory_path = os.path.realpath(os.path.join(os.path.dirname(__file__), '../../domain/forcefield'))
 
 class AtomicForcefield:
     def __init__(self):
         top_path = os.path.join(
             _forcefield_directory_path,
             "protein-allhdg5-5_new.top")
         with open(top_path, 'rt', encoding = 'utf-8') as f:
@@ -54,25 +41,20 @@
                 residue.amino_acid.three_letter_code, [
                     atom.name for atom in residue.atoms]):
                 return criterium.class_name
 
         return None
 
     def get_vanderwaals_parameters(self, atom: Atom):
-        type_ = self._get_type(atom)
-
-        return self._vanderwaals_parameters[type_]
-
-    def _get_type(self, atom: Atom):
         atom_name = atom.name
 
         if atom.residue.amino_acid is None:
-            raise UnknownAtomError(f"no amino acid for {atom}")
-
-        residue_name = atom.residue.amino_acid.three_letter_code
+            _log.warning(f"no amino acid for {atom}; three letter code set to XXX")
+            residue_name = 'XXX'
+        else: residue_name = atom.residue.amino_acid.three_letter_code
 
         type_ = None
 
         # check top
         top_key = (residue_name, atom_name)
         if top_key in self._top_rows:
             type_ = self._top_rows[top_key]["type"]
@@ -82,19 +64,20 @@
         if residue_class is not None:
             for action in self._patch_actions:
                 if action.type in [PatchActionType.MODIFY, PatchActionType.ADD] and \
                         residue_class == action.selection.residue_type and "TYPE" in action:
 
                     type_ = action["TYPE"]
 
-        if type_ is None:
-            raise UnknownAtomError(
-                f"not mentioned in top or patch: {top_key}")
+        if type_ is None: # pylint: disable=no-else-return
+            _log.warning(f"Atom {atom} is unknown to the forcefield; vanderwaals_parameters set to (0.0, 0.0, 0.0, 0.0)")
+            return VanderwaalsParam(0.0, 0.0, 0.0, 0.0)
+        else:
+            return self._vanderwaals_parameters[type_]
 
-        return type_
 
     def get_charge(self, atom: Atom):
         """
             Args:
                 atom(Atom): the atom to get the charge for
             Returns(float): the charge of the given atom
         """
@@ -115,15 +98,15 @@
             for action in self._patch_actions:
                 if action.type in [
                         PatchActionType.MODIFY,
                         PatchActionType.ADD] and residue_class == action.selection.residue_type:
 
                     charge = float(action["CHARGE"])
 
-        if charge is None:
-            raise UnknownAtomError(
-                f"not mentioned in top or patch: {top_key}")
-
-        return charge
+        if charge is None: # pylint: disable=no-else-return
+            _log.warning(f"Atom {atom} is unknown to the forcefield; charge is set to 0.0")
+            return 0.0
+        else:
+            return charge
 
 
 atomic_forcefield = AtomicForcefield()
```

### Comparing `deeprankcore-1.0.0/deeprankcore/domain/forcefield/patch.top` & `deeprankcore-2.0.0/deeprankcore/domain/forcefield/patch.top`

 * *Files identical despite different names*

### Comparing `deeprankcore-1.0.0/deeprankcore/domain/forcefield/protein-allhdg5-4_new.param` & `deeprankcore-2.0.0/deeprankcore/domain/forcefield/protein-allhdg5-4_new.param`

 * *Files identical despite different names*

### Comparing `deeprankcore-1.0.0/deeprankcore/domain/forcefield/protein-allhdg5-5_new.top` & `deeprankcore-2.0.0/deeprankcore/domain/forcefield/protein-allhdg5-5_new.top`

 * *Files identical despite different names*

### Comparing `deeprankcore-1.0.0/deeprankcore/feature/amino_acid.py` & `deeprankcore-2.0.0/deeprankcore/features/components.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,64 @@
+import logging
 from typing import Optional
 
-import numpy
-from deeprankcore.models.graph import Graph
-from deeprankcore.models.variant import SingleResidueVariant
-from deeprankcore.models.structure import Atom, Residue
-from deeprankcore.domain.features import nodefeats as Nfeat
+import numpy as np
+
+from deeprankcore.domain import nodestorage as Nfeat
+from deeprankcore.molstruct.atom import Atom
+from deeprankcore.molstruct.residue import Residue
+from deeprankcore.molstruct.variant import SingleResidueVariant
+from deeprankcore.utils.graph import Graph
+from deeprankcore.utils.parsing import atomic_forcefield
+
+_log = logging.getLogger(__name__)
 
 def add_features( # pylint: disable=unused-argument
     pdb_path: str, graph: Graph,
     single_amino_acid_variant: Optional[SingleResidueVariant] = None
     ):
 
     for node in graph.nodes:
         if isinstance(node.id, Residue):
             residue = node.id
         elif isinstance(node.id, Atom):
             atom = node.id
             residue = atom.residue
+            
+            node.features[Nfeat.ATOMTYPE] = atom.element.onehot
+            node.features[Nfeat.PDBOCCUPANCY] = atom.occupancy
+            node.features[Nfeat.ATOMCHARGE] = atomic_forcefield.get_charge(atom)
         else:
             raise TypeError(f"Unexpected node type: {type(node.id)}") 
 
         node.features[Nfeat.RESTYPE] = residue.amino_acid.onehot
         node.features[Nfeat.RESCHARGE] = residue.amino_acid.charge
-        node.features[Nfeat.RESSIZE] = residue.amino_acid.size
         node.features[Nfeat.POLARITY] = residue.amino_acid.polarity.onehot
-        node.features[Nfeat.HBDONORS] = residue.amino_acid.count_hydrogen_bond_donors
-        node.features[Nfeat.HBACCEPTORS] = residue.amino_acid.count_hydrogen_bond_acceptors
+        node.features[Nfeat.RESSIZE] = residue.amino_acid.size
+        node.features[Nfeat.RESMASS] = residue.amino_acid.mass
+        node.features[Nfeat.RESPI] = residue.amino_acid.pI
+        node.features[Nfeat.HBDONORS] = residue.amino_acid.hydrogen_bond_donors
+        node.features[Nfeat.HBACCEPTORS] = residue.amino_acid.hydrogen_bond_acceptors
 
-        if single_amino_acid_variant is not None:
 
+        if single_amino_acid_variant is not None:
             wildtype = single_amino_acid_variant.wildtype_amino_acid
             variant = single_amino_acid_variant.variant_amino_acid
 
             if residue == single_amino_acid_variant.residue:
                 node.features[Nfeat.VARIANTRES] = variant.onehot
                 node.features[Nfeat.DIFFCHARGE] = variant.charge - wildtype.charge
-                node.features[Nfeat.DIFFSIZE] = variant.size - wildtype.size
                 node.features[Nfeat.DIFFPOLARITY] = variant.polarity.onehot - wildtype.polarity.onehot
-                node.features[Nfeat.DIFFHBDONORS] = variant.count_hydrogen_bond_donors - wildtype.count_hydrogen_bond_donors
-                node.features[Nfeat.DIFFHBACCEPTORS] = variant.count_hydrogen_bond_acceptors - wildtype.count_hydrogen_bond_acceptors
+                node.features[Nfeat.DIFFSIZE] = variant.size - wildtype.size
+                node.features[Nfeat.DIFFMASS] = variant.mass - wildtype.mass
+                node.features[Nfeat.DIFFPI] = variant.pI - wildtype.pI
+                node.features[Nfeat.DIFFHBDONORS] = variant.hydrogen_bond_donors - wildtype.hydrogen_bond_donors
+                node.features[Nfeat.DIFFHBACCEPTORS] = variant.hydrogen_bond_acceptors - wildtype.hydrogen_bond_acceptors
             else:
                 node.features[Nfeat.VARIANTRES] = residue.amino_acid.onehot
                 node.features[Nfeat.DIFFCHARGE] = 0
+                node.features[Nfeat.DIFFPOLARITY] = np.zeros(residue.amino_acid.polarity.onehot.shape)
                 node.features[Nfeat.DIFFSIZE] = 0
-                node.features[Nfeat.DIFFPOLARITY] = numpy.zeros(residue.amino_acid.polarity.onehot.shape)
+                node.features[Nfeat.DIFFMASS] = 0
+                node.features[Nfeat.DIFFPI] = 0
                 node.features[Nfeat.DIFFHBDONORS] = 0
-                node.features[Nfeat.DIFFHBACCEPTORS] = 0
+                node.features[Nfeat.DIFFHBACCEPTORS] = 0
```

### Comparing `deeprankcore-1.0.0/deeprankcore/feature/pssm.py` & `deeprankcore-2.0.0/deeprankcore/features/conservation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 from typing import Optional
-import numpy
-from deeprankcore.models.variant import SingleResidueVariant
-from deeprankcore.models.amino_acid import amino_acids
-from deeprankcore.models.structure import Residue, Atom
-from deeprankcore.models.graph import Graph
-from deeprankcore.domain.features import nodefeats as Nfeat
 
-profile_amino_acid_order = sorted(amino_acids, key=lambda aa: aa.one_letter_code)
+import numpy as np
+
+from deeprankcore.domain import nodestorage as Nfeat
+from deeprankcore.domain.aminoacidlist import amino_acids
+from deeprankcore.molstruct.atom import Atom
+from deeprankcore.molstruct.residue import Residue
+from deeprankcore.molstruct.variant import SingleResidueVariant
+from deeprankcore.utils.graph import Graph
 
 
 def add_features( # pylint: disable=unused-argument
     pdb_path: str, graph: Graph,
-    single_amino_acid_variant: Optional[SingleResidueVariant] = None):
+    single_amino_acid_variant: Optional[SingleResidueVariant] = None
+    ):
+
+    profile_amino_acid_order = sorted(amino_acids, key=lambda aa: aa.three_letter_code)
 
     for node in graph.nodes:
         if isinstance(node.id, Residue):
             residue = node.id
-
         elif isinstance(node.id, Atom):
             atom = node.id
             residue = atom.residue
         else:
             raise TypeError(f"Unexpected node type: {type(node.id)}")
 
         pssm_row = residue.get_pssm()
-
-        profile = numpy.array([pssm_row.get_conservation(amino_acid)
-                               for amino_acid in profile_amino_acid_order])
-
+        profile = np.array([pssm_row.get_conservation(amino_acid) for amino_acid in profile_amino_acid_order])
         node.features[Nfeat.PSSM] = profile
         node.features[Nfeat.INFOCONTENT] = pssm_row.information_content
 
-        if single_amino_acid_variant is not None:
-
+        if single_amino_acid_variant is not None:            
             if residue == single_amino_acid_variant.residue:
                 # only the variant residue can have a variant and wildtype amino acid
-
                 conservation_wildtype = pssm_row.get_conservation(single_amino_acid_variant.wildtype_amino_acid)
                 conservation_variant = pssm_row.get_conservation(single_amino_acid_variant.variant_amino_acid)
-
                 node.features[Nfeat.CONSERVATION] = conservation_wildtype
                 node.features[Nfeat.DIFFCONSERVATION] = conservation_variant - conservation_wildtype
             else:
                 # all nodes must have the same features, so set them to zero here
                 node.features[Nfeat.CONSERVATION] = 0.0
-                node.features[Nfeat.DIFFCONSERVATION] = 0.0
+                node.features[Nfeat.DIFFCONSERVATION] = 0.0
```

### Comparing `deeprankcore-1.0.0/deeprankcore/foutnet.py` & `deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/foutnet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 import torch
-from torch.nn import Parameter
 import torch.nn.functional as F
 from torch import nn
-
-from torch_scatter import scatter_mean
-
-from torch_geometric.nn.inits import uniform
+from torch.nn import Parameter
 from torch_geometric.nn import max_pool_x
+from torch_geometric.nn.inits import uniform
+from torch_scatter import scatter_mean
 
-from deeprankcore.community_pooling import get_preloaded_cluster, community_pooling
+from deeprankcore.utils.community_pooling import (community_pooling,
+                                                  get_preloaded_cluster)
 
 
 class FoutLayer(torch.nn.Module):
 
     """
     This layer is described by eq. (1) of
     Protein Interface Predition using Graph Convolutional Network
     by Alex Fout et al. NIPS 2018
 
     Args:
         in_channels (int): Size of each input sample.
         out_channels (int): Size of each output sample.
         bias (bool, optional): If set to :obj:`False`, the layer will not learn
-            an additive bias. (default: :obj:`True`)
+            an additive bias. Defaults to True.
     """
 
-    def __init__(self, in_channels, out_channels, bias=True):
+    def __init__(self, in_channels: int, out_channels: int, bias: bool = True):
 
         super().__init__()
 
         self.in_channels = in_channels
         self.out_channels = out_channels
 
         # Wc and Wn are the center and neighbor weight matrix
-        self.Wc = Parameter(torch.Tensor(in_channels, out_channels))
-        self.Wn = Parameter(torch.Tensor(in_channels, out_channels))
+        self.wc = Parameter(torch.Tensor(in_channels, out_channels))
+        self.wn = Parameter(torch.Tensor(in_channels, out_channels))
 
         if bias:
             self.bias = Parameter(torch.Tensor(out_channels))
         else:
             self.register_parameter("bias", None)
 
         self.reset_parameters()
 
     def reset_parameters(self):
         size = self.in_channels
-        uniform(size, self.Wc)
-        uniform(size, self.Wn)
+        uniform(size, self.wc)
+        uniform(size, self.wn)
         uniform(size, self.bias)
 
     def forward(self, x, edge_index):
 
         num_node = len(x)
 
         # alpha = x * Wc
-        alpha = torch.mm(x, self.Wc)
+        alpha = torch.mm(x, self.wc)
 
         # beta = x * Wn
-        beta = torch.mm(x, self.Wn)
+        beta = torch.mm(x, self.wn)
 
         # gamma_i = 1/Ni Sum_j x_j * Wn
         # there might be a better way than looping over the nodes
         gamma = torch.zeros(num_node, self.out_channels).to(alpha.device)
         for n in range(num_node):
             index = edge_index[:, edge_index[0, :] == n][1, :]
             gamma[n, :] = torch.mean(beta[index, :], dim=0)
```

### Comparing `deeprankcore-1.0.0/deeprankcore/ginet.py` & `deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/ginet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
-
-from torch_scatter import scatter_mean
-from torch_scatter import scatter_sum
-
-# torch_geometric import
-from torch_geometric.nn.inits import uniform
 from torch_geometric.nn import max_pool_x
+from torch_geometric.nn.inits import uniform
+from torch_scatter import scatter_mean, scatter_sum
 
-# deeprankcore import
-from deeprankcore.community_pooling import get_preloaded_cluster, community_pooling
+from deeprankcore.utils.community_pooling import (community_pooling,
+                                                  get_preloaded_cluster)
 
 
 class GINetConvLayer(torch.nn.Module):
     def __init__(self, in_channels, out_channels, number_edge_features=1, bias=False):
 
         super().__init__()
```

### Comparing `deeprankcore-1.0.0/deeprankcore/ginet_nocluster.py` & `deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/ginet_nocluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
-
-from torch_scatter import scatter_mean
-from torch_scatter import scatter_sum
-
-# torch_geometric import
 from torch_geometric.nn.inits import uniform
+from torch_scatter import scatter_mean, scatter_sum
 
 
 class GINetConvLayer(torch.nn.Module):
     def __init__(self, in_channels, out_channels, number_edge_features=1, bias=False):
 
         super().__init__()
```

### Comparing `deeprankcore-1.0.0/deeprankcore/h5x/h5x_menu.py` & `deeprankcore-2.0.0/deeprankcore/tools/visualization/h5x_menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-from h5xplorer.menu_tools import (
-    get_current_item,
-    get_current_hdf5_group,
-    get_group_data,
-    get_multilevel_actions,
-    send_dict_to_console)
-from h5xplorer.menu_plot import (
-    plot_histogram,
-    plot_line,
-    plot2d)
+from h5xplorer.menu_plot import plot2d, plot_histogram, plot_line
+from h5xplorer.menu_tools import (get_current_hdf5_group, get_current_item,
+                                  get_group_data, get_multilevel_actions,
+                                  send_dict_to_console)
 
 
 def context_menu(self, treeview, position): # noqa: MC0001
-    """Generate a right-click menu for the items"""
+    """Generate a right-click menu for the items."""
 
     all_item = get_current_item(self, treeview, single=False)
 
     if len(all_item) == 1:
 
         item = all_item[0]
         data = get_group_data(get_current_hdf5_group(self, item))
```

### Comparing `deeprankcore-1.0.0/deeprankcore/make_uml.sh` & `deeprankcore-2.0.0/deeprankcore/tools/classdiagrams.sh`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Notice:
 #  - Run the script in the `deeprank-core/deeprankcore`
 #  - Do keep .svg files in the same folder to view diagrams interactively
 ###############################################################################
 
 # Create output dir
-[[ ! -d uml ]] && mkdir uml
-[[ -d uml ]] && rm -f uml/*
-cd uml
+[[ ! -d class_diagrams ]] && mkdir class_diagrams
+[[ -d class_diagrams ]] && rm -f class_diagrams/*
+cd class_diagrams
 
 # Generate .puml for the project
 # output: packages_npl.pul and classes_npl.puml
 echo "Generating PlantUML .puml files..."
 pyreverse -my -o puml --ignore tests -p npl ..
 
 # Generate .puml for all classes
@@ -37,17 +37,17 @@
 done
 
 # Generate UML .svg images
 # Output: {classname}.svg, UML for each class
 printf "\nGenerating UML .svg diagrams:\n"
 for i in `awk '/^class/{print $4}' classes_npl.puml`; do
     cat $i.puml | plantuml -tsvg -pipe > $i.svg
-    echo "  uml/$i.svg"
+    echo "  class_diagrams/$i.svg"
 done
 
 # Output:
 #  packages_npl.svg, UML package diagram (modules)
 #  classes_npl.svg, UML for all classes
 plantuml -tsvg -I classes_npl.puml -I packages_npl.puml
-echo "  uml/classes_npl.svg"
-echo "  uml/packages_npl.svg"
+echo "  class_diagrams/classes_npl.svg"
+echo "  class_diagrams/packages_npl.svg"
 echo "Done"
```

### Comparing `deeprankcore-1.0.0/deeprankcore/models/grid.py` & `deeprankcore-2.0.0/deeprankcore/utils/grid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,273 +1,344 @@
-"""
-This module holds the classes that are used when working with a 3D grid.
-"""
-
+"""This module holds the classes that are used when working with a 3D grid."""
 
+import itertools
+import logging
 from enum import Enum
-from typing import Dict
-import numpy
+from typing import Dict, List, Union
+
 import h5py
-import itertools
+import numpy as np
 from scipy.signal import bspline
 
+from deeprankcore.domain import gridstorage
+
+_log = logging.getLogger(__name__)
 
 
 class MapMethod(Enum):
     """This holds the value of either one of 4 grid mapping methods.
+
     A mapping method determines how feature point values are divided over the grid points.
     """
 
     GAUSSIAN = 1
     FAST_GAUSSIAN = 2
     BSP_LINE = 3
     NEAREST_NEIGHBOURS = 4
 
 
+class Augmentation:
+    """A rotation around an axis, to be applied to a feature before mapping it to a grid."""
+
+    def __init__(self, axis: np.ndarray, angle: float):
+        self._axis = axis
+        self._angle = angle
+
+    @property
+    def axis(self) -> np.ndarray:
+        return self._axis
+
+    @property
+    def angle(self) -> float:
+        return self._angle
+
+
 class GridSettings:
     """Objects of this class hold the settings to build a grid.
+
     The grid is basically a multi-divided 3D cube with
     the following properties:
-     - points_count: the number of points on one edge of the cube
-     - size: the length in Å of one edge of the cube
-     - resolution: the size in Å of one edge subdivision. Also the distance between two points on the edge.
+    - points_counts: the number of points on the x, y, z edges of the cube
+    - sizes: x, y, z sizes of the box in Å
+    - resolutions: the size in Å of one x, y, z edge subdivision. Also the distance between two points on the edge.
     """
 
-    def __init__(self, points_count: int, size: float):
-        self._points_count = points_count
-        self._size = size
+    def __init__(
+        self,
+        points_counts: List[int],
+        sizes: List[float]
+    ):
+        assert len(points_counts) == 3
+        assert len(sizes) == 3
+
+        self._points_counts = points_counts
+        self._sizes = sizes
 
     @property
-    def resolution(self) -> float:
-        return self._size / self._points_count
+    def resolutions(self) -> List[float]:
+        return [self._sizes[i] / self._points_counts[i] for i in range(3)]
 
     @property
-    def size(self) -> float:
-        return self._size
+    def sizes(self) -> List[float]:
+        return self._sizes
 
     @property
-    def points_count(self) -> int:
-        return self._points_count
+    def points_counts(self) -> List[int]:
+        return self._points_counts
 
 
 class Grid:
-    """An instance of this class holds everything that the grid is made of:
+    """
+    An instance of this class holds everything that the grid is made of:
     - coordinates of points
     - names of features
     - feature values on each point
     """
 
-    def __init__(self, id_: str, settings: GridSettings, center: numpy.array):
+    def __init__(self, id_: str, center: List[float], settings: GridSettings):
         self.id = id_
 
+        self._center = np.array(center)
+
         self._settings = settings
-        self._center = center
 
-        self._set_mesh(settings, center)
+        self._set_mesh(self._center, settings)
 
         self._features = {}
 
-    def _set_mesh(self, settings: GridSettings, center: numpy.array):
-        "builds the grid points"
-
-        half_size = settings.size / 2
-
-        min_x = center[0] - half_size
-        max_x = center[0] + half_size
-        self._xs = numpy.linspace(min_x, max_x, num=settings.points_count)
+    def _set_mesh(self, center: np.ndarray, settings: GridSettings):
+        """Builds the grid points."""
 
-        min_y = center[1] - half_size
-        max_y = center[1] + half_size
-        self._ys = numpy.linspace(min_y, max_y, num=settings.points_count)
+        half_size_x = settings.sizes[0] / 2
+        half_size_y = settings.sizes[1] / 2
+        half_size_z = settings.sizes[2] / 2
+
+        min_x = center[0] - half_size_x
+        max_x = min_x + (settings.points_counts[0] - 1.0) * settings.resolutions[0]
+        self._xs = np.linspace(min_x, max_x, num=settings.points_counts[0])
+
+        min_y = center[1] - half_size_y
+        max_y = min_y + (settings.points_counts[1] - 1.0) * settings.resolutions[1]
+        self._ys = np.linspace(min_y, max_y, num=settings.points_counts[1])
+
+        min_z = center[2] - half_size_z
+        max_z = min_z + (settings.points_counts[2] - 1.0) * settings.resolutions[2]
+        self._zs = np.linspace(min_z, max_z, num=settings.points_counts[2])
 
-        min_z = center[2] - half_size
-        max_z = center[2] + half_size
-        self._zs = numpy.linspace(min_z, max_z, num=settings.points_count)
-
-        self._ygrid, self._xgrid, self._zgrid = numpy.meshgrid(
+        self._ygrid, self._xgrid, self._zgrid = np.meshgrid(
             self._ys, self._xs, self._zs
         )
 
     @property
-    def xs(self) -> numpy.array:
+    def center(self) -> np.ndarray:
+        return self._center
+
+    @property
+    def xs(self) -> np.array:
         return self._xs
 
     @property
-    def xgrid(self) -> numpy.array:
+    def xgrid(self) -> np.array:
         return self._xgrid
 
     @property
-    def ys(self) -> numpy.array:
+    def ys(self) -> np.array:
         return self._ys
 
     @property
-    def ygrid(self) -> numpy.array:
+    def ygrid(self) -> np.array:
         return self._ygrid
 
     @property
-    def zs(self) -> numpy.array:
+    def zs(self) -> np.array:
         return self._zs
 
     @property
-    def zgrid(self) -> numpy.array:
+    def zgrid(self) -> np.array:
         return self._zgrid
 
     @property
-    def center(self) -> numpy.array:
-        return self._center
-
-    @property
-    def features(self) -> Dict[str, numpy.array]:
+    def features(self) -> Dict[str, np.array]:
         return self._features
 
-    def add_feature_values(self, feature_name: str, data: numpy.ndarray):
+    def add_feature_values(self, feature_name: str, data: np.ndarray):
         """Makes sure feature values per grid point get stored.
 
         This method may be called repeatedly to add on to existing grid point values.
         """
 
         if feature_name not in self._features:
             self._features[feature_name] = data
         else:
             self._features[feature_name] += data
 
     def _get_mapped_feature_gaussian(
-        self, position: numpy.ndarray, value: float
-    ) -> numpy.ndarray:
+        self, position: np.ndarray, value: float
+    ) -> np.ndarray:
 
         beta = 1.0
 
         fx, fy, fz = position
-        distances = numpy.sqrt(
+        distances = np.sqrt(
             (self.xgrid - fx) ** 2 + (self.ygrid - fy) ** 2 + (self.zgrid - fz) ** 2
         )
 
-        return value * numpy.exp(-beta * distances)
+        return value * np.exp(-beta * distances)
 
     def _get_mapped_feature_fast_gaussian(
-        self, position: numpy.ndarray, value: float
-    ) -> numpy.ndarray:
+        self, position: np.ndarray, value: float
+    ) -> np.ndarray:
 
         beta = 1.0
         cutoff = 5.0 * beta
 
         fx, fy, fz = position
-        distances = numpy.sqrt(
+        distances = np.sqrt(
             (self.xgrid - fx) ** 2 + (self.ygrid - fy) ** 2 + (self.zgrid - fz) ** 2
         )
 
-        data = numpy.zeros(distances.shape)
+        data = np.zeros(distances.shape)
 
-        data[distances < cutoff] = value * numpy.exp(
+        data[distances < cutoff] = value * np.exp(
             -beta * distances[distances < cutoff]
         )
 
         return data
 
     def _get_mapped_feature_bsp_line(
-        self, position: numpy.ndarray, value: float
-    ) -> numpy.ndarray:
+        self, position: np.ndarray, value: float
+    ) -> np.ndarray:
 
         order = 4
 
         fx, fy, fz = position
         bsp_data = (
-            bspline((self.xgrid - fx) / self.resolution, order)
-            * bspline((self.ygrid - fy) / self.resolution, order)
-            * bspline((self.zgrid - fz) / self.resolution, order)
+            bspline((self.xgrid - fx) / self._settings.resolutions[0], order)
+            * bspline((self.ygrid - fy) / self._settings.resolutions[1], order)
+            * bspline((self.zgrid - fz) / self._settings.resolutions[2], order)
         )
 
         return value * bsp_data
 
     def _get_mapped_feature_nearest_neighbour( # pylint: disable=too-many-locals
-        self, position: numpy.ndarray, value: float
-    ) -> numpy.ndarray:
+        self, position: np.ndarray, value: float
+    ) -> np.ndarray:
 
         fx, _, _ = position
-        distances_x = numpy.abs(self.xs - fx)
-        distances_y = numpy.abs(self.ys - fx)
-        distances_z = numpy.abs(self.zs - fx)
-
-        indices_x = numpy.argsort(distances_x)[:2]
-        indices_y = numpy.argsort(distances_y)[:2]
-        indices_z = numpy.argsort(distances_z)[:2]
+        distances_x = np.abs(self.xs - fx)
+        distances_y = np.abs(self.ys - fx)
+        distances_z = np.abs(self.zs - fx)
+
+        indices_x = np.argsort(distances_x)[:2]
+        indices_y = np.argsort(distances_y)[:2]
+        indices_z = np.argsort(distances_z)[:2]
 
         sorted_x = distances_x[indices_x]
-        weights_x = sorted_x / numpy.sum(sorted_x)
+        weights_x = sorted_x / np.sum(sorted_x)
 
         sorted_y = distances_y[indices_y]
-        weights_y = sorted_y / numpy.sum(sorted_y)
+        weights_y = sorted_y / np.sum(sorted_y)
 
         sorted_z = distances_z[indices_z]
-        weights_z = sorted_z / numpy.sum(sorted_z)
+        weights_z = sorted_z / np.sum(sorted_z)
 
         indices = [indices_x, indices_y, indices_z]
         points = list(itertools.product(*indices))
 
         weight_products = list(itertools.product(weights_x, weights_y, weights_z))
-        weights = [numpy.sum(p) for p in weight_products]
+        weights = [np.sum(p) for p in weight_products]
 
-        neighbour_data = numpy.zeros(
+        neighbour_data = np.zeros(
             (self.xs.shape[0], self.ys.shape[0], self.zs.shape[0])
         )
 
         for point_index, point in enumerate(points):
             weight = weights[point_index]
 
             neighbour_data[point] = weight * value
 
         return neighbour_data
 
+    def _get_atomic_density_koes(self, position: np.ndarray, vanderwaals_radius: float) -> np.ndarray:
+        """Function to map individual atomic density on the grid.
+
+        The formula is equation (1) of the Koes paper
+        Protein-Ligand Scoring with Convolutional NN Arxiv:1612.02751v1.
+
+        Returns:
+            np.ndarray: The mapped density.
+        """
+
+        distances = np.sqrt(np.square(self.xgrid - position[0]) +
+                            np.square(self.ygrid - position[1]) +
+                            np.square(self.zgrid - position[2]))
+
+        density_data = np.zeros(distances.shape)
+
+        indices_close = distances < vanderwaals_radius
+        indices_far = (distances >= vanderwaals_radius) & (distances < 1.5 * vanderwaals_radius)
+
+        density_data[indices_close] = np.exp(-2.0 * np.square(distances[indices_close]) /  np.square(vanderwaals_radius))
+        density_data[indices_far] = 4.0 / np.square(np.e) / np.square(vanderwaals_radius) * np.square(distances[indices_far]) - \
+                                    12.0 / np.square(np.e) / vanderwaals_radius * distances[indices_far] + \
+                                    9.0 / np.square(np.e)
+
+        return density_data
+
     def map_feature(
         self,
-        position: numpy.ndarray,
+        position: np.ndarray,
         feature_name: str,
-        feature_value: numpy.ndarray,
+        feature_value: Union[np.ndarray, float],
         method: MapMethod,
     ):
-        "Maps point feature data at a given position to the grid, using the given method."
+        """Maps point feature data at a given position to the grid, using the given method.
+        
+        The feature_value should either be a single number or a one-dimensional array.
+        """
+
+        # determine whether we're dealing with a single number of multiple numbers:
+        index_names_values = []
+        if isinstance(feature_value, float):
+            index_names_values = [(feature_name, feature_value)]
 
-        for index, value in enumerate(feature_value):
+        elif isinstance(feature_value, int):
+            index_names_values = [(feature_name, float(feature_value))]
+
+        else:
+            for index, value in enumerate(feature_value):
+                index_name = f"{feature_name}_{index:03d}"
+                index_names_values.append((index_name, value))
 
-            index_name = f"{feature_name}_{index:03d}"
+        # map the data to the grid
+        for index_name, value in index_names_values:
 
             if method == MapMethod.GAUSSIAN:
                 grid_data = self._get_mapped_feature_gaussian(position, value)
 
             elif method == MapMethod.FAST_GAUSSIAN:
                 grid_data = self._get_mapped_feature_fast_gaussian(position, value)
 
-            # elif method == MapMethod.BSP_LINE:
-            #     grid_data = self._get_mapped_feature_bsp_line(position, value)
+            elif method == MapMethod.BSP_LINE:
+                grid_data = self._get_mapped_feature_bsp_line(position, value)
 
-            elif method == MapMethod.NEAREST_NEIGHBOUR:
+            elif method == MapMethod.NEAREST_NEIGHBOURS:
                 grid_data = self._get_mapped_feature_nearest_neighbour(position, value)
 
             # set to grid
             self.add_feature_values(index_name, grid_data)
 
     def to_hdf5(self, hdf5_path: str):
-        "Write the grid data to hdf5, according to deeprank standards."
+        """Write the grid data to hdf5, according to deeprank standards."""
 
         with h5py.File(hdf5_path, "a") as hdf5_file:
 
             # create a group to hold everything
             grid_group = hdf5_file.require_group(self.id)
 
             # store grid points
-            points_group = grid_group.create_group("grid_points")
+            points_group = grid_group.require_group("grid_points")
             points_group.create_dataset("x", data=self.xs)
             points_group.create_dataset("y", data=self.ys)
             points_group.create_dataset("z", data=self.zs)
             points_group.create_dataset("center", data=self.center)
 
             # store grid features
-            features_group = grid_group.require_group("mapped_features")
+            features_group = grid_group.require_group(gridstorage.MAPPED_FEATURES)
             for feature_name, feature_data in self.features.items():
 
-                feature_group = features_group.require_group(feature_name)
-                feature_group.create_dataset(
-                    "value",
+                features_group.create_dataset(
+                    feature_name,
                     data=feature_data,
                     compression="lzf",
                     chunks=True,
                 )
```

### Comparing `deeprankcore-1.0.0/deeprankcore/models/metrics.py` & `deeprankcore-2.0.0/deeprankcore/utils/exporters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,108 @@
-import lzma
-import os
-import csv
-from typing import List, Tuple, Any, Dict, Optional
-from math import sqrt
 import logging
+import os
 import random
+from math import sqrt
+from typing import Any, Dict, List, Optional, Tuple
+
+import pandas as pd
 from matplotlib import pyplot
+from sklearn.metrics import roc_auc_score
 from torch import argmax, tensor
 from torch.nn.functional import cross_entropy
 from torch.utils.tensorboard import SummaryWriter
-from sklearn.metrics import roc_auc_score
-import pandas as pd
 
 _log = logging.getLogger(__name__)
 
 
-class MetricsExporter:
-    "The class implements an object, to be called when a neural network generates output"
+class OutputExporter:
+    """The class implements a general exporter to be called when a neural network generates outputs."""
+
+    def __init__(self, directory_path: str = None):
+        
+        if directory_path is None:
+            directory_path = "./output"
+        self._directory_path = directory_path
+
+        if not os.path.exists(self._directory_path):
+            os.makedirs(self._directory_path)
 
     def __enter__(self):
         "overridable"
         return self
 
     def __exit__(self, exception_type, exception, traceback):
         "overridable"
         pass # pylint: disable=unnecessary-pass
 
     def process(self, pass_name: str, epoch_number: int, # pylint: disable=too-many-arguments
-                entry_names: List[str], output_values: List[Any], target_values: List[Any]):
+                entry_names: List[str], output_values: List[Any], target_values: List[Any], loss: float):
         "the entry_names, output_values, target_values MUST have the same length"
         pass # pylint: disable=unnecessary-pass
 
-    def is_compatible_with(self, output_data_shape: int, target_data_shape: Optional[int]) -> bool:  # pylint: disable=unused-argument
+    def is_compatible_with( # pylint: disable=unused-argument
+        self,
+        output_data_shape: int,
+        target_data_shape: Optional[int] = None) -> bool:
         "true if this exporter can work with the given data shapes"
-
         return True
 
 
-class MetricsExporterCollection:
-    "allows a series of metrics exporters to be used at the same time"
+class OutputExporterCollection:
+    """It allows a series of output exporters to be used at the same time."""
 
-    def __init__(self, *args: Tuple[MetricsExporter]):
-        self._metrics_exporters = args
+    def __init__(self, *args: List[OutputExporter]):
+        self._output_exporters = args
 
     def __enter__(self):
-        for metrics_exporter in self._metrics_exporters:
-            metrics_exporter.__enter__()
+        for output_exporter in self._output_exporters:
+            output_exporter.__enter__()
 
         return self
 
     def __exit__(self, exception_type, exception, traceback):
-        for metrics_exporter in self._metrics_exporters:
-            metrics_exporter.__exit__(exception_type, exception, traceback)
+        for output_exporter in self._output_exporters:
+            output_exporter.__exit__(exception_type, exception, traceback)
 
     def process(self, pass_name: str, epoch_number: int, # pylint: disable=too-many-arguments
-                entry_names: List[str], output_values: List[Any], target_values: List[Any]):
-        for metrics_exporter in self._metrics_exporters:
-            metrics_exporter.process(pass_name, epoch_number, entry_names, output_values, target_values)
+                entry_names: List[str], output_values: List[Any], target_values: List[Any], loss: float):
+        for output_exporter in self._output_exporters:
+            output_exporter.process(pass_name, epoch_number, entry_names, output_values, target_values, loss)
 
     def __iter__(self):
-        return iter(self._metrics_exporters)
-
+        return iter(self._output_exporters)
 
-class TensorboardBinaryClassificationExporter(MetricsExporter):
-    """ Exports to tensorboard, works for binary classification only.
 
-        Currently outputs to tensorboard:
-         - Mathews Correlation Coefficient (MCC)
-         - Accuracy
-         - ROC area under the curve
+class TensorboardBinaryClassificationExporter(OutputExporter):
+    """Exporter for tensorboard, works for binary classification only.
 
-        Outputs are done per epoch.
+    Currently outputs to tensorboard:
+    - Mathews Correlation Coefficient (MCC)
+    - Accuracy
+    - ROC area under the curve
+    Outputs are computed for each epoch.
     """
 
     def __init__(self, directory_path: str):
-        self._directory_path = directory_path
+        super().__init__(directory_path)
         self._writer = SummaryWriter(log_dir=directory_path)
 
     def __enter__(self):
         self._writer.__enter__()
         return self
 
     def __exit__(self, exception_type, exception, traceback):
         self._writer.__exit__(exception_type, exception, traceback)
 
     def process(self, pass_name: str, epoch_number: int, # pylint: disable=too-many-arguments, too-many-locals
-                entry_names: List[str], output_values: List[Any], target_values: List[Any]):
+                entry_names: List[str], output_values: List[Any], target_values: List[Any], loss: float):
         "write to tensorboard"
 
-        loss = cross_entropy(tensor(output_values), tensor(target_values)).item()
-        self._writer.add_scalar(f"{pass_name} cross entropy loss", loss, epoch_number)
+        ce_loss = cross_entropy(tensor(output_values), tensor(target_values)).item()
+        self._writer.add_scalar(f"{pass_name} cross entropy loss", ce_loss, epoch_number)
 
         probabilities = []
         fp, fn, tp, tn = 0, 0, 0, 0
         for entry_index, _ in enumerate(entry_names):
             probability = output_values[entry_index][1]
             probabilities.append(probability)
 
@@ -126,83 +135,45 @@
         self._writer.add_scalar(f"{pass_name} accuracy", accuracy, epoch_number)
 
         # for ROC curves to work, we need both class values in the set
         if len(set(target_values)) == 2:
             roc_auc = roc_auc_score(target_values, probabilities)
             self._writer.add_scalar(f"{pass_name} ROC AUC", roc_auc, epoch_number)
 
-    def is_compatible_with(self, output_data_shape: int, target_data_shape: Optional[int]) -> bool:
-        "for regression, target data is needed and output data must be a list of two-dimensional values"
+    def is_compatible_with(self, output_data_shape: int, target_data_shape: Optional[int] = None) -> bool:
+        """For regression, target data is needed and output data must be a list of two-dimensional values."""
 
         return output_data_shape == 2 and target_data_shape == 1
 
 
-class OutputExporter(MetricsExporter):
-    """ A metrics exporter that writes CSV output tables, containing every single data point.
-
-        Included are:
-            - entry names
-            - output values
-            - target values
-
-        The user can load these output tables in excel.
-
-        Outputs are done per epoch.
-    """
-
-    def __init__(self, directory_path: str):
-        self._directory_path = directory_path
-
-    def get_filename(self, pass_name, epoch_number):
-        "returns the filename for the table"
-        return os.path.join(self._directory_path, f"output-{pass_name}-epoch-{epoch_number}.csv.xz")
-
-    def process(self, pass_name: str, epoch_number: int, # pylint: disable=too-many-arguments
-                entry_names: List[str], output_values: List[Any], target_values: List[Any]):
-        "write the output to the table"
-
-        with lzma.open(self.get_filename(pass_name, epoch_number), 'wt', newline='\n') as f:
-            w = csv.writer(f, delimiter=',')
-
-            w.writerow(["entry", "output", "target"])
-
-            for entry_index, entry_name in enumerate(entry_names):
-                output_value = output_values[entry_index]
-                target_value = target_values[entry_index]
-
-                _log.debug(f"writerow [{entry_name}, {output_value}, {target_value}]") # pylint: disable=logging-fstring-interpolation
-
-                w.writerow([entry_name, str(output_value), str(target_value)])
-
+class ScatterPlotExporter(OutputExporter):
+    """An output exporter that can make scatter plots, containing every single data point.
 
-class ScatterPlotExporter(MetricsExporter):
-    """ A metrics exporter that ocasionally makes scatter plots, containing every single data point.
-
-        On the X-axis: targets values
-        On the Y-axis: output values
+    On the X-axis: targets values
+    On the Y-axis: output values
     """
 
     def __init__(self, directory_path: str, epoch_interval: int = 1):
-        """ Args:
-                directory_path: where to store the plots
-                epoch_interval: how often to make a plot, 5 means: every 5 epochs
+        """ 
+        Args:
+            directory_path (str): Where to store the plots.
+            epoch_interval (int, optional): How often to make a plot, 5 means: every 5 epochs. Defaults to 1.
         """
-
+        super().__init__(directory_path)
         self._epoch_interval = epoch_interval
-        self._directory_path = directory_path
 
     def __enter__(self):
         self._plot_data = {}
         return self
 
     def __exit__(self, exception_type, exception, traceback):
         self._plot_data.clear()
 
     def get_filename(self, epoch_number):
-        "returns the filename for the table"
+        """Returns the filename for the table."""
         return os.path.join(self._directory_path, f"scatter-{epoch_number}.png")
 
     @staticmethod
     def _get_color(pass_name):
 
         pass_name = pass_name.lower().strip()
 
@@ -213,15 +184,14 @@
             return "red"
 
         if pass_name == ("test", "testing"):
             return "green"
 
         return random.choice(["yellow", "cyan", "magenta"])
 
-
     @staticmethod
     def _plot(epoch_number: int, data: Dict[str, Tuple[List[float], List[float]]], png_path: str):
 
         pyplot.title(f"Epoch {epoch_number}")
 
         for pass_name, (truth_values, prediction_values) in data.items():
             pyplot.scatter(truth_values, prediction_values, color=ScatterPlotExporter._get_color(pass_name), label=pass_name)
@@ -230,72 +200,84 @@
         pyplot.ylabel("prediction")
 
         pyplot.legend()
         pyplot.savefig(png_path)
         pyplot.close()
 
     def process(self, pass_name: str, epoch_number: int, # pylint: disable=too-many-arguments
-                entry_names: List[str], output_values: List[Any], target_values: List[Any]):
-        "make the plot, if the epoch matches with the interval"
+                entry_names: List[str], output_values: List[Any], target_values: List[Any], loss: float):
+        """Make the plot, if the epoch matches with the interval."""
 
         if epoch_number % self._epoch_interval == 0:
 
             if epoch_number not in self._plot_data:
                 self._plot_data[epoch_number] = {}
 
             self._plot_data[epoch_number][pass_name] = (target_values, output_values)
 
             path = self.get_filename(epoch_number)
             self._plot(epoch_number, self._plot_data[epoch_number], path)
 
-    def is_compatible_with(self, output_data_shape: int, target_data_shape: Optional[int]) -> bool:
-        "for regression, target data is needed and output data must be a list of one-dimensional values"
+    def is_compatible_with(self, output_data_shape: int, target_data_shape: Optional[int] = None) -> bool:
+        """For regression, target data is needed and output data must be a list of one-dimensional values."""
 
         return output_data_shape == 1 and target_data_shape == 1
 
-class ConciseOutputExporter(MetricsExporter):
-    # tbd: if either we want to uniform it with MetricsExporter interface, or if we want to delete the other exporters
-    """ A metrics exporter that writes a CSV output table, containing every single data point.
-
-        Included are:
-            - phase (train/valid/test)
-            - epoch
-            - entry names
-            - output values
-            - target values
-            - loss per epoch
 
-        The user can then load the csv table into a Pandas df, and plotting metrics
+class HDF5OutputExporter(OutputExporter):
+    """An output exporter that saves every single data point in an hdf5 file.
+
+    It is the most general output exporter implemented, and the information
+    contained in the hdf5 file generated allows the user to compute any kind
+    of metrics, for both classification and regression.
+    Results saved are:
+    - phase (train/valid/test)
+    - epoch
+    - entry name
+    - output value/s
+    - target value
+    - loss per epoch
+    The user can then read the content of the hdf5 file into a Pandas dataframe.
     """
 
-    def __init__(
-        self,
-        directory_path: str):
+    def __init__(self, directory_path: str):
 
-        self._directory_path = directory_path
-        d = {'phase': [], 'epoch': [], 'entry': [], 'output': [], 'target': [], 'loss': []}
-        self.df = pd.DataFrame(data=d)
+        self.phase = None
+        super().__init__(directory_path)
+
+    def __enter__(self):
+
+        self.d = {'phase': [], 'epoch': [], 'entry': [], 'output': [], 'target': [], 'loss': []}
+        self.df = pd.DataFrame(data=self.d)
+
+        return self
+
+    def __exit__(self, exception_type, exception, traceback):
 
-    def epoch_process( # pylint: disable=too-many-arguments
+        if self.phase is not None:
+            if self.phase == "validation":
+                self.phase = "training"
+
+            self.df.to_hdf(
+                os.path.join(self._directory_path, 'output_exporter.hdf5'),
+                key=self.phase,
+                mode='a')
+
+    def process( # pylint: disable=too-many-arguments
         self,
         pass_name: str,
         epoch_number: int, 
         entry_names: List[str],
         output_values: List[Any],
         target_values: List[Any],
         loss: float):
 
+        self.phase = pass_name
         pass_name = [pass_name] * len(output_values)
         loss = [loss] * len(output_values)
         epoch_number = [epoch_number] * len(output_values)
 
         d_epoch = {'phase': pass_name, 'epoch': epoch_number, 'entry': entry_names, 'output': output_values, 'target': target_values, 'loss': loss}
         df_epoch = pd.DataFrame(data=d_epoch)
 
         self.df = pd.concat([self.df, df_epoch])
-
-    def save_all_metrics(self):
-
-        self.df.to_hdf(
-            os.path.join(self._directory_path, 'metrics.hdf5'),
-            key='metrics',
-            mode='w')
+        self.df.reset_index(drop=True, inplace=True)
```

### Comparing `deeprankcore-1.0.0/deeprankcore/models/pssm.py` & `deeprankcore-2.0.0/deeprankcore/utils/pssmdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Optional, Dict, List
+from typing import Dict, List, Optional
 
-from deeprankcore.models.amino_acid import AminoAcid
+from deeprankcore.molstruct.aminoacid import AminoAcid
 
 
 class PssmRow:
-    "holds data for one position-specific scoring matrix row"
+    """Holds data for one position-specific scoring matrix row."""
 
     def __init__(self, conservations: Dict[AminoAcid, float], information_content: float):
         self._conservations = conservations
         self._information_content = information_content
 
     @property
     def conservations(self) -> Dict[AminoAcid, float]:
@@ -19,25 +19,25 @@
         return self._information_content
 
     def get_conservation(self, amino_acid: AminoAcid) -> float:
         return self._conservations[amino_acid]
 
 
 class PssmTable:
-    "holds data for one position-specific scoring table"
+    """Holds data for one position-specific scoring table."""
 
     def __init__(self, rows: Optional[List[PssmRow]] = None):
         if rows is None:
             self._rows = {}
         else:
             self._rows = rows
 
     def __contains__(self, residue) -> bool:
         return residue in self._rows
 
     def __getitem__(self, residue) -> PssmRow:
         return self._rows[residue]
 
     def update(self, other):
-        "can be used to merge two non-overlapping scoring tables"
+        """Can be used to merge two non-overlapping scoring tables."""
 
-        self._rows.update(other._rows) # pylint: disable=protected-access
+        self._rows.update(other._rows) # pylint: disable=protected-access
```

### Comparing `deeprankcore-1.0.0/deeprankcore/models/variant.py` & `deeprankcore-2.0.0/deeprankcore/molstruct/variant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-
-from deeprankcore.models.amino_acid import AminoAcid
-from deeprankcore.models.structure import Residue
+from deeprankcore.molstruct.aminoacid import AminoAcid
+from deeprankcore.molstruct.residue import Residue
 
 
 class SingleResidueVariant:
     "represents an amino acid replacement"
 
     def __init__(self, residue: Residue, variant_amino_acid: AminoAcid):
         self._residue = residue
```

### Comparing `deeprankcore-1.0.0/deeprankcore/naive_gnn.py` & `deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/naive_gnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Example of network that doesn't require clusters.  
 
 import torch
-from torch.nn import Module, Linear, Sequential, ReLU
-
+from torch.nn import Linear, Module, ReLU, Sequential
 from torch_scatter import scatter_mean, scatter_sum
 
+
 class NaiveConvolutionalLayer(Module):
 
     def __init__(self, count_node_features, count_edge_features):
         super().__init__()
         message_size = 32
         edge_input_size = 2 * count_node_features + count_edge_features
         self._edge_mlp = Sequential(Linear(edge_input_size, message_size), ReLU())
@@ -28,27 +28,27 @@
         # update nodes
         node_input = torch.cat([node_features, message_sums_per_node], dim=1)
         node_output = self._node_mlp(node_input)
         return node_output
 
 class NaiveNetwork(Module):
 
-    def __init__(self, input_shape, output_shape, input_shape_edge):
+    def __init__(self, input_shape: int, output_shape: int, input_shape_edge: int):
         """
-            Args:
-                input_shape(int): number of node input features
-                output_shape(int): number of output value per graph
-                input_shape_edge(int): number of edge input features
+        Args:
+            input_shape (int): Number of node input features.
+            output_shape (int): Number of output value per graph.
+            input_shape_edge (int): Number of edge input features.
         """
         super().__init__()
         self._external1 = NaiveConvolutionalLayer(input_shape, input_shape_edge)
         self._external2 = NaiveConvolutionalLayer(input_shape, input_shape_edge)
         hidden_size = 128
         self._graph_mlp = Sequential(Linear(input_shape, hidden_size), ReLU(), Linear(hidden_size, output_shape))
 
     def forward(self, data):
         external_updated1_node_features = self._external1(data.x, data.edge_index, data.edge_attr)
         external_updated2_node_features = self._external2(external_updated1_node_features, data.edge_index, data.edge_attr)
         means_per_graph_external = scatter_mean(external_updated2_node_features, data.batch, dim=0)
         graph_input = means_per_graph_external
         z = self._graph_mlp(graph_input)
-        return z
+        return z
```

### Comparing `deeprankcore-1.0.0/deeprankcore/sGAT.py` & `deeprankcore-2.0.0/deeprankcore/neuralnets/gnn/sgat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 import torch
-from torch.nn import Parameter
 import torch.nn.functional as F
 from torch import nn
-
-from torch_scatter import scatter_mean
-
-# torch_geometric import
-from torch_geometric.nn.inits import uniform
+from torch.nn import Parameter
 from torch_geometric.nn import max_pool_x
+from torch_geometric.nn.inits import uniform
+from torch_scatter import scatter_mean
 
-# deeprankcore import
-from deeprankcore.community_pooling import get_preloaded_cluster, community_pooling
+from deeprankcore.utils.community_pooling import (community_pooling,
+                                                  get_preloaded_cluster)
 
 
-class sGraphAttentionLayer(torch.nn.Module):
+class SGraphAttentionLayer(torch.nn.Module):
 
     """
     This is a new layer that is similar to the graph attention network but simpler
     z_i =  1 / Ni \\Sum_j a_ij * [x_i || x_j] * W + b_i
     || is the concatenation operator: [1,2,3] || [4,5,6] = [1,2,3,4,5,6]
     Ni is the number of neighbor of node i
     \\Sum_j runs over the neighbors of node i
     a_ij is the edge attribute between node i and j
     Args:
         in_channels (int): Size of each input sample.
         out_channels (int): Size of each output sample.
         bias (bool, optional): If set to :obj:`False`, the layer will not learn
-            an additive bias. (default: :obj:`True`)
+            an additive bias. Defaults to True.
     """
 
-    def __init__(self, in_channels, out_channels, bias=True, undirected=True):
+    def __init__(self, in_channels: int, out_channels: int, bias: bool = True, undirected=True):
 
         super().__init__()
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.undirected = undirected
 
@@ -82,20 +79,20 @@
 
         return out
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.in_channels}, {self.out_channels})"
 
 
-class sGAT(torch.nn.Module):
+class SGAT(torch.nn.Module):
     def __init__(self, input_shape, output_shape=1, input_shape_edge=None): # pylint: disable=unused-argument
         super().__init__()
 
-        self.conv1 = sGraphAttentionLayer(input_shape, 16)
-        self.conv2 = sGraphAttentionLayer(16, 32)
+        self.conv1 = SGraphAttentionLayer(input_shape, 16)
+        self.conv2 = SGraphAttentionLayer(16, 32)
 
         self.fc1 = torch.nn.Linear(32, 64)
         self.fc2 = torch.nn.Linear(64, output_shape)
 
         self.clustering = "mcl"
 
     def forward(self, data):
```

### Comparing `deeprankcore-1.0.0/deeprankcore/tools/embedding.py` & `deeprankcore-2.0.0/deeprankcore/tools/visualization/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from sklearn.manifold import TSNE, SpectralEmbedding, MDS
+from sklearn.manifold import MDS, TSNE, SpectralEmbedding
+
 
 def manifold_embedding(pos,method='tsne'):
     n_components = 2
     n_neighbors = 100
 
     if method == 'tsne':
         tsne = TSNE(n_components=n_components, init='pca', random_state=0, perplexity=5.0)
```

### Comparing `deeprankcore-1.0.0/deeprankcore/tools/forcefield/residue.py` & `deeprankcore-2.0.0/deeprankcore/utils/parsing/residue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,52 @@
 import re
-from deeprankcore.models.forcefield.residue import (
-    ResidueClassCriterium,
-    ALL_AMINO_ACIDS,
-)
+from typing import List, Union
 
 
+class ResidueClassCriterium:
+    def __init__(
+        self,
+        class_name: str,
+        amino_acid_names: Union[str, List[str]],
+        present_atom_names: List[str],
+        absent_atom_names: List[str],
+    ):
+        self.class_name = class_name
+
+        self.amino_acid_names = amino_acid_names
+
+        self.present_atom_names = present_atom_names
+        self.absent_atom_names = absent_atom_names
+
+    def matches(self, amino_acid_name: str, atom_names: List[str]) -> bool:
+
+        # check the amino acid name
+        if self.amino_acid_names != "all":
+            if not any(
+
+                    amino_acid_name == crit_amino_acid_name
+                    for crit_amino_acid_name in self.amino_acid_names
+
+            ):
+
+                return False
+
+        # check the atom names that should be absent
+        if any(atom_name in self.absent_atom_names for atom_name in atom_names):
+
+            return False
+
+        # check the atom names that should be present
+        if not all(atom_name in atom_names for atom_name in self.present_atom_names):
+
+            return False
+
+        # all checks passed
+        return True
+
 class ResidueClassParser:
     _RESIDUE_CLASS_PATTERN = re.compile(r"([A-Z]{3,4}) *\: *name *\= *(all|[A-Z]{3})")
     _RESIDUE_ATOMS_PATTERN = re.compile(r"(present|absent)\(([A-Z0-9\, ]+)\)")
 
     @staticmethod
     def parse(file_):
         result = []
@@ -36,12 +74,11 @@
                 ResidueClassCriterium(
                     class_name, amino_acid_names, present_atom_names, absent_atom_names
                 )
             )
         return result
 
     @staticmethod
-    def _parse_amino_acids(string):
+    def _parse_amino_acids(string: str):
         if string.strip() == "all":
-            return ALL_AMINO_ACIDS
-
+            return string.strip()
         return [name.strip() for name in string.split(",")]
```

### Comparing `deeprankcore-1.0.0/deeprankcore/tools/forcefield/top.py` & `deeprankcore-2.0.0/deeprankcore/utils/parsing/top.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-import re
 import logging
-from deeprankcore.models.forcefield.top import TopRowObject
+import re
+from typing import Any, Dict
 
 logging.getLogger(__name__)
 
+class TopRowObject:
+    def __init__(self, residue_name: str,
+                 atom_name: str, kwargs: Dict[str, Any]):
+        self.residue_name = residue_name
+        self.atom_name = atom_name
+        self.kwargs = kwargs
+
+    def __getitem__(self, key):
+        return self.kwargs[key]
 
 class TopParser:
     _VAR_PATTERN = re.compile(r"([^\s]+)\s*=\s*([^\s\(\)]+|\(.*\))")
     _LINE_PATTERN = re.compile(
         r"^([A-Z0-9]{3})\s+atom\s+([A-Z0-9]{1,4})\s+(.+)\s+end\s*(\s+\!\s+[ _A-Za-z0-9]+)?$"
     )
     _NUMBER_PATTERN = re.compile(r"\-?[0-9]+(\.[0-9]+)?")
```

### Comparing `deeprankcore-1.0.0/deeprankcore/tools/pdb.py` & `deeprankcore-2.0.0/deeprankcore/utils/buildgraph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 import logging
-from typing import List
+import os
 import subprocess
+from typing import List, Union
 
-from scipy.spatial import distance_matrix
-import numpy
+import numpy as np
 from pdb2sql import interface as get_interface
+from scipy.spatial import distance_matrix
 
-from deeprankcore.models.structure import Atom, Residue, Chain, Structure, AtomicElement
-from deeprankcore.models.amino_acid import amino_acids
-from deeprankcore.models.pair import Pair
-from deeprankcore.domain.forcefield import atomic_forcefield
-from deeprankcore.models.contact import ResidueContact, AtomicContact
-from deeprankcore.feature.atomic_contact import get_coulomb_potentials, get_lennard_jones_potentials
-
+from deeprankcore.domain.aminoacidlist import amino_acids
+from deeprankcore.molstruct.atom import Atom, AtomicElement
+from deeprankcore.molstruct.pair import Pair
+from deeprankcore.molstruct.residue import Residue
+from deeprankcore.molstruct.structure import Chain, PDBStructure
 
 _log = logging.getLogger(__name__)
 
 
-def is_xray(pdb_file):
-    "check that an open pdb file is an x-ray structure"
-
-    for line in pdb_file:
-        if line.startswith("EXPDTA") and "X-RAY DIFFRACTION" in line:
-            return True
-
-    return False
-
-
 def add_hydrogens(input_pdb_path, output_pdb_path):
-    "this requires reduce: https://github.com/rlabduke/reduce"
+    """This requires reduce: https://github.com/rlabduke/reduce."""
 
     with open(output_pdb_path, "wt", encoding = "utf-8") as f:
         p = subprocess.run(["reduce", input_pdb_path], stdout=subprocess.PIPE, check=True)
         for line in p.stdout.decode().split("\n"):
             f.write(line.replace("   new", "").replace("   std", "") + "\n")
 
 
@@ -46,246 +35,204 @@
                 other_atom.change_altloc(atom)
                 return
 
     # not there yet, add it
     residue.add_atom(atom)
 
 
-def get_structure(pdb, id_): # pylint: disable=too-many-locals
-    """Builds a structure from rows in a pdb file
+_amino_acids_by_code = {
+    amino_acid.three_letter_code: amino_acid for amino_acid in amino_acids
+}
+
+
+_elements_by_name = {element.name: element for element in AtomicElement}
+
+
+def _add_atom_data_to_structure(structure: PDBStructure,  # pylint: disable=too-many-arguments, too-many-locals
+                                x: float, y: float, z: float,
+                                atom_name: str,
+                                altloc: str, occupancy: float,
+                                element_name: str,
+                                chain_id: str,
+                                residue_number: int,
+                                residue_name: str,
+                                insertion_code: str):
+
+    """
+    This is a subroutine, to be used in other methods for converting pdb2sql atomic data into a
+    deeprank structure object. It should be called for one atom.
+
     Args:
-        pdb (pdb2sql object): the pdb structure that we're investigating
-        id (str): unique id for the pdb structure
-    Returns (Structure): the structure object, giving access to chains, residues, atoms
+        structure (:class:`PDBStructure`): Where this atom should be added to.
+        x (float): x-coordinate of atom.
+        y (float): y-coordinate of atom.
+        z (float): z-coordinate of atom.
+        atom_name (str): Name of atom: 'CA', 'C', 'N', 'O', 'CB', etc.
+        altloc (str): Pdb alternative location id for this atom (can be empty): 'A', 'B', 'C', etc.
+        occupancy (float): Pdb occupancy of this atom, ranging from 0.0 to 1.0. Should be used with altloc.
+        element_name (str): Pdb element symbol of this atom: 'C', 'O', 'H', 'N', 'S'.
+        chain_id (str): Pdb chain identifier: 'A', 'B', 'C', etc.
+        residue_number (int): Pdb residue number, a positive integer.
+        residue_name (str): Pdb residue name: "ALA", "CYS", "ASP", etc.
+        insertion_code (str): Pdb residue insertion code (can be empty) : '', 'A', 'B', 'C', etc.
     """
 
-    amino_acids_by_code = {
-        amino_acid.three_letter_code: amino_acid for amino_acid in amino_acids
-    }
-    elements_by_name = {element.name: element for element in AtomicElement}
+    # Make sure not to take the same atom twice.
+    if altloc is not None and altloc != "" and altloc != "A":
+        return
+
+    # We use None to indicate that the residue has no insertion code.
+    if insertion_code == "":
+        insertion_code = None
+
+    # The amino acid is only valid when we deal with protein residues.
+    if residue_name in _amino_acids_by_code:
+        amino_acid = _amino_acids_by_code[residue_name]
+    else:
+        amino_acid = None
+
+    # Turn the x,y,z into a vector:
+    atom_position = np.array([x, y, z])
+
+    # Init chain.
+    if not structure.has_chain(chain_id):
+
+        chain = Chain(structure, chain_id)
+        structure.add_chain(chain)
+    else:
+        chain = structure.get_chain(chain_id)
+
+    # Init residue.
+    if not chain.has_residue(residue_number, insertion_code):
+
+        residue = Residue(chain, residue_number, amino_acid, insertion_code)
+        chain.add_residue(residue)
+    else:
+        residue = chain.get_residue(residue_number, insertion_code)
+
+    # Init atom.
+    atom = Atom(
+        residue, atom_name, _elements_by_name[element_name], atom_position, occupancy
+    )
+    _add_atom_to_residue(atom, residue)
+
+
+def get_structure(pdb, id_: str):
+    """Builds a structure from rows in a pdb file.
+
+    Args:
+        pdb (pdb2sql object): The pdb structure that we're investigating.
+        id (str): Unique id for the pdb structure.
+
+    Returns: 
+        PDBStructure: The structure object, giving access to chains, residues, atoms.
+    """
 
     # We need these intermediary dicts to keep track of which residues and
     # chains have already been created.
-    chains = {}
-    residues = {}
-
-    structure = Structure(id_)
+    structure = PDBStructure(id_)
 
     # Iterate over the atom output from pdb2sql
     for row in pdb.get(
         "x,y,z,rowID,name,altLoc,occ,element,chainID,resSeq,resName,iCode", model=0
     ):
 
         (
             x,
             y,
             z,
             _,
             atom_name,
             altloc,
             occupancy,
-            element,
+            element_name,
             chain_id,
             residue_number,
             residue_name,
             insertion_code,
         ) = row
 
-        # Make sure not to take the same atom twice.
-        if altloc is not None and altloc != "" and altloc != "A":
-            continue
-
-        # We use None to indicate that the residue has no insertion code.
-        if insertion_code == "":
-            insertion_code = None
-
-        # The amino acid is only valid when we deal with protein residues.
-        if residue_name in amino_acids_by_code:
-            amino_acid = amino_acids_by_code[residue_name]
-        else:
-            amino_acid = None
-
-        # Turn the x,y,z into a vector:
-        atom_position = numpy.array([x, y, z])
-
-        # Init chain.
-        if chain_id not in chains:
-
-            chain = Chain(structure, chain_id)
-            chains[chain_id] = chain
-            structure.add_chain(chain)
-        else:
-            chain = chains[chain_id]
-
-        # Init residue.
-        residue_id = (chain_id, residue_number, insertion_code)
-        if residue_id not in residues:
-
-            residue = Residue(chain, residue_number, amino_acid, insertion_code)
-            residues[residue_id] = residue
-            chain.add_residue(residue)
-        else:
-            residue = residues[residue_id]
-
-        # Init atom.
-        atom = Atom(
-            residue, atom_name, elements_by_name[element], atom_position, occupancy
-        )
-        _add_atom_to_residue(atom, residue)
+        _add_atom_data_to_structure(structure,
+                                    x, y, z,
+                                    atom_name,
+                                    altloc, occupancy,
+                                    element_name,
+                                    chain_id,
+                                    residue_number,
+                                    residue_name,
+                                    insertion_code)
 
     return structure
 
 
-def get_atomic_contacts(atoms: List[Atom]) -> List[AtomicContact]:
-    """Computes all the contacts between a given list of atoms.
-    It doesn't pair atoms with themselves, so no zero divisions are expected.
-
-    Warning: do not call this on all atoms in the structure, since this can lead to
-             excessive memory consumption! Be sure to use queries to make a selection.
-    """
-
-    atom_postions = [atom.position for atom in atoms]
-
-    # calculate distance matrix
-    interatomic_distances = distance_matrix(atom_postions, atom_postions, p=2)
-
-    # get forcefield parameters
-    atom_charges = [atomic_forcefield.get_charge(atom) for atom in atoms]
-    atom_vanderwaals_parameters = [
-        atomic_forcefield.get_vanderwaals_parameters(atom) for atom in atoms
-    ]
-
-    # calculate potentials
-    interatomic_electrostatic_potentials = get_coulomb_potentials(
-        interatomic_distances, atom_charges
-    )
-    interatomic_vanderwaals_potentials = get_lennard_jones_potentials(
-        interatomic_distances, atoms, atom_vanderwaals_parameters
-    )
-
-    # build contacts
-    contacts = []
-
-    count_atoms = len(atoms)
-    for atom1_index in range(count_atoms):
-        for atom2_index in range(
-            atom1_index + 1, count_atoms
-        ):  # don't make the same contact twice and don't pair an atom with itself
-
-            contacts.append(
-                AtomicContact( # pylint: disable=too-many-function-args
-                    atoms[atom1_index],
-                    atoms[atom2_index],
-                    interatomic_distances[atom1_index][atom2_index],
-                    interatomic_electrostatic_potentials[atom1_index][atom2_index],
-                    interatomic_vanderwaals_potentials[atom1_index][atom2_index],
-                )
-            )
-    return contacts
-
-
-def get_residue_contacts(residues: List[Residue]) -> List[ResidueContact]:
-    """Computes all the contacts between a given list of residues.
-    It doesn't pair residues with themselves, so no zero divisions are expected.
-
-    Warning: do not call this on all residues in the structure, since this can lead to
-             excessive memory consumption! Be sure to use queries to make a selection.
-    """
-
-    atoms = []
-    for residue in residues:
-        atoms += residue.atoms
-
-    atomic_contacts = get_atomic_contacts(atoms)
-
-    # start with empty dictionaries, to hold the distance and energies per
-    # contact
-    residue_minimum_distances = {}
-    residue_electrostatic_potential_sums = {}
-    residue_vanderwaals_potential_sums = {}
-
-    # iterate over all interatomic contacts
-    for atomic_contact in atomic_contacts:
-        if (
-            atomic_contact.atom1.residue != atomic_contact.atom2.residue
-        ):  # don't pair a residue with itself
-
-            residue1 = atomic_contact.atom1.residue
-            residue2 = atomic_contact.atom2.residue
-
-            residue_pair = Pair(residue1, residue2)
-
-            if residue_pair not in residue_minimum_distances:
-
-                # initialize distance and energies per residue contact
-                residue_minimum_distances[residue_pair] = 1e99
-                residue_electrostatic_potential_sums[residue_pair] = 0.0
-                residue_vanderwaals_potential_sums[residue_pair] = 0.0
-
-            # aggregate
-            residue_minimum_distances[residue_pair] = min(
-                residue_minimum_distances[residue_pair], atomic_contact.distance
-            )
-            residue_electrostatic_potential_sums[
-                residue_pair
-            ] += atomic_contact.electrostatic_potential
-            residue_vanderwaals_potential_sums[
-                residue_pair
-            ] += atomic_contact.vanderwaals_potential
-
-    # convert to residue contacts
-    residue_contacts = []
-    for residue_pair, distance in residue_minimum_distances.items():
-        residue_contacts.append(
-            ResidueContact( # pylint: disable=too-many-function-args
-                residue_pair.item1,
-                residue_pair.item2,
-                distance,
-                residue_electrostatic_potential_sums[residue_pair],
-                residue_vanderwaals_potential_sums[residue_pair],
-            )
-        )
-    return residue_contacts
-
-
-def get_residue_distance(residue1, residue2):
-    """Get the shortest distance between two atoms from two different given residues.
+def get_contact_atoms( # pylint: disable=too-many-locals
+    pdb_path: str,
+    chain_id1: str,
+    chain_id2: str,
+    distance_cutoff: float
+) -> List[Atom]:
+    """Gets the contact atoms from pdb2sql and wraps them in python objects."""
 
-    Args:
-        residue1(deeprank residue object): the first residue
-        residue2(deeprank residue object): the second residue
+    interface = get_interface(pdb_path)
+    try:
+        atom_indexes = interface.get_contact_atoms(cutoff=distance_cutoff, chain1=chain_id1, chain2=chain_id2)
+        rows = interface.get("x,y,z,name,element,altLoc,occ,chainID,resSeq,resName,iCode",
+                             rowID=atom_indexes[chain_id1] + atom_indexes[chain_id2])
+    finally:
+        interface._close()  # pylint: disable=protected-access
 
-    Returns(float): the shortest distance
-    """
+    pdb_name = os.path.splitext(os.path.basename(pdb_path))[0]
 
-    residue1_atom_positions = numpy.array([atom.position for atom in residue1.atoms])
-    residue2_atom_positions = numpy.array([atom.position for atom in residue2.atoms])
+    structure = PDBStructure(f"contact_atoms_{pdb_name}")
 
-    distances = distance_matrix(residue1_atom_positions, residue2_atom_positions, p=2)
+    for row in rows:
+        (
+            x,
+            y,
+            z,
+            atom_name,
+            element_name,
+            altloc,
+            occupancy,
+            chain_id,
+            residue_number,
+            residue_name,
+            insertion_code
+        ) = row
 
-    return numpy.min(distances)
+        _add_atom_data_to_structure(structure,
+                                    x, y, z,
+                                    atom_name,
+                                    altloc, occupancy,
+                                    element_name,
+                                    chain_id,
+                                    residue_number,
+                                    residue_name,
+                                    insertion_code)
 
+    return structure.get_atoms()
 
 def get_residue_contact_pairs( # pylint: disable=too-many-locals
     pdb_path: str,
-    structure: Structure,
+    structure: PDBStructure,
     chain_id1: str,
     chain_id2: str,
     distance_cutoff: float,
 ) -> List[Pair]:
     """Get the residues that contact each other at a protein-protein interface.
 
     Args:
-        pdb_path: the path of the pdb file, that the structure was built from
-        structure: from which to take the residues
-        chain_id1: first protein chain identifier
-        chain_id2: second protein chain identifier
-        distance_cutoff: max distance between two interacting residues
+        pdb_path (str): The path of the pdb file, that the structure was built from.
+        structure (:class:`PDBStructure`): From which to take the residues.
+        chain_id1 (str): First protein chain identifier.
+        chain_id2 (str): Second protein chain identifier.
+        distance_cutoff (float): Max distance between two interacting residues.
 
-    Returns: the pairs of contacting residues
+    Returns: 
+        List[Pair]: The pairs of contacting residues.
     """
 
     # Find out which residues are pairs
     interface = get_interface(pdb_path)
     try:
         contact_residues = interface.get_contact_residues(
             cutoff=distance_cutoff,
@@ -338,62 +285,38 @@
                 )
 
             residue_pairs.add(Pair(residue1, residue2))
 
     return residue_pairs
 
 
-def get_surrounding_residues(structure, residue, radius):
+def get_surrounding_residues(structure: Union[Chain, PDBStructure], residue: Residue, radius: float):
     """Get the residues that lie within a radius around a residue.
 
     Args:
-        structure(deeprank structure object): the structure to take residues from
-        residue(deeprank residue object): the residue in the structure
-        radius(float): max distance in Ångström between atoms of the residue and the other residues
+        structure (Union[:class:`Chain`, :class:`PDBStructure`]): The structure to take residues from.
+        residue (:class:`Residue`): The residue in the structure.
+        radius (float): Max distance in Ångström between atoms of the residue and the other residues.
 
-    Returns: (a set of deeprank residues): the surrounding residues
+    Returns: 
+        (a set of deeprank residues): The surrounding residues.
     """
 
     structure_atoms = structure.get_atoms()
     residue_atoms = residue.atoms
 
     structure_atom_positions = [atom.position for atom in structure_atoms]
     residue_atom_positions = [atom.position for atom in residue_atoms]
 
     distances = distance_matrix(structure_atom_positions, residue_atom_positions, p=2)
 
     close_residues = set([])
 
     for structure_atom_index, structure_atom in enumerate(structure_atoms):
 
-        shortest_distance = numpy.min(distances[structure_atom_index, :])
+        shortest_distance = np.min(distances[structure_atom_index, :])
 
         if shortest_distance < radius:
 
             close_residues.add(structure_atom.residue)
 
     return close_residues
-
-
-def find_neighbour_atoms(atoms, max_distance):
-    """For a given list of atoms, find the pairs of atoms that lie next to each other.
-
-    Args:
-        atoms(list of deeprank atom objects): the atoms to look at
-        max_distance(float): max distance between two atoms in Ångström
-
-    Returns: (a set of deeprank atom object pairs): the paired atoms
-    """
-
-    atom_positions = [atom.position for atom in atoms]
-
-    distances = distance_matrix(atom_positions, atom_positions, p=2)
-
-    neighbours = distances < max_distance
-
-    pairs = set([])
-
-    for atom1_index, atom2_index in numpy.transpose(numpy.nonzero(neighbours)):
-        if atom1_index != atom2_index:
-            pairs.add(Pair(atoms[atom1_index], atoms[atom2_index]))
-
-    return pairs
```

### Comparing `deeprankcore-1.0.0/deeprankcore/tools/pssm.py` & `deeprankcore-2.0.0/deeprankcore/utils/parsing/pssm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from typing import TextIO
 
-from deeprankcore.models.structure import Residue, Chain
-from deeprankcore.models.pssm import PssmRow, PssmTable
-from deeprankcore.models.amino_acid import amino_acids
-
-amino_acids_by_letter = {
-    amino_acid.one_letter_code: amino_acid for amino_acid in amino_acids
-}
+from deeprankcore.domain.aminoacidlist import amino_acids
+from deeprankcore.molstruct.residue import Residue
+from deeprankcore.molstruct.structure import Chain
+from deeprankcore.utils.pssmdata import PssmRow, PssmTable
 
 
 def parse_pssm(file_: TextIO, chain: Chain) -> PssmTable:
-    """
-    Read the PSSM data.
+    """Read the PSSM data.
 
     Args:
-        file_(python text file object): the pssm file
-        chain(deeprank Chain object): the chain that the pssm file represents, residues from this chain must match the pssm file
+        file_ (python text file object): The pssm file.
+        chain (:class:`Chain`): The chain that the pssm file represents, residues from this chain must match the pssm file.
 
-    Returns(ConservationTable): the position-specific scoring table, parsed from the pssm file
+    Returns
+        PssmTable: The position-specific scoring table, parsed from the pssm file.
     """
 
+    amino_acids_by_letter = {amino_acid.one_letter_code: amino_acid for amino_acid in amino_acids}
     conservation_rows = {}
 
     # Read the pssm header.
     header = next(file_).split()
     column_indices = {
         column_name.strip(): index for index, column_name in enumerate(header)
     }
```

### Comparing `deeprankcore-1.0.0/deeprankcore/tools/visualization.py` & `deeprankcore-2.0.0/deeprankcore/tools/visualization/plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 import logging
 from copy import deepcopy
 from typing import Optional
-import plotly.graph_objs as go
-import matplotlib.pyplot as plt
 
-import h5py
-import numpy
-import networkx
 import community
+import h5py
 import markov_clustering
+import matplotlib.pyplot as plt
+import networkx
+import numpy as np
+import plotly.graph_objs as go
 
-from deeprankcore.tools.embedding import manifold_embedding
-from deeprankcore.domain.features import groups
-from deeprankcore.domain.features import edgefeats
-
+from deeprankcore.domain import edgestorage as Efeat
+from deeprankcore.domain import nodestorage as Nfeat
+from deeprankcore.tools.visualization.embedding import manifold_embedding
 
 _log = logging.getLogger(__name__)
 
 
 def _get_node_key(value):
     if isinstance(value, str):
         return value
 
     key = ""
     for item in value:
-        if isinstance(item, (bytes, numpy.bytes_)):
+        if isinstance(item, (bytes, np.bytes_)):
             key = item.decode()
 
         elif isinstance(item, str):
             key += item
 
         else:
             key += str(item)
 
     return key
 
 
 def hdf5_to_networkx(graph_group: h5py.Group) -> networkx.Graph: # pylint: disable=too-many-locals
-    """Read a hdf5 group into a networkx graph"""
+    """Read a hdf5 group into a networkx graph."""
 
     graph = networkx.Graph()
 
     # read nodes
-    node_features_group = graph_group[groups.NODE]
-    node_names = [_get_node_key(key) for key in node_features_group[groups.NAME][()]]
+    node_features_group = graph_group[Nfeat.NODE]
+    node_names = [_get_node_key(key) for key in node_features_group[Nfeat.NAME][()]]
     node_features = {}
     node_feature_names = list(node_features_group.keys())
     for node_feature_name in node_feature_names:
         node_features[node_feature_name] = node_features_group[node_feature_name][()]
 
     for node_index, node_name in enumerate(node_names):
         graph.add_node(node_name)
         for node_feature_name in node_feature_names:
             graph.nodes[node_name][node_feature_name] = node_features[
                 node_feature_name
             ][node_index]
 
     # read edges
-    edge_features_group = graph_group[groups.EDGE]
-    edge_names = edge_features_group[groups.NAME][()]
-    edge_node_indices = edge_features_group[groups.INDEX][()]
+    edge_features_group = graph_group[Efeat.EDGE]
+    edge_names = edge_features_group[Efeat.NAME][()]
+    edge_node_indices = edge_features_group[Efeat.INDEX][()]
     edge_features = {}
     edge_feature_names = list(edge_features_group.keys())
     for edge_feature_name in edge_feature_names:
         edge_features[edge_feature_name] = edge_features_group[edge_feature_name][()]
 
     for edge_index, _ in enumerate(edge_names):
         node1_index, node2_index = edge_node_indices[edge_index]
@@ -77,48 +76,48 @@
                 edge_index
             ]
 
     return graph
 
 
 def _get_edge_type_name(value):
-    if isinstance(value, (bytes, numpy.bytes_)):
+    if isinstance(value, (bytes, np.bytes_)):
 
         return value.decode()
 
     return value
 
 
 def plotly_2d( # noqa
     graph: networkx.Graph,
     out: Optional[str] = None,
     offline: bool = False,
     iplot: bool = True,
     disable_plot: bool = False,
     method: str = "louvain",
 ):
-    """Plots the interface graph in 2D"""
+    """Plots the interface graph in 2D."""
 
     if offline:
-        import plotly.offline as py # pylint: disable=import-outside-toplevel
+        import plotly.offline as py  # pylint: disable=import-outside-toplevel
     else:
-        import chart_studio.plotly as py # pylint: disable=import-outside-toplevel
+        import chart_studio.plotly as py  # pylint: disable=import-outside-toplevel
 
-    pos = numpy.array(
-        [v.tolist() for _, v in networkx.get_node_attributes(graph, groups.POSITION).items()]
+    pos = np.array(
+        [v.tolist() for _, v in networkx.get_node_attributes(graph, Nfeat.POSITION).items()]
     )
-    pos2D = manifold_embedding(pos)
-    dict_pos = dict(zip(graph.nodes, pos2D))
-    networkx.set_node_attributes(graph, dict_pos, "pos2D")
+    pos2d = manifold_embedding(pos)
+    dict_pos = dict(zip(graph.nodes, pos2d))
+    networkx.set_node_attributes(graph, dict_pos, "pos2d")
 
     # remove interface edges for clustering
     gtmp = deepcopy(graph)
     ebunch = []
     for e in graph.edges:
-        if graph.edges[e][edgefeats.SAMECHAIN] == 0.0:
+        if graph.edges[e][Efeat.SAMECHAIN] == 0.0:
             ebunch.append(e)
     gtmp.remove_edges_from(ebunch)
 
     if method == "louvain":
         cluster = community.best_partition(gtmp)
 
     elif method == "mcl":
@@ -129,27 +128,27 @@
         cluster = {}
         node_key = list(graph.nodes.keys())
         for ic, c in enumerate(mcl_clust):
             for node in c:
                 cluster[node_key[node]] = ic
 
     # get the colormap for the clsuter line
-    ncluster = numpy.max([v for _, v in cluster.items()]) + 1
+    ncluster = np.max([v for _, v in cluster.items()]) + 1
     cmap = plt.cm.nipy_spectral
     N = cmap.N
     cmap = [cmap(i) for i in range(N)]
     cmap = cmap[:: int(N / ncluster)]
     cmap = "plasma"
 
     edge_trace_list, internal_edge_trace_list = [], []
 
     node_connect = {}
     for edge in graph.edges:
 
-        same_chain = graph.edges[edge[0], edge[1]][edgefeats.SAMECHAIN]
+        same_chain = graph.edges[edge[0], edge[1]][Efeat.SAMECHAIN]
         if same_chain == 1.0: # internal
             trace = go.Scatter(
                 x=[],
                 y=[],
                 text=[],
                 mode="lines",
                 hoverinfo=None,
@@ -166,16 +165,16 @@
                 hoverinfo=None,
                 showlegend=False,
                 line=go.scatter.Line(color="rgb(210,210,210)", width=1),
             )
         else:
             continue
 
-        x0, y0 = graph.nodes[edge[0]]["pos2D"]
-        x1, y1 = graph.nodes[edge[1]]["pos2D"]
+        x0, y0 = graph.nodes[edge[0]]["pos2d"]
+        x1, y1 = graph.nodes[edge[1]]["pos2d"]
 
         trace["x"] += (x0, x1, None)
         trace["y"] += (y0, y1, None)
 
         if same_chain == 1.0: # internal
             internal_edge_trace_list.append(trace)
 
@@ -183,61 +182,61 @@
             edge_trace_list.append(trace)
 
         for i in [0, 1]:
             if edge[i] not in node_connect:
                 node_connect[edge[i]] = 1
             else:
                 node_connect[edge[i]] += 1
-    node_trace_A = go.Scatter(
+    node_trace_a = go.Scatter(
         x=[],
         y=[],
         text=[],
         mode="markers",
         hoverinfo="text",
         marker=dict(
             color="rgb(227,28,28)",
             size=[],
             line=dict(color=[], width=4, colorscale=cmap),
         ),
     )
     # 'rgb(227,28,28)'
-    node_trace_B = go.Scatter(
+    node_trace_b = go.Scatter(
         x=[],
         y=[],
         text=[],
         mode="markers",
         hoverinfo="text",
         marker=dict(
             color="rgb(0,102,255)",
             size=[],
             line=dict(color=[], width=4, colorscale=cmap),
         ),
     )
     # 'rgb(0,102,255)'
-    node_trace = [node_trace_A, node_trace_B]
+    node_trace = [node_trace_a, node_trace_b]
 
     for x, node in enumerate(graph.nodes):
 
         index = 0
-        if groups.CHAINID in graph.nodes[node]:
+        if Nfeat.CHAINID in graph.nodes[node]:
             if x == 0:
-                first_chain = graph.nodes[node][groups.CHAINID]
-            if graph.nodes[node][groups.CHAINID] != first_chain: # This is not very pythonic, but somehow I'm stuck on how to do this without enumerating
+                first_chain = graph.nodes[node][Nfeat.CHAINID]
+            if graph.nodes[node][Nfeat.CHAINID] != first_chain: # This is not very pythonic, but somehow I'm stuck on how to do this without enumerating
                 index = 1
         
-        pos = graph.nodes[node]["pos2D"]
+        pos = graph.nodes[node]["pos2d"]
 
         node_trace[index]["x"] += (pos[0],)
         node_trace[index]["y"] += (pos[1],)
         node_trace[index]["text"] += (
             "[Clst:" + str(cluster[node]) + "] " + " ".join(node),
         )
 
         nc = node_connect[node]
-        node_trace[index]["marker"]["size"] += (5 + 15 * numpy.tanh(nc / 5),)
+        node_trace[index]["marker"]["size"] += (5 + 15 * np.tanh(nc / 5),)
         node_trace[index]["marker"]["line"]["color"] += (cluster[node],)
 
     fig = go.Figure(
         data=[*internal_edge_trace_list, *edge_trace_list, *node_trace],
         layout=go.Layout(
             title="<br>tSNE connection graph",
             titlefont=dict(size=16),
@@ -269,34 +268,35 @@
 def plotly_3d( # pylint: disable=too-many-locals, too-many-branches # noqa: MC0001
     graph: networkx.Graph,
     out: Optional[str] = None,
     offline: bool = False,
     iplot: bool = True,
     disable_plot: bool = False,
 ):
-    """Plots interface graph in 3D
+    """Plots interface graph in 3D.
 
     Args:
-        graph(deeprank graph object): the graph to be plotted
-        out ([type], optional): [description]. Defaults to None.
-        offline (bool, optional): [description]. Defaults to False.
-        iplot (bool, optional): [description]. Defaults to True.
+        graph (:class:`networkx.Graph`): The graph to be plotted.
+        out (str, optional): Defaults to None.
+        offline (bool, optional): Defaults to False.
+        iplot (bool, optional): Defaults to True.
+        disable_plot (bool, optional): Defaults to False.
     """
 
     if offline:
-        import plotly.offline as py # pylint: disable=import-outside-toplevel
+        import plotly.offline as py  # pylint: disable=import-outside-toplevel
     else:
-        import chart_studio.plotly as py # pylint: disable=import-outside-toplevel
+        import chart_studio.plotly as py  # pylint: disable=import-outside-toplevel
 
     edge_trace_list, internal_edge_trace_list = [], []
     node_connect = {}
 
     for edge in graph.edges:
 
-        same_chain = graph.edges[edge[0], edge[1]][edgefeats.SAMECHAIN]
+        same_chain = graph.edges[edge[0], edge[1]][Efeat.SAMECHAIN]
         if same_chain == 1.0: # internal
             trace = go.Scatter3d(
                 x=[],
                 y=[],
                 z=[],
                 text=[],
                 mode="lines",
@@ -315,16 +315,16 @@
                 hoverinfo=None,
                 showlegend=False,
                 line=go.scatter3d.Line(color="rgb(210,210,210)", width=2),
             )
         else:
             continue
 
-        x0, y0, z0 = graph.nodes[edge[0]][groups.POSITION]
-        x1, y1, z1 = graph.nodes[edge[1]][groups.POSITION]
+        x0, y0, z0 = graph.nodes[edge[0]][Nfeat.POSITION]
+        x1, y1, z1 = graph.nodes[edge[1]][Nfeat.POSITION]
 
         trace["x"] += (x0, x1, None)
         trace["y"] += (y0, y1, None)
         trace["z"] += (z0, z1, None)
 
         if same_chain == 1.0: # internal
             internal_edge_trace_list.append(trace)
@@ -334,64 +334,64 @@
 
         for i in [0, 1]:
             if edge[i] not in node_connect:
                 node_connect[edge[i]] = 1
             else:
                 node_connect[edge[i]] += 1
 
-    node_trace_A = go.Scatter3d(
+    node_trace_a = go.Scatter3d(
         x=[],
         y=[],
         z=[],
         text=[],
         mode="markers",
         hoverinfo="text",
         marker=dict(
             color="rgb(227,28,28)",
             size=[],
             symbol="circle",
             line=dict(color="rgb(50,50,50)", width=2),
         ),
     )
 
-    node_trace_B = go.Scatter3d(
+    node_trace_b = go.Scatter3d(
         x=[],
         y=[],
         z=[],
         text=[],
         mode="markers",
         hoverinfo="text",
         marker=dict(
             color="rgb(0,102,255)",
             size=[],
             symbol="circle",
             line=dict(color="rgb(50,50,50)", width=2),
         ),
     )
 
-    node_trace = [node_trace_A, node_trace_B]
+    node_trace = [node_trace_a, node_trace_b]
 
     for x, node in enumerate(graph.nodes):
 
         index = 0
-        if groups.CHAINID in graph.nodes[node]:
+        if Nfeat.CHAINID in graph.nodes[node]:
             if x == 0:
-                first_chain = graph.nodes[node][groups.CHAINID]
-            if graph.nodes[node][groups.CHAINID] != first_chain: # This is not very puythonic, but somehow I'm stuck on how to do this without enumerating
+                first_chain = graph.nodes[node][Nfeat.CHAINID]
+            if graph.nodes[node][Nfeat.CHAINID] != first_chain: # This is not very puythonic, but somehow I'm stuck on how to do this without enumerating
                 index = 1
 
-        pos = graph.nodes[node][groups.POSITION]
+        pos = graph.nodes[node][Nfeat.POSITION]
 
         node_trace[index]["x"] += (pos[0],)
         node_trace[index]["y"] += (pos[1],)
         node_trace[index]["z"] += (pos[2],)
         node_trace[index]["text"] += (" ".join(node),)
 
         nc = node_connect[node]
-        node_trace[index]["marker"]["size"] += (5 + 15 * numpy.tanh(nc / 5),)
+        node_trace[index]["marker"]["size"] += (5 + 15 * np.tanh(nc / 5),)
 
     fig = go.Figure(
         data=[*node_trace, *internal_edge_trace_list, *edge_trace_list],
         layout=go.Layout(
             title="<br>Connection graph",
             titlefont=dict(size=16),
             showlegend=False,
```

### Comparing `deeprankcore-1.0.0/deeprankcore.egg-info/PKG-INFO` & `deeprankcore-2.0.0/deeprankcore.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deeprankcore
-Version: 1.0.0
-Summary: deeprank-core allows to train graph neural networks to classify protein-protein interface with a greater flexibility for the user.
+Version: 2.0.0
+Summary: deeprankcore allows to train graph neural networks to classify protein-protein interface with a greater flexibility for the user.
 Home-page: https://github.com/DeepRank/deeprank-core
 Project-URL: Bug Tracker, https://github.com/DeepRank/deeprank-core/issues
 Keywords: graph neural network,protein-protein interface,pytorch
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -15,354 +15,323 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: publishing
 License-File: LICENSE
 
-# Deeprank-Core
+# DeeprankCore
 
 | Badges | |
 |:----:|----|
 | **fairness** |  [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6403/badge)](https://bestpractices.coreinfrastructure.org/projects/6403) |
 | **package** |  [![PyPI version](https://badge.fury.io/py/deeprankcore.svg)](https://badge.fury.io/py/deeprankcore) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f3f98b2d1883493ead50e3acaa23f2cc)](https://app.codacy.com/gh/DeepRank/deeprank-core?utm_source=github.com&utm_medium=referral&utm_content=DeepRank/deeprank-core&utm_campaign=Badge_Grade) |
 | **docs** | [![Documentation Status](https://readthedocs.org/projects/deeprankcore/badge/?version=latest)](https://deeprankcore.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/450496579.svg)](https://zenodo.org/badge/latestdoi/450496579) |
 | **tests** | [![Build Status](https://github.com/DeepRank/deeprank-core/actions/workflows/build.yml/badge.svg)](https://github.com/DeepRank/deeprank-core/actions) ![Linting status](https://github.com/DeepRank/deeprank-core/actions/workflows/linting.yml/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/DeepRank/deeprank-core/badge.svg?branch=main)](https://coveralls.io/github/DeepRank/deeprank-core?branch=main) |
-| **license** |  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  |
+| **license** |  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/license/apache-2-0/)  |
 
 
 ## Overview
 
 ![alt-text](./deeprankcore.png)
 
-Deeprank-Core is a deep learning framework for data mining Protein-Protein Interactions (PPIs) using Graph Neural Networks. 
 
-Deeprank-Core contains useful APIs for pre-processing PPIs data, computing features and targets, as well as training and testing GNN models.
+DeeprankCore is a Deep Learning (DL) framework for data mining Protein-Protein Interactions (PPIs) using either Graph Neural Networks (GNNs) or Convolutional Neural Networks (CNNs). It is an improved and unified version of the previously developed [deeprank](https://github.com/DeepRank/deeprank) and [Deeprank-GNN](https://github.com/DeepRank/Deeprank-GNN).
 
-#### Features:
+DeeprankCore contains useful APIs for pre-processing PPI data, computing features and targets, as well as training and testing GNN and CNN models.
+
+Main features:
 - Predefined atom-level and residue-level PPI feature types
   - e.g. atomic density, vdw energy, residue contacts, PSSM, etc.
 - Predefined target type
   - e.g. binary class, CAPRI categories, DockQ, RMSD, FNAT, etc.
 - Flexible definition of both new features and targets
-- Graphs feature mapping
+- Graphs and grids feature mapping
 - Efficient data storage in HDF5 format
-- Support both classification and regression (based on PyTorch and PyTorch Geometric)
+- Support both classification and regression (based on [PyTorch](https://pytorch.org/) and [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/))
 
-Deeprank-Core documentation can be found here : https://deeprankcore.rtfd.io/.
+DeeprankCore extensive documentation can be found [here](https://deeprankcore.rtfd.io/).
 
 ## Table of contents
 
-- [Deeprank-Core](#deeprank-core)
+- [DeeprankCore](#deeprankcore)
   - [Overview](#overview)
-      - [Features:](#features)
   - [Table of contents](#table-of-contents)
   - [Installation](#installation)
     - [Dependencies](#dependencies)
-    - [Deeprank-core Package](#deeprank-core-package)
+    - [Deeprank-Core Package](#deeprank-core-package)
   - [Documentation](#documentation)
-  - [Getting Started](#getting-started)
-    - [Data generation](#data-generation)
-    - [Data exploration](#data-exploration)
-    - [Dataset(s)](#datasets)
+  - [Quick start](#quick-start)
+    - [Data mapping](#data-mapping)
+    - [Datasets](#datasets)
+      - [GraphDataset](#graphdataset)
+      - [GridDataset](#griddataset)
     - [Training](#training)
-      - [Custom GNN](#custom-gnn)
   - [h5x support](#h5x-support)
-  - [For the developers](#for-the-developers)
-    - [Software release](#software-release)
+  - [Package development](#package-development)
 
 ## Installation
 
 ### Dependencies
 
-Before installing deeprank-core you need to install:
+Before installing deeprankcore you need to install:
 
  * [reduce](https://github.com/rlabduke/reduce): follow the instructions in the README of the reduce repository.
     * **How to build it without sudo privileges on a Linux machine**. After having run `make` in the reduce/ root directory, go to reduce/reduce_src/Makefile and modify `/usr/local/` to a folder in your home directory, such as `/home/user_name/apps`. Note that such a folder needs to be added to the PATH in the `.bashrc` file. Then run `make install` from reduce/. 
  * [msms](https://ssbio.readthedocs.io/en/latest/instructions/msms.html): `conda install -c bioconda msms`. *For MacOS with M1 chip users*: you can follow [these instructions](https://ssbio.readthedocs.io/en/latest/instructions/msms.html).
- * [pytorch](https://pytorch.org/): `conda install pytorch -c pytorch`. Note that by default the CPU version of pytorch will be installed, but you can also customize that installation following the instructions on pytorch website.
+ * [DSSP 4](https://swift.cmbi.umcn.nl/gv/dssp/): 
+    * on ubuntu 22.04 or newer: `sudo apt-get install dssp`
+    * on older versions of ubuntu or on mac, or lacking sudo sudo priviliges: install from [here](https://github.com/pdb-redo/dssp), following the instructions listed.
+   * CPU only: `conda install pytorch==2.0.0 torchvision==0.15.0 torchaudio==2.0.0 cpuonly -c pytorch`
+   * if using GPU: `conda install pytorch==2.0.0 torchvision==0.15.0 torchaudio==2.0.0 pytorch-cuda=11.7 -c pytorch -c nvidia`
+ * [pytorch-geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html): `conda install pyg -c pyg`
+ * [Dependencies for pytorch geometric from wheels](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html#installation-from-wheels): `pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-${TORCH}+${CUDA}.html`. 
+    - Here, `${TORCH}` and `${CUDA}` should be replaced by the pytorch and CUDA versions installed. You can find these using:
+      - `python -c "import torch; print(torch.__version__)"` and
+      - `python -c "import torch; print(torch.version.cuda)"`
+    - For example: `https://data.pyg.org/whl/torch-2.0.0+cpu.html`
+ * Only if you have a MacOS with M1 chip, additional steps are needed:
+    * `conda install pytables`
+    * See [this](https://stackoverflow.com/questions/30145751/python3-cant-find-and-import-pyqt5) solution to install PyQt5 or run `conda install pyqt`
 
-### Deeprank-core Package
+### Deeprank-Core Package
 
-Once the dependencies installed, you can install the latest release of deeprank-core using the PyPi package manager:
+Once the dependencies installed, you can install the latest release of deeprankcore using the PyPi package manager:
 
 ```
 pip install deeprankcore
 ```
 
 You can get all the new developments by cloning the repo and installing the code with
 
 ```
 git clone https://github.com/DeepRank/deeprank-core
 cd deeprank-core
 pip install -e ./
 ```
 
- * For MacOS with M1 chip users only: see [this](https://stackoverflow.com/questions/30145751/python3-cant-find-and-import-pyqt5) solution if you run into problems with PyQt5 during deeprank-core installation.
-
 ## Documentation
 
-The documentation can be found [here](https://deeprankcore.rtfd.io/).
+More extensive and detailed documentation can be found [here](https://deeprankcore.rtfd.io/).
 
-## Getting Started
+## Quick start
 
-### Data generation
+### Data mapping
 
-The process of generating graphs takes as input `.pdb` files representing protein-protein structural complexes and the correspondent Position-Specific Scoring Matrices (PSSMs) in the form of `.pssm` files. Query objects describe how the graphs should be built.
+For each protein-protein complex, a query can be created and added to the `QueryCollection` object, to be processed later on. Different types of queries exist, based on the molecular resolution needed:
+- In a `ProteinProteinInterfaceResidueQuery` each node represents one amino acid residue
+- In a `ProteinProteinInterfaceAtomicQuery` each node represents one atom within the amino acid residues.
+A query takes as inputs:
+- a `.pdb` file, representing the protein-protein structural complex
+- the ids of the two chains composing the complex, and 
+- the correspondent Position-Specific Scoring Matrices (PSSMs), in the form of `.pssm` files.
 
 ```python
-from deeprankcore.preprocess import preprocess
-from deeprankcore.models.query import ProteinProteinInterfaceResidueQuery
-from deeprankcore.feature import bsa, pssm, amino_acid, biopython
+from deeprankcore.query import QueryCollection, ProteinProteinInterfaceResidueQuery
 
-feature_modules = [bsa, pssm, biopython, atomic_contact]
-
-queries = []
+queries = QueryCollection()
 
 # Append data points
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_1w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_1w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 0
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_2w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_2w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 1
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
-queries.append(ProteinProteinInterfaceResidueQuery(
-    pdb_path = "1ATN_3w.pdb",
+queries.add(ProteinProteinInterfaceResidueQuery(
+    pdb_path = "tests/data/pdb/1ATN/1ATN_3w.pdb",
     chain_id1 = "A",
     chain_id2 = "B",
     targets = {
         "binary": 0
     },
     pssm_paths = {
-        "A": "1ATN.A.pdb.pssm",
-        "B": "1ATN.B.pdb.pssm"
+        "A": "tests/data/pssm/1ATN/1ATN.A.pdb.pssm",
+        "B": "tests/data/pssm/1ATN/1ATN.B.pdb.pssm"
     }
 ))
 
-# Generate graphs and save them in hdf5 files
-# The default creates a number of hdf5 files equals to the cpu cores available
-# See deeprankcore.preprocess.preprocess for more details
-output_paths = preprocess(feature_modules, queries, "<output_folder>/<prefix_for_outputs>")
-
 ```
 
-The user is free to implement his/her own query class. Each implementation requires the `build_graph` method to be present.
+The user is free to implement a custom query class. Each implementation requires the `build` method to be present.
 
+The queries can then be processed into 3D-graphs only or both 3D-graphs and 3D-grids, depending on which kind of network will be used later for training. 
 
-### Data exploration
+```python
+from deeprankcore.features import components, conservation, contact, exposure, irc, surfacearea
+from deeprankcore.utils.grid import GridSettings, MapMethod
 
-As representative example, the following is the hdf5 structure generated by the previous phase for `1ATN_1w.pdb`, so for one single graph:
+feature_modules = [components, conservation, contact, exposure, irc, surfacearea]
 
-```bash
-└── ppi-1ATN_1w:A-B
-    ├── edge_features
-    │   ├── _index
-    │   ├── _name
-    │   ├── covalent
-    │   ├── distance
-    │   ├── electrostatic
-    │   ├── same_chain
-    │   ├── vanderwaals
-    ├── node_features
-    │   ├── _chain_id
-    │   ├── _name
-    │   ├── _position
-    │   ├── bsa
-    │   ├── hse
-    │   ├── info_content
-    │   ├── res_depth
-    │   ├── pssm
-    └── target_values
-        └── binary
+# Save data into 3D-graphs only
+hdf5_paths = queries.process(
+    "<output_folder>/<prefix_for_outputs>",
+    feature_modules = feature_modules)
 
+# Save data into 3D-graphs and 3D-grids
+hdf5_paths = queries.process(
+    "<output_folder>/<prefix_for_outputs>",
+    feature_modules = feature_modules,
+    grid_settings = GridSettings(
+        # the number of points on the x, y, z edges of the cube
+        points_counts = [20, 20, 20],
+        # x, y, z sizes of the box in Å
+        sizes = [1.0, 1.0, 1.0]),
+    grid_map_method = MapMethod.GAUSSIAN)
 ```
 
-This graph represents the interface between two proteins contained in the `.pdb` file at the residue level. Each graph generated by deeprank-core has the above structure (apart from the features and the target that are specified by the user). 
-
-It is always a good practice to first explore the data, and then make decision about splitting them in training, test and validation sets. For this purpose, users can either use [HDF5View](https://www.hdfgroup.org/downloads/hdfview/), a visual tool written in Java for browsing and editing HDF5 files, or Python packages such as [h5py](https://docs.h5py.org/en/stable/). Few examples for the latter:
+### Datasets
 
-```python
-import h5py
-from deeprankcore.domain.features import groups
+Data can be split in sets implementing custom splits according to the specific application. Assuming that the training, validation and testing ids have been chosen (keys of the HDF5 file/s), then the `DeeprankDataset` objects can be defined.
 
-with h5py.File("<hdf5_path.hdf5>", "r") as hdf5:
+#### GraphDataset
 
-    # List of all graphs in hdf5, each graph representing a ppi
-    ids = list(hdf5.keys())
+For training GNNs the user can create a `GraphDataset` instance:
 
-    # List of all node features
-    node_features = list(hdf5[ids[0]]["node_features"]) 
-    # List of all edge features
-    edge_features = list(hdf5[ids[0]]["edge_features"])
-    # List of all edge targets
-    targets = list(hdf5[ids[0]]["target_values"])
-
-    # BSA feature for ids[0], numpy.ndarray
-    node_feat_polarity = hdf5[ids[0]]["node_features"]["bsa"][:] 
-     # Electrostatic feature for ids[0], numpy.ndarray
-    edge_feat_electrostatic = hdf5[ids[0]]["edge_features"]["electrostatic"][:]
-```
-
-### Dataset(s)
-
-Data can be split in sets implementing custom splits according to the specific application. Utility splitting functions are currently under development.
+```python
+from deeprankcore.dataset import GraphDataset
 
-Assuming that the training, validation and testing ids have been chosen (keys of the hdf5 file), then the corresponding graphs can be saved in hdf5 files containing only references (external links) to the original one. For example:
+node_features = ["bsa", "res_depth", "hse", "info_content", "pssm"]
+edge_features = ["distance"]
+target = "binary"
 
-```python
-from deeprankcore.DataSet import save_hdf5_keys
+# Creating GraphDataset objects
+dataset_train = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = train_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
+)
+dataset_val = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = valid_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
 
-save_hdf5_keys("<original_hdf5_path.hdf5>", train_ids, "<train_hdf5_path.hdf5>")
-save_hdf5_keys("<original_hdf5_path.hdf5>", valid_ids, "<val_hdf5_path.hdf5>")
-save_hdf5_keys("<original_hdf5_path.hdf5>", test_ids, "<test_hdf5_path.hdf5>")
+)
+dataset_test = GraphDataset(
+    hdf5_path = hdf5_paths,
+    subset = test_ids, 
+    node_features = node_features,
+    edge_features = edge_features,
+    target = target
+)
 ```
 
-Now the HDF5DataSet objects can be defined:
+#### GridDataset
+
+For training CNNs the user can create a `GridDataset` instance:
 
 ```python
-from deeprankcore.DataSet import HDF5DataSet
+from deeprankcore.dataset import GridDataset
 
-node_features = ["bsa", "res_depth", "hse", "info_content", "pssm"]
-edge_features = ["distance"]
+features = ["bsa", "res_depth", "hse", "info_content", "pssm", "distance"]
+target = "binary"
 
-# Creating HDF5DataSet objects
-dataset_train = HDF5DataSet(
-    hdf5_path = "<train_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+# Creating GraphDataset objects
+dataset_train = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = train_ids, 
+    features = features,
+    target = target
 )
-dataset_val = HDF5DataSet(
-    hdf5_path = "<val_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+dataset_val = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = valid_ids, 
+    features = features,
+    target = target
 
 )
-dataset_test = HDF5DataSet(
-    hdf5_path = "<test_hdf5_path.hdf5>",
-    node_feature = node_features,
-    edge_feature = edge_features,
-    target = "binary"
+dataset_test = GridDataset(
+    hdf5_path = hdf5_paths,
+    subset = test_ids, 
+    features = features,
+    target = target
 )
 ```
 
 ### Training
 
-Let's define a Trainer instance, using for example of the already existing GNNs, GINet:
+Let's define a `Trainer` instance, using for example of the already existing `GINet`. Because `GINet` is a GNN, it requires a dataset instance of type `GraphDataset`.
 
 ```python
-from deeprankcore.Trainer import Trainer
-from deeprankcore.ginet import GINet
-from deeprankcore.models.metrics import OutputExporter, ScatterPlotExporter
-
-metrics_output_directory = "./metrics"
-metrics_exporters = [OutputExporter(metrics_output_directory)]
+from deeprankcore.trainer import Trainer
+from deeprankcore.neuralnets.gnn.naive_gnn import NaiveNetwork
 
 trainer = Trainer(
+    NaiveNetwork,
     dataset_train,
     dataset_val,
-    dataset_test,
-    GINet,
-    batch_size = 64,
-    metrics_exporters = metrics_exporters
+    dataset_test
 )
 
 ```
 
-Optimizer (`torch.optim.Adam` by default) and loss function can be defined by using dedicated functions:
+The same can be done using a CNN, for example `CnnClassification`. Here a dataset instance of type `GridDataset` is required.
 
 ```python
-import torch
-
-trainer.configure_optimizers(torch.optim.Adamax, lr = 0.001, weight_decay = 1e-04)
+from deeprankcore.trainer import Trainer
+from deeprankcore.neuralnets.cnn.model3d import CnnClassification
 
+trainer = Trainer(
+    CnnClassification,
+    dataset_train,
+    dataset_val,
+    dataset_test
+)
 ```
 
-Then the Trainer can be trained and tested, and the model can be saved:
+By default, the `Trainer` class creates the folder `./output` for storing predictions information collected later on during training and testing. `HDF5OutputExporter` is the exporter used by default, but the user can specify any other implemented exporter or implement a custom one.
 
-```python
-trainer.train(nepoch = 50, validate = True)
-trainer.test()
-trainer.save_model(filename = "<output_model_path.pth.tar>")
+Optimizer (`torch.optim.Adam` by default) and loss function can be defined by using dedicated functions:
 
-```
+```python
+import torch
 
+trainer.configure_optimizers(torch.optim.Adamax, lr = 0.001, weight_decay = 1e-04)
 
-#### Custom GNN
+```
 
-It is also possible to define new network architectures:
+Then the `Trainer` can be trained and tested; the best model in terms of validation loss is saved by default, and the user can modify so or indicate where to save it using the `train()` method parameter `filename`.
 
 ```python
-import torch 
-
-def normalized_cut_2d(edge_index, pos):
-    row, col = edge_index
-    edge_attr = torch.norm(pos[row] - pos[col], p=2, dim=1)
-    return normalized_cut(edge_index, edge_attr, num_nodes=pos.size(0))
-
-class CustomNet(torch.nn.Module):
-    def __init__(self):
-        super(Net, self).__init__()
-        self.conv1 = SplineConv(d.num_features, 32, dim=2, kernel_size=5)
-        self.conv2 = SplineConv(32, 64, dim=2, kernel_size=5)
-        self.fc1 = torch.nn.Linear(64, 128)
-        self.fc2 = torch.nn.Linear(128, 1)
-
-    def forward(self, data):
-        data.x = F.elu(self.conv1(data.x, data.edge_index, data.edge_attr))
-        weight = normalized_cut_2d(data.edge_index, data.pos)
-        cluster = graclus(data.edge_index, weight)
-        data = max_pool(cluster, data)
-
-        data.x = F.elu(self.conv2(data.x, data.edge_index, data.edge_attr))
-        weight = normalized_cut_2d(data.edge_index, data.pos)
-        cluster = graclus(data.edge_index, weight)
-        x, batch = max_pool_x(cluster, data.x, data.batch)
-
-        x = scatter_mean(x, batch, dim=0)
-        x = F.elu(self.fc1(x))
-        x = F.dropout(x, training=self.training)
-        return F.log_softmax(self.fc2(x), dim=1)
-
-trainer = Trainer(
-    dataset_train,
-    dataset_val,
-    dataset_test,
-    CustomNet,
+trainer.train(
+    nepoch = 50,
     batch_size = 64,
-    metrics_exporters = metrics_exporters
-)
-
-trainer.train(nepoch=50)
+    validate = True,
+    filename = "<my_folder/model.pth.tar>")
+trainer.test()
 
 ```
 
 ## h5x support
 
-After installing  `h5xplorer`  (https://github.com/DeepRank/h5xplorer), you can execute the python file `deeprankcore/h5x/h5x.py` to explorer the connection graph used by deeprank-core. The context menu (right click on the name of the structure) allows to automatically plot the graphs using `plotly` as shown below.
-
-![alt-text](./h5_deeprankcore.png)
-
-## For the developers
+After installing  `h5xplorer`  (https://github.com/DeepRank/h5xplorer), you can execute the python file `deeprankcore/h5x/h5x.py` to explorer the connection graph used by deeprankcore. The context menu (right click on the name of the structure) allows to automatically plot the graphs using `plotly`.
 
-### Software release
+## Package development
 
-Before creating a new package release, make sure to have updated all version strings in the source code. An easy way to do it is to run `bump2version [part]` from command line after having installed [bump2version](https://pypi.org/project/bump2version/) on your local environment. Instead of `[part]`, type the part of the version to increase, e.g. minor. The settings in `.bumpversion.cfg` will take care of updating all the files containing version strings. 
+- Branching
+  - When creating a new branch, please use the following convention: `<issue_number>_<description>_<author_name>`.
+- Pull Requests
+  - When creating a pull request, please use the following convention: `<type>: <description>`. Example _types_ are `fix:`, `feat:`, `build:`, `chore:`, `ci:`, `docs:`, `style:`, `refactor:`, `perf:`, `test:`, and others based on the [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines).
+- Software release
+  - Before creating a new package release, make sure to have updated all version strings in the source code. An easy way to do it is to run `bump2version [part]` from command line after having installed [bump2version](https://pypi.org/project/bump2version/) on your local environment. Instead of `[part]`, type the part of the version to increase, e.g. minor. The settings in `.bumpversion.cfg` will take care of updating all the files containing version strings.
```

### Comparing `deeprankcore-1.0.0/setup.cfg` & `deeprankcore-2.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [metadata]
 name = deeprankcore
 authors = [
-	{ name = "Giulia Crocioni", email = "g.crocioni@esciencecenter.nl" },
+	{ name = "Giulia Crocioni", email = "g.crocioni@esciencecenter.nl"},
 	{ name = "Coos Baakman", email = "coos.baakman@radboudumc.nl"},
+	{ name = "Dani Bodor", email = "d.bodor@esciencecenter.nl"},
 	{ name = "Daniel Rademaker"},
 	{ name = "Gayatri Ramakrishnan"},
 	{ name = "Sven van der Burg"},
 	{ name = "Li Xue"},
 	{ name = "Daniil Lepikhov"},
 	]
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-description = deeprank-core allows to train graph neural networks to classify protein-protein interface with a greater flexibility for the user.
+description = deeprankcore allows to train graph neural networks to classify protein-protein interface with a greater flexibility for the user.
 keywords = 
 	graph neural network
 	protein-protein interface
 	pytorch
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Bug Tracker = https://github.com/DeepRank/deeprank-core/issues
 url = https://github.com/DeepRank/deeprank-core
-version = 1.0.0
+version = 2.0.0
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
 python_requires = >= 3.9
 install_requires = 
@@ -40,37 +41,33 @@
 	h5py >= 3.6.0
 	h5xplorer
 	networkx >= 2.6.3
 	matplotlib >= 3.5.1
 	pdb2sql >= 0.5.1
 	scikit-learn >= 1.0.2
 	chart-studio >= 1.1.0
-	biopython >= 1.79
+	biopython >= 1.81
 	python-louvain >= 0.16
 	markov-clustering >= 0.0.6.dev0
 	tqdm >= 4.63.0
-	freesasa >= 2.1.0
+	freesasa == 2.1.0
 	tensorboard >= 2.9.0
 	protobuf <= 3.20.1
-	torch-scatter >= 2.0.6
-	torch-sparse >= 0.6.13
-	torch-cluster >= 1.6.0
-	torch-spline-conv >= 1.2.1
-	torch-geometric >= 2.0.4
 
 [options.extras_require]
 dev = 
 	yapf
 	isort
 doc = 
 	recommonmark
 	sphinx
 	sphinx_rtd_theme
 test = 
-	prospector[with_pyroma]
+	pylint <= 2.15.3
+	prospector[with_pyroma] <= 1.7.7
 	bump2version
 	coverage
 	pycodestyle
 	pytest
 	pytest-cov
 	pytest-runner
 	coveralls
```

