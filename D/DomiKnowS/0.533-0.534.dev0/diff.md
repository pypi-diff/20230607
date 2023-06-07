# Comparing `tmp/DomiKnowS-0.533.tar.gz` & `tmp/DomiKnowS-0.534.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DomiKnowS-0.533.tar", last modified: Sat Apr 15 03:29:10 2023, max compression
+gzip compressed data, was "DomiKnowS-0.534.dev0.tar", last modified: Wed Jun  7 01:14:54 2023, max compression
```

## Comparing `DomiKnowS-0.533.tar` & `DomiKnowS-0.534.dev0.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/DomiKnowS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 03:29:10.608038 DomiKnowS-0.533/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-15 03:28:05.000000 DomiKnowS-0.533/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/compiler/OntologyMLGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/data/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/allennlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/graph/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)   107933 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/dataNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/dataNodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/logicalConstrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/program/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/batchprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/callbackprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/lossprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/program/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/ilpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/iml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/lossModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/learnerModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/query_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/relation_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/sensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/torch/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/torch/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/solver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/allennlpInferenceSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/allennlplogInferenceSolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/solver/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/constructor/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/dummyILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gekkoILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gekkoILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gurobiILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)   107605 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gurobiILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpBooleanMethodsCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpOntSolverFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/lcLossBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/lcLossSampleBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/mini_solver_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/solver/session/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/session/gurobi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/session/solver_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:29:10.608038 DomiKnowS-0.533/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-15 03:28:05.000000 DomiKnowS-0.533/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.428527 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.428527 DomiKnowS-0.534.dev0/domiknows/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/compiler/OntologyMLGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/data/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/allennlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108201 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/dataNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/dataNodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/logicalConstrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.436528 DomiKnowS-0.534.dev0/domiknows/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/batchprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/callbackprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/lossprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.436528 DomiKnowS-0.534.dev0/domiknows/program/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/gbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/ilpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/iml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/lossModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.436528 DomiKnowS-0.534.dev0/domiknows/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learnerModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/query_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/relation_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/torch/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/torch/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/domiknows/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/allennlpInferenceSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/allennlplogInferenceSolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/domiknows/solver/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/constructor/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/dummyILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103195 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolverFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/lcLossBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/lcLossSampleBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/mini_solver_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/domiknows/solver/session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/session/gurobi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/session/solver_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/setup.py
```

### Comparing `DomiKnowS-0.533/DomiKnowS.egg-info/PKG-INFO` & `DomiKnowS-0.534.dev0/DomiKnowS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.533
+Version: 0.534.dev0
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.533/DomiKnowS.egg-info/SOURCES.txt` & `DomiKnowS-0.534.dev0/DomiKnowS.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 domiknows/compiler/compiler.py
 domiknows/data/__init__.py
 domiknows/data/reader.py
 domiknows/data/allennlp/__init__.py
 domiknows/data/allennlp/reader.py
 domiknows/graph/__init__.py
 domiknows/graph/base.py
+domiknows/graph/candidates.py
 domiknows/graph/concept.py
 domiknows/graph/dataNode.py
 domiknows/graph/dataNodeConfig.py
 domiknows/graph/graph.py
 domiknows/graph/logicalConstrain.py
 domiknows/graph/property.py
 domiknows/graph/relation.py
@@ -38,14 +39,15 @@
 domiknows/program/lossprogram.py
 domiknows/program/metric.py
 domiknows/program/model_program.py
 domiknows/program/program.py
 domiknows/program/tracker.py
 domiknows/program/model/__init__.py
 domiknows/program/model/base.py
+domiknows/program/model/gbi.py
 domiknows/program/model/ilpu.py
 domiknows/program/model/iml.py
 domiknows/program/model/lossModel.py
 domiknows/program/model/pytorch.py
 domiknows/program/model/torch.py
 domiknows/sensor/__init__.py
 domiknows/sensor/learner.py
```

### Comparing `DomiKnowS-0.533/PKG-INFO` & `DomiKnowS-0.534.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.533
+Version: 0.534.dev0
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.533/domiknows/base.py` & `DomiKnowS-0.534.dev0/domiknows/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/compiler/OntologyMLGraph.py` & `DomiKnowS-0.534.dev0/domiknows/compiler/OntologyMLGraph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/data/allennlp/reader.py` & `DomiKnowS-0.534.dev0/domiknows/data/allennlp/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/data/reader.py` & `DomiKnowS-0.534.dev0/domiknows/data/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/allennlp/base.py` & `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/allennlp/metrics.py` & `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/metrics.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/allennlp/model.py` & `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/model.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/allennlp/utils.py` & `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/base.py` & `DomiKnowS-0.534.dev0/domiknows/graph/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/concept.py` & `DomiKnowS-0.534.dev0/domiknows/graph/concept.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/dataNode.py` & `DomiKnowS-0.534.dev0/domiknows/graph/dataNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 from collections import OrderedDict, namedtuple
-from  time import process_time_ns
+from time import process_time_ns
 import re
+
 from .dataNodeConfig import dnConfig 
 
 from ordered_set import OrderedSet 
 
 from domiknows import getRegrTimer_logger, getProductionModeStatus
-from domiknows.graph.logicalConstrain import eqL
 from domiknows.solver import ilpOntSolverFactory
 
 import logging
 from logging.handlers import RotatingFileHandler
 from .property import Property
 from .concept import Concept, EnumConcept
 
@@ -72,14 +72,16 @@
 # Class representing single data instance with relation links to other data nodes
 class DataNode:
     def __init__(self, instanceID = None, instanceValue = None, ontologyNode = None, relationLinks = {}, attributes = {}):
 
         self.instanceID = instanceID                     # The data instance id (e.g. paragraph number, sentence number, phrase  number, image number, etc.)
         self.instanceValue = instanceValue               # Optional value of the instance (e.g. paragraph text, sentence text, phrase text, image bitmap, etc.)
         self.ontologyNode = ontologyNode                 # Reference to the node in the ontology graph (e.g. Concept) which is the type of this instance (e.g. paragraph, sentence, phrase, etc.)
+        
+        self.graph =  self.ontologyNode.sup
         if relationLinks:
             self.relationLinks = relationLinks           # Dictionary mapping relation name to RealtionLinks
         else:
             self.relationLinks = {}
             
         self.impactLinks = {}                            # Dictionary with dataNodes impacting this dataNode by having it as a subject of its relation
         
@@ -811,88 +813,14 @@
             
             resultForCurrent = self.__getRelationAttrNames(_conceptRelation, usedGraph)
             
             if bool(resultForCurrent):
                 return resultForCurrent
         
         return None 
-    
-    # Find DataNodes starting from the given DataNode following provided path
-    #     path can contain eqL statement selecting DataNodes from the DataNodes collecting on the path
-    def getEdgeDataNode(self, path):
-        # Path is empty
-        if isinstance(path, eqL):
-            path = [path]
-        if len(path) == 0:
-            return [self]
-
-        # Path has single element
-        if (not isinstance(path[0], eqL)) and len(path) == 1:
-            relDns = self.getDnsForRelation(path[0])
-                    
-            if relDns is None or len(relDns) == 0 or relDns[0] is None:
-                return [None]
-            
-            return relDns
-                
-        # Path has at least 2 elements - will perform recursion
-
-        if isinstance(path[0], eqL): # check if eqL
-            path0 = path[0].e[0][0]
-        else:
-            path0 = path[0]
-
-        relDns = None         
-        if self.isRelation(path0):
-            relDns = self.getDnsForRelation(path0)
-        else: # if not relation then has to be attribute in eql
-            attributeValue = self.getAttribute(path[0].e[1]).item()
-            requiredValue = path[0].e[2]
-             
-            if attributeValue in requiredValue:
-                return [self]
-            elif (True in  requiredValue ) and attributeValue == 1:
-                return [self]
-            elif (False in  requiredValue ) and attributeValue == 0:
-                attributeValue = False
-            else:
-                return [None]
-          
-        # Check if it is a valid relation link  with not empty set of connected datanodes      
-        if relDns is None or len(relDns) == 0 or relDns[0] is None:
-            return [None]
-            relDns = []
-            
-        # if eqL then filter DataNode  
-        if isinstance(path[0], eqL):
-            _cDns = []
-            for cDn in relDns:
-                if isinstance(path[0].e[1], str):
-                    path0e1 = path[0].e[1]
-                else:
-                    path0e1 = path[0].e[1].name
-                    
-                if path0e1 in cDn.attributes or ("rootDataNode" in cDn.attributes and (path0.name + "/" + path0e1) in cDn.attributes["rootDataNode"].attributes["propertySet"]):
-                    if cDn.getAttribute(path0e1).item() in path[0].e[2]:
-                        _cDns.append(cDn)
-                    
-            relDns = _cDns
-        
-        # recursion
-        rDNS = []
-        for cDn in relDns:
-            rDn = cDn.getEdgeDataNode(path[1:])
-            
-            if rDn:
-                rDNS.extend(rDn)
-                
-        if rDNS:
-            return rDNS
-        else:
-            return [None]
 
     # cache
     collectedConceptsAndRelations = None
     
     # Collect all the concepts and relation from the data graph and translate them to tuple form
     def collectConceptsAndRelations(self, conceptsAndRelations = None):
         if conceptsAndRelations is None:
@@ -1080,55 +1008,83 @@
                 if keySoftMax not in dn.attributes:
                     dn.attributes[keySoftMax] = torch.empty(c[3], dtype=torch.float)
                     
                 dnSoftmax = tExp[dn.getInstanceID()]/tExpSum
                 dn.attributes[keySoftMax][c[2]] = dnSoftmax.item()
 
     # Calculate local for datanote argMax and softMax
-    def inferLocal(self):
+    def inferLocal(self, keys=("softmax", "argmax")):
         conceptsRelations = self.collectConceptsAndRelations() 
-        
+                
         for c in conceptsRelations:
             cRoot = self.findRootConceptOrRelation(c[0])
             dns = self.findDatanodes(select = cRoot)
             
             if not dns:
                 continue
             
             vs = []
             
             for dn in dns:
-                keySoftmax = "<" + c[0].name + ">/local/softmax"
-                if keySoftmax in dn.attributes:
-                    continue
+                if "softmax" in keys or "normalizedProb" in keys:
+                    keySoftmax = "<" + c[0].name + ">/local/softmax"
+                    if not keySoftmax in dn.attributes: # Already calculated ?                    
+                        v = dn.getAttribute(c[0])
+                        
+                        # check if v is None or not a tensor
+                        if v is None or not torch.is_tensor(v):
+                            continue
+                        
+                        if not(isinstance(v, torch.FloatTensor) or isinstance(v, torch.cuda.FloatTensor)):
+                            v = v.float()
+                            
+                        vSoftmaxT = torch.nn.functional.softmax(v, dim=-1)
+                        
+                        # Replace nan with 1/len
+                        #for i, s in enumerate(vSoftmaxT):
+                        #   if s != s:
+                        #       vSoftmaxT[i] = 1/len(v)
+                        
+                        dn.attributes[keySoftmax] = vSoftmaxT
+                    else:
+                        vSoftmaxT = dn.getAttribute(keySoftmax)
                 
