# Comparing `tmp/matgl-0.3.0.tar.gz` & `tmp/matgl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.3.0.tar", last modified: Sun May  7 20:32:51 2023, max compression
+gzip compressed data, was "matgl-0.4.0.tar", last modified: Tue Jun  6 23:35:35 2023, max compression
```

## Comparing `matgl-0.3.0.tar` & `matgl-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.781227 matgl-0.3.0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.3.0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     8114 2023-05-07 20:32:51.781087 matgl-0.3.0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     6964 2023-05-07 18:00:44.000000 matgl-0.3.0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.774402 matgl-0.3.0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      128 2023-05-07 20:31:54.000000 matgl-0.3.0/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.775451 matgl-0.3.0/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.3.0/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3574 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     2819 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.775967 matgl-0.3.0/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.3.0/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15713 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5404 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.776732 matgl-0.3.0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.3.0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5323 2023-05-02 13:08:40.000000 matgl-0.3.0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      551 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11083 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.777668 matgl-0.3.0/matgl/graph/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.3.0/matgl/graph/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4907 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/tests/test_compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     5528 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/tests/test_converters.py
--rw-r--r--   0 shyue      (501) staff       (20)     7995 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/tests/test_data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.779068 matgl-0.3.0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      551 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2099 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3586 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2168 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3336 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16489 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3961 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3726 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.779481 matgl-0.3.0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      158 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11793 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)    12277 2023-05-07 18:28:45.000000 matgl-0.3.0/matgl/models/_megnet.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.780836 matgl-0.3.0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.3.0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      809 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    17696 2023-05-03 17:18:57.000000 matgl-0.3.0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)     1916 2023-05-07 18:28:45.000000 matgl-0.3.0/matgl/utils/remote.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.3.0/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.775219 matgl-0.3.0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     8114 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      972 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       10 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     3117 2023-05-07 18:00:44.000000 matgl-0.3.0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-05-07 20:32:51.781270 matgl-0.3.0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2074 2023-05-02 13:08:40.000000 matgl-0.3.0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.995392 matgl-0.4.0/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-04-22 15:15:07.000000 matgl-0.4.0/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     7749 2023-06-06 23:35:35.995156 matgl-0.4.0/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     6552 2023-06-06 21:45:12.000000 matgl-0.4.0/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.988373 matgl-0.4.0/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      128 2023-06-06 23:32:20.000000 matgl-0.4.0/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.989387 matgl-0.4.0/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:14:12.000000 matgl-0.4.0/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3959 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2768 2023-05-08 21:40:46.000000 matgl-0.4.0/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.990024 matgl-0.4.0/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:14:12.000000 matgl-0.4.0/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15940 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5317 2023-05-31 00:31:01.000000 matgl-0.4.0/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.991109 matgl-0.4.0/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-04-22 15:15:07.000000 matgl-0.4.0/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5280 2023-05-31 00:31:01.000000 matgl-0.4.0/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11012 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.991707 matgl-0.4.0/matgl/graph/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:22.000000 matgl-0.4.0/matgl/graph/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/tests/test_compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/tests/test_converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/tests/test_data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.993134 matgl-0.4.0/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2047 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3573 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2247 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6123 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3572 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16522 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3976 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3691 2023-06-06 23:32:04.000000 matgl-0.4.0/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.993667 matgl-0.4.0/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      167 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10127 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9613 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/models/_megnet.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.994830 matgl-0.4.0/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-04-22 15:15:07.000000 matgl-0.4.0/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      809 2023-05-08 21:40:46.000000 matgl-0.4.0/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6638 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17730 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-04-22 15:15:07.000000 matgl-0.4.0/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    12203 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.989151 matgl-0.4.0/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     7749 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      992 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       46 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2639 2023-06-06 21:45:12.000000 matgl-0.4.0/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-06 23:35:35.995441 matgl-0.4.0/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2144 2023-06-06 21:45:12.000000 matgl-0.4.0/setup.py
```

### Comparing `matgl-0.3.0/LICENSE` & `matgl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.3.0/PKG-INFO` & `matgl-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.3.0
+Version: 0.4.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -16,152 +16,151 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+Provides-Extra: munch
+Provides-Extra: pymatgen
 License-File: LICENSE
 
