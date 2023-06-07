# Comparing `tmp/hybrid-graph-0.4.tar.gz` & `tmp/hybrid-graph-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid-graph-0.4.tar", last modified: Wed Jun  7 07:45:17 2023, max compression
+gzip compressed data, was "hybrid-graph-0.5.tar", last modified: Wed Jun  7 07:59:47 2023, max compression
```

## Comparing `hybrid-graph-0.4.tar` & `hybrid-graph-0.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.169839 hybrid-graph-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 07:44:59.000000 hybrid-graph-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 07:45:17.169839 hybrid-graph-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-07 07:44:59.000000 hybrid-graph-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/amazon/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/amazon/amazon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/dataset_info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/grand/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/grand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/grand/grand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/hg_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_formatter/HybridGraphFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/hg_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_samplers/graph_saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_samplers/random_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/hg_spliter/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_spliter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_spliter/spliter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/datasets/musae/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/datasets/standard/
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/standard/GraphStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/standard/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/io/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/io/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/models/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/linearprobe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.169839 hybrid-graph-0.4/hg/hybrid_graph/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/plt_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.169839 hybrid-graph-0.4/hybrid_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:45:17.169839 hybrid-graph-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-07 07:44:59.000000 hybrid-graph-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 07:59:37.000000 hybrid-graph-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 07:59:47.507726 hybrid-graph-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-07 07:59:37.000000 hybrid-graph-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/amazon/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/amazon/amazon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/dataset_info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/grand/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/grand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/grand/grand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/hg_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_formatter/HybridGraphFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/hg_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_samplers/graph_saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_samplers/random_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/hg_spliter/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_spliter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/hg_spliter/spliter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/musae/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/musae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/musae/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/musae/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/musae/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/musae/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.503726 hybrid-graph-0.5/hg/datasets/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/standard/GraphStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/datasets/standard/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/hg/hybrid_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/hg/hybrid_graph/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/io/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/hg/hybrid_graph/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/hg/hybrid_graph/models/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/models/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/models/gnn/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/models/gnn/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/models/gnn/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/models/gnn/linearprobe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/hg/hybrid_graph/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/sessions/plt_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/sessions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 07:59:37.000000 hybrid-graph-0.5/hg/hybrid_graph/sessions/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:59:47.507726 hybrid-graph-0.5/hybrid_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 07:59:47.000000 hybrid-graph-0.5/hybrid_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 07:59:47.000000 hybrid-graph-0.5/hybrid_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:59:47.000000 hybrid-graph-0.5/hybrid_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 07:59:47.000000 hybrid-graph-0.5/hybrid_graph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 07:59:47.000000 hybrid-graph-0.5/hybrid_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-07 07:59:47.000000 hybrid-graph-0.5/hybrid_graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:59:47.507726 hybrid-graph-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-07 07:59:37.000000 hybrid-graph-0.5/setup.py
```

### Comparing `hybrid-graph-0.4/LICENSE` & `hybrid-graph-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/PKG-INFO` & `hybrid-graph-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybrid-graph
-Version: 0.4
+Version: 0.5
 Summary: A python package for accessing and Hybrid-graph Datasets and train-eval framework for GNNs
 Home-page: https://github.com/Zehui127/hybrid-graph-benchmark/
 Author: Xiangyu Zhao;Zehui Li
 Author-email: zehui.li22@imperial.ac.uk, x.zhao22@imperial.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hybrid-graph-0.4/README.md` & `hybrid-graph-0.5/README.md`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/__init__.py` & `hybrid-graph-0.5/hg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/amazon/amazon.py` & `hybrid-graph-0.5/hg/datasets/amazon/amazon.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/dataset_info.yaml` & `hybrid-graph-0.5/hg/datasets/dataset_info.yaml`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/grand/grand.py` & `hybrid-graph-0.5/hg/datasets/grand/grand.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/hg_formatter/HybridGraphFormatter.py` & `hybrid-graph-0.5/hg/datasets/hg_formatter/HybridGraphFormatter.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/hg_samplers/graph_saint.py` & `hybrid-graph-0.5/hg/datasets/hg_samplers/graph_saint.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/hg_samplers/random_sampler.py` & `hybrid-graph-0.5/hg/datasets/hg_samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/hg_spliter/spliter.py` & `hybrid-graph-0.5/hg/datasets/hg_spliter/spliter.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/musae/facebook.py` & `hybrid-graph-0.5/hg/datasets/musae/facebook.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/musae/github.py` & `hybrid-graph-0.5/hg/datasets/musae/github.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/musae/twitch.py` & `hybrid-graph-0.5/hg/datasets/musae/twitch.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/musae/wikipedia.py` & `hybrid-graph-0.5/hg/datasets/musae/wikipedia.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/datasets/standard/GraphStats.py` & `hybrid-graph-0.5/hg/datasets/standard/GraphStats.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/cli.py` & `hybrid-graph-0.5/hg/hybrid_graph/cli.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/io/factory.py` & `hybrid-graph-0.5/hg/hybrid_graph/io/factory.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/models/__init__.py` & `hybrid-graph-0.5/hg/hybrid_graph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/baseline.py` & `hybrid-graph-0.5/hg/hybrid_graph/models/gnn/baseline.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/gat.py` & `hybrid-graph-0.5/hg/hybrid_graph/models/gnn/gat.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/hyper.py` & `hybrid-graph-0.5/hg/hybrid_graph/models/gnn/hyper.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/linearprobe.py` & `hybrid-graph-0.5/hg/hybrid_graph/models/gnn/linearprobe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import yaml
 import torch
 import torch.nn.functional as F
 import torch.nn as nn
 from torch_geometric.nn import GCNConv, HypergraphConv, GAT
-from .attention import Attention
 
 
 class LPGCNHyperGCN(torch.nn.Module):
     def __init__(
             self, info, *args, **kwargs):
         super().__init__()
         dim = 64
```

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/sessions/plt_wrapper.py` & `hybrid-graph-0.5/hg/hybrid_graph/sessions/plt_wrapper.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/sessions/test.py` & `hybrid-graph-0.5/hg/hybrid_graph/sessions/test.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hg/hybrid_graph/sessions/train.py` & `hybrid-graph-0.5/hg/hybrid_graph/sessions/train.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/hybrid_graph.egg-info/PKG-INFO` & `hybrid-graph-0.5/hybrid_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybrid-graph
-Version: 0.4
+Version: 0.5
 Summary: A python package for accessing and Hybrid-graph Datasets and train-eval framework for GNNs
 Home-page: https://github.com/Zehui127/hybrid-graph-benchmark/
 Author: Xiangyu Zhao;Zehui Li
 Author-email: zehui.li22@imperial.ac.uk, x.zhao22@imperial.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hybrid-graph-0.4/hybrid_graph.egg-info/SOURCES.txt` & `hybrid-graph-0.5/hybrid_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.4/setup.py` & `hybrid-graph-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hybrid-graph",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     package_data={'hg': ['datasets/dataset_info.yaml']},
     install_requires=[
         'torch',
         'torch_scatter',
         'torch_sparse',
         'torch_geometric==2.2.0',
```