-                v = dn.getAttribute(c[0])
-                vSoftmaxT = torch.nn.functional.softmax(v, dim=-1)
+                if "normalizedProb" in keys:
+                    keyNormalizedProb = "<" + c[0].name + ">/local/normalizedProb"
+                    if not keyNormalizedProb in dn.attributes: # Already calculated ?   
+                        vSoftmaxT = dn.attributes[keySoftmax]
+                        
+                        # Clamps the softmax probabilities
+                        vector = torch.clamp(vSoftmaxT, min=1e-12, max=1 - 1e-12) 
+                        
+                        # Calculates their entropy;
+                        entropy = torch.distributions.Categorical(torch.log(vector)).entropy() / vector.shape[0]
+                        
+                        # Multiplies the reverse of entropy to the vector divided by its mean value. P
+                        vNormalizedProbT = (1/entropy.item()) * (vector/torch.mean(vector))
+                        
+                        dn.attributes[keyNormalizedProb] = vNormalizedProbT
                 
-                # Replace nan with 1/len
-                #for i, s in enumerate(vSoftmaxT):
-                #   if s != s:
-                #       vSoftmaxT[i] = 1/len(v)
-                
-                dn.attributes[keySoftmax] = vSoftmaxT
-                
-                keyArgmax  = "<" + c[0].name + ">/local/argmax"
-                vArgmax = torch.clone(v)
-                vArgmaxIndex = torch.argmax(v).item()
-                
-                for i, _ in enumerate(v):
-                    if i == vArgmaxIndex:
-                        vArgmax[i] = 1
-                    else:
-                        vArgmax[i] = 0
-                                
-                dn.attributes[keyArgmax] = vArgmax
+                if "argmax" in keys:
+                    keyArgmax  = "<" + c[0].name + ">/local/argmax"
+                    v = dn.getAttribute(c[0])
+                    vArgmax = torch.clone(v)
+                    vArgmaxIndex = torch.argmax(v).item()
+                    
+                    for i, _ in enumerate(v):
+                        if i == vArgmaxIndex:
+                            vArgmax[i] = 1
+                        else:
+                            vArgmax[i] = 0
+                                    
+                    dn.attributes[keyArgmax] = vArgmax
+                    
         
     # Calculate ILP prediction for data graph with this instance as a root based on the provided list of concepts and relations
-    def inferILPResults(self, *_conceptsRelations, fun=None, epsilon = 0.00001, minimizeObjective = False, ignorePinLCs = False):
+    def inferILPResults(self, *_conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001, minimizeObjective = False, ignorePinLCs = False):
         if len(_conceptsRelations) == 0:
             _DataNode__Logger.info('Called with empty list of concepts and relations for inference')
         else:
             _DataNode__Logger.info('Called with - %s - list of concepts and relations for inference'%([x.name if isinstance(x, Concept) else x for x in _conceptsRelations]))
             
         # Check if concepts and/or relations have been provided for inference, if provide translate then to tuple concept info form
         _conceptsRelations = self.collectConceptsAndRelations(_conceptsRelations) # Collect all concepts and relations from graph as default set
@@ -1140,16 +1096,32 @@
             _DataNode__Logger.info('Found - %s - as a set of concepts and relations for inference'%([x[1] if isinstance(x, tuple) else x for x in _conceptsRelations]))
                 
         myilpOntSolver, conceptsRelations = self.__getILPSolver(_conceptsRelations)
         
         # Call ilpOntsolver with the collected probabilities for chosen candidates
         _DataNode__Logger.info("Calling ILP solver")
         
-        self.inferLocal()
-        myilpOntSolver.calculateILPSelection(self, *conceptsRelations, fun=fun, epsilon = epsilon, minimizeObjective = minimizeObjective, ignorePinLCs = ignorePinLCs)    
+        if "local" in key:
+            keys = (key[1],)
+            self.inferLocal(keys=keys)
+            
+        myilpOntSolver.calculateILPSelection(self, *conceptsRelations, key=key, fun=fun, epsilon = epsilon, minimizeObjective = minimizeObjective, ignorePinLCs = ignorePinLCs)    
+        
+    def inferGBIResults(self, *_conceptsRelations, model, builder):
+        if len(_conceptsRelations) == 0:
+            _DataNode__Logger.info('Called with empty list of concepts and relations for inference')
+        else:
+            _DataNode__Logger.info('Called with - %s - list of concepts and relations for inference'%([x.name if isinstance(x, Concept) else x for x in _conceptsRelations]))
+            
+        # Check if concepts and/or relations have been provided for inference, if provide translate then to tuple concept info form
+        _conceptsRelations = self.collectConceptsAndRelations(_conceptsRelations) # Collect all concepts and relations from graph as default set
+
+        from domiknows.program.model.gbi import GBIModel
+        myGBIModel = GBIModel(self.graph, model)
+        myGBIModel.calculateGBISelection(builder, _conceptsRelations)
         
     # Calculate the percentage of results satisfying each logical constraint 
     def verifyResultsLC(self, key = "/local/argmax"):
                 
         myilpOntSolver, _ = self.__getILPSolver(conceptsRelations = self.collectConceptsAndRelations())
 
         self.inferLocal()
@@ -1598,15 +1570,15 @@
         isRoot = True    
         for _, iDnList in testedDn.impactLinks.items(): # Check if its impacts are connected to Dn in the new Root list
             if iDnList:
                 for iDn in iDnList:
                     if iDn in visitedDns:
                         continue
                     
-                    if not self.__isRootDn(iDn, checkedDns, visitedDns):
+                    if self.__isRootDn(iDn, checkedDns, visitedDns):
                         isRoot = False
                         break
                     
             if not isRoot:
                 break
             
         return isRoot
@@ -1698,15 +1670,15 @@
             # Find if all the needed attribute were initialized
             allAttrInit = True
             for relationAttributeName, _ in conceptInfo['relationAttrsGraph'].items():
                 if relationAttributeName not in relationAttrsCache:
                     allAttrInit = False
                     break
             
-            if allAttrInit: #Create links for the ralation DataNode
+            if allAttrInit: #Create links for the relation DataNode
                 # Find DataNodes connected by this relation based on graph definition
                 existingDnsForAttr = OrderedDict() # DataNodes for Attributes of the relation
                 for relationAttributeName, relationAttributeConcept in conceptInfo['relationAttrsGraph'].items():
                     _existingDnsForAttr = self.findDataNodesInBuilder(select = relationAttributeConcept.name)
                      
                     if _existingDnsForAttr:
                         existingDnsForAttr[relationAttributeName] = _existingDnsForAttr
@@ -1727,15 +1699,15 @@
                             isInRelation = candidate.item()
                             if isInRelation == 0:
                                 continue
                             
                             candidateDn = existingDnsForAttr[attribute][candidateIndex]
                             
                             if attributeIndex == 0:
-                                candidateDn.addRelationLink(relationName, relationDn)
+                                candidateDn.addRelationLink(attribute, relationDn)
                             
                             relationDn.addRelationLink(attribute, candidateDn)  
                             relationDn.attributes[keyDataName] = vInfo.value[relationDnIndex] # Add / /Update value of the attribute
                 
                 _DataNodeBulder__Logger.info('Create links between the relation %s and instance dataNode of types'%(conceptInfo['concept'].name))
             else:
                 # Just add the sensor value to relation DataNodes