+# matGL
+
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
-# Table of Contents
-* [Introduction](#introduction)
-* [Status](#status)
-* [Architectures](#architectures)
-* [Installation](#installation)
-* [Usage](#usage)
-* [Documentation](#documentation)
-* [References](#references)
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Status](#status)
+- [Architectures](#architectures)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Docs](#docs)
+- [References](#references)
 
-<a name="introduction"></a>
-# Introduction
+## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials. Mathematical graphs are a natural
 representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been shown
 to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
 and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
 The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
 implemented in TensorFlow.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
-<a name="status"></a>
-# Status
+## Status
 
 - Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
 - Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
 
-<a name="architectures"></a>
-# Architectures
+## Architectures
 
-## MEGNet
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MEGNet.png?raw=true"  width="50%">
+## MEGNet
 
 The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
 learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
 array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
 Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
 (See "Learning properties of ordered and disordered materials from multi-fidelity data").
 
 Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
 attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet.png?raw=true"  width="50%">
-
 [M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
 incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation.
 
 As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
-  machine learning interatomic potentials (ML-IAPs). However, a key feature of a graph representation is its
+  machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
-  *universal IAP* that can work across the entire periodic table of the elements by training on relaxations performed
+  *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
   in the [Materials Project](http://materialsproject.org).
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
-  surrogate models for property predictions, achieving in many cases accuracies that better or similar to other
+  surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
-For detailed performance benchmarks, please refer to the publication in the [References](#references) section.
+For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
-<a name="installation"></a>
-# Installation
+## Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
 ```
 
 For the latest dev version, please clone this repo and install using:
 
 ```bash
 python setup.py -e .
 ```
 
-
-<a name="usage"></a>
-# Usage
+## Usage
 
 The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
-from matgl.models._megnet import MEGNet
+from matgl.models import MEGNet
 
-# load the pre-trained MEGNet model for formation energy model.
+## load the pre-trained MEGNet model for formation energy model.
 model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
-# This is the structure obtained from the Materials Project.
+## This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-eform = model.predict_structure(struct)
-print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
+e_form = model.predict_structure(struct)
+print(f"The predicted formation energy for CsCl is {float(e_form):5f} eV/atom.")
 ```
 
-A full example is in [here](examples/Using%20MEGNet%20Pre-trained%20Models%20for%20Property%20Predictions.ipynb).
+A full example is in [here](examples/Pre-trained%20MEGNet%20for%20Property%20Predictions.ipynb).
 
+## Docs
 
-<a name="documentation"></a>
-# Additional information
-- [Documentation Page](http://materialsvirtuallab.github.io/matgl)
-- [API documentation](https://materialsvirtuallab.github.io/matgl/modules.html)
+<http://materialsvirtuallab.github.io/matgl>
 
-<a name="references"></a>
-# References
+## References
 
 Please cite the following works:
 
 - MEGNet
+
     ```txt
     Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
     Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
     ```
+
 - Multi-fidelity MEGNet
+
     ```txt
     Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
     Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
     ```
+
 - M3GNet
+
     ```txt
     Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
     2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
     ```
 
-# Acknowledgements
+## Acknowledgments
 
 This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
 Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
```

### Comparing `matgl-0.3.0/README.md` & `matgl-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,143 +1,140 @@
+# matGL
+
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
-# Table of Contents
-* [Introduction](#introduction)
-* [Status](#status)
-* [Architectures](#architectures)
-* [Installation](#installation)
-* [Usage](#usage)
-* [Documentation](#documentation)
-* [References](#references)
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Status](#status)
+- [Architectures](#architectures)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Docs](#docs)
+- [References](#references)
 
-<a name="introduction"></a>
-# Introduction
+## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials. Mathematical graphs are a natural
 representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been shown
 to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
 and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
 The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
 implemented in TensorFlow.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
-<a name="status"></a>
-# Status
+## Status
 
 - Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
 - Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
 
-<a name="architectures"></a>
-# Architectures
+## Architectures
 
-## MEGNet
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MEGNet.png?raw=true"  width="50%">
+## MEGNet
 
 The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
 learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
 array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
 Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
 (See "Learning properties of ordered and disordered materials from multi-fidelity data").
 
 Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
 attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet.png?raw=true"  width="50%">
-
 [M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
 incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation.
 
 As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
-  machine learning interatomic potentials (ML-IAPs). However, a key feature of a graph representation is its
+  machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
-  *universal IAP* that can work across the entire periodic table of the elements by training on relaxations performed
+  *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
   in the [Materials Project](http://materialsproject.org).
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
-  surrogate models for property predictions, achieving in many cases accuracies that better or similar to other
+  surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
-For detailed performance benchmarks, please refer to the publication in the [References](#references) section.
+For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
-<a name="installation"></a>
-# Installation
+## Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
 ```
 
 For the latest dev version, please clone this repo and install using:
 
 ```bash
 python setup.py -e .
 ```
 
-
-<a name="usage"></a>
-# Usage
+## Usage
 
 The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
-from matgl.models._megnet import MEGNet
+from matgl.models import MEGNet
 
-# load the pre-trained MEGNet model for formation energy model.
+## load the pre-trained MEGNet model for formation energy model.
 model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
-# This is the structure obtained from the Materials Project.
+## This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-eform = model.predict_structure(struct)
-print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
+e_form = model.predict_structure(struct)
+print(f"The predicted formation energy for CsCl is {float(e_form):5f} eV/atom.")
 ```
 
-A full example is in [here](examples/Using%20MEGNet%20Pre-trained%20Models%20for%20Property%20Predictions.ipynb).
+A full example is in [here](examples/Pre-trained%20MEGNet%20for%20Property%20Predictions.ipynb).
 
+## Docs
 
-<a name="documentation"></a>
-# Additional information
-- [Documentation Page](http://materialsvirtuallab.github.io/matgl)
-- [API documentation](https://materialsvirtuallab.github.io/matgl/modules.html)
+<http://materialsvirtuallab.github.io/matgl>
 
-<a name="references"></a>
-# References
+## References
 
 Please cite the following works:
 
 - MEGNet
+
     ```txt
     Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
     Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
     ```
+
 - Multi-fidelity MEGNet
+
     ```txt
     Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
     Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
     ```
+
 - M3GNet
+
     ```txt
     Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
     2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
     ```
 
-# Acknowledgements
+## Acknowledgments
 
 This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
 Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
```

### Comparing `matgl-0.3.0/matgl/apps/pes.py` & `matgl-0.4.0/matgl/apps/pes.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 Implementation of Interatomic Potentials
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
-import torch.nn as nn
+from torch import nn
 from torch.autograd import grad
 
 from matgl.layers import AtomRef
+from matgl.models import M3GNet
 
 
 class Potential(nn.Module):
     """
     A class representing an interatomic potential.
     """
 
     def __init__(
         self,
-        model: nn.Module,
+        model: M3GNet,
+        data_mean: torch.tensor | None = None,
+        data_std: torch.tensor | None = None,
         element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
         calc_stresses: bool = True,
         calc_hessian: bool = False,
     ):
         """
         :param model: M3GNet model
@@ -33,38 +36,45 @@
         :param calc_hessian: Enable hessian calculations
         """
         super().__init__()
         self.model = model
         self.calc_forces = calc_forces
         self.calc_stresses = calc_stresses
         self.calc_hessian = calc_hessian
+        self.element_refs: AtomRef | None
         if element_refs is not None:
-            self.element_ref_calc = AtomRef(property_offset=element_refs)
-        self.element_refs = element_refs
+            self.element_refs = AtomRef(property_offset=element_refs)
+        else:
+            self.element_refs = None
+
+        self.data_mean = data_mean if data_mean is not None else torch.zeros(1)
+        self.data_std = data_std if data_std is not None else torch.ones(1)
 
     def forward(
         self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None
     ) -> tuple:
         """
         Args:
             g: DGL graph
             state_attr: State attrs
+            l_g: Line graph.
 
         Returns:
             energies, forces, stresses, hessian: torch.tensor
         """
         forces = torch.zeros(1)
         stresses = torch.zeros(1)
         hessian = torch.zeros(1)
         if self.calc_forces:
             g.ndata["pos"].requires_grad_(True)
-        total_energies = self.model(g=g, state_attr=state_attr, l_g=l_g)
+        total_energies = self.data_std * self.model(g=g, state_attr=state_attr, l_g=l_g) + self.data_mean
         if self.element_refs is not None:
-            property_offset = torch.squeeze(self.element_ref_calc(g))
+            property_offset = torch.squeeze(self.element_refs(g))
             total_energies += property_offset
+
         if self.calc_forces:
             grads = grad(
                 total_energies,
                 [g.ndata["pos"], g.edata["bond_vec"]],
                 grad_outputs=torch.ones_like(total_energies),
                 create_graph=True,
                 retain_graph=True,
```

### Comparing `matgl-0.3.0/matgl/config.py` & `matgl-0.4.0/matgl/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import os
 from pathlib import Path
 
 import numpy as np
 import torch
 
-# CWD = os.path.dirname(os.path.abspath(__file__))
 DEFAULT_ELEMENT_TYPES = (
     "H",
     "He",
     "Li",
     "Be",
     "B",
     "C",
```

### Comparing `matgl-0.3.0/matgl/ext/ase.py` & `matgl-0.4.0/matgl/ext/ase.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         Get a DGL graph from an input Structure.
 
         :param structure: pymatgen structure object
         :return:
             g: DGL graph
             state_attr: state features
         """
-
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
         Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
         atomic_number = np.array(atoms.get_atomic_numbers())
         lattice_matrix = np.ascontiguousarray(np.array(atoms.get_cell()), dtype=float)
         volume = atoms.get_volume()
@@ -121,29 +120,29 @@
     def __init__(
         self,
         potential: Potential,
         state_attr: torch.tensor = None,
         stress_weight: float = 1.0,
         **kwargs,
     ):
-        """
-
+        r"""
         Args:
             potential (Potential): m3gnet.models.Potential
+            state_attr (tensor): State attribute
             compute_stress (bool): whether to calculate the stress
             stress_weight (float): the stress weight.
-            **kwargs:
+            **kwargs: Kwargs pass through to super().__init__().
         """
         super().__init__(**kwargs)
         self.potential = potential
         self.compute_stress = potential.calc_stresses
         self.compute_hessian = potential.calc_hessian
         self.stress_weight = stress_weight
         self.state_attr = state_attr
-        self.element_types = potential.model.element_types
+        self.element_types = potential.model.element_types  # type: ignore
         self.cutoff = potential.model.cutoff
 
     def calculate(
         self,
         atoms: Atoms | None = None,
         properties: list | None = None,
         system_changes: list | None = None,
@@ -151,16 +150,14 @@
         """
         Args:
             atoms (ase.Atoms): ase Atoms object
             properties (list): list of properties to calculate
             system_changes (list): monitor which properties of atoms were
                 changed for new calculation. If not, the previous calculation
                 results will be loaded.
-        Returns:
-
         """
         properties = properties or ["energy"]
         system_changes = system_changes or all_changes
         super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
         graph, state_attr_default = Atoms2Graph(self.element_types, self.cutoff).get_graph(atoms)  # type: ignore
         if self.state_attr is not None:
             energies, forces, stresses, hessians = self.potential(graph, self.state_attr)
@@ -187,25 +184,23 @@
         potential: Potential = None,
         state_attr: torch.tensor = None,
         optimizer: Optimizer | str = "FIRE",
         relax_cell: bool = True,
         stress_weight: float = 0.01,
     ):
         """
-
         Args:
-            potential (Potential): a M3GNet potential,
-                a str path to a saved model or a short name for saved model
+            potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
                 that comes with M3GNet distribution
+            state_attr (torch.tensor): State attr.
             optimizer (str or ase Optimizer): the optimization algorithm.
                 Defaults to "FIRE"
             relax_cell (bool): whether to relax the lattice cell
             stress_weight (float): the stress weight for relaxation
         """
-
         if isinstance(optimizer, str):
             optimizer_obj = OPTIMIZERS.get(optimizer, None)
         elif optimizer is None:
             raise ValueError("Optimizer cannot be None")
         else:
             optimizer_obj = optimizer
 
@@ -223,25 +218,24 @@
         fmax: float = 0.1,
         steps: int = 500,
         traj_file: str = None,
         interval=1,
         verbose=False,
         **kwargs,
     ):
-        """
-
+        r"""
         Args:
             atoms (Atoms): the atoms for relaxation
             fmax (float): total force tolerance for relaxation convergence.
                 Here fmax is a sum of force and stress forces
             steps (int): max number of steps for relaxation
             traj_file (str): the trajectory file for saving
             interval (int): the step interval for saving the trajectories
-            **kwargs:
-        Returns:
+            verbose (bool): Whether to have verbose output.
+            **kwargs: Kwargs pass-through to optimizer.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = self.ase_adaptor.get_atoms(atoms)
         atoms.set_calculator(self.calculator)
         stream = sys.stdout if verbose else io.StringIO()
         with contextlib.redirect_stdout(stream):
             obs = TrajectoryObserver(atoms)
@@ -339,33 +333,32 @@
         compressibility_au: float | None = None,
         trajectory: str | Trajectory | None = None,
         logfile: str | None = None,
         loginterval: int = 1,
         append_trajectory: bool = False,
     ):
         """
-
         Args:
             atoms (Atoms): atoms to run the MD
             potential (Potential): potential for calculating the energy, force,
                 stress of the atoms
+            state_attr (torch.tensor): State attr.
             ensemble (str): choose from 'nvt' or 'npt'. NPT is not tested,
                 use with extra caution
             temperature (float): temperature for MD simulation, in K
             timestep (float): time step in fs
             pressure (float): pressure in eV/A^3
             taut (float): time constant for Berendsen temperature coupling
             taup (float): time constant for pressure coupling
             compressibility_au (float): compressibility of the material in A^3/eV
             trajectory (str or Trajectory): Attach trajectory object
             logfile (str): open this file for recording MD outputs
             loginterval (int): write to log file every interval steps
             append_trajectory (bool): Whether to append to prev trajectory
         """
-
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         self.atoms = atoms
         self.atoms.set_calculator(M3GNetCalculator(potential=potential, state_attr=state_attr))
 
         if taut is None:
             taut = 100 * timestep * units.fs
@@ -382,19 +375,17 @@
                 logfile=logfile,
                 loginterval=loginterval,
                 append_trajectory=append_trajectory,
             )
 
         elif ensemble.lower() == "npt":
             """
-
             NPT ensemble default to Inhomogeneous_NPTBerendsen thermo/barostat
             This is a more flexible scheme that fixes three angles of the unit
             cell but allows three lattice parameter to change independently.
-
             """
 
             self.dyn = Inhomogeneous_NPTBerendsen(
                 self.atoms,
                 timestep * units.fs,
                 temperature_K=temperature,
                 pressure_au=pressure,
@@ -451,15 +442,12 @@
         self.dyn.run(steps)
 
     def set_atoms(self, atoms: Atoms):
         """
         Set new atoms to run MD
         Args:
             atoms (Atoms): new atoms for running MD
-
-        Returns:
-
         """
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.set_calculator(calculator)
```

### Comparing `matgl-0.3.0/matgl/ext/pymatgen.py` & `matgl-0.4.0/matgl/ext/pymatgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,9 +139,8 @@
         g.edata["pbc_offset"] = torch.tensor(images)
         g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
         g.ndata["attr"] = tensor(Z)
         g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in structure]))
         g.ndata["pos"] = tensor(cart_coords)
         g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
-        g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
```

### Comparing `matgl-0.3.0/matgl/graph/compute.py` & `matgl-0.4.0/matgl/graph/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     g: DGL graph
 
     Returns:
     bond_vec (torch.tensor): bond distance between two atoms
     bond_dist (torch.tensor): vector from src node to dst node
     """
     bond_vec = torch.zeros(g.num_edges(), 3)
-    bond_dist = torch.zeros(g.num_edges())
     bond_vec[:, :] = (
         g.ndata["pos"][g.edges()[1][:].long(), :]
         + torch.squeeze(torch.matmul(g.edata["pbc_offset"].unsqueeze(1), torch.squeeze(g.edata["lattice"])))
         - g.ndata["pos"][g.edges()[0][:].long(), :]
     )
 
     bond_dist = torch.norm(bond_vec, dim=1)
```

### Comparing `matgl-0.3.0/matgl/graph/converters.py` & `matgl-0.4.0/matgl/graph/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 
         Args:
             structure: Input structure or molecule.
 
         Returns:
             DGLGraph object, state_attr
         """
-        pass
```

### Comparing `matgl-0.3.0/matgl/graph/data.py` & `matgl-0.4.0/matgl/graph/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """
 Tools to construct a data for DGL grphs
 """
 from __future__ import annotations
 
 import json
 import os
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import dgl
 import numpy as np
 import torch
 from dgl.data import DGLDataset
 from dgl.data.utils import load_graphs, save_graphs
 from dgl.dataloading import GraphDataLoader
 from tqdm import trange
 
 from matgl.graph.compute import compute_pair_vector_and_distance, create_line_graph
-from matgl.graph.converters import GraphConverter
 from matgl.layers import BondExpansion
 
+if TYPE_CHECKING:
+    from matgl.graph.converters import GraphConverter
 
-def _collate_fn(batch):
+
+def collate_fn(batch):
     """
     Merge a list of dgl graphs to form a batch
     """
     graphs, labels, state_attr = map(list, zip(*batch))
     g = dgl.batch(graphs)
     labels = torch.tensor(labels, dtype=torch.float32)
     state_attr = torch.stack(state_attr)
     return g, labels, state_attr
 
 
-def _collate_fn_efs(batch):
+def collate_fn_efs(batch):
     """
     Merge a list of dgl graphs to form a batch
     """
     graphs, line_graphs, state_attr, energies, forces, stresses = map(list, zip(*batch))
     g = dgl.batch(graphs)
     l_g = dgl.batch(line_graphs)
     e = torch.tensor(energies, dtype=torch.float32)
@@ -89,16 +91,15 @@
             batch_size=batch_size,
             shuffle=False,
             collate_fn=collate_fn,
             num_workers=num_workers,
             pin_memory=pin_memory,
         )
         return train_loader, val_loader, test_loader
-    else:
-        return train_loader, val_loader
+    return train_loader, val_loader
 
 
 class MEGNetDataset(DGLDataset):
     """
     Create a dataset including dgl graphs
     """
 
@@ -115,15 +116,15 @@
         name: str = "MEGNETDataset",
         graph_labels: list | None = None,
     ):
         """
         Args:
         structures: Pymatgen strutcure
         labels: property values
-        label: label name
+        label_name: label name
         converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
         initial: initial distance for Gaussian expansions
         final: final distance for Gaussian expansions
         num_centers: number of Gaussian functions
         width: width of Gaussian functions
         name: Name of dataset
         graph_labels: graph attributes either integers and floating point numbers
@@ -226,21 +227,21 @@
         threebody_cutoff: float,
         name="M3GNETDataset",
         graph_labels: list | None = None,
     ):
         """
         Args:
         structures: Pymatgen strutcure
-        labels: property values
-        label: label name
-        converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
-        initial: initial distance for Gaussian expansions
-        final: final distance for Gaussian expansions
-        num_centers: number of Gaussian functions
-        width: width of Gaussian functions
+        energies: Target energies
+        forces: Target forces
+        stresses: Target stresses
+        converter: dgl graph converter
+        threebody_cutoff: cutoff for three body
+        name: name of dataset
+        graph_labels: state attributes
         """
         self.converter = converter
         self.structures = structures
         self.energies = energies
         self.forces = forces
         self.threebody_cutoff = threebody_cutoff
         self.stresses = np.zeros(len(self.energies)) if stresses is None else stresses
```

### Comparing `matgl-0.3.0/matgl/graph/tests/test_compute.py` & `matgl-0.4.0/matgl/graph/tests/test_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,29 +57,29 @@
 
 
 class TestCompute(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         cls.s1 = Structure(Lattice.cubic(3.17), ["Mo", "Mo"], [[0.01, 0, 0], [0.5, 0.5, 0.5]])
         element_types = get_element_list([cls.s1])
-        p2g = Structure2Graph(element_types=element_types, cutoff=5.0)
+        p2g = Structure2Graph(element_types=element_types, cutoff=5.0)  # type: ignore
         graph, state = p2g.get_graph(cls.s1)
         cls.g1 = graph
         cls.state1 = state
 
         coords = [
             [0.000000, 0.000000, 0.000000],
             [0.000000, 0.000000, 1.089000],
             [1.026719, 0.000000, -0.363000],
             [-0.513360, -0.889165, -0.363000],
             [-0.513360, 0.889165, -0.363000],
         ]
         methane = Molecule(["C", "H", "H", "H", "H"], coords)
         element_types = get_element_list([methane])
-        p2g = Molecule2Graph(element_types=element_types, cutoff=2.0)
+        p2g = Molecule2Graph(element_types=element_types, cutoff=2.0)  # type: ignore
         graph, state = p2g.get_graph(methane)
         cls.g2 = graph
         cls.state2 = state
 
     def test_compute_pair_vector(self):
         bv, bd = compute_pair_vector_and_distance(self.g1)
         self.g1.edata["bond_vec"] = bv
```

### Comparing `matgl-0.3.0/matgl/graph/tests/test_converters.py` & `matgl-0.4.0/matgl/graph/tests/test_converters.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,90 +24,90 @@
             [-0.513360, 0.889165, -0.363000],
         ]
         methane = Molecule(["C", "H", "H", "H", "H"], coords)
         element_types = get_element_list([methane])
         p2g = Molecule2Graph(element_types=element_types, cutoff=1.5)
         graph, state = p2g.get_graph(methane)
         # check the number of nodes
-        self.assertTrue(np.allclose(graph.num_nodes(), 5))
+        assert np.allclose(graph.num_nodes(), 5)
         # check the number of edges
-        self.assertTrue(np.allclose(graph.num_edges(), 8))
+        assert np.allclose(graph.num_edges(), 8)
         # check the src_ids
-        self.assertTrue(np.allclose(graph.edges()[0].numpy(), [0, 0, 0, 0, 1, 2, 3, 4]))
+        assert np.allclose(graph.edges()[0].numpy(), [0, 0, 0, 0, 1, 2, 3, 4])
         # check the dst_ids
-        self.assertTrue(np.allclose(graph.edges()[1].numpy(), [1, 2, 3, 4, 0, 0, 0, 0]))
+        assert np.allclose(graph.edges()[1].numpy(), [1, 2, 3, 4, 0, 0, 0, 0])
         # check the atomic features of atom C
-        self.assertTrue(np.allclose(graph.ndata["attr"][0], [0, 1]))
+        assert np.allclose(graph.ndata["attr"][0], [0, 1])
         # check the atomic features of atom H
-        self.assertTrue(np.allclose(graph.ndata["attr"][1], [1, 0]))
+        assert np.allclose(graph.ndata["attr"][1], [1, 0])
         # check the shape of state features
-        self.assertTrue(np.allclose(len(state), 2))
+        assert np.allclose(len(state), 2)
         # check the value of state features
-        self.assertTrue(np.allclose(state, [3.208492, 0.8]))
+        assert np.allclose(state, [3.208492, 0.8])
         # check the position of atom 0
-        self.assertTrue(np.allclose(graph.ndata["pos"][0], [0.000000, 0.000000, 0.000000]))
+        assert np.allclose(graph.ndata["pos"][0], [0.0, 0.0, 0.0])
 
     def test_get_graph_from_structure(self):
         structure_LiFePO4 = self.get_structure("LiFePO4")
         element_types = get_element_list([structure_LiFePO4])
         p2g = Structure2Graph(element_types=element_types, cutoff=4.0)
         graph, state = p2g.get_graph(structure_LiFePO4)
         # check the number of nodes
-        self.assertTrue(np.allclose(graph.num_nodes(), structure_LiFePO4.num_sites))
+        assert np.allclose(graph.num_nodes(), structure_LiFePO4.num_sites)
         # check the atomic feature of atom 0
-        self.assertTrue(np.allclose(graph.ndata["attr"][0].numpy(), [1, 0, 0, 0]))
+        assert np.allclose(graph.ndata["attr"][0].numpy(), [1, 0, 0, 0])
         # check the atomic feature of atom 4
-        self.assertTrue(np.allclose(graph.ndata["attr"][4].numpy(), [0, 0, 0, 1]))
+        assert np.allclose(graph.ndata["attr"][4].numpy(), [0, 0, 0, 1])
         # check the number of bonds
-        self.assertTrue(np.allclose(graph.num_edges(), 704))
+        assert np.allclose(graph.num_edges(), 704)
         # check the state features
-        self.assertTrue(np.allclose(state, [0.0, 0.0]))
+        assert np.allclose(state, [0.0, 0.0])
         structure_BaTiO3 = Structure.from_prototype("perovskite", ["Ba", "Ti", "O"], a=4.04)
         element_types = get_element_list([structure_BaTiO3])
         p2g = Structure2Graph(element_types=element_types, cutoff=4.0)
         graph, state = p2g.get_graph(structure_BaTiO3)
         # check the number of nodes
-        self.assertTrue(np.allclose(graph.num_nodes(), structure_BaTiO3.num_sites))
+        assert np.allclose(graph.num_nodes(), structure_BaTiO3.num_sites)
         # check the atomic features of atom 0
-        self.assertTrue(np.allclose(graph.ndata["attr"][0], [0, 0, 1]))
+        assert np.allclose(graph.ndata["attr"][0], [0, 0, 1])
         # check the atomic features of atom 1
-        self.assertTrue(np.allclose(graph.ndata["attr"][1], [0, 1, 0]))
+        assert np.allclose(graph.ndata["attr"][1], [0, 1, 0])
         # check the number of edges
-        self.assertTrue(np.allclose(graph.num_edges(), 76))
+        assert np.allclose(graph.num_edges(), 76)
         # check the state features
-        self.assertTrue(np.allclose(state, [0.0, 0.0]))
+        assert np.allclose(state, [0.0, 0.0])
         # check the position of atom 0
-        self.assertTrue(np.allclose(graph.ndata["pos"][0], [0.0, 0.0, 0.0]))
+        assert np.allclose(graph.ndata["pos"][0], [0.0, 0.0, 0.0])
         # check the pbc offset from node 0 to image atom 6
-        self.assertTrue(np.allclose(graph.edata["pbc_offset"][0], [-1, -1, -1]))
-        # cheeck the lattice vector
-        self.assertTrue(np.allclose(graph.edata["lattice"][0], [[4.04, 0.0, 0.0], [0.0, 4.04, 0.0], [0.0, 0.0, 4.04]]))
+        assert np.allclose(graph.edata["pbc_offset"][0], [-1, -1, -1])
+        # check the lattice vector
+        assert np.allclose(graph.edata["lattice"][0], [[4.04, 0.0, 0.0], [0.0, 4.04, 0.0], [0.0, 0.0, 4.04]])
         # check the volume
-        self.assertTrue(np.allclose(graph.ndata["volume"][0], [65.939264]))
+        assert np.allclose(graph.ndata["volume"][0], [65.939264])
 
     def test_get_graph_from_atoms(self):
         structure_LiFePO4 = self.get_structure("LiFePO4")
         element_types = get_element_list([structure_LiFePO4])
         adaptor = AseAtomsAdaptor()
         structure_ase = adaptor.get_atoms(structure_LiFePO4)
         p2g = Atoms2Graph(element_types=element_types, cutoff=4.0)
         graph, state = p2g.get_graph(structure_ase)
         # check the number of nodes
-        self.assertTrue(np.allclose(graph.num_nodes(), len(structure_ase.get_atomic_numbers())))
+        assert np.allclose(graph.num_nodes(), len(structure_ase.get_atomic_numbers()))
         # check the atomic feature of atom 0
-        self.assertTrue(np.allclose(graph.ndata["attr"][0].numpy(), [1, 0, 0, 0]))
+        assert np.allclose(graph.ndata["attr"][0].numpy(), [1, 0, 0, 0])
         # check the atomic feature of atom 4
-        self.assertTrue(np.allclose(graph.ndata["attr"][4].numpy(), [0, 0, 0, 1]))
+        assert np.allclose(graph.ndata["attr"][4].numpy(), [0, 0, 0, 1])
         # check the number of bonds
-        self.assertTrue(np.allclose(graph.num_edges(), 704))
+        assert np.allclose(graph.num_edges(), 704)
         # check the state features
-        self.assertTrue(np.allclose(state, [0.0, 0.0]))
+        assert np.allclose(state, [0.0, 0.0])
 
     def test_get_element_list(self):
         cscl = Structure.from_spacegroup("Pm-3m", Lattice.cubic(3), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
         naf = Structure.from_spacegroup("Pm-3m", Lattice.cubic(3), ["Na", "F"], [[0, 0, 0], [0.5, 0.5, 0.5]])
         elem_list = get_element_list([cscl, naf])
-        self.assertEqual(elem_list, ("F", "Na", "Cl", "Cs"))
+        assert elem_list == ("F", "Na", "Cl", "Cs")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `matgl-0.3.0/matgl/graph/tests/test_data.py` & `matgl-0.4.0/matgl/graph/tests/test_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pymatgen.util.testing import PymatgenTest
 
 from matgl.ext.pymatgen import Molecule2Graph, Structure2Graph, get_element_list
 from matgl.graph.data import (
     M3GNetDataset,
     MEGNetDataset,
     MGLDataLoader,
-    _collate_fn,
+    collate_fn,
 )
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class DatasetTest(PymatgenTest):
     def test_megnet_dataset(self):
@@ -26,19 +26,19 @@
         structures = [s1, s2]
         label = [-1.0, 2.0]
         element_types = get_element_list([s1, s2])
         cry_graph = Structure2Graph(element_types=element_types, cutoff=4.0)
         dataset = MEGNetDataset(structures=structures, converter=cry_graph, labels=label, label_name="label")
         g1, label1, state1 = dataset[0]
         g2, label2, state2 = dataset[1]
-        self.assertTrue(label1 == label[0])
-        self.assertTrue(g1.num_edges() == cry_graph.get_graph(s1)[0].num_edges())
-        self.assertTrue(g1.num_nodes() == cry_graph.get_graph(s1)[0].num_nodes())
-        self.assertTrue(g2.num_edges() == cry_graph.get_graph(s2)[0].num_edges())
-        self.assertTrue(g2.num_nodes() == cry_graph.get_graph(s2)[0].num_nodes())
+        assert label1 == label[0]
+        assert g1.num_edges() == cry_graph.get_graph(s1)[0].num_edges()
+        assert g1.num_nodes() == cry_graph.get_graph(s1)[0].num_nodes()
+        assert g2.num_edges() == cry_graph.get_graph(s2)[0].num_edges()
+        assert g2.num_nodes() == cry_graph.get_graph(s2)[0].num_nodes()
 
     def test_megnet_dataset_for_mol(self):
         coords = [
             [0.000000, 0.000000, 0.000000],
             [0.000000, 0.000000, 1.089000],
             [1.026719, 0.000000, -0.363000],
             [-0.513360, -0.889165, -0.363000],
@@ -50,19 +50,19 @@
         label = [1.0, 2.0]
         structures = [methane, methane]
         dataset = MEGNetDataset(
             structures=structures, converter=mol_graph, labels=label, label_name="label", name="MolDataset"
         )
         g1, label1, state1 = dataset[0]
         g2, label2, state2 = dataset[1]
-        self.assertTrue(label1 == label[0])
-        self.assertTrue(g1.num_edges() == mol_graph.get_graph(methane)[0].num_edges())
-        self.assertTrue(g1.num_nodes() == mol_graph.get_graph(methane)[0].num_nodes())
-        self.assertTrue(g2.num_edges() == mol_graph.get_graph(methane)[0].num_edges())
-        self.assertTrue(g2.num_nodes() == mol_graph.get_graph(methane)[0].num_nodes())
+        assert label1 == label[0]
+        assert g1.num_edges() == mol_graph.get_graph(methane)[0].num_edges()
+        assert g1.num_nodes() == mol_graph.get_graph(methane)[0].num_nodes()
+        assert g2.num_edges() == mol_graph.get_graph(methane)[0].num_edges()
+        assert g2.num_nodes() == mol_graph.get_graph(methane)[0].num_nodes()
 
     def test_m3gnet_dataset(self):
         s1 = self.get_structure("LiFePO4")
         s2 = self.get_structure("BaNiO3")
         structures = [s1, s2]
         energies = [-1.0, 2.0]
         forces = [np.zeros((28, 3)).tolist(), np.zeros((10, 3)).tolist()]
@@ -75,21 +75,21 @@
             threebody_cutoff=4.0,
             energies=energies,
             forces=forces,
             stresses=stresses,
         )
         g1, l_g1, state1, energies_g1, forces_g1, stresses_g1 = dataset[0]
         g2, l_g2, state2, energies_g2, forces_g2, stresses_g2 = dataset[1]
-        self.assertTrue(energies_g1 == energies[0])
-        self.assertTrue(g1.num_edges() == cry_graph.get_graph(s1)[0].num_edges())
-        self.assertTrue(g1.num_nodes() == cry_graph.get_graph(s1)[0].num_nodes())
-        self.assertTrue(g2.num_edges() == cry_graph.get_graph(s2)[0].num_edges())
-        self.assertTrue(g2.num_nodes() == cry_graph.get_graph(s2)[0].num_nodes())
-        self.assertTrue(np.shape(forces_g1)[0], 28)
-        self.assertTrue(np.shape(forces_g2)[0], 10)
+        assert energies_g1 == energies[0]
+        assert g1.num_edges() == cry_graph.get_graph(s1)[0].num_edges()
+        assert g1.num_nodes() == cry_graph.get_graph(s1)[0].num_nodes()
+        assert g2.num_edges() == cry_graph.get_graph(s2)[0].num_edges()
+        assert g2.num_nodes() == cry_graph.get_graph(s2)[0].num_nodes()
+        assert np.shape(forces_g1)[0], 28
+        assert np.shape(forces_g2)[0], 10
 
     def test_megnet_dataloader(self):
         s1 = self.get_structure("LiFePO4")
         s2 = self.get_structure("BaNiO3")
         structures = [s1, s1, s1, s1, s1, s1, s1, s1, s1, s1, s2, s2, s2, s2, s2, s2, s2, s2, s2, s2]
         label = np.zeros(20)
         element_types = get_element_list([s1, s2])
@@ -101,21 +101,21 @@
             shuffle=True,
             random_state=42,
         )
         train_loader, val_loader, test_loader = MGLDataLoader(
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
-            collate_fn=_collate_fn,
+            collate_fn=collate_fn,
             batch_size=2,
             num_workers=1,
         )
-        self.assertTrue(len(train_loader) == 8)
-        self.assertTrue(len(val_loader) == 1)
-        self.assertTrue(len(test_loader) == 1)
+        assert len(train_loader) == 8
+        assert len(val_loader) == 1
+        assert len(test_loader) == 1
 
     def test_megnet_dataloader_for_mol(self):
         coords = [
             [0.000000, 0.000000, 0.000000],
             [0.000000, 0.000000, 1.089000],
             [1.026719, 0.000000, -0.363000],
             [-0.513360, -0.889165, -0.363000],
@@ -133,21 +133,21 @@
             shuffle=True,
             random_state=42,
         )
         train_loader, val_loader, test_loader = MGLDataLoader(
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
-            collate_fn=_collate_fn,
+            collate_fn=collate_fn,
             batch_size=2,
             num_workers=1,
         )
-        self.assertTrue(len(train_loader) == 3)
-        self.assertTrue(len(val_loader) == 1)
-        self.assertTrue(len(test_loader) == 1)
+        assert len(train_loader) == 3
+        assert len(val_loader) == 1
+        assert len(test_loader) == 1
 
     def test_m3gnet_dataloader(self):
         s1 = self.get_structure("LiFePO4")
         s2 = self.get_structure("BaNiO3")
         structures = [s1, s2, s1, s2, s1, s2, s1, s2, s1, s2, s1, s2, s1, s2, s1, s2, s1, s2, s1, s2]
         energies = np.zeros(20)
         f1 = np.zeros((28, 3)).tolist()
@@ -171,21 +171,21 @@
             shuffle=True,
             random_state=42,
         )
         train_loader, val_loader, test_loader = MGLDataLoader(
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
-            collate_fn=_collate_fn,
+            collate_fn=collate_fn,
             batch_size=2,
             num_workers=1,
         )
-        self.assertTrue(len(train_loader) == 8)
-        self.assertTrue(len(val_loader) == 1)
-        self.assertTrue(len(test_loader) == 1)
+        assert len(train_loader) == 8
+        assert len(val_loader) == 1
+        assert len(test_loader) == 1
 
     @classmethod
     def tearDownClass(cls):
         for fn in ("dgl_graph.bin", "dgl_line_graph.bin", "state_attr.pt", "labels.json"):
             try:
                 os.remove(fn)
             except FileNotFoundError:
```

### Comparing `matgl-0.3.0/matgl/layers/_activations.py` & `matgl-0.4.0/matgl/layers/_activations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
-Custome Activation Fucntions
+Custom activation functions
 """
 from __future__ import annotations
 
 import math
 
 import torch
-import torch.nn as nn
+from torch import nn
 
 
 class SoftPlus2(nn.Module):
     """
     SoftPlus2 activation function:
     out = log(exp(x)+1) - log(2)
     softplus function that is 0 at x=0, the implementation aims at avoiding overflow
-
-    Arguments:
-
     """
 
     def __init__(self) -> None:
         """Initializes the SoftPlus2 class."""
         super().__init__()
         self.ssp = nn.Softplus()
 
     def forward(self, x: torch.tensor) -> torch.tensor:
         """
         Evaluate activation function given the input tensor x.
-        Arguments:
+
+        Args:
             x (torch.tensor): Input tensor
 
         Returns:
             out (torch.tensor): Output tensor
         """
         return self.ssp(x) - math.log(2.0)
 
@@ -48,15 +46,15 @@
         - See related paper:
         https://arxiv.org/pdf/1602.01321.pdf
 
     """
 
     def __init__(self, alpha: float = None):
         """
-        Arguments:
+        Args:
             alpha (float): adjustable Torch parameter during the training
         """
         super().__init__()
 
         # initialize alpha
         if alpha is None:
             self.alpha = nn.Parameter(torch.tensor(0.0))
@@ -64,19 +62,19 @@
             self.alpha = nn.Parameter(torch.tensor(alpha))
 
         self.alpha.requires_grad_(True)
 
     def forward(self, x: torch.tensor) -> torch.tensor:
         """
         Evaluate activation function given the input tensor x.
-        Arguments:
+
+        Args:
             x (torch.tensor): Input tensor
 
         Returns:
             out (torch.tensor): Output tensor
         """
         if self.alpha == 0.0:
             return x
-        elif self.alpha < 0.0:
+        if self.alpha < 0.0:
             return -torch.log(1.0 - self.alpha * (x + self.alpha)) / self.alpha
-        else:
-            return (torch.exp(self.alpha * x) - 1.0) / self.alpha + self.alpha
+        return (torch.exp(self.alpha * x) - 1.0) / self.alpha + self.alpha
```

### Comparing `matgl-0.3.0/matgl/layers/_atom_ref.py` & `matgl-0.4.0/matgl/layers/_atom_ref.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 atomic energy offset. Used for predicting extensive properties.
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
-import torch.nn as nn
 from pymatgen.core import Molecule, Structure
+from torch import nn
 
 
 class AtomRef(nn.Module):
     """
     Get total property offset for a system:
     """
 
     def __init__(
         self,
         property_offset: np.array,  # type: ignore
     ) -> None:
         """
-        Parameters:
+        Args:
         -----------
         property_offset (np.array): a array of elemental property offset
         """
         super().__init__()
         self.property_offset = torch.tensor(property_offset)
         self.max_z = self.property_offset.size(dim=0)
 
@@ -46,28 +46,26 @@
                 atomic_numbers = [element_list.index(site.specie.symbol) for site in s.sites]
             else:
                 one_hot_vecs = s.ndata["attr"]
                 atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
             features[i] = np.bincount(atomic_numbers, minlength=self.max_z)
         return features
 
-    def fit(self, structs_or_graphs: list, element_list: tuple[str], properties: np.typing.NDArray) -> bool:
+    def fit(self, structs_or_graphs: list, element_list: tuple[str], properties: np.typing.NDArray) -> None:
         """
         Fit the elemental reference values for the properties
 
         Args:
-        structs_or_graphs: pymatgen Structures or dgl graphs
-        properties (np.ndarray): array of extensive properties
-
-        Returns:
+            structs_or_graphs: pymatgen Structures or dgl graphs
+            element_list (tuple): a list of element types
+            properties (np.ndarray): array of extensive properties
         """
         features = self.get_feature_matrix(structs_or_graphs, element_list)
         self.property_offset = np.linalg.pinv(features.T.dot(features)).dot(features.T.dot(properties))
         self.property_offset = torch.tensor(self.property_offset)
-        return True
 
     def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None):
         """
         Get the total property offset for a system
 
         Args:
         g: a batch of dgl graphs
@@ -82,13 +80,12 @@
                 property_offset_batched = self.property_offset[i].repeat(g.num_nodes(), 1)
                 offset = property_offset_batched * g.ndata["attr"]
                 g.ndata["atomic_offset"] = torch.sum(offset, 1)
                 offset_batched = dgl.readout_nodes(g, "atomic_offset")
                 offset_batched_with_state.append(offset_batched)
             offset_batched_with_state = torch.stack(offset_batched_with_state)  # type: ignore
             return offset_batched_with_state[state_attr]  # type: ignore
-        else:
-            property_offset_batched = self.property_offset.repeat(g.num_nodes(), 1)
-            offset = property_offset_batched * g.ndata["attr"]
-            g.ndata["atomic_offset"] = torch.sum(offset, 1)
-            offset_batched = dgl.readout_nodes(g, "atomic_offset")
-            return offset_batched
+        property_offset_batched = self.property_offset.repeat(g.num_nodes(), 1)
+        offset = property_offset_batched * g.ndata["attr"]
+        g.ndata["atomic_offset"] = torch.sum(offset, 1)
+        offset_batched = dgl.readout_nodes(g, "atomic_offset")
+        return offset_batched
```

### Comparing `matgl-0.3.0/matgl/layers/_bond.py` & `matgl-0.4.0/matgl/layers/_bond.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Generate bond features based on spherical bessel functions or gaussian expansion
 """
 from __future__ import annotations
 
 import torch
-import torch.nn as nn
+from torch import nn
 
 from matgl.utils.maths import GaussianExpansion, SphericalBesselFunction
 
 
 class BondExpansion(nn.Module):
     """
     Expand pair distances into a set of spherical bessel or gaussian functions.
@@ -23,24 +23,24 @@
         smooth: bool = False,
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
     ) -> None:
         """
-        Parameters:
-        ----------
-        max_l (int): order of angular part
-        max_n (int): order of radial part
-        cutoff (float): cutoff radius
-        rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
-        smooth (bool): whether apply the smooth version of spherical bessel functions or not
-        initial (float): initial point for gaussian expansion
-        final (float): final point for gaussian expansion
-        width (float): width of gaussian function
+        Args:
+            max_l (int): order of angular part
+            max_n (int): order of radial part
+            cutoff (float): cutoff radius
+            rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
+            smooth (bool): whether apply the smooth version of spherical bessel functions or not
+            initial (float): initial point for gaussian expansion
+            final (float): final point for gaussian expansion
+            num_centers (int): Number of centers for gaussian expansion.
+            width (float): width of gaussian function
         """
         super().__init__()
 
         self.max_n = max_n
         self.cutoff = cutoff
         self.max_l = max_l
         self.smooth = smooth
```

### Comparing `matgl-0.3.0/matgl/layers/_core.py` & `matgl-0.4.0/matgl/layers/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Implementations of multi-layer perceptron (MLP) and other helper classes.
 """
 from __future__ import annotations
 
 from typing import Callable
 
 import torch
-import torch.nn as nn
 from dgl import DGLGraph, broadcast_edges, softmax_edges, sum_edges
+from torch import nn
 from torch.nn import LSTM, Linear, Module, ModuleList
 
 
 class MLP(nn.Module):
     """
     An implementation of a multi-layer perceptron.
     """
```

### Comparing `matgl-0.3.0/matgl/layers/_embedding.py` & `matgl-0.4.0/matgl/layers/_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 """
 Embedding node, edge and optional state attributes
 """
 from __future__ import annotations
 
 import torch
-import torch.nn as nn
+from torch import nn
 
-from ._core import MLP
+from matgl.layers._core import MLP
 
 
 class EmbeddingBlock(nn.Module):
     """
     Embedding block for generating node, bond and state features
     """
 
     def __init__(
         self,
         degree_rbf: int,
         activation: nn.Module,
         dim_node_embedding: int,
-        dim_edge_embedding: int,
+        dim_edge_embedding: int | None = None,
         dim_state_feats: int | None = None,
         ntypes_node: int | None = None,
-        include_state_embedding: bool = False,
+        include_state: bool = False,
         ntypes_state: int | None = None,
         dim_state_embedding: int | None = None,
     ):
         """
 
         Args:
             degree_rbf (int): number of rbf
             activation (nn.Module): activation type
             dim_node_embedding (int): dimensionality of node features
             dim_edge_embedding (int): dimensionality of edge features
             dim_state_feats: dimensionality of state features
             ntypes_node: number of node labels
-            include_state_embedding: Whether to include state embedding
+            include_state: Whether to include state embedding
             ntypes_state: number of state labels
             dim_state_embedding: dimensionality of state embedding
         """
         super().__init__()
-        self.include_states = include_state_embedding
+        self.include_state = include_state
         self.ntypes_state = ntypes_state
         self.dim_node_embedding = dim_node_embedding
         self.dim_edge_embedding = dim_edge_embedding
         self.dim_state_feats = dim_state_feats
         self.ntypes_node = ntypes_node
         self.dim_state_embedding = dim_state_embedding
         self.activation = activation
         if ntypes_state and dim_state_embedding is not None:
             self.layer_state_embedding = nn.Embedding(ntypes_state, dim_state_embedding)  # type: ignore
         if ntypes_node is not None:
             self.layer_node_embedding = nn.Embedding(ntypes_node, dim_node_embedding)
-        self.layer_edge_embedding = MLP(
-            [degree_rbf, self.dim_edge_embedding], activation=activation, activate_last=True
-        )
+        if dim_edge_embedding is not None:
+            dim_edges = [degree_rbf, dim_edge_embedding]
+            self.layer_edge_embedding = MLP(dim_edges, activation=activation, activate_last=True)
 
     def forward(self, node_attr, edge_attr, state_attr):
         """
         Output embedded features
 
         Args:
         node_attr: node attribute
@@ -66,25 +66,28 @@
         state_attr: state attribute
 
         Returns:
         node_feat: embedded node features
         edge_feat: embedded edge features
         state_feat: embedded state features
         """
-
         if self.ntypes_node is not None:
             node_feat = self.layer_node_embedding(node_attr)
         else:
             node_embed = MLP([node_attr.shape[-1], self.dim_node_embedding], activation=self.activation)
             node_feat = node_embed(node_attr.to(torch.float32))
-
-        edge_feat = self.layer_edge_embedding(edge_attr.to(torch.float32))
-        if self.include_states is True:
+        if self.dim_edge_embedding is not None:
+            edge_feat = self.layer_edge_embedding(edge_attr.to(torch.float32))
+        else:
+            edge_feat = edge_attr
+        if self.include_state is True:
             if self.ntypes_state and self.dim_state_embedding is not None:
                 state_feat = self.layer_state_embedding(state_attr)
-            else:
+            elif self.dim_state_feats is not None:
                 state_attr = torch.unsqueeze(state_attr, 0)
                 state_embed = MLP([state_attr.shape[-1], self.dim_state_feats], activation=self.activation)
                 state_feat = state_embed(state_attr.to(torch.float32))
+            else:
+                state_feat = state_attr
         else:
             state_feat = None
         return node_feat, edge_feat, state_feat
```

### Comparing `matgl-0.3.0/matgl/layers/_graph_convolution.py` & `matgl-0.4.0/matgl/layers/_graph_convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Graph convolution layer (GCL) implementations.
 """
+
 from __future__ import annotations
 
 import dgl
 import dgl.function as fn
 import torch
-import torch.nn as nn
+from torch import nn
 from torch.nn import Dropout, Identity, Module
 
-from matgl.utils.maths import broadcast_states_to_bonds
-
-from ._core import MLP, GatedMLP
+from matgl.layers._core import MLP, GatedMLP
 
 
 class MEGNetGraphConv(Module):
     """
     A MEGNet graph convolution layer in DGL.
     """
 
@@ -96,21 +95,19 @@
         """
         Perform attribute (global state) update.
 
         :param graph: Input graph
         :param state_attrs: Input attributes
         :return: Output tensor for attributes
         """
-        u = state_attrs
-        ue = dgl.readout_edges(graph, feat="e", op="mean")
-        uv = dgl.readout_nodes(graph, feat="v", op="mean")
-        ue = torch.squeeze(ue)
-        uv = torch.squeeze(uv)
-        u = torch.squeeze(u)
-        inputs = torch.hstack([u, ue, uv])
+        u_edge = dgl.readout_edges(graph, feat="e", op="mean")
+        u_vertex = dgl.readout_nodes(graph, feat="v", op="mean")
+        u_edge = torch.squeeze(u_edge)
+        u_vertex = torch.squeeze(u_vertex)
+        inputs = torch.hstack([state_attrs.squeeze(), u_edge, u_vertex])
         state_attr = self.state_func(inputs)
         return state_attr
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
@@ -233,19 +230,19 @@
         edge_weight_func: Module,
         node_update_func: Module,
         node_weight_func: Module,
         state_update_func: Module | None,
     ):
         """
         Parameters:
-        include_states (bool): Whether including state
+        include_state (bool): Whether including state
         edge_update_func (Module): Update function for edges (Eq. 4)
         edge_weight_func (Module): Weight function for radial basis functions (Eq. 4)
         node_update_func (Module): Update function for nodes (Eq. 5)
-        node_weight_func (Module): Weight function for radieal basis functions (Eq. 5)
+        node_weight_func (Module): Weight function for radial basis functions (Eq. 5)
         attr_update_func (Module): Update function for state feats (Eq. 6)
         """
         super().__init__()
         self.include_states = include_states
         self.edge_update_func = edge_update_func
         self.edge_weight_func = edge_weight_func
         self.node_update_func = node_update_func
@@ -261,20 +258,20 @@
         state_dims: list[int] | None,
         activation: Module,
     ) -> M3GNetGraphConv:
         """
         M3GNetGraphConv initialization
 
         Args:
-        degree (int): max_n*max_l
-        include_states (bool): whether including state or not
-        edge_dim (list): NN architecture for edge update function
-        node_dim (list): NN architecture for node update function
-        state_dim (list): NN architecture for state update function
-        activation (nn.Nodule): activation function
+            degree (int): max_n*max_l
+            include_states (bool): whether including state or not
+            edge_dims (list): NN architecture for edge update function
+            node_dims (list): NN architecture for node update function
+            state_dims (list): NN architecture for state update function
+            activation (nn.Nodule): activation function
 
         Returns:
         M3GNetGraphConv (class)
         """
         edge_update_func = GatedMLP(in_feats=edge_dims[0], dims=edge_dims[1:])
         edge_weight_func = nn.Linear(in_features=degree, out_features=edge_dims[-1], bias=False)
 
@@ -321,43 +318,44 @@
         return edge_update
 
     def node_update_(self, graph: dgl.DGLGraph, state_attr: torch.Tensor) -> torch.Tensor:
         """
         Perform node update.
 
         Args:
-        graph: DGL graph
+            graph: DGL graph
+            state_attr: State attributes
 
         Returns:
-        node_update: node features update
+            node_update: node features update
         """
         eij = graph.edata["e"]
         src_id = graph.edges()[0]
         vi = graph.ndata["v"][src_id]
         dst_id = graph.edges()[1]
         vj = graph.ndata["v"][dst_id]
         rbf = graph.edata["rbf"]
         rbf = rbf.float()
         if self.include_states:
-            u = broadcast_states_to_bonds(graph, state_attr)
+            u = dgl.broadcast_edges(graph, state_attr)
             inputs = torch.hstack([vi, vj, eij, u])
         else:
             inputs = torch.hstack([vi, vj, eij])
         graph.edata["mess"] = self.node_update_func(inputs) * self.node_weight_func(rbf)
         graph.update_all(fn.copy_e("mess", "mess"), fn.sum("mess", "ve"))
         node_update = graph.ndata.pop("ve")
         return node_update
 
     def state_update_(self, graph: dgl.DGLGraph, state_attrs: torch.Tensor) -> torch.Tensor:
         """
         Perform attribute (global state) update.
 
         Args:
-        graph: DGL graph
-        attrs: graph features
+            graph: DGL graph
+            state_attrs: graph features
 
         Returns:
         state_update: state_features update
         """
         u = state_attrs
         uv = dgl.readout_nodes(graph, feat="v", op="mean")
         inputs = torch.hstack([u, uv])
@@ -405,52 +403,52 @@
         self,
         degree: int,
         activation: Module,
         conv_hiddens: list[int],
         num_node_feats: int,
         num_edge_feats: int,
         num_state_feats: int | None = None,
-        include_states: bool = False,
+        include_state: bool = False,
         dropout: float | None = None,
     ) -> None:
         """
         :param degree: Dimension of radial basis functions
         :param num_node_feats: Number of node features
         :param num_edge_feats: Number of edge features
         :param num_state_feats: Number of state features
         :param conv_hiddens: Dimension of hidden layers
         :param activation: Activation type
-        :param include_states: Including state features or not
+        :param include_state: Including state features or not
         :param dropout: Probability of an element to be zero in dropout layer
         """
         super().__init__()
 
         self.activation = activation
 
         # compute input sizes
-        if include_states:
+        if include_state:
             edge_in = 2 * num_node_feats + num_edge_feats + num_state_feats  # type: ignore
             node_in = 2 * num_node_feats + num_edge_feats + num_state_feats  # type: ignore
             attr_in = num_node_feats + num_state_feats  # type: ignore
             self.conv = M3GNetGraphConv.from_dims(
                 degree,
-                include_states,
+                include_state,
                 edge_dims=[edge_in, *conv_hiddens, num_edge_feats],
                 node_dims=[node_in, *conv_hiddens, num_node_feats],
                 state_dims=[attr_in, *conv_hiddens, num_state_feats],  # type: ignore
                 activation=self.activation,
             )
         else:
             edge_in = 2 * num_node_feats + num_edge_feats  # 2*NDIM+EDIM
             node_in = 2 * num_node_feats + num_edge_feats  # 2*NDIM+EDIM
             self.conv = M3GNetGraphConv.from_dims(
                 degree,
-                include_states,
-                edge_dims=[edge_in, *conv_hiddens] + [num_edge_feats],
-                node_dims=[node_in, *conv_hiddens] + [num_node_feats],
+                include_state,
+                edge_dims=[edge_in, *conv_hiddens, num_edge_feats],
+                node_dims=[node_in, *conv_hiddens, num_node_feats],
                 state_dims=None,  # type: ignore
                 activation=self.activation,
             )
 
         self.dropout = Dropout(dropout) if dropout else None
 
     def forward(
```

### Comparing `matgl-0.3.0/matgl/layers/_readout.py` & `matgl-0.4.0/matgl/layers/_readout.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 Readout layer for M3GNet
 """
 
 from __future__ import annotations
 
 import dgl
 import torch
-import torch.nn as nn
 from dgl.nn import Set2Set
+from torch import nn
 
-from ._core import EdgeSet2Set, GatedMLP
+from matgl.layers._core import EdgeSet2Set, GatedMLP
 
 
 class Set2SetReadOut(nn.Module):
     """
     The Set2Set readout function
     """
 
     def __init__(
         self,
         num_steps: int,
         num_layers: int,
         field: str,
     ):
         """
-        Paramaters:
-            num_steps (int): number of LSTM steps
-            field (str): the field of MaterialGraph to perform the readout
+        Args:
+            num_steps (int): Number of LSTM steps
+            num_layers (int): Number of layers.
+            field (str): Field of graph to perform the readout
         """
         super().__init__()
         self.field = field
         self.num_steps = num_steps
         self.num_layers = num_layers
 
     def forward(self, g: dgl.DGLGraph):
@@ -49,20 +50,20 @@
 class ReduceReadOut(nn.Module):
     """
     Reduce atom or bond attributes into lower dimensional tensors as readout.
     This could be summing up the atoms or bonds, or taking the mean, etc.
     """
 
     def __init__(self, op: str = "mean", field: str = "node_feat"):
-        super().__init__()
         """
-        Parameters:
+        Args:
             op (str): op for the reduction
-            field (str): the field of MaterialGraph to perform the reduction
+            field (str): Field of graph to perform the reduction
         """
+        super().__init__()
         self.op = op
         self.field = field
 
     def forward(self, g: dgl.DGLGraph):
         """
         Args:
             g: DGL graph
@@ -79,30 +80,30 @@
 class WeightedReadOut(nn.Module):
     """
     Feed node features into Gated MLP as readout.
     """
 
     def __init__(self, in_feats: int, dims: list[int], num_targets: int):
         """
-        Parameters:
+        Args:
            in_feats: input features (nodes)
            dims: NN architecture for Gated MLP
            num_targets: number of target properties
         """
         super().__init__()
         self.in_feats = in_feats
-        self.dims = [in_feats, *dims] + [num_targets]
+        self.dims = [in_feats, *dims, num_targets]
         self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
     def forward(self, g: dgl.DGLGraph):
         """
         Args:
             g: DGL graph
         Returns:
-            atomic_prperties: torch.tensor
+            atomic_properties: torch.tensor
         """
         atomic_properties = self.gated(g.ndata["node_feat"])
         return atomic_properties
 
 
 class WeightedReadOutPair(nn.Module):
     """
```

### Comparing `matgl-0.3.0/matgl/layers/_three_body.py` & `matgl-0.4.0/matgl/layers/_three_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Three-Body interaction implementations.
 """
 
 from __future__ import annotations
 
 import dgl
 import torch
-import torch.nn as nn
+from torch import nn
 
 from matgl.utils.maths import (
     SphericalBesselFunction,
     SphericalHarmonicsFunction,
     combine_sbf_shf,
     get_segment_indices_from_n,
     scatter_sum,
@@ -42,69 +42,65 @@
         # retrieve formulas
         self.shf = SphericalHarmonicsFunction(self.max_l, self.use_phi)
         if self.use_smooth:
             self.sbf = SphericalBesselFunction(self.max_l, self.max_n * self.max_l, self.cutoff, self.use_smooth)
         else:
             self.sbf = SphericalBesselFunction(self.max_l, self.max_n, self.cutoff, self.use_smooth)
 
-    def forward(self, graph, line_graph):
+    def forward(self, line_graph):
         sbf = self.sbf(line_graph.edata["triple_bond_lengths"])
         shf = self.shf(line_graph.edata["cos_theta"], line_graph.edata["phi"])
-        return combine_sbf_shf(
-            sbf, shf, max_n=self.max_n, max_l=self.max_l, use_phi=self.use_phi, use_smooth=self.use_smooth
-        )
+        return combine_sbf_shf(sbf, shf, max_n=self.max_n, max_l=self.max_l, use_phi=self.use_phi)
 
 
 class ThreeBodyInteractions(nn.Module):
     """
     Include 3D interactions to the bond update
     """
 
     def __init__(self, update_network_atom: nn.Module, update_network_bond: nn.Module, **kwargs):
-        """
+        r"""
         Args:
             update_network_atom: MLP for node features in Eq.2
             update_network_bond: Gated-MLP for edge features in Eq.3
-            **kwargs:
+            **kwargs: Kwargs pass-through to nn.Module.__init__().
         """
         super().__init__(**kwargs)
         self.update_network_atom = update_network_atom
         self.update_network_bond = update_network_bond
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         line_graph: dgl.DGLGraph,
         three_basis: torch.tensor,
         three_cutoff: float,
         node_feat: torch.tensor,
         edge_feat: torch.tensor,
-        **kwargs,
     ):
         """
         Args:
             graph: dgl graph
+            line_graph: line graph.
             three_basis: three body basis expansion
             three_cutoff: cutoff radius
             node_feat: node features
             edge_feat: edge features
-            **kwargs:
-        Returns:
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
         three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
         weights = torch.reshape(
             three_cutoff[torch.stack(list(line_graph.edges()), dim=1).to(torch.int64)], (-1, 2)  # type: ignore
         )
         weights = torch.prod(weights, axis=-1)
-        weights = basis * weights[:, None]
+        basis = basis * weights[:, None]
         new_bonds = scatter_sum(
             basis.to(torch.float32),
             segment_ids=get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
             num_segments=graph.num_edges(),
             dim=0,
         )
         edge_feat_updated = edge_feat + self.update_network_bond(new_bonds)
```

### Comparing `matgl-0.3.0/matgl/models/_m3gnet.py` & `matgl-0.4.0/matgl/models/_m3gnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Core M3GNet model
 """
 from __future__ import annotations
 
 import logging
-import os
 
 import dgl
 import torch
-import torch.nn as nn
+from torch import nn
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import (
     compute_pair_vector_and_distance,
     compute_theta_and_phi,
     create_line_graph,
 )
@@ -20,29 +19,27 @@
     MLP,
     BondExpansion,
     EmbeddingBlock,
     GatedMLP,
     M3GNetBlock,
     ReduceReadOut,
     Set2SetReadOut,
+    SoftExponential,
+    SoftPlus2,
     SphericalBesselWithHarmonics,
     ThreeBodyInteractions,
     WeightedReadOut,
 )
 from matgl.utils.cutoff import polynomial_cutoff
+from matgl.utils.io import IOMixIn
 
 logger = logging.getLogger(__file__)
-CWD = os.path.dirname(os.path.abspath(__file__))
 
-MODEL_NAME = "m3gnet"
 
-MODEL_PATHS = {"MP-2021.2.8-EFS": os.path.join(CWD, "..", "..", "pretrained_models", "MP-2021.2.8-EFS")}
-
-
-class M3GNet(nn.Module):
+class M3GNet(nn.Module, IOMixIn):
     """
     The main M3GNet model
     """
 
     def __init__(
         self,
         element_types: tuple[str],
@@ -57,24 +54,22 @@
         rbf_type="SphericalBessel",
         is_intensive: bool = True,
         readout_type: str = "weighted_atom",
         task_type: str = "regression",
         cutoff: float = 5.0,
         threebody_cutoff: float = 4.0,
         units: int = 64,
-        data_mean: float = 0.0,
-        data_std: float = 1.0,
         ntargets: int = 1,
         use_smooth: bool = False,
         use_phi: bool = False,
         niters_set2set: int = 3,
         nlayers_set2set: int = 3,
         field: str = "node_feat",
-        include_state_embedding: bool = False,
-        activation: str = "swish",
+        include_state: bool = False,
+        activation_type: str = "swish",
         **kwargs,
     ):
         r"""
         Args:
             element_types (tuple): list of elements appearing in the dataset
             dim_node_embedding (int): number of embedded atomic features
             dim_edge_embedding (int): number of edge features
@@ -82,46 +77,47 @@
             dim_state_feats (int): number of state features after linear layer
             dim_state_types (int): number of state labels
             max_n (int): number of radial basis expansion
             max_l (int): number of angular expansion
             nblocks (int): number of convolution blocks
             rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
             is_intensive (bool): whether the prediction is intensive
-            readout (str): the readout function type. choose from `set2set`,
+            readout_type (str): the readout function type. choose from `set2set`,
                 `weighted_atom` and `reduce_atom`, default to `weighted_atom`
             task_type (str): `classification` or `regression`, default to
                 `regression`
             cutoff (float): cutoff radius of the graph
             threebody_cutoff (float): cutoff radius for 3 body interaction
             units (int): number of neurons in each MLP layer
-            data_mean (float): optional `mean` value of the target
-            data_std (float): optional `std` of the target
             ntargets (int): number of target properties
             use_smooth (bool): whether using smooth Bessel functions
             use_phi (bool): whether using phi angle
             field (str): using either "node_feat" or "edge_feat" for Set2Set and Reduced readout
             niters_set2set (int): number of set2set iterations
             nlayers_set2set (int): number of set2set layers
-            include_state_embedding (bool): whether to include states features
-            activation (str): activation type. choose from 'swish', 'tanh', 'sigmoid'
-            **kwargs:
+            include_state (bool): whether to include states features
+            activation_type (str): activation type. choose from 'swish', 'tanh', 'sigmoid', 'softplus2', 'softexp'
+            **kwargs: For future flexibility. Not used at the moment.
         """
-
-        # Store M3GNet model args for loading trained model
-        self.model_args = {k: v for k, v in locals().items() if k not in ["self", "__class__", "kwargs"]}
-        self.model_args.update(kwargs)
-
         super().__init__()
 
-        if activation == "swish":
-            self.activation = nn.SiLU()  # type: ignore
-        elif activation == "tanh":
-            self.activation = nn.Tanh()  # type: ignore
-        elif activation == "sigmoid":
-            self.activation = nn.Sigmoid()  # type: ignore
+        self.save_args(locals(), kwargs)
+
+        if activation_type == "swish":
+            activation = nn.SiLU()  # type: ignore
+        elif activation_type == "tanh":
+            activation = nn.Tanh()  # type: ignore
+        elif activation_type == "sigmoid":
+            activation = nn.Sigmoid()  # type: ignore
+        elif activation_type == "softplus2":
+            activation = SoftPlus2()  # type: ignore
+        elif activation_type == "softexp":
+            activation = SoftExponential()  # type: ignore
+        else:
+            raise Exception("Undefined activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
 
         if element_types is None:
             self.element_types = DEFAULT_ELEMENT_TYPES
         else:
             self.element_types = element_types  # type: ignore
 
         self.bond_expansion = BondExpansion(max_l, max_n, cutoff, rbf_type=rbf_type, smooth=use_smooth)
@@ -132,17 +128,17 @@
 
         self.embedding = EmbeddingBlock(
             degree_rbf=degree_rbf,
             dim_node_embedding=dim_node_embedding,
             dim_edge_embedding=dim_edge_embedding,
             ntypes_node=len(element_types),
             dim_state_feats=dim_state_feats,
-            include_state_embedding=include_state_embedding,
+            include_state=include_state,
             dim_state_embedding=dim_state_embedding,
-            activation=self.activation,
+            activation=activation,
         )
 
         self.basis_expansion = SphericalBesselWithHarmonics(
             max_n=max_n, max_l=max_l, cutoff=cutoff, use_phi=use_phi, use_smooth=use_smooth
         )
         self.three_body_interactions = nn.ModuleList(
             {
@@ -156,115 +152,69 @@
             }
         )
 
         self.graph_layers = nn.ModuleList(
             {
                 M3GNetBlock(
                     degree=degree_rbf,
-                    activation=self.activation,
+                    activation=activation,
                     conv_hiddens=[units, units],
                     num_node_feats=dim_node_embedding,
                     num_edge_feats=dim_edge_embedding,
                     num_state_feats=dim_state_feats,
-                    include_states=include_state_embedding,
+                    include_state=include_state,
                 )
                 for _ in range(nblocks)
             }
         )
         if is_intensive:
             input_feats = dim_node_embedding if field == "node_feat" else dim_edge_embedding
             if readout_type == "set2set":
                 self.readout = Set2SetReadOut(num_steps=niters_set2set, num_layers=nlayers_set2set, field=field)
-                readout_feats = (
-                    2 * input_feats + dim_state_feats if include_state_embedding else 2 * input_feats  # type: ignore
-                )
+                readout_feats = 2 * input_feats + dim_state_feats if include_state else 2 * input_feats  # type: ignore
             else:
                 self.readout = ReduceReadOut("mean", field=field)
-                readout_feats = (
-                    input_feats + dim_state_feats if include_state_embedding else input_feats  # type: ignore
-                )
+                readout_feats = input_feats + dim_state_feats if include_state else input_feats  # type: ignore
 
-            dims_final_layer = [readout_feats] + [units, units] + [ntargets]
-            self.final_layer = MLP(dims_final_layer, self.activation, activate_last=False)
+            dims_final_layer = [readout_feats, units, units, ntargets]
+            self.final_layer = MLP(dims_final_layer, activation, activate_last=False)
             if task_type == "classification":
                 self.sigmoid = nn.Sigmoid()
 
         else:
             if task_type == "classification":
                 raise ValueError("Classification task cannot be extensive")
             self.final_layer = WeightedReadOut(in_feats=dim_node_embedding, dims=[units, units], num_targets=ntargets)
 
         self.max_n = max_n
         self.max_l = max_l
         self.n_blocks = nblocks
         self.units = units
         self.cutoff = cutoff
         self.threebody_cutoff = threebody_cutoff
-        self.include_states = include_state_embedding
+        self.include_states = include_state
         self.task_type = task_type
         self.is_intensive = is_intensive
-        self.data_mean = data_mean
-        self.data_std = data_std
-
-    def as_dict(self):
-        out = {"state_dict": self.state_dict(), "model_args": self.model_args}
-        return out
-
-    @classmethod
-    def from_dict(cls, dict, **kwargs):
-        """
-        build a M3GNet from a saved dictionary
-        """
-        model = M3GNet(**dict["model_args"])
-        model.load_state_dict(dict["state_dict"], **kwargs)
-        return model
-
-    @classmethod
-    def from_dir(cls, path, **kwargs):
-        """
-        build a M3GNet from a saved directory
-        """
-        file_name = os.path.join(path, MODEL_NAME + ".pt")
-        state = torch.load(file_name)
-        model = M3GNet.from_dict(state["model"], **kwargs)
-        return model
-
-    @classmethod
-    def load(cls, model_dir: str = "MP-2021.2.8-EFS") -> M3GNet:
-        """
-        Load the model weights from pre-trained model (m3gnet.pt)
-        Args:
-            model_dir (str): directory for saved model. Defaults to "MP-2021.2.8-EFS".
-
-        Returns: M3GNet object.
-        """
-        if model_dir in MODEL_PATHS:
-            return cls.from_dir(MODEL_PATHS[model_dir])
-
-        if os.path.isdir(model_dir) and "m3gnet.pt" in os.listdir(model_dir):
-            return cls.from_dir(model_dir)
-
-        raise ValueError(f"{model_dir} not found in available pretrained_models {list(MODEL_PATHS.keys())}")
 
     def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None):
         """Performs message passing and updates node representations.
 
         Parameters
         ----------
         g : DGLGraph
             DGLGraph for a batch of graphs.
         state_attr : torch.tensor
             State attrs for a batch of graphs.
         l_g : DGLGraph
             DGLGraph for a batch of line graphs.
 
-        Returns
+        Returns:
         -------
-        ouput : torch.tensor
-            Ouput property for a batch of graphs
+        output : torch.tensor
+            Output property for a batch of graphs
         """
         node_types = g.ndata["node_type"]
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
         g.edata["bond_vec"] = bond_vec
         g.edata["bond_dist"] = bond_dist
 
         expanded_dists = self.bond_expansion(g.edata["bond_dist"])
@@ -273,15 +223,15 @@
         else:
             valid_three_body = g.edata["bond_dist"] <= self.threebody_cutoff
             l_g.ndata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
             l_g.ndata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
             l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
         l_g.apply_edges(compute_theta_and_phi)
         g.edata["rbf"] = expanded_dists
-        three_body_basis = self.basis_expansion(g, l_g)
+        three_body_basis = self.basis_expansion(l_g)
         three_body_cutoff = polynomial_cutoff(g.edata["bond_dist"], self.threebody_cutoff)
         num_node_feats, num_edge_feats, num_state_feats = self.embedding(node_types, g.edata["rbf"], state_attr)
         for i in range(self.n_blocks):
             num_edge_feats = self.three_body_interactions[i](
                 g, l_g, three_body_basis, three_body_cutoff, num_node_feats, num_edge_feats
             )
             num_edge_feats, num_node_feats, num_state_feats = self.graph_layers[i](
@@ -294,9 +244,8 @@
             vec = torch.hstack([node_vec, state_attr]) if self.include_states else node_vec
             output = self.final_layer(vec)
             if self.task_type == "classification":
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             output = dgl.readout_nodes(g, "atomic_properties", op="sum")
-        output = output * self.data_std + self.data_mean
         return torch.squeeze(output)
```

### Comparing `matgl-0.3.0/matgl/models/_megnet.py` & `matgl-0.4.0/matgl/models/_megnet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,98 @@
 """
 Implementation of MEGNet model.
 """
 from __future__ import annotations
 
 import logging
-from pathlib import Path
 
 import dgl
 import torch
-import torch.nn as nn
 from dgl.nn import Set2Set
 from pymatgen.core import Structure
+from torch import nn
 
-from matgl.config import DEFAULT_ELEMENT_TYPES, MATGL_CACHE, PRETRAINED_MODELS_BASE_URL
+from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.ext.pymatgen import Structure2Graph
 from matgl.graph.compute import compute_pair_vector_and_distance
 from matgl.graph.converters import GraphConverter
-from matgl.layers import MLP, BondExpansion, EdgeSet2Set, MEGNetBlock, SoftExponential, SoftPlus2
-from matgl.utils.remote import RemoteFile
+from matgl.layers import MLP, BondExpansion, EdgeSet2Set, EmbeddingBlock, MEGNetBlock, SoftExponential, SoftPlus2
+from matgl.utils.io import IOMixIn
 
 logger = logging.getLogger(__file__)
 
 
-class MEGNet(nn.Module):
+class MEGNet(nn.Module, IOMixIn):
     """
     DGL implementation of MEGNet.
     """
 
     def __init__(
         self,
         dim_node_embedding: int = 16,
         dim_edge_embedding: int = 100,
         dim_state_embedding: int = 2,
+        ntypes_state: int | None = None,
         nblocks: int = 3,
         hidden_layer_sizes_input: tuple[int, ...] = (64, 32),
         hidden_layer_sizes_conv: tuple[int, ...] = (64, 64, 32),
         hidden_layer_sizes_output: tuple[int, ...] = (32, 16),
         nlayers_set2set: int = 1,
         niters_set2set: int = 2,
         activation_type: str = "softplus2",
         is_classification: bool = False,
-        layer_node_embedding: nn.Module | None = None,
-        layer_edge_embedding: nn.Module | None = None,
-        layer_state_embedding: nn.Module | None = None,
-        include_state_embedding: bool = False,
+        include_state: bool = True,
         dropout: float | None = None,
         graph_transformations: list | None = None,
         element_types: tuple[str, ...] | None = None,
-        data_mean: torch.tensor | None = None,
-        data_std: torch.tensor | None = None,
         bond_expansion: BondExpansion | None = None,
         cutoff: float = 4.0,
         gauss_width: float = 0.5,
         **kwargs,
     ):
         """
         Construct a MEGNet model. Useful defaults for all arguments have been specified based on MEGNet formation energy
         model.
 
         Args:
             dim_node_embedding: Dimension of node embedding.
             dim_edge_embedding: Dimension of edge embedding.
             dim_state_embedding: Dimension of state embedding.
+            ntypes_state: Number of state types.
             nblocks: Number of blocks.
             hidden_layer_sizes_input: Architecture of dense layers before the graph convolution
             hidden_layer_sizes_conv: Architecture of dense layers for message and update functions
             nlayers_set2set: Number of layers in Set2Set layer
-            niters_set2set: Number of iteratons in Set2Set layer
+            niters_set2set: Number of iterations in Set2Set layer
             hidden_layer_sizes_output: Architecture of dense layers for concatenated features after graph convolution
-            activation_types: Activation used for non-linearity
+            activation_type: Activation used for non-linearity
             is_classification: Whether this is classification task or not
             layer_node_embedding: Architecture of embedding layer for node attributes
             layer_edge_embedding: Architecture of embedding layer for edge attributes
             layer_state_embedding: Architecture of embedding layer for state attributes
-            include_state_embedding: Whether the state embedding is included
+            include_state: Whether the state embedding is included
             dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according to
                 a Bernoulli distribution
             graph_transformations: Perform a graph transformation, e.g., incorporate three-body interactions, prior to
                 performing the GCL updates.
             element_types: Elements included in the training set
-            data_mean: Mean of target properties in the training set. Defaults to 0.
-            data_std: Standard deviation of target properties in the training set. Defaults to 1.
             bond_expansion: Gaussian expansion for edge attributes
             cutoff: cutoff for forming bonds
             gauss_width: width of Gaussian function for bond expansion
-            **kwargs:
+            **kwargs: For future flexibility. Not used at the moment.
         """
-        # Store MEGNet model args for loading trained model
-        self.model_args = {k: v for k, v in locals().items() if k not in ["self", "__class__", "kwargs"]}
-        self.model_args.update(kwargs)
-
         super().__init__()
 
+        self.save_args(locals(), kwargs)
+
         self.element_types = element_types or DEFAULT_ELEMENT_TYPES
         self.cutoff = cutoff
         self.bond_expansion = bond_expansion or BondExpansion(
             rbf_type="Gaussian", initial=0.0, final=cutoff + 1.0, num_centers=dim_edge_embedding, width=gauss_width
         )
-        self.data_mean = data_mean or torch.zeros(1)
-        self.data_std = data_std or torch.ones(1)
-
-        self.layer_edge_embedding = layer_edge_embedding if layer_edge_embedding else nn.Identity()
-        if layer_node_embedding is None:
-            self.layer_node_embedding = nn.Embedding(len(self.element_types), dim_node_embedding)
-        else:
-            self.layer_node_embedding = layer_node_embedding
-        self.layer_state_embedding = layer_state_embedding or nn.Identity()
 
         node_dims = [dim_node_embedding, *hidden_layer_sizes_input]
         edge_dims = [dim_edge_embedding, *hidden_layer_sizes_input]
         state_dims = [dim_state_embedding, *hidden_layer_sizes_input]
 
         if activation_type == "swish":
             activation = nn.SiLU()  # type: ignore
@@ -120,14 +103,24 @@
         elif activation_type == "softplus2":
             activation = SoftPlus2()  # type: ignore
         elif activation_type == "softexp":
             activation = SoftExponential()  # type: ignore
         else:
             raise Exception("Undefined activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
 
+        self.embedding = EmbeddingBlock(
+            degree_rbf=dim_edge_embedding,
+            dim_node_embedding=dim_node_embedding,
+            ntypes_node=len(self.element_types),
+            ntypes_state=ntypes_state,
+            include_state=include_state,
+            dim_state_embedding=dim_state_embedding,
+            activation=activation,
+        )
+
         self.edge_encoder = MLP(edge_dims, activation, activate_last=True)
         self.node_encoder = MLP(node_dims, activation, activate_last=True)
         self.state_encoder = MLP(state_dims, activation, activate_last=True)
 
         dim_blocks_in = hidden_layer_sizes_input[-1]
         dim_blocks_out = hidden_layer_sizes_conv[-1]
         block_args = {
@@ -154,15 +147,15 @@
             activate_last=False,
         )
 
         self.dropout = nn.Dropout(dropout) if dropout else None
 
         self.is_classification = is_classification
         self.graph_transformations = graph_transformations or [nn.Identity()] * nblocks
-        self.include_state_embedding = include_state_embedding
+        self.include_state_embedding = include_state
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
         state_feat: torch.Tensor,
@@ -173,20 +166,18 @@
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_feat: State features.
         :return: Prediction
         """
         graph_transformations = self.graph_transformations
-        edge_feat = self.edge_encoder(self.layer_edge_embedding(edge_feat))
-        node_feat = self.node_encoder(self.layer_node_embedding(node_feat))
-        if self.include_state_embedding:
-            state_feat = self.state_encoder(self.layer_state_embedding(state_feat))
-        else:
-            state_feat = self.state_encoder(state_feat)
+        node_feat, edge_feat, state_feat = self.embedding(node_feat, edge_feat, state_feat)
+        edge_feat = self.edge_encoder(edge_feat)
+        node_feat = self.node_encoder(node_feat)
+        state_feat = self.state_encoder(state_feat)
 
         for gt, block in zip(graph_transformations, self.blocks):
             output = block(gt(graph), edge_feat, node_feat, state_feat)
             edge_feat, node_feat, state_feat = output
 
         node_vec = self.node_s2s(graph, node_feat)
         edge_vec = self.edge_s2s(graph, edge_feat)
@@ -207,86 +198,37 @@
         return output
 
     def predict_structure(
         self,
         structure: Structure,
         state_feats: torch.tensor | None = None,
         graph_converter: GraphConverter | None = None,
+        data_mean: float | None = None,
+        data_std: float | None = None,
     ):
         """
         Convenience method to directly predict property from structure.
+
         Args:
             structure (Structure): Pymatgen structure
             state_feats (torch.tensor): graph attributes
             graph_converter: Object that implements a get_graph_from_structure.
+            data_mean: Mean of the data. Used when the original data has been scaled.
+            data_std: Std of the data. Used when the original data has been scaled.
+
         Returns:
             output (torch.tensor): output property
         """
         if graph_converter is None:
             graph_converter = Structure2Graph(element_types=self.element_types, cutoff=self.cutoff)
         g, state_feats_default = graph_converter.get_graph(structure)
         if state_feats is None:
             state_feats = torch.tensor(state_feats_default)
+        if data_mean is None:
+            data_mean = torch.zeros(1)
+        if data_std is None:
+            data_std = torch.ones(1)
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
         g.edata["edge_attr"] = self.bond_expansion(bond_dist)
-
-        output = self.data_std * self(g, g.edata["edge_attr"], g.ndata["node_type"], state_feats) + self.data_mean
+        output = data_mean + data_std * self(g, g.edata["edge_attr"], g.ndata["node_type"], state_feats)
 
         return output.detach()
-
-    def as_dict(self):
-        out = {"state_dict": self.state_dict(), "model_args": self.model_args}
-        return out
-
-    @classmethod
-    def from_dict(cls, dict, **kwargs):
-        """
-        build a MEGNet from a saved dictionary
-        """
-        model = MEGNet(**dict["model_args"])
-        model.load_state_dict(dict["state_dict"], **kwargs)
-        return model
-
-    def save(self, path: str | Path):
-        path = Path(path)
-        torch.save(self.model_args, path / "model.pt")
-        torch.save(self.state_dict(), path / "state.pt")
-
-    @classmethod
-    def load(cls, path: str | Path) -> MEGNet:
-        """
-        Load the model weights from a directory.
-
-        Args:
-            path (str|path): Path to saved model or name of pre-trained model. The search order is
-                path, followed by model name in PRETRAINED_MODELS_PATH, followed by download from
-                PRETRAINED_MODELS_BASE_URL.
-
-        Returns: MEGNet object.
-        """
-        path = Path(path)
-        if (path / "model.pt").exists() and (path / "state.pt").exists():
-            model_path = path / "model.pt"
-            state_path = path / "state.pt"
-        elif (MATGL_CACHE / path / "model.pt").exists() and (MATGL_CACHE / path / "state.pt").exists():
-            model_path = MATGL_CACHE / path / "model.pt"
-            state_path = MATGL_CACHE / path / "state.pt"
-        else:
-            try:
-                model_file = RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/model.pt")
-                state_file = RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/state.pt")
-                model_path = model_file.local_path
-                state_path = state_file.local_path
-            except BaseException:
-                raise ValueError(
-                    f"No valid model found in {model_path} or among pre-trained_models at "
-                    f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
-                )
-
-        if not torch.cuda.is_available():
-            state = torch.load(state_path, map_location=torch.device("cpu"))
-        else:
-            state = torch.load(state_path)
-        model_args = torch.load(model_path)
-        model = cls(**model_args)
-        model.load_state_dict(state)
-        return model
```

### Comparing `matgl-0.3.0/matgl/utils/cutoff.py` & `matgl-0.4.0/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.3.0/matgl/utils/maths.py` & `matgl-0.4.0/matgl/utils/maths.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import os
 from functools import lru_cache
 from math import pi, sqrt
 
 import numpy as np
 import sympy
 import torch
-import torch.nn as nn
 from scipy.optimize import brentq
 from scipy.special import spherical_jn
+from torch import nn
 
 from matgl.config import DataType
 
 CWD = os.path.dirname(os.path.abspath(__file__))
 
 """
 Precomputed Spherical Bessel function roots in a 2D array with dimension [128, 128]. The n-th (0-based index) root of
@@ -116,14 +116,15 @@
 
     def __init__(self, max_l: int, max_n: int = 5, cutoff: float = 5.0, smooth: bool = False):
         """
         Args:
             max_l: int, max order (excluding l)
             max_n: int, max number of roots used in each l
             cutoff: float, cutoff radius
+            smooth: Whether to smooth the function.
         """
         self.max_l = max_l
         self.max_n = max_n
         self.cutoff = cutoff
         self.smooth = smooth
         if smooth:
             self.funcs = self._calculate_smooth_symbolic_funcs()
@@ -246,15 +247,15 @@
         self.orig_funcs = [sympy.simplify(i).evalf() for i in funcs]
         self.funcs = [sympy.lambdify([costheta, phi], i, [{"conjugate": _conjugate}, torch]) for i in self.orig_funcs]
         self.funcs[0] = _y00
 
     def __call__(self, costheta, phi=None):
         """
         Args:
-            theta: torch.tensor, the azimuthal angle
+            costheta: Cosine of the azimuthal angle
             phi: torch.tensor, the polar angle
 
         Returns: [n, m] spherical harmonic results, where n is the number
             of angles. The column is arranged following
             `[Y_0^0, Y_1^{-1}, Y_1^{0}, Y_1^1, Y_2^{-2}, ...]`
         """
         costheta = torch.tensor(costheta, dtype=torch.complex64)
@@ -272,15 +273,15 @@
     for i, b in enumerate(block_size):
         indices.append(torch.tile(col_index[start : start + b], [repeats[i]]))
         start += b
     indices = torch.cat(indices, axis=0)
     return torch.index_select(array, 1, indices)
 
 
-def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool, use_smooth: bool):
+def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool):
     """
     Combine the spherical Bessel function and the spherical Harmonics function
 
     For the spherical Bessel function, the column is ordered by
         [n=[0, ..., max_n-1], n=[0, ..., max_n-1], ...], max_l blocks,
 
     For the spherical Harmonics function, the column is ordered by
@@ -539,20 +540,22 @@
     return data
 
 
 def broadcast(input_tensor: torch.tensor, target_tensor: torch.tensor, dim: int):
     """
     Broadcast input tensor along a given dimension to match the shape of the target tensor.
     Modified from torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
+
     Args:
         input_tensor: The tensor to broadcast.
         target_tensor: The tensor whose shape to match.
         dim: The dimension along which to broadcast.
+
     Returns:
-        resulting inout tensor after broadcasting
+        resulting input tensor after broadcasting
     """
     if input_tensor.dim() == 1:
         for _ in range(0, dim):
             input_tensor = input_tensor.unsqueeze(0)
     for _ in range(input_tensor.dim(), target_tensor.dim()):
         input_tensor = input_tensor.unsqueeze(-1)
     target_shape = list(target_tensor.shape)
```

### Comparing `matgl-0.3.0/matgl/utils/sb_roots.npy` & `matgl-0.4.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.3.0/matgl.egg-info/PKG-INFO` & `matgl-0.4.0/matgl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.3.0
+Version: 0.4.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -16,152 +16,151 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+Provides-Extra: munch
+Provides-Extra: pymatgen
 License-File: LICENSE
 
+# matGL
+
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
-# Table of Contents
-* [Introduction](#introduction)
-* [Status](#status)
-* [Architectures](#architectures)
-* [Installation](#installation)
-* [Usage](#usage)
-* [Documentation](#documentation)
-* [References](#references)
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Status](#status)
+- [Architectures](#architectures)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Docs](#docs)
+- [References](#references)
 
-<a name="introduction"></a>
-# Introduction
+## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials. Mathematical graphs are a natural
 representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been shown
 to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
 and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
 The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
 implemented in TensorFlow.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
-<a name="status"></a>
-# Status
+## Status
 
 - Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
 - Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
 
-<a name="architectures"></a>
-# Architectures
+## Architectures
 
-## MEGNet
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MEGNet.png?raw=true"  width="50%">
+## MEGNet
 
 The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
 learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
 array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
 Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
 (See "Learning properties of ordered and disordered materials from multi-fidelity data").
 
 Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
 attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet.png?raw=true"  width="50%">
-
 [M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
 incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation.
 
 As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
-  machine learning interatomic potentials (ML-IAPs). However, a key feature of a graph representation is its
+  machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
-  *universal IAP* that can work across the entire periodic table of the elements by training on relaxations performed
+  *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
   in the [Materials Project](http://materialsproject.org).
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
-  surrogate models for property predictions, achieving in many cases accuracies that better or similar to other
+  surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
-For detailed performance benchmarks, please refer to the publication in the [References](#references) section.
+For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
-<a name="installation"></a>
-# Installation
+## Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
 ```
 
 For the latest dev version, please clone this repo and install using:
 
 ```bash
 python setup.py -e .
 ```
 
-
-<a name="usage"></a>
-# Usage
+## Usage
 
 The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
-from matgl.models._megnet import MEGNet
+from matgl.models import MEGNet
 
-# load the pre-trained MEGNet model for formation energy model.
+## load the pre-trained MEGNet model for formation energy model.
 model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
-# This is the structure obtained from the Materials Project.
+## This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-eform = model.predict_structure(struct)
-print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
+e_form = model.predict_structure(struct)
+print(f"The predicted formation energy for CsCl is {float(e_form):5f} eV/atom.")
 ```
 
-A full example is in [here](examples/Using%20MEGNet%20Pre-trained%20Models%20for%20Property%20Predictions.ipynb).
+A full example is in [here](examples/Pre-trained%20MEGNet%20for%20Property%20Predictions.ipynb).
 
+## Docs
 
-<a name="documentation"></a>
-# Additional information
-- [Documentation Page](http://materialsvirtuallab.github.io/matgl)
-- [API documentation](https://materialsvirtuallab.github.io/matgl/modules.html)
+<http://materialsvirtuallab.github.io/matgl>
 
-<a name="references"></a>
-# References
+## References
 
 Please cite the following works:
 
 - MEGNet
+
     ```txt
     Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
     Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
     ```
+
 - Multi-fidelity MEGNet
+
     ```txt
     Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
     Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
     ```
+
 - M3GNet
+
     ```txt
     Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
     2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
     ```
 
-# Acknowledgements
+## Acknowledgments
 
 This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
 Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
```

### Comparing `matgl-0.3.0/matgl.egg-info/SOURCES.txt` & `matgl-0.4.0/matgl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,10 +32,11 @@
 matgl/layers/_readout.py
 matgl/layers/_three_body.py
 matgl/models/__init__.py
 matgl/models/_m3gnet.py
 matgl/models/_megnet.py
 matgl/utils/__init__.py
 matgl/utils/cutoff.py
+matgl/utils/io.py
 matgl/utils/maths.py
-matgl/utils/remote.py
-matgl/utils/sb_roots.npy
+matgl/utils/sb_roots.npy
+matgl/utils/training.py
```

### Comparing `matgl-0.3.0/pyproject.toml` & `matgl-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
 requires = [
-     # pin NumPy version used in the build
-     "oldest-supported-numpy",
-     "setuptools>=58.0.3"
+  # pin NumPy version used in the build
+  "oldest-supported-numpy",
+  "setuptools>=58.0.3",
 ]
 build-backend = "setuptools.build_meta"
 numpy = "1.24.2"
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
 include = '\.pyi?$'
 exclude = '''
-
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
     | \.mypy_cache
     | \.tox
@@ -31,89 +30,71 @@
 '''
 
 [tool.ruff]
 target-version = "py39"
 line-length = 120
 select = [
   "B",   # flake8-bugbear
-  "C40", # flake8-comprehensions
-  # "D",   # pydocstyle
-  "E",   # pycodestyle
+  "C4",  # flake8-comprehensions
+  "D",   # pydocstyle
+  "E",   # pycodestyle error
+  "EXE", # flake8-executable
   "F",   # pyflakes
   "I",   # isort
-  "PLE", # pylint error
-  "PLW", # pylint warning
+  "ICN", # flake8-import-conventions
+  "ISC", # flake8-implicit-str-concat
+  "PD",  # pandas-vet
+  "PIE", # flake8-pie
+  "PL",  # pylint
+  "PT",  # flake8-pytest-style
+  "PYI", # flakes8-pyi
   "Q",   # flake8-quotes
+  "RET", # flake8-return
+  "RSE", # flake8-raise
   "RUF", # Ruff-specific rules
   "SIM", # flake8-simplify
   "TID", # tidy imports
+  "TID", # flake8-tidy-imports
   "UP",  # pyupgrade
-  "W",   # pycodestyle
+  "W",   # pycodestyle warning
   "YTT", # flake8-2020
 ]
 ignore = [
   "B019",    # functools.lru_cache on methods can lead to memory leaks
-  "B023",    # Function definition does not bind loop variable
-  "B028",    # No explicit stacklevel keyword argument found
-  "B904",    # Within an except clause, raise exceptions with ...
   "D100",    # Missing docstring in public module
   "D104",    # Missing docstring in public package
   "D105",    # Missing docstring in magic method
   "D107",    # Missing docstring in __init__
   "D200",    # One-line docstring should fit on one line with quotes
   "D205",    # 1 blank line required between summary line and description
   "D212",    # Multi-line docstring summary should start at the first line
   "D415",    # First line should end with a period, question mark, or exclamation point
-  "PLR2004", # Magic number
+  "PLR",     # pylint refactor
   "PLW0603", # Using the global statement to update variables is discouraged
-  "PLW2901", # Outer for loop variable overwritten by inner assignment target
+  "PLW2901", # redefined-loop-name
+  "RET504",  # unnecessary-assign
   "SIM105",  # Use contextlib.suppress(OSError) instead of try-except-pass
-  "SIM115",  # Use context handler for opening files
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
-exclude = [
-    ".eggs",
-    ".git",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-    "examples"
-]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "*/tests/*" = ["D"]
 "tasks.py" = ["D"]
 
 [tool.pytest.ini_options]
 addopts = "--durations=30 --quiet -rXs --color=yes -p no:warnings"
 
 [tool.mypy]
 ignore_missing_imports = true
 explicit_package_bases = true
 no_implicit_optional = false
-exclude = ['tests', 'examples']
+exclude = ['examples', 'tests']
 
 [[tool.mypy.overrides]]
-module = ["tabulate.*", "requests.*"]
+module = ["requests.*", "tabulate.*"]
 ignore_missing_imports = true
 
 [tool.codespell]
-ignore-words-list = """
-titel,alls,ans,nd,mater,nwo,te,hart,ontop,ist,ot,fo,nax,coo,coul,ser,leary,thre,
-fase,rute,reson,titels,ges,scalr,strat,struc,hda,nin,ons,pres,kno,loos,lamda
-"""
-skip = "pymatgen/analysis/aflow_prototypes.json"
+ignore-words-list = "mater,te,nd"
 check-filenames = true
```

### Comparing `matgl-0.3.0/setup.py` & `matgl-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import os
 import re
 
-import numpy
+import numpy as np
 from setuptools import find_packages, setup
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
@@ -41,27 +41,28 @@
     ],
     packages=find_packages(),
     package_data={
         "matgl": ["*.json", "*.md"],
         "matgl.utils": ["*.npy"],
     },
     include_package_data=True,
-    install_requires=(
-        "torch",
-        "dgl",
-    ),
+    install_requires=("torch", "dgl"),
+    extras_require={
+        "munch": ["munch"],
+        "pymatgen": ["pymatgen"],
+    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    include_dirs=[numpy.get_include()],
+    include_dirs=[np.get_include()],
 )
```