@@ -1757,15 +1729,15 @@
  
             if len(existingDnsForRelation) != vInfo.len:
                 _DataNodeBulder__Logger.error('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
                 raise ValueError('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
  
             if len(existingDnsForRelationSorted) == 1:
                 if vInfo.dim == 0:
-                    existingDnsForRelationSorted[0].attributes[keyDataName] = vInfo.value.item() # Add / /Update value of the attribute
+                    existingDnsForRelationSorted[0].attributes[keyDataName] = vInfo.value # Add / /Update value of the attribute
             elif vInfo.dim > 0:
                 for i, rDn in existingDnsForRelationSorted.items(): # Loop through all relations links dataNodes
                     rDn.attributes[keyDataName] = vInfo.value[i] # Add / /Update value of the attribute
             else:
                 pass
 
     def __createInitialdDataNode(self, vInfo, conceptInfo, keyDataName):
@@ -2351,17 +2323,19 @@
     # Method returning constructed DataNode - the fist in the list
     def getDataNode(self, context="interference", device='auto'):
         self.__addGetDataNodeCounter()
         
         if context=="interference":
             if self.skeletonDataNode:
                 self.myLoggerTime.info("DataNode Builder is using skeleton datanode mode")
-            self.myLoggerTime.info("DataNode Builder the set method called - %i times"%(self['Counter_setitem']))
-            elapsedInMsDataNodeBuilder = sum(self['DataNodeTime'])/1000000
-            self.myLoggerTime.info(f"DataNode Builder used - {elapsedInMsDataNodeBuilder:.8f}ms")
+            if 'Counter' + '_setitem' in self:
+                self.myLoggerTime.info("DataNode Builder the set method called - %i times"%(self['Counter' + '_setitem']))
+            if 'DataNodeTime' in self:
+                elapsedInMsDataNodeBuilder = sum(self['DataNodeTime'])/1000000
+                self.myLoggerTime.info(f"DataNode Builder used - {elapsedInMsDataNodeBuilder:.8f}ms")
         
         if dict.__contains__(self, 'dataNode'):
             _dataNode = dict.__getitem__(self, 'dataNode')
             
             if len(_dataNode) > 0:  
                 returnDn = _dataNode[0]
                 
@@ -2413,17 +2387,19 @@
         _DataNodeBulder__Logger.error('Returning None - there are no dataNode')
         return None
     
     # Method returning all constructed DataNodes 
     def getBatchDataNodes(self):
         self.__addGetDataNodeCounter()
         
-        self.myLoggerTime.info("DataNode Builder the set method called - %i times"%(self['Counter_setitem']))
-        elapsedInMsDataNodeBuilder = sum(self['DataNodeTime'])/1000000
-        self.myLoggerTime.info(f"DataNode Builder used - {elapsedInMsDataNodeBuilder:.8f}ms")
+        if 'Counter' + '_setitem' in self:
+            self.myLoggerTime.info("DataNode Builder the set method called - %i times"%(self['Counter' + '_setitem' ]))
+        if 'DataNodeTime' in self:
+            elapsedInMsDataNodeBuilder = sum(self['DataNodeTime'])/1000000
+            self.myLoggerTime.info(f"DataNode Builder used - {elapsedInMsDataNodeBuilder:.8f}ms")
         
         if dict.__contains__(self, 'dataNode'):
             _dataNode = dict.__getitem__(self, 'dataNode')
             
             if len(_dataNode) > 0:  
                 
                 _DataNodeBulder__Logger.info('Returning %i dataNodes - %s'%(len(_dataNode),_dataNode))
```

### Comparing `DomiKnowS-0.533/domiknows/graph/graph.py` & `DomiKnowS-0.534.dev0/domiknows/graph/graph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/logicalConstrain.py` & `DomiKnowS-0.534.dev0/domiknows/graph/logicalConstrain.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 import logging
 import torch
 myLogger = logging.getLogger(ilpConfig['log_name'])
 ifLog =  ilpConfig['ifLog']
         
 V = namedtuple("V", ['name', 'v'], defaults= [None, None])
 
-class LogicalConstrain:
-    def __init__(self, *e, p=100, active = True, sampleEntries  = False, name = None):
-        self.headLC = True # Indicate that it is head constrain and should be process individually
-        self.active = active
-        self.sampleEntries = sampleEntries
-        
+class LcElement:
+    def __init__(self, *e,  name = None):
+        from .relation import IsA, HasA
+
         if not e:
-            myLogger.error("Logical Constraint initialized is empty")
-            raise LogicalConstrain.LogicalConstrainError("Logical Constraint initialized is empty")
+            myLogger.error("Logical Element initialized is empty")
+            raise LcElement.LcElementError("Logical Element initialized is empty")
         
         updatedE = []
         for _, eItem in enumerate(e):
-            if isinstance(eItem, (LogicalConstrain, Concept)):
+            if isinstance(eItem, (LcElement, Concept, HasA, IsA)):
                 updatedE.append(eItem)
             elif callable(eItem):
                 newEItem = eItem.__call__()
                 updatedE.extend(newEItem)
             elif isinstance(eItem, list):
                 updatedE.extend(eItem)
             else:
@@ -38,87 +36,99 @@
             if isinstance(eItem, Concept):
                 updatedE.append((eItem, eItem.name, None, 1))
             else:
                 updatedE.append(eItem)
                 
         self.e = updatedE
 
-        # -- Find the graph for this Logical Constraint - based on context defined in the concept used in constrain definition
+        # -- Find the graph for this Logical Element - based on context defined in the concept used in constraint definition
         self.graph = None
        
         conceptOrLc = None
         
         for _, eItem in enumerate(self.e):
-            if isinstance(eItem, LogicalConstrain):
+            if isinstance(eItem, (LcElement, HasA, IsA)):
                 conceptOrLc = eItem
                 break
-            elif isinstance(eItem, tuple):
-                conceptOrLc = eItem[0]
-                break
+            elif isinstance(eItem, tuple): # Concept
+                if isinstance(eItem[0], Concept):
+                    conceptOrLc = eItem[0]
+                    break
     
         if conceptOrLc is None:
-            myLogger.error("Logical Constraint is incorrect")
-            raise LogicalConstrain.LogicalConstrainError("Logical Constraint is incorrect")
+            myLogger.error("Logical Element is incorrect")
+            raise LcElement.LcElementError("Logical Element is incorrect")
             
         if isinstance(conceptOrLc, Concept):
             if self.__getContext(conceptOrLc):
                 self.graph = self.__getContext(conceptOrLc)[-1]
+        elif isinstance(conceptOrLc, (HasA, IsA)):
+            self.graph = conceptOrLc.graph
         elif isinstance(conceptOrLc, str):
             self.graph = None
         else:
             self.graph = conceptOrLc.graph
                 
         if self.graph == None:
-            myLogger.error("Logical Constraint initialized is not associated with graph")
-            raise LogicalConstrain.LogicalConstrainError("Logical Constraint initialized is not associated with graph")
+            myLogger.error("Logical Element initialized is not associated with graph")
+            raise LcElement.LcElementError("Logical Element initialized is not associated with graph")
                      
-        # Create Logical Constraint id based on number of existing Logical Constraint in the graph
+        # Create Logical Element id based on number of existing Logical Element in the graph
         self.lcName = "LC%i"%(len(self.graph.logicalConstrains))
         
         if name is not None:
             self.name = name
         else:
             self.name = self.lcName
+     
+    class LcElementError(Exception):
+        pass
+    
+    def __str__(self):
+        return self.__class__.__name__
+    
+    def __repr__(self):
+        return  self.lcName + '(' + self.__class__.__name__ + ')'
             
-        # Add the constrain to the graph
+    def __getContext(self, e):
+        if isinstance(e, LcElement):
+            return self.__getContext(e.e[0])
+        else:
+            return e._context
+
+class LogicalConstrain(LcElement):
+    def __init__(self, *e, p=100, active = True, sampleEntries  = False, name = None):
+        super().__init__(*e, name = name)
+        
+        self.headLC = True # Indicate that it is head constraint and should be process individually
+        self.active = active
+        self.sampleEntries = sampleEntries
+        
+        # Add the constraint to the graph
+        assert self.graph is not None
         self.graph.logicalConstrains[self.lcName] = self
-                
-        # Go though constrain, find nested constrains and change their property headLC to indicate that their are nested and should not be process individually
+        
+         # Go though constraint, find nested constrains and change their property headLC to indicate that their are nested and should not be process individually
         for e_item in self.e:
             if isinstance(e_item, LogicalConstrain):
                 e_item.headLC = False
                 
-        # Check soft constrain is activated though p - if certainty in the validity of the constrain or the user preference is provided by p
+        # Check soft constraint is activated though p - if certainty in the validity of the constraint or the user preference is provided by p
         if p < 0:
             self.p = 0
             myLogger.warning("%s Logical Constraint created with p equal %i sets it to 0"%(self.lcName,p))
         elif p > 100:
             self.p = 100
             myLogger.warning("%s Logical Constraint created with p equal %i sets it to 100"%(self.lcName,p))
         else:
             self.p = p
-     
-    class LogicalConstrainError(Exception):
-        pass
-    
-    def __str__(self):
-        return self.__class__.__name__
-    
-    def __repr__(self):
-        return  self.lcName + '(' + self.__class__.__name__ + ')'
-          
+        
     def __call__(self, model, myIlpBooleanProcessor, v): 
         pass 
-            
-    def __getContext(self, e):
-        if isinstance(e, LogicalConstrain):
-            return self.__getContext(e.e[0])
-        else:
-            return e._context
-       
+    
     def getLcConcepts(self):
         lcConcepts = set()
         
         for _, eItem in enumerate(self.e):
             if isinstance(eItem, V):
                 if eItem[1] and eItem[1][1]:
                     if isinstance(eItem[1][1], eqL):
@@ -129,29 +139,38 @@
             elif isinstance(eItem, LogicalConstrain):
                 lcConcepts.update(eItem.getLcConcepts())
             elif isinstance(eItem, tuple) and (len(eItem) == 4):
                 lcConcepts.add(eItem[0].name)
                 
         return lcConcepts
         
-    # Get string representation of  Logical Constraintt
+    # Get string representation of  Logical Constraint
     def strEs(self):
         strsE = []
         for _, eItem in enumerate(self.e):
             if isinstance(eItem, V):
                 new_V = []
                 if eItem[0] is not None:
                     new_V.append(eItem[0])
                     #if eItem[1] is not None: new_V.append(',')
                 if eItem[1]:
                     if isinstance(eItem[1], eqL):
                         strsE.append("eql")
                     else:
-                        from domiknows.graph import Relation
-                        new_v = [v if isinstance(v, (str, tuple, LogicalConstrain, Relation)) else v.name for v in eItem[1]]
+                        new_v = []
+                        for v in eItem[1]:
+                            if isinstance(v, (str, LogicalConstrain)):
+                                new_v.append(v)
+                            elif isinstance(v, (tuple)):
+                                v_tuple = [w if isinstance(w, (str, tuple, LogicalConstrain)) else w.name for w in v]
+                                new_v.append(v_tuple)
+                            else:
+                                new_v.append(v.name)
+
+                        #new_v = [v if isinstance(v, (str, tuple, LogicalConstrain)) else v.name for v in eItem[1]]
                         new_V.append("path={}".format(tuple(new_v)))
                 strsE.append("{}".format(tuple(new_V)))
             elif isinstance(eItem, Concept):
                 strsE.append(eItem.name)
             elif isinstance(eItem, LogicalConstrain):
                 strsE.append(eItem.__repr__())
             elif isinstance(eItem, tuple) and (len(eItem) == 4):
@@ -194,15 +213,15 @@
             for cv in currentILPVars:
                 singleVar = lcFun(model, cv, onlyConstrains = headConstrain)
                 cSingleVar.append(singleVar)
                 
             singleV.append(cSingleVar)
         
         if headConstrain:
-            if ifLog: myLogger.debug("%s Logical Constraint is the head constrain - only ILP constrain created"%(lcName))
+            if ifLog: myLogger.debug("%s Logical Constraint is the head constraint - only ILP constraint created"%(lcName))
         
         if model is not None:
             model.update()
         
         return singleV
     
     # Collects setups of ILP variables for logical methods calls for the created Logical Constraint - recursive method
@@ -312,38 +331,39 @@
                 tVars.append(lcFun(model, *t, onlyConstrains = headConstrain))
                 
             rVars.append(tVars)
         
         # Return results from created ILP constraints - 
         # None if headConstrain is True or no ILP constraint created, ILP variable representing the value of ILP constraint, loss calculated
         return rVars
-    
+
     def createILPCount(self, model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = "COUNT"):         
         try:
             lcVariableNames = [e for e in iter(v)]
         except StopIteration:
             pass
         
-        if cLimit== None:
-            cLimit
+        if cLimit == None:
+            cLimit = 1
+            
         lcVariableName0 = lcVariableNames[0] # First variable
         lcVariableSet0 =  v[lcVariableName0]
 
         zVars = [] # Output ILP variables
         
         for i, _ in enumerate(lcVariableSet0):
             varsSetup = []
 
             var = []
             for currentV in iter(v):
                 var.extend(v[currentV][i])
                 
             if len(var) == 0:
                 if not (headConstrain or integrate):
-                    varsSetup.append([None])
+                    zVars.append([None])
                     
                 continue
             
             if headConstrain or integrate:
                 varsSetup.extend(var)
             else:
                 varsSetup.append(var)
@@ -358,22 +378,27 @@
                                                              logicMethodName = logicMethodName)])
            
         if model is not None:
             model.update()
             
         return zVars
     
-    def createILPAccumulatedCount(self, model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = "COUNT"):         
+    def createILPAccumulatedCount(self, model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = "COUNT"):  
+        
+        # Ignore value of integrate
+        integrate = True
+               
         try:
             lcVariableNames = [e for e in iter(v)]
         except StopIteration:
             pass
         
-        if cLimit== None:
-            cLimit
+        if cLimit == None:
+            cLimit = 1
+            
         lcVariableName0 = lcVariableNames[0] # First variable
         lcVariableSet0 =  v[lcVariableName0]
 
         zVars = [] # Output ILP variables
         
         # Accumulate all variables
         varsSetup = []
@@ -392,16 +417,18 @@
             if headConstrain or integrate:
                 varsSetup.extend(var)
             else:
                 varsSetup.append(var)
              
         # -- Use ILP variable setup to create constrains   
         if headConstrain or integrate:
-            zVars.append([myIlpBooleanProcessor.countVar(model, *varsSetup, onlyConstrains = headConstrain, limitOp = cOperation, limit=cLimit, 
-                                                         logicMethodName = logicMethodName)])
+            r = myIlpBooleanProcessor.countVar(model, *varsSetup, onlyConstrains = headConstrain, limitOp = cOperation, limit=cLimit, 
+                                                     logicMethodName = logicMethodName)
+            for _ in lcVariableSet0:
+                zVars.append([r])
         else:
             for current_var in varsSetup:
                 zVars.append([myIlpBooleanProcessor.countVar(model, *current_var, onlyConstrains = headConstrain, limitOp = cOperation, limit=cLimit, 
                                                          logicMethodName = logicMethodName)])
        
         if model is not None:
             model.update()
@@ -481,14 +508,17 @@
         with torch.set_grad_enabled(myIlpBooleanProcessor.grad): 
             return self.createILPConstrains('Epq', myIlpBooleanProcessor.ifVar, model, v, headConstrain)
      
 # ----------------- Auxiliary
      
 class eqL(LogicalConstrain):
     def __init__(self, *e, active = True, sampleEntries = False, name = None):
+        #if e is len 2 and element index 1 is of type String
+        if len(e) == 2 and isinstance(e[1], str):
+            e = (e[0],  "instanceID", e[1])  
         LogicalConstrain.__init__(self, *e, p=100)
         self.headLC = False
     
 class fixedL(LogicalConstrain):
     def __init__(self, *e, p=100, active = True, sampleEntries = False, name = None):
         LogicalConstrain.__init__(self, *e, p=p, active=active, sampleEntries  = sampleEntries, name=name)
         
@@ -609,8 +639,19 @@
             cLimit = self.e[-1]
         else:
             cLimit = 1
             
         cOperation = '<='
         
         with torch.set_grad_enabled(myIlpBooleanProcessor.grad):
-            return self.createILPAccumulatedCount(model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = str(self))
+            return self.createILPAccumulatedCount(model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = str(self))
+        
+# ----------------- forall
+class forAllL(LogicalConstrain):
+    def __init__(self, *e, p=100, active = True, sampleEntries = False, name = None):
+        LogicalConstrain.__init__(self, *e, p=p, active=active, sampleEntries  = sampleEntries, name=name)
+        
+    def __call__(self, model, myIlpBooleanProcessor, v, headConstrain = False, integrate = False): 
+        with torch.set_grad_enabled(myIlpBooleanProcessor.grad):
+            return self.createILPConstrains('If', myIlpBooleanProcessor.ifVar, model, v, headConstrain)        
+    
+
```

### Comparing `DomiKnowS-0.533/domiknows/graph/property.py` & `DomiKnowS-0.534.dev0/domiknows/graph/property.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/graph/relation.py` & `DomiKnowS-0.534.dev0/domiknows/graph/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,18 @@
     @property
     def dst(self):
         return self._dst
 
     @dst.setter
     def dst(self, dst):
         self._dst = dst
+        
+    @property
+    def graph(self):
+        return self._sup
 
     def what(self):
         return {'src': self.src, 'dst': self.dst}
 
     __metaclass__ = abc.ABCMeta
 
     def set_apply(self, name, sub):
```

### Comparing `DomiKnowS-0.533/domiknows/graph/trial.py` & `DomiKnowS-0.534.dev0/domiknows/graph/trial.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/batchprogram.py` & `DomiKnowS-0.534.dev0/domiknows/program/batchprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/callbackprogram.py` & `DomiKnowS-0.534.dev0/domiknows/program/callbackprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/loss.py` & `DomiKnowS-0.534.dev0/domiknows/program/loss.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/lossprogram.py` & `DomiKnowS-0.534.dev0/domiknows/program/lossprogram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import logging
 import torch
 import numpy as np
 from tqdm import tqdm
 
+from domiknows.program.model.pytorch import SolverModel
+
+
 from .program import LearningBasedProgram, get_len
 from ..utils import consume, entuple, detuple
-from .model.lossModel import PrimalDualModel, SampleLosslModel
+from .model.lossModel import PrimalDualModel, SampleLossModel
 from .model.base import Mode
 
+from .model.gbi import GBIModel
+
 # Primal-dual need multiple backward through constraint loss.
 # It requires retain_graph=True.
 # Memory leak problem with `backward(create_graph=True)`
 # https://github.com/pytorch/pytorch/issues/4661#issuecomment-596526199
 # workaround with following functions based on `grad()`
 def backward(loss, parameters):
     parameters = list(parameters)
@@ -112,15 +117,16 @@
 
                 metricName = 'loss'
                 metricResult = self.model.loss
                     
                 if self.dbUpdate is not None:
                     self.dbUpdate(desc, metricName, metricResult)
                     
-            if self.cmodel.loss and self.cmodel.loss is not None:
+            if self.cmodel.loss is not None and  repr(self.cmodel.loss) == "'None'":
+                losSTr = str(self.cmodel.loss)
                 desc = name if self.epoch is None else f'Epoch {self.epoch} {name}'
                 self.logger.info(' - Constraint loss:')
                 self.logger.info(self.cmodel.loss)
 
                 metricName = 'Constraint_loss'
                 metricResult = self.cmodel.loss
 
@@ -151,17 +157,14 @@
                     if key == 'ILP':
                         ilpMetric = metric
 
                     if key == 'softmax':
                         softmaxMetric = metric
 #         super().call_epoch(name=name, dataset=dataset, epoch_fn=epoch_fn, **kwargs)
         
-
-    
-
     def train_epoch(
         self, dataset,
         c_lr=1,
         c_warmup_iters=10,  # warmup
         c_freq_increase=1,  # d
         c_freq_increase_freq=1,
         c_lr_decay=0,  # strategy
@@ -187,15 +190,19 @@
             if self.copt is not None:
                 self.copt.zero_grad()
             mloss, metric, *output = self.model(data)  # output = (datanode, builder)
             if iter < c_warmup_iters:
                 loss = mloss
             else:
                 closs, *_ = self.cmodel(output[1])
-                loss = mloss + self.beta * closs
+                if torch.is_nonzero(closs):
+                    loss = mloss + self.beta * closs
+                    self.logger.info('closs is not zero')
+                else:
+                    loss = mloss
             if self.opt is not None and loss:
                 loss.backward()
                 self.opt.step()
                 iter += 1
             if (
                 self.copt is not None and
                 loss and
@@ -272,15 +279,15 @@
     def __init__(self, graph, Model, beta=1, **kwargs):
         super().__init__(graph, Model, CModel=PrimalDualModel, beta=beta, **kwargs)
         
 class SampleLossProgram(LossProgram):
     logger = logging.getLogger(__name__)
 
     def __init__(self, graph, Model, beta=1, **kwargs):
-        super().__init__(graph, Model, CModel=SampleLosslModel, beta=beta, **kwargs)
+        super().__init__(graph, Model, CModel=SampleLossModel, beta=beta, **kwargs)
 
 
     def train(
         self,
         training_set,
         valid_set=None,
         test_set=None,
@@ -354,8 +361,20 @@
                 self.copt is not None and
                 loss
             ):
                 self.copt.step()
             
             yield (loss, metric, *output[:1])
 
-        c_session['iter'] = iter
+        c_session['iter'] = iter    
+        
+class GBIProgram(LossProgram):
+    logger = logging.getLogger(__name__)
+
+    def __init__(self, graph, Model, poi, beta=1, **kwargs):
+        mySolverModel= SolverModel(graph,
+                           poi=poi,
+                           inferTypes=['local/argmax', 'local/softmax'],
+                           metric={})
+        super().__init__(graph, Model, CModel=GBIModel, beta=beta, solver_model = mySolverModel, poi=poi, **kwargs)
+        from domiknows.utils import setDnSkeletonMode
+        setDnSkeletonMode(True)
```

### Comparing `DomiKnowS-0.533/domiknows/program/metric.py` & `DomiKnowS-0.534.dev0/domiknows/program/metric.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/model/ilpu.py` & `DomiKnowS-0.534.dev0/domiknows/program/model/ilpu.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/model/iml.py` & `DomiKnowS-0.534.dev0/domiknows/program/model/iml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 
 import torch
 
 from .pytorch import SolverModel
 from ...graph.concept import EnumConcept
 
-
+# Inference-Masked Loss
 class IMLModel(SolverModel):
     def poi_loss(self, data_item, prop, sensors):
         output_sensor, target_sensor = sensors
         logit = output_sensor(data_item)
         labels = target_sensor(data_item)
         if len(logit) == 0:
             return None
```

### Comparing `DomiKnowS-0.533/domiknows/program/model/lossModel.py` & `DomiKnowS-0.534.dev0/domiknows/program/model/lossModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     
 class PrimalDualModel(LossModel):
     logger = logging.getLogger(__name__)
 
     def __init__(self, graph, tnorm=DataNode.tnormsDefault, device='auto'):
         super().__init__(graph, tnorm=tnorm, device=device)
         
-class SampleLosslModel(torch.nn.Module):
+class SampleLossModel(torch.nn.Module):
     logger = logging.getLogger(__name__)
 
     # def __init__(self, graph, sample = False, sampleSize = 0, sampleGlobalLoss = False):
     #     super().__init__(graph, sample=sample, sampleSize=sampleSize, sampleGlobalLoss=sampleGlobalLoss)
 
     def __init__(self, graph, 
                  tnorm=DataNode.tnormsDefault, 
@@ -161,15 +161,15 @@
             
         if not build and not isinstance(builder, DataNodeBuilder):
             raise ValueError('PrimalDualModel must be invoked with `build` on or with provided DataNode Builder.')
         
         if (builder.needsBatchRootDN()):
             builder.addBatchRootDN()
         
-#         self.loss.reset()
+#       self.loss.reset()
 
         datanode = builder.getDataNode(device=self.device)
         
         # Call the loss calculation returns a dictionary, keys are matching the constraints
         constr_loss = datanode.calculateLcLoss(tnorm=self.tnorm, sample=self.sample, sampleSize = self.sampleSize, sampleGlobalLoss = self.sampleGlobalLoss)
         import math
         lmbd_loss = []
@@ -202,15 +202,15 @@
                         loss_ = -1 * torch.log(loss_value)
                         key_loss += loss_
 
                     else:
                         loss_ = 0
                     
                 else:
-                    if constr_loss["globalSuccessCountet"] > 0:
+                    if constr_loss["globalSuccessCounter"] > 0:
                         lcSuccesses = constr_loss["globalSuccesses"]
                     if lossTensor.sum().item() != 0:
                         tidx = (lcSuccesses == 1).nonzero().squeeze(-1)
                         true_val = lossTensor[tidx]
                         
                         if true_val.sum().item() != 0: 
                             if not replace_mul:
@@ -230,16 +230,14 @@
                             else:
                                 loss_value = true_val.logsumexp(dim=0) - lossTensor.logsumexp(dim=0)
                                 key_loss += -1 * loss_value
 
                         else:
                             loss_ = 0
                         
-                        
-
                         # if loss['lossTensor'].nansum().item() <= 1:
                         #     loss_value = loss['lossTensor']
                         #     # loss_value = loss_value[loss_value.nonzero()].squeeze(-1)
                         # else:
                         #     _idx = []
                         #     for i in torch.unique(loss['lossTensor']):
                         #         _idx.append((loss['lossTensor'] == i.item()).nonzero(as_tuple=True)[0][0].item())
@@ -265,15 +263,15 @@
         all_losses = [key_losses[key] for key in key_losses]
         if all_losses:
             all_losses = torch.stack(all_losses)
 
             satisfied_num = len( set(constr_loss.keys()) - set(key_losses.keys()) )
             unsatisfied_num = len(set(constr_loss.keys())) - satisfied_num
             #self.logger.info(f'-- number of satisfied constraints are {satisfied_num}')
-            #self.logger.info(f'-- number of unstatisfied constraints are {unsatisfied_num}')
+            #self.logger.info(f'-- number of unsatisfied constraints are {unsatisfied_num}')
             for key in key_losses:
                 if self.sampleSize != -1:
                     if replace_mul:
                         loss_val = (key_losses[key] / all_losses.sum()) * key_losses[key]
                     else:
                         loss_val = key_losses[key]
                 else:
```

### Comparing `DomiKnowS-0.533/domiknows/program/model/pytorch.py` & `DomiKnowS-0.534.dev0/domiknows/program/model/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,17 @@
             data_hash = data_hash or self.data_hash(data_item)
             sensor.fill_hash(data_hash)
         for sensor in self.graph.get_sensors(ReaderSensor):
             sensor.fill_data(data_item)
         if build:
             data_item.update({"graph": self.graph, 'READER': 0})
             builder = DataNodeBuilder(data_item)
+            *out, = self.populate(builder)
             if (builder.needsBatchRootDN()):
                 builder.addBatchRootDN()
-            *out, = self.populate(builder)
             datanode = builder.getDataNode(context="build", device=self.device)
             return (*out, datanode, builder)
         else:
             *out, = self.populate(data_item)
             return (*out,)
 
     def populate(self):
@@ -211,52 +211,56 @@
                         local_metric = self.poi_metric(builder, prop, sensors)
                         if local_metric is not None:
                             metric[(*sensors,)] = local_metric
         
         return loss, metric
 
 class SolverModel(PoiModel):
-    def __init__(self, graph, poi=None, loss=None, metric=None, inferTypes=None, inference_with = None, device='auto'):
+    def __init__(self, graph, poi=None, loss=None, metric=None, inferTypes=None, inference_with = None, probKey = ("local" , "softmax"), device='auto'):
         super().__init__(graph, poi=poi, loss=loss, metric=metric, device=device)
         
         if inferTypes == None:
             self.inferTypes = ['ILP']
         else:
             self.inferTypes = inferTypes
             
         if inference_with == None:
             self.inference_with = []
         else:
             self.inference_with = inference_with
+            
+        self.probKey = probKey
 
     def inference(self, builder):
-        for prop in self.poi:
+        for i, prop in enumerate(self.poi):
             for sensor in prop.find(TorchSensor):
                 sensor(builder)
 #             for output_sensor, target_sensor in self.find_sensors(prop):
 #             # make sure the sensors are evaluated
 #                 output = output_sensor(builder)
 #                 target = target_sensor(builder)
 #         print("Done with the computation")
 
         # Check if this is batch
         if (builder.needsBatchRootDN()):
             builder.addBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         # trigger inference
 #         fun=lambda val: torch.tensor(val, dtype=float).softmax(dim=-1).detach().cpu().numpy().tolist()
-        for infertype in self.inferTypes:
-            {
-                'ILP': lambda :datanode.inferILPResults(*self.inference_with, fun=None, epsilon=None),
-                'local/argmax': lambda :datanode.inferLocal(),
-                'local/softmax': lambda :datanode.inferLocal(),
-                'argmax': lambda :datanode.infer(),
-                'softmax': lambda :datanode.infer(),
-            }[infertype]()
-#         print("Done with the inference")
+        if datanode:
+            for infertype in self.inferTypes:
+                {
+                    'ILP': lambda :datanode.inferILPResults(*self.inference_with, key=self.probKey, fun=None, epsilon=None),
+                    'local/argmax': lambda :datanode.inferLocal(),
+                    'local/softmax': lambda :datanode.inferLocal(),
+                    'argmax': lambda :datanode.infer(),
+                    'softmax': lambda :datanode.infer(),
+                    'GBI': lambda :datanode.inferGBIResults(*self.inference_with, model=self, builder=builder),
+                }[infertype]()
+    #         print("Done with the inference")
         return builder
 
     def populate(self, builder, run=True):
         data_item = self.inference(builder)
         return super().populate(builder, run=False)
```

### Comparing `DomiKnowS-0.533/domiknows/program/model/torch.py` & `DomiKnowS-0.534.dev0/domiknows/program/model/torch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/program/model_program.py` & `DomiKnowS-0.534.dev0/domiknows/program/model_program.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from domiknows.utils import setDnSkeletonMode
 from .program import LearningBasedProgram
 from .model.pytorch import PoiModel, PoiModelToWorkWithLearnerWithLoss, SolverModel, SolverModelDictLoss
 from .model.iml import IMLModel
 
-
 class POIProgram(LearningBasedProgram):
     def __init__(self, graph, **kwargs):
         super().__init__(graph, PoiModel, **kwargs)
 
 
 class SolverPOIProgram(LearningBasedProgram):
     def __init__(self, graph, **kwargs):
         super().__init__(graph, SolverModel, **kwargs)
+        # Check if the 'inferTypes' is in the kwargs and has GBI then setDnSkeletonMode(True)
+        if 'inferTypes' in kwargs:         
+            if 'GBI' in kwargs['inferTypes']:
+                setDnSkeletonMode(True)
         
         
 class SolverPOIDictLossProgram(LearningBasedProgram):
     def __init__(self, graph, **kwargs):
         super().__init__(graph, SolverModelDictLoss, **kwargs)
```

### Comparing `DomiKnowS-0.533/domiknows/program/program.py` & `DomiKnowS-0.534.dev0/domiknows/program/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
                 self.call_epoch('Testing', test_set, self.test_epoch, **kwargs)
         if not test_every_epoch:
             self.call_epoch('Testing', test_set, self.test_epoch, **kwargs)
         # reset epoch after everything
         self.epoch = None
         self.stop = None
 
-    def train_epoch(self, dataset):
+    def train_epoch(self, dataset, **kwargs):
         self.model.mode(Mode.TRAIN)
         self.model.reset()
         for data_item in dataset:
             if self.opt is not None:
                 self.opt.zero_grad()
             loss, metric, *output = self.model(data_item)
             if self.opt and loss:
@@ -304,15 +304,15 @@
             yield (loss, metric, *output[:1])
 
     def test(self, dataset, device=None, **kwargs):
         if device is not None:
             self.to(device)
         self.call_epoch('Testing', dataset, self.test_epoch, **kwargs)
 
-    def test_epoch(self, dataset):
+    def test_epoch(self, dataset, **kwargs):
         self.model.mode(Mode.TEST)
         self.model.reset()
         with torch.no_grad():
             for data_item in dataset:
                 loss, metric, *output = self.model(data_item)
                 yield (loss, metric, *output[:1])
```

### Comparing `DomiKnowS-0.533/domiknows/program/tracker.py` & `DomiKnowS-0.534.dev0/domiknows/program/tracker.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/allennlp/base.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/allennlp/learner.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/allennlp/module.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/module.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/allennlp/sensor.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/learnerModels.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learnerModels.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/learners.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learners.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/query_sensor.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/query_sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/relation_sensors.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/relation_sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/sensors.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/spacy.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/transformers.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/pytorch/utils.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/sensor.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/torch/learner.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/torch/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/sensor/torch/sensor.py` & `DomiKnowS-0.534.dev0/domiknows/sensor/torch/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/allennlpInferenceSolver.py` & `DomiKnowS-0.534.dev0/domiknows/solver/allennlpInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/allennlplogInferenceSolver.py` & `DomiKnowS-0.534.dev0/domiknows/solver/allennlplogInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/constructor/constructor.py` & `DomiKnowS-0.534.dev0/domiknows/solver/constructor/constructor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/dummyILPOntSolver.py` & `DomiKnowS-0.534.dev0/domiknows/solver/dummyILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/gekkoILPBooleanMethods.py` & `DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/gekkoILPOntSolver.py` & `DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/gurobiILPBooleanMethods.py` & `DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPBooleanMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,26 +417,26 @@
     def ifVar(self, m, var1, var2, onlyConstrains = False):
         logicMethodName = "IF"
 
         # -- Consider None
         hasNone = False
         if var1 is None: # antecedent 
             antecedent = 1 # when None
-            self.myLogger.info("%s called with antecedent equals None"%(logicMethodName))
-            self.myLogger.info("%s called with consequent equals %s"%(logicMethodName,var2))
+            #self.myLogger.info("%s called with antecedent equals None"%(logicMethodName))
+            #self.myLogger.info("%s called with consequent equals %s"%(logicMethodName,var2))
 
             hasNone = True
         else:
             antecedent = var1
 
         if var2 is None: # consequent
             consequent = 0 # when None
             if not hasNone: # not yet
-                self.myLogger.info("%s called with antecedent equals %s"%(logicMethodName,var1))
-                self.myLogger.info("%s called with consequent equals None"%(logicMethodName))
+                #self.myLogger.info("%s called with antecedent equals %s"%(logicMethodName,var1))
+                #self.myLogger.info("%s called with consequent equals None"%(logicMethodName))
                 hasNone = True
         else:
             consequent = var2
         # --
     
         varsInfo = self.preprocessLogicalMethodVar((antecedent,consequent), logicMethodName, "if",  minN=2)
         
@@ -452,16 +452,19 @@
                     return 
                 elif consequent: # antecedent is True
                     # Applying if results in True
                     if self.ifLog: self.myLogger.debug("%s is True - antecedent and consequent are True"%(logicMethodName))
                     if hasNone: self.myLogger.info("%s is True - antecedent and consequent are True"%(logicMethodName))
                     return 
                 else: # antecedent and not consequent
-                    raise Exception("ILP model is infeasible - %s is called with the antecedent True and the consequent False - the result of applying %s is False"
-                                    %(logicMethodName,logicMethodName))
+                    self.myLogger.warn("%s is called with the antecedent True and the consequent False - the result of applying %s would be False making ILP model is infeasible - ignoring it"%(logicMethodName,logicMethodName))
+                    return
+                
+                    #raise Exception("ILP model is infeasible - %s is called with the antecedent True and the consequent False - the result of applying %s is False"
+                    #                %(logicMethodName,logicMethodName))
             elif self.__varIsNumber(antecedent): # antecedent is boolean and consequent is the ILP variable
                 if not antecedent:
                     # Applying if results in True
                     if self.ifLog: self.myLogger.debug("%s is True - antecedent is False"%(logicMethodName))
                     if hasNone: self.myLogger.info("%s is True - antecedent is False"%(logicMethodName))
                     return 
                 else: # antecedent is True
```

### Comparing `DomiKnowS-0.533/domiknows/solver/gurobiILPOntSolver.py` & `DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPOntSolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 from domiknows.graph.concept import Concept, EnumConcept
 from domiknows.solver.ilpOntSolver import ilpOntSolver
 from domiknows.solver.gurobiILPBooleanMethods import gurobiILPBooleanProcessor
 from domiknows.solver.lcLossBooleanMethods import lcLossBooleanMethods
 from domiknows.solver.lcLossSampleBooleanMethods import lcLossSampleBooleanMethods
 from domiknows.solver.ilpBooleanMethodsCalculator import booleanMethodsCalculator
 
-from domiknows.graph import LogicalConstrain, V, fixedL, ifL
-from _functools import reduce
+from domiknows.graph import LcElement, LogicalConstrain, V, fixedL, ifL, forAllL
+from domiknows.graph import CandidateSelection
 from domiknows.utils import getReuseModel
 
+from domiknows.graph.candidates import getCandidates
+
 class gurobiILPOntSolver(ilpOntSolver):
     ilpSolver = 'Gurobi'
 
     def __init__(self, graph, ontologiesTuple, _ilpConfig, reuse_model=False) -> None:
         super().__init__(graph, ontologiesTuple, _ilpConfig)
         self.myIlpBooleanProcessor = gurobiILPBooleanProcessor()
         self.myLcLossBooleanMethods = lcLossBooleanMethods()
@@ -58,44 +60,41 @@
     # Get Ground Truth for provided concept
     def __getLabel(self, dn, conceptRelation, fun=None, epsilon = None):
         value = dn.getAttribute(conceptRelation, 'label')
         
         return value
         
     # Get and calculate probability for provided concept
-    def __getProbability(self, dn, conceptRelation, fun=None, epsilon = 0.00001):
+    def getProbability(self, dn, conceptRelation, key = ("local" , "softmax"), fun=None, epsilon = 0.00001):
         if not dn:
             valueI = None
         else:
-            valueI = dn.getAttribute(conceptRelation, "local" , "softmax")
+            valueI = dn.getAttribute(conceptRelation, *key)
                     
-        if valueI is None: # No probability value - return negative probability 
-            return [float("nan"), float("nan")]
-        
-        if conceptRelation[2] is not None:
+        if conceptRelation[2] is not None: # This is mutliclass - need to convert it to binary for ILP 
             value = torch.empty(2, dtype=torch.float)
             
             value[0] = 1 - valueI[conceptRelation[2]]
             value[1] = valueI[conceptRelation[2]]
-        else:
+        else: # This is binary 
             value = valueI
 
         # Process probability through function and apply epsilon
         if epsilon is not None:
             if value[0] > 1-epsilon:
                 value[0] = 1-epsilon
             elif value[1] > 1-epsilon:
                 value[1] = 1-epsilon
                 
             if value[0] < epsilon:
                 value[0] = epsilon
             elif value[1] < epsilon:
                 value[1] = epsilon
                
-            # Apply fun on probabilities 
+            # Apply fun on probabilities if defined
             if fun is not None:
                 value = fun(value)
             
         return value # Return probability
     
     def countLCVariables(self, rootDn, *conceptsRelations):
         # Collect LC variables 
@@ -116,15 +115,15 @@
             ilpVarCount[currentConceptName] = len(dns)
             
             if currentConceptRelation[2] is None:
                 ilpVarCount[currentConceptName] += len(dns)
        
         return ilpVarCount
     
-    def createObjective(self, xDict, rootDn, *conceptsRelations, dnFun = None, fun=None, epsilon = 0.00001):
+    def createObjective(self, xDict, rootDn, *conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001):
         Q = None
         conceptToDNSCash = {}        
         
         x = list(xDict.values())
         index = 0
         for currentConceptRelation in conceptsRelations: 
             currentName = currentConceptRelation[0]
@@ -136,15 +135,15 @@
                 dns = rootDn.findDatanodes(select = rootConcept)
                 conceptToDNSCash[currentName] = dns
        
             for dn in dns:
                 if x[index] == None:
                     continue
                 
-                currentProbability = dnFun(dn, currentConceptRelation, fun=fun, epsilon=epsilon)
+                currentProbability = self.getProbability(dn, currentConceptRelation, key=key, fun=fun, epsilon=epsilon)
                 
                 if currentProbability == None or (torch.is_tensor(currentProbability) and currentProbability.dim() == 0) or len(currentProbability) < 2:
                     self.myLogger.warning("Probability not provided for variable concept %s in dataNode %s - skipping it"%(currentName,dn.getInstanceID()))
                     x[index] = None
                 
                 # Check if probability is NaN or if and has to be skipped
                 elif self.valueToBeSkipped(currentProbability[1]):
@@ -170,15 +169,15 @@
                                            %(dn.getInstanceID(), currentName, currentProbability[1]))
                         
                     Q += currentProbability[0] * x[index] 
                     index += 1  
            
         return Q
     
-    def createILPVariables(self, m, x, rootDn, *conceptsRelations, dnFun = None, fun=None, epsilon = 0.00001):
+    def createILPVariables(self, m, x, rootDn, *conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001):
         Q = None
         
         # Create ILP variables 
         for currentConceptRelation in conceptsRelations: 
             rootConcept = rootDn.findRootConceptOrRelation(currentConceptRelation[0])
             dns = rootDn.findDatanodes(select = rootConcept)
             xkey = '<' + currentConceptRelation[0].name + '>/ILP/x'  
@@ -192,15 +191,15 @@
                     
                 if currentConceptRelation[2] is None:
                     if currentConceptRelation[2] is not None:
                         x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]] = None
                     else:
                         x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), 0] = None
                         
-                currentProbability = dnFun(dn, currentConceptRelation, fun=fun, epsilon=epsilon)
+                currentProbability = self.getProbability(dn, currentConceptRelation, key=key, fun=fun, epsilon=epsilon)
                 
                 if currentProbability == None or (torch.is_tensor(currentProbability) and currentProbability.dim() == 0) or len(currentProbability) < 2:
                     self.myLogger.warning("Probability not provided for variable concept %s in dataNode %s - skipping it"%(currentConceptRelation[0].name,dn.getInstanceID()))
                     continue
                 
                 # Check if probability is NaN or if and has to be skipped
                 if self.valueToBeSkipped(currentProbability[1]):
@@ -298,15 +297,15 @@
             
             if c[0] not in multiclassDict:
                 multiclassDict[c[0]] = []
             
             multiclassDict[c[0]].append(c)
             
         for mc in multiclassDict:
-            # Add constrain which restrict number of muliclass labels assigned to one for the given instance
+            # Add constraint which restrict number of muliclass labels assigned to one for the given instance
             rootConcept = rootDn.findRootConceptOrRelation(mc)
             dns = rootDn.findDatanodes(select = rootConcept)
             xkey = '<' + mc.name + '>/ILP/x'  
             
             for dn in dns:
                 var = []
                 for mlabel in multiclassDict[mc]: 
@@ -926,46 +925,84 @@
             if vDnLabel == -100:
                 return None
             elif vDnLabel == i:
                 return 1
             else:
                 return 0
         
-    def __constructLogicalConstrains(self, lc, booleanProcesor, m, dn, p, key = None, lcVariablesDns = None, headLC = False, loss = False, sample = False, vNo = None, verify=False):
+        
+    def __addLossTovDns(self, loss, vDns):
+        if loss and vDns:
+            vDnsOriginal = vDns
+            vDnsList = [v[0] for v in  vDns]
+            
+            updatedVDns = []
+            try:
+                if len(vDnsList) > 1:
+                    tStack = torch.stack(vDnsList, dim=1)
+                else:
+                    tStack = vDnsList[0]
+                tsqueezed = torch.squeeze(tStack, dim=0)
+
+            except IndexError as ie:
+                tsqueezed = torch.stack(vDnsList, dim=0)
+                pass
+        
+            if not len(tsqueezed.shape):
+                tsqueezed = torch.unsqueeze(tsqueezed, 0)
+                
+            tList = [tsqueezed]
+            updatedVDns.append(tList)
+            
+            return updatedVDns
+        else:
+            return vDns
+    
+    def __constructLogicalConstrains(self, lc, booleanProcessor, m, dn, p, key = None, lcVariablesDns = None, headLC = False, loss = False, sample = False, vNo = None, verify=False):
         if key == None:
             key = ""
+            
         if lcVariablesDns == None:
             lcVariablesDns = OrderedDict()
             
         lcVariables = OrderedDict()
+        
         if sample:
             sampleInfo = OrderedDict()
             lcVariablesSet = OrderedDict()
+            
         if vNo == None:
             vNo = [1, 1]
         
         firstV = None
         integrate = False
         
         for eIndex, e in enumerate(lc.e): 
             if  isinstance(e, V):
                 continue # Already processed in the previous Concept 
             
-            if isinstance(e, (Concept,  LogicalConstrain, tuple)): 
+            if isinstance(e, (Concept,  LcElement, tuple)): 
                 # Look one step ahead in the parsed logical constraint and get variables names (if present) after the current concept
                 if eIndex + 1 < len(lc.e) and isinstance(lc.e[eIndex+1], V):
                     variable = lc.e[eIndex+1]
                 else:
                     if isinstance(e, LogicalConstrain):
                         variable = V(name="_lc" + str(vNo[1]))
                         vNo[1] += 1
+                    elif isinstance(e, tuple) and isinstance(e[0], CandidateSelection):
+                        e[0].CandidateSelectionVariable = e[1]
+                        e = e[0]
+                        
+                        variable = V(name="_cs" + str(vNo[1]))
+                        vNo[1] += 1
                     else:
                         if firstV == None:
                             variable = V(name="_x" + str(vNo[0]) )
-                            firstV = variable.name
+                            if not isinstance(lc, CandidateSelection):
+                                firstV = variable.name
                             vNo[0] += 1
                         else:
                             variable = V(name="_x" + str(vNo[0]), v = (firstV,))
                             vNo[0] += 1
                     
                 if variable.name:
                     variableName = variable.name
@@ -980,135 +1017,24 @@
                     lcVariablesDns[newvVariableName] = lcVariablesDns[variableName]
                     if None in lcVariablesDns:
                         pass
   
                     lcVariables[newvVariableName] = lcVariables[variableName]
 
                 elif isinstance(e, (Concept, tuple)): # -- Concept 
-                    conceptName = e[0].name
-                        
-                    # -- Collect dataNode for the logical constraint (path)
-                    
-                    dnsList = [] # Stores lists of dataNodes for each corresponding dataNode 
-                    
-                    if variable.v == None: # No path - just concept
-                        if variable.name == None:
-                            self.myLogger.error('The element %s of logical constraint %s has no name for variable'%(conceptName, lc.lcName))
-                            return None
-                                                 
-                        rootConcept = dn.findRootConceptOrRelation(conceptName)
-                        _dns = dn.findDatanodes(select = rootConcept)
-                        dnsList = [[dn] for dn in _dns]
-                    else: # Path specified
-                        from domiknows.graph.logicalConstrain import eqL
-                        if not isinstance(variable.v, eqL):
-                            if len(variable.v) == 0:
-                                self.myLogger.error('The element %s of logical constraint %s has empty part v of the variable'%(conceptName, lc.lcName))
-                                return None
-                          
-                        # -- Prepare paths
-                        path = variable.v
-                        paths = []
-                        
-                        if isinstance(path, eqL):
-                            paths.append(path)
-                        elif isinstance(path[0], str) and len(path) == 1:
-                            paths.append(path)
-                        elif isinstance(path[0], str) and not isinstance(path[1], tuple):
-                            paths.append(path)
-                        else: # If many paths
-                            for i, vE in enumerate(variable.v):
-                                if i == 0 and isinstance(vE, str):
-                                    continue
-                                
-                                paths.append(vE)
-                                
-                        pathsCount = len(paths)
-                        
-                        # -- Process  paths
-                        dnsListForPaths = []
-                        for i, v in enumerate(paths):
-                            dnsListForPaths.append([])
-                            
-                            # Get name of the referred variable 
-                            if isinstance(path, eqL):
-                                referredVariableName = None
-                            else:
-                                referredVariableName = v[0] 
-                        
-                            if referredVariableName not in lcVariablesDns: # Not yet defined - it has to be the current lc element dataNodes list
-                                rootConcept = dn.findRootConceptOrRelation(conceptName)
-                                _dns = dn.findDatanodes(select = rootConcept)
-                                referredDns = [[dn] for dn in _dns]
-                                integrate = True
-                            else: # already defined in the logical constraint from the v part 
-                                referredDns = lcVariablesDns[referredVariableName] # Get DataNodes for referred variables already defined in the logical constraint
-                                
-                            # Get variables from dataNodes selected  based on referredVariableName
-                            for listOfDataNodes in referredDns:
-                                eDns = [] 
-                                
-                                for currentReferredDataNode in listOfDataNodes:
-                                    if currentReferredDataNode is None:
-                                        continue
-                                    
-                                    # -- Get DataNodes for the edge defined by the path part of the v
-                                    if isinstance(path, eqL):
-                                        _eDns = currentReferredDataNode.getEdgeDataNode(v) 
-                                    else:
-                                        _eDns = currentReferredDataNode.getEdgeDataNode(v[1:]) 
-                                    
-                                    if _eDns and _eDns[0]:
-                                        eDns.extend(_eDns)
-                                    elif not isinstance(path, eqL):
-                                        vNames = [v if isinstance(v, str) else v.name for v in v[1:]]
-                                        if lc.__str__() != "fixedL":
-                                            self.myLogger.info('%s has no path %s requested by %s for concept %s'%(currentReferredDataNode, vNames, lc.lcName, conceptName))
-                                if not eDns:
-                                    eDns = [None] # None - to keep track of candidates
-                                    
-                                dnsListForPaths[i].append(eDns)
-                           
-                        # -- Select a single dns list or Combine the collected lists of dataNodes based on paths 
-                        dnsList = []
-                        newIntersection = True
-                        if newIntersection:
-                            if pathsCount == 1: # Single path
-                                dnsList = dnsListForPaths[0]
-                            else:
-                                # --- Assume Intersection - TODO: in future use lo if defined to determine if different operation                                
-                                for i in range(len(dnsListForPaths[0])):
-                                    try:
-                                        se = [set(dnsListForPaths[item][i]) for item in range(pathsCount)]
-                                    except IndexError as ei:
-                                        continue
-                                    dnsListR = reduce(set.intersection, se)
-                                    dnsList.append(list(dnsListR))
-                        else:
-                            dnsList = dnsListForPaths[0]
-                           
-                            # -- Combine the collected lists of dataNodes based on paths 
-                            for l in dnsListForPaths[1:]:
-                                # --- Assume Intersection - TODO: in future use lo if defined to determine if different  operation
-                                _d = []
-                                for i in range(len(l)):
-                                    di = []
-                                    for x in dnsList[i]:
-                                        if x in l[i]:
-                                            di.append(x)
-                                            
-                                    if not di:
-                                        di = [None]
-                                        
-                                    _d.append(di)
-                                    
-                                dnsList = _d
+                    # -- Get dataNodes candidates 
+                    dnsList = getCandidates(dn, e, variable, lcVariablesDns, lc, self.myLogger, integrate = integrate)
+                    lcVariablesDns[variableName] = dnsList
                                 
+                    if isinstance(lc, CandidateSelection):
+                        continue
+                    
                     # -- Get ILP variables from collected DataNodes for the given element of logical constraint
                     
+                    conceptName = e[0].name
                     vDns = [] # Stores ILP variables
                     if sample:
                         sampleInfoForVariable = []
                     xPkey = '<' + conceptName + ">" + key
                     
                     for dns in dnsList:
                         _vDns = []
@@ -1168,17 +1094,15 @@
                             pass
                         
                         vDns.append(_vDns)
                         
                         if sample:
                             sampleInfoForVariable.append(_sampleInfoForVariable)
                         
-                    # -- Store dataNodes and ILP variables
-                    
-                    lcVariablesDns[variableName] = dnsList
+                    # -- Store ILP variables
                     
                     if None in lcVariablesDns:
                         pass
                     
                     if vDns and loss and not sample:
                         vDnsList = [v[0] for v in vDns]
                         try:
@@ -1195,51 +1119,55 @@
                             lcVariables[variableName] = vDns
                     else:
                         lcVariables[variableName] = vDns
                     
                     if sample:
                         sampleInfo[variableName] = sampleInfoForVariable
                 
-                elif isinstance(e, LogicalConstrain): # -- nested LogicalConstrain - process recursively 
-                    self.myLogger.info('Processing Nested %s(%s) - %s'%(e.lcName, e, e.strEs()))
-                    if sample:
-                        vDns, sampleInfoLC, lcVariablesLC = self.__constructLogicalConstrains(e, booleanProcesor, m, dn, p, key = key, 
-                                                                               lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
-                        sampleInfo = {**sampleInfo, **sampleInfoLC} # sampleInfo|sampleInfoLC in python 9
-                        
-                        lcVariablesSet = {**lcVariablesSet, **lcVariablesLC}
-                    else:
-                        vDns = self.__constructLogicalConstrains(e, booleanProcesor, m, dn, p, key = key, 
-                                                                 lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
-                        
-                        if loss and vDns:
-                            vDnsOriginal = vDns
-                            vDnsList = [v[0] for v in  vDns]
-                            vDns = []
-                            try:
-                                if len(vDnsList) > 1:
-                                    tStack = torch.stack(vDnsList, dim=1)
-                                else:
-                                    tStack = vDnsList[0]
-                                tsqueezed = torch.squeeze(tStack, dim=0)
+                if isinstance(e, LcElement):
 
-                            except IndexError as ie:
-                                tsqueezed = torch.stack(vDnsList, dim=0)
-                                pass
+                    if isinstance(e, CandidateSelection): # -- nested LogicalConstrain - process recursively 
+                        lcVariablesDnsNew = self.__constructLogicalConstrains(e, booleanProcessor, m, dn, p, key = key, 
+                                                                     lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
+                         
+                        lcVariablesDns = lcVariablesDnsNew
+                        vDns = None
+                        if lcVariablesDns:
+                            length_of_list = len(next(iter(lcVariablesDns.values())))
+
+                            if sample:
+                                vDns = [[torch.ones(p, device=self.current_device, requires_grad=False, dtype=torch.bool)] for _ in range(length_of_list)]
+                            elif loss:
+                                vDns = [[torch.zeros(length_of_list, device=self.current_device, requires_grad=True, dtype=torch.float64)]]
+                                vDns = self.__addLossTovDns(loss, vDns)
+                            else:
+                                vDns = [[1] for _ in range(length_of_list)]
+                                   
+                    if isinstance(e, LogicalConstrain): # -- nested LogicalConstrain - process recursively 
+                        self.myLogger.info('Processing Nested %s(%s) - %s'%(e.lcName, e, e.strEs()))
+
+                        if sample:
+                            vDns, sampleInfoLC, lcVariablesLC = self.__constructLogicalConstrains(e, booleanProcessor, m, dn, p, key = key, 
+                                                                                   lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
+                            sampleInfo = {**sampleInfo, **sampleInfoLC} # sampleInfo|sampleInfoLC in python 9
+                            
+                            lcVariablesSet = {**lcVariablesSet, **lcVariablesLC}
+                        else:
+                            vDns = self.__constructLogicalConstrains(e, booleanProcessor, m, dn, p, key = key, 
+                                                                     lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
+                            
+                            vDns = self.__addLossTovDns(loss, vDns)
                         
-                            if not len(tsqueezed.shape):
-                                tsqueezed = torch.unsqueeze(tsqueezed, 0)
-                                
-                            tList = [tsqueezed]
-                            vDns.append(tList)
-                                                
+                                                    
                     if vDns == None:
                         self.myLogger.warning('Not found data for %s(%s) nested Logical Constraint required to build %s(%s) - skipping it'%(e.lcName,e,lc.lcName,lc))
                         return None
                         
+                    countValid = sum(1 for sublist in vDns if sublist and any(elem is not None for elem in sublist))
+                    self.myLogger.info('Size of candidate list returned by %s(%s) nested Logical Constraint is %i of which %i is not None'%(e.lcName,e,len(vDns),countValid))
                     lcVariables[variableName] = vDns   
             # Int - limit 
             elif isinstance(e, int): 
                 if eIndex == 0:
                     pass # if this lc using it
                 else:
                     pass # error!
@@ -1247,19 +1175,22 @@
                 if eIndex == 2:
                     pass # if this lc using it
                 else:
                     pass # error!
             else:
                 self.myLogger.error('Logical Constraint %s has incorrect element %s'%(lc,e))
                 return None
-        if sample:
+            
+        if isinstance(lc, CandidateSelection):
+            return lc(lcVariablesDns, keys=lc.CandidateSelectionVariable)
+        elif sample:
             lcVariablesSet[lc] = lcVariables
-            return lc(m, booleanProcesor, lcVariables, headConstrain = headLC, integrate = integrate), sampleInfo, lcVariablesSet
+            return lc(m, booleanProcessor, lcVariables, headConstrain = headLC, integrate = integrate), sampleInfo, lcVariablesSet
         elif verify and headLC:
-            return lc(m, booleanProcesor, lcVariables, headConstrain = headLC, integrate = integrate), lcVariables
+            return lc(m, booleanProcessor, lcVariables, headConstrain = headLC, integrate = integrate), lcVariables
         else:
             if loss:
                 slpitT = False
                 for v in lcVariables:
                     if lcVariables[v] and len(lcVariables[v]) > 1:
                         slpitT = True
                         break
@@ -1271,20 +1202,20 @@
                          
                         lcVSplitted = torch.split(lcVariables[v][0][0], 1)
                         lcVariables[v] = []
                         
                         for s in lcVSplitted:
                             lcVariables[v].append([s]) 
                     
-            return lc(m, booleanProcesor, lcVariables, headConstrain = headLC, integrate = integrate)
+            return lc(m, booleanProcessor, lcVariables, headConstrain = headLC, integrate = integrate)
     
     # ---------------
                 
     # -- Main method of the solver - creating ILP constraints plus objective, invoking the ILP solver and returning the result of the ILP solver classification  
-    def calculateILPSelection(self, dn, *conceptsRelations, fun=None, epsilon = 0.00001, minimizeObjective = False, ignorePinLCs = False):
+    def calculateILPSelection(self, dn, *conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001, minimizeObjective = False, ignorePinLCs = False):
         if self.ilpSolver == None:
             self.myLogger.warning('ILP solver not provided - returning')
             self.myLoggerTime.warning('ILP solver not provided - returning')
             
             return 
         
         self.current_device = dn.current_device
@@ -1315,17 +1246,17 @@
             if not reusingModel:
                 # If not reusing the model or if the right model was yet saved - create new Gurabi model
                 m = Model("decideOnClassificationResult" + str(start), gurobiEnv)
                 m.params.outputflag = 0
                 x = OrderedDict()
                 
                 # Create ILP Variables for concepts and objective
-                Q = self.createILPVariables(m, x, dn, *conceptsRelations, dnFun = self.__getProbability, fun=fun, epsilon = epsilon)
+                Q = self.createILPVariables(m, x, dn, *conceptsRelations, key=key, fun=fun, epsilon = epsilon)
             else:
-                Q = self.createObjective(x, dn, *conceptsRelations, dnFun = self.__getProbability, fun=fun, epsilon = epsilon)
+                Q = self.createObjective(x, dn, *conceptsRelations, key=key, fun=fun, epsilon = epsilon)
             
             endVariableInit = process_time() # timer()
             elapsedVariablesInMs = (endVariableInit - start) *1000
             self.myLoggerTime.info('ILP Variables Init - time: %ims'%(elapsedVariablesInMs))
 
             if not reusingModel:
                 # Add constraints based on ontology and graph definition
@@ -1936,15 +1867,19 @@
                     current_lcLosses['loss'] = None
 
                 endLC = process_time_ns() # timer()
                 elapsedInNsLC = endLC - startLC
                 elapsedInMsLC = elapsedInNsLC/1000000
                 current_lcLosses['elapsedInMsLC'] += elapsedInMsLC
 
-                self.myLoggerTime.info('Processing time for %s with %i entries is: %ims'%(currentLcName, len(lossList),  current_lcLosses['elapsedInMsLC']))
+                if lossList is not None:
+                    self.myLoggerTime.info('Processing time for %s with %i entries is: %ims'%(currentLcName, len(lossList),  current_lcLosses['elapsedInMsLC']))
+                else:
+                    self.myLoggerTime.info('Processing time for %s with %i entries is: %ims'%(currentLcName, 0,  current_lcLosses['elapsedInMsLC']))
+
                 [h.flush() for h in self.myLoggerTime.handlers]
             
         else: # -----------Sample
             globalSuccesses = torch.ones(sampleSize, device = self.current_device)
             
             for currentLcName in lcLosses:
                 startLC = process_time_ns() # timer()
@@ -2162,15 +2097,15 @@
                 
                 if verifyListLen:
                     current_verifyResult['satisfied'] = (verifyListSatisfied / verifyListLen) * 100
                 else:
                     current_verifyResult['satisfied'] = float("nan")
                     
                 # If  this if logical constraints
-                if type(lc) is ifL: # if LC
+                if type(lc) is ifL or type(lc) is forAllL: # if LC
                     firstKey = next(iter(lcVariables)) # antecedent variable name in the given if LC
                     firstLcV = lcVariables[firstKey]   # values of antecedent 
                     
                     ifVerifyList = []
                     
                     ifVerifyListLen = 0
                     ifVerifyListSatisfied = 0
```

### Comparing `DomiKnowS-0.533/domiknows/solver/ilpBooleanMethods.py` & `DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethods.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,143 +8,143 @@
 class ilpBooleanProcessor(object):
     __metaclass__ = abc.ABCMeta
     
     def __init__(self, _ildConfig = ilpConfig) -> None:
         super().__init__()
 
     # NOT Negation
-    # Create new variable varNOT, create constrain 1 - var == varNOT, return varNOT
+    # Create new variable varNOT, create constraint 1 - var == varNOT, return varNOT
     # 1 - var == varNOT
-    # if onlyConstrains then only construct constrain 1 - var >= 0
+    # if onlyConstrains then only construct constraint 1 - var >= 0
     @abc.abstractmethod
     def notVar(self, m, _var, onlyConstrains = False): pass
     
     # AND Conjunction with 2 variable
     # Create new variable varAND, create constrains:
     # varAND <= var1
     # varAND <= var2 
     # var1 + var2 <= varAND + 2 - 1
     # return varAND
-    # if onlyConstrains then only construct constrain var1 + var2 >= 2
+    # if onlyConstrains then only construct constraint var1 + var2 >= 2
     @abc.abstractmethod
     def and2Var(self, m, _var1, _var2,  onlyConstrains = False): pass
         
     # AND Conjunction
     # Create new variable varAND, create constrains:
     # varAND <= var1
     # varAND <= var2
     # ....
     # varAND <= varN
     # var1 + var2 + .. + varN <= varAND + N - 1
     # return varAND
-    # if onlyConstrains then only construct constrain var1 + var2 + .. + varN >= N
+    # if onlyConstrains then only construct constraint var1 + var2 + .. + varN >= N
     @abc.abstractmethod
     def andVar(self, m, *_var, onlyConstrains = False): pass
        
     # OR Disjunction with 2 variables
     # Create new variable varOR, create constrains:
     # var1 <= varOR
     # var2 <= varOR 
     # var1 + var2 >= varOR 
     # return varOR
-    # if onlyConstrains then only construct constrain var1 + var2 >= 1
+    # if onlyConstrains then only construct constraint var1 + var2 >= 1
     #
     # if limit > 1
     # var1 + var2 - (limit - 1) >= varOR 
-    # if onlyConstrains then only construct constrain var1 + var2 >= limit
+    # if onlyConstrains then only construct constraint var1 + var2 >= limit
     @abc.abstractmethod
     def or2Var(self, m, _var1, _var2,  onlyConstrains = False): pass
         
     # OR Disjunction
     # Create new variable varOR, create constrains:
     # var1 <= varOR
     # var2 <= varOR 
     # ...
     # varN <= varOR
     # var1 + var2 + ... + varN >= varOR
     # return varOR
-    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN >= 1
+    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN >= 1
     # if limit > 1
     # var1 + var2 + ... + varN - (limit - 1) >= varOR 
-    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN >= limit
+    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN >= limit
     @abc.abstractmethod
     def orVar(self, m, *_var, onlyConstrains = False): pass
 
     # NAND (Alternative denial) with 2 variables
     # Create new variable varNAND, create constrains:
     # not(varNAND) <= var1
     # not(varNAND) <= var2 
     # var1 + var2 <= not(varNAND) + 2 - 1
     # return varNAND
-    # if onlyConstrains then only construct constrain var1 + var2 <= 1
+    # if onlyConstrains then only construct constraint var1 + var2 <= 1
     @abc.abstractmethod
     def nand2Var(self, m, _var1, _var2): pass
 
     # NAND (Alternative denial)
     # Create new variable varNAND, create constrains:
     # not(varNAND) <= var1
     # not(varNAND) <= var2 
     # ...
     # not(varNAND <= varN 
     # var1 + var2 + ... + varN <= not(varNAND) + N - 1
     # return varNAND
-    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN <= N -1
+    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN <= N -1
     @abc.abstractmethod
     def nandVar(self, m, *_var, onlyConstrains = False): pass
   
     # NOR (Joint Denial) 2 variables
     # Create new variable varNOR, create constrains:
     # var1 <= not(varNOR)
     # var2 <= not(varNOR) 
     # var1 + var2 >= not(varNOR)
     # return varNOR
-    # if onlyConstrains then only construct constrain var1 + var2 <= 0
+    # if onlyConstrains then only construct constraint var1 + var2 <= 0
     @abc.abstractmethod
     def nor2Var(self, m, _var1, _var2): pass
 
     # NOR (Joint Denial)
     # Create new variable varNOR, create constrains:
     # var1 <= not(varNOR)
     # var2 <= not(varNOR) 
     # ...
     # varN <= not(varNOR)
     # var1 + var2 + ... + varN >= not(varNOR)
     # return varNOR
-    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN <= 0
+    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN <= 0
     @abc.abstractmethod
     def norVar(self, m, *_var, onlyConstrains = False): pass
 
     # XOR Exclusive Disjunction 
     # Create new variable varXOR, create constrains:
     # var1 + var2 + varXOR <= 2
     # -var1 - var2 + varXOR <= 0
     # var1 - var2 + varXOR >= 0
     # -var1 + var2 + varXOR >= 0
     # return varXOR
-    # if onlyConstrains then only construct constrain var1 + var2 <= 1 and var1 + var2 >= 1 
+    # if onlyConstrains then only construct constraint var1 + var2 <= 1 and var1 + var2 >= 1 
     @abc.abstractmethod
     def xorVar(self, m, _var1, _var2,  onlyConstrains = False): pass
 
     # IF Implication
     # Create new variable varIF, create constrains:
     # 1 - var1 <= varIF
     # var2 <= varIF
     # 1 - var1 + var2 >= varIF
     # return varIF
-    # if onlyConstrains then only construct constrain var1 <= var2
+    # if onlyConstrains then only construct constraint var1 <= var2
     @abc.abstractmethod
     def ifVar(self, m, _var1, _var2,  onlyConstrains = False): pass
 
     # XNOR Equivalence (EQ)
     # Create new variable varEQ, create constrains:
     # var1 + var2 - varEQ <= 1
     # var1 + var2 + varEQ >= 1
     # -var1 + var2 + varEQ <= 1
     # var1 - var2 + varEQ <= 1
     # return varEQ
-    # if onlyConstrains then only construct constrain var1 >= var2 and var1 <= var2
+    # if onlyConstrains then only construct constraint var1 >= var2 and var1 <= var2
     @abc.abstractmethod
     def epqVar(self, m, _var1, _var2,  onlyConstrains = False): pass
     
-    # Create constrain var == label, return 1
+    # Create constraint var == label, return 1
     @abc.abstractmethod
     def fixedVar(self, m, _var, onlyConstrains = False): pass
```

### Comparing `DomiKnowS-0.533/domiknows/solver/ilpBooleanMethodsCalculator.py` & `DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                 varFixed.append(v)
         
         var = varFixed
         # --
         
         countSuccess = 0
 
-        varSum = sum(list(var)).item()
+        varSum = sum(list(var))
 
         if limitOp == '>=':
             if varSum >= limit:
                 countSuccess = 1
         elif limitOp == '<=':
             if varSum <= limit:
                 countSuccess = 1
```

### Comparing `DomiKnowS-0.533/domiknows/solver/ilpOntSolver.py` & `DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/ilpOntSolverFactory.py` & `DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolverFactory.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/lcLossBooleanMethods.py` & `DomiKnowS-0.534.dev0/domiknows/solver/lcLossBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/lcLossSampleBooleanMethods.py` & `DomiKnowS-0.534.dev0/domiknows/solver/lcLossSampleBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/mini_solver_debug.py` & `DomiKnowS-0.534.dev0/domiknows/solver/mini_solver_debug.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/session/gurobi_session.py` & `DomiKnowS-0.534.dev0/domiknows/solver/session/gurobi_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/solver/session/solver_session.py` & `DomiKnowS-0.534.dev0/domiknows/solver/session/solver_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/domiknows/utils.py` & `DomiKnowS-0.534.dev0/domiknows/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.533/setup.py` & `DomiKnowS-0.534.dev0/setup.py`

 * *Files identical despite different names*

