# Comparing `tmp/hybrid-graph-0.3.tar.gz` & `tmp/hybrid-graph-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid-graph-0.3.tar", last modified: Tue Jun  6 17:50:54 2023, max compression
+gzip compressed data, was "hybrid-graph-0.4.tar", last modified: Wed Jun  7 07:45:17 2023, max compression
```

## Comparing `hybrid-graph-0.3.tar` & `hybrid-graph-0.4.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-06 17:50:43.000000 hybrid-graph-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 17:50:54.664113 hybrid-graph-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-06 17:50:43.000000 hybrid-graph-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/amazon/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/amazon/amazon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/dataset_info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/grand/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/grand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/grand/grand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.656113 hybrid-graph-0.3/hg/datasets/hg_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_formatter/HybridGraphFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/hg_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_samplers/graph_saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_samplers/random_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/hg_spliter/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_spliter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/hg_spliter/spliter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/musae/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/musae/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/datasets/standard/
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/standard/GraphStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/datasets/standard/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/hybrid_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/hybrid_graph/io/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/io/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.660113 hybrid-graph-0.3/hg/hybrid_graph/models/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/linearprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/models/gnn/toynet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/hg/hybrid_graph/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/plt_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-06 17:50:43.000000 hybrid-graph-0.3/hg/hybrid_graph/sessions/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:50:54.664113 hybrid-graph-0.3/hybrid_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-06 17:50:54.000000 hybrid-graph-0.3/hybrid_graph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:50:54.664113 hybrid-graph-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 17:50:43.000000 hybrid-graph-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.169839 hybrid-graph-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 07:44:59.000000 hybrid-graph-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 07:45:17.169839 hybrid-graph-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-07 07:44:59.000000 hybrid-graph-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/amazon/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/amazon/amazon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/dataset_info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/grand/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/grand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/grand/grand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/hg_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_formatter/HybridGraphFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/hg_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_samplers/graph_saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_samplers/random_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.161838 hybrid-graph-0.4/hg/datasets/hg_spliter/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_spliter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/hg_spliter/spliter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/datasets/musae/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/musae/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/datasets/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/standard/GraphStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/datasets/standard/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/io/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.165838 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/models/gnn/linearprobe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.169839 hybrid-graph-0.4/hg/hybrid_graph/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/plt_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 07:44:59.000000 hybrid-graph-0.4/hg/hybrid_graph/sessions/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:17.169839 hybrid-graph-0.4/hybrid_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-07 07:45:17.000000 hybrid-graph-0.4/hybrid_graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:45:17.169839 hybrid-graph-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-07 07:44:59.000000 hybrid-graph-0.4/setup.py
```

### Comparing `hybrid-graph-0.3/LICENSE` & `hybrid-graph-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/PKG-INFO` & `hybrid-graph-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: hybrid-graph
-Version: 0.3
+Version: 0.4
 Summary: A python package for accessing and Hybrid-graph Datasets and train-eval framework for GNNs
 Home-page: https://github.com/Zehui127/hybrid-graph-benchmark/
 Author: Xiangyu Zhao;Zehui Li
 Author-email: zehui.li22@imperial.ac.uk, x.zhao22@imperial.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align='center'>
-<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
+<img src="https://github.com/Zehui127/hybrid-graph-benchmark/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
 </p>
 
 ------------------------------------------------------------------
 
 [![paper](https://img.shields.io/badge/Download-Raw%20Data-green)](https://zenodo.org/record/7982540)
 [![PyPI version](https://img.shields.io/pypi/v/hybrid-graph?color=purple)](https://pypi.org/project/hybrid-graph/)
-[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
 [![paper](https://img.shields.io/badge/Document-Website-purple)](https://zehui127.github.io/hybrid-graph-benchmark/)
+[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
 <!-- [![paper](https://img.shields.io/badge/Paper-Open%20Review-orange)]() -->
 <!-- [![paper](https://img.shields.io/badge/Access-PyTorch%20Geometric-green)](https://pytorch-geometric.readthedocs.io/en/latest/index.html) -->
 <!-- ![]() -->
 
 This is a benchmark dataset for evaluating **hybrid-graph** (hypergraph and hierarchical graph) learning algorithms. It contains:
  - 23 real-world higer-order graphs from the domains of biology, social media, and wikipedia
  - Built-in functionalities for preprocessing hybrid-graphs
  - A framework to easily train and evaluate Graph Neural Networks
 <!-- ![](https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/img/architecture.png?raw=true) -->
-<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
+<img src="https://github.com/Zehui127/hybrid-graph-benchmark/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
 
 
 # Installation
 ## Requirements
 First, install the required PyTorch packages. You will need to know the version of CUDA you have installed, as well as the version of PyTorch you want to use. Replace `${TORCH}` and `${CUDA}` with these versions in the following commands:
 
 ```bash
```

### Comparing `hybrid-graph-0.3/README.md` & `hybrid-graph-0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <p align='center'>
-<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
+<img src="https://github.com/Zehui127/hybrid-graph-benchmark/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
 </p>
 
 ------------------------------------------------------------------
 
 [![paper](https://img.shields.io/badge/Download-Raw%20Data-green)](https://zenodo.org/record/7982540)
 [![PyPI version](https://img.shields.io/pypi/v/hybrid-graph?color=purple)](https://pypi.org/project/hybrid-graph/)
-[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
 [![paper](https://img.shields.io/badge/Document-Website-purple)](https://zehui127.github.io/hybrid-graph-benchmark/)
+[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
 <!-- [![paper](https://img.shields.io/badge/Paper-Open%20Review-orange)]() -->
 <!-- [![paper](https://img.shields.io/badge/Access-PyTorch%20Geometric-green)](https://pytorch-geometric.readthedocs.io/en/latest/index.html) -->
 <!-- ![]() -->
 
 This is a benchmark dataset for evaluating **hybrid-graph** (hypergraph and hierarchical graph) learning algorithms. It contains:
  - 23 real-world higer-order graphs from the domains of biology, social media, and wikipedia
  - Built-in functionalities for preprocessing hybrid-graphs
  - A framework to easily train and evaluate Graph Neural Networks
 <!-- ![](https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/img/architecture.png?raw=true) -->
-<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
+<img src="https://github.com/Zehui127/hybrid-graph-benchmark/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
 
 
 # Installation
 ## Requirements
 First, install the required PyTorch packages. You will need to know the version of CUDA you have installed, as well as the version of PyTorch you want to use. Replace `${TORCH}` and `${CUDA}` with these versions in the following commands:
 
 ```bash
```

### Comparing `hybrid-graph-0.3/hg/datasets/__init__.py` & `hybrid-graph-0.4/hg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/amazon/amazon.py` & `hybrid-graph-0.4/hg/datasets/amazon/amazon.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/dataset_info.yaml` & `hybrid-graph-0.4/hg/datasets/dataset_info.yaml`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/grand/grand.py` & `hybrid-graph-0.4/hg/datasets/grand/grand.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/hg_formatter/HybridGraphFormatter.py` & `hybrid-graph-0.4/hg/datasets/hg_formatter/HybridGraphFormatter.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/hg_samplers/graph_saint.py` & `hybrid-graph-0.4/hg/datasets/hg_samplers/graph_saint.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/hg_samplers/random_sampler.py` & `hybrid-graph-0.4/hg/datasets/hg_samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/hg_spliter/spliter.py` & `hybrid-graph-0.4/hg/datasets/hg_spliter/spliter.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/musae/facebook.py` & `hybrid-graph-0.4/hg/datasets/musae/facebook.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/musae/github.py` & `hybrid-graph-0.4/hg/datasets/musae/github.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/musae/twitch.py` & `hybrid-graph-0.4/hg/datasets/musae/twitch.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/musae/wikipedia.py` & `hybrid-graph-0.4/hg/datasets/musae/wikipedia.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/datasets/standard/GraphStats.py` & `hybrid-graph-0.4/hg/datasets/standard/GraphStats.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/cli.py` & `hybrid-graph-0.4/hg/hybrid_graph/cli.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/io/factory.py` & `hybrid-graph-0.4/hg/hybrid_graph/io/factory.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/models/__init__.py` & `hybrid-graph-0.4/hg/hybrid_graph/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-from .gnn.toynet import ToyNet
 from .gnn.baseline import GCNNet, SAGENet
-from .gnn.hybrid import HybridGCN, HybridSAGE
 from .gnn.gat import GATNet, GATV2Net
 from .gnn.hyper import HyperGCN, HyperGAT
-from .gnn.linearprobe import LPGCNHyperGCN, CATTGCNHyperGCN,LPGGATGCN, LPGATHyperGCN, LPHYPERHYPER, LPGCNGCN, LPGGATGAT
+from .gnn.linearprobe import LPGCNHyperGCN,LPGGATGCN, LPGATHyperGCN, LPHYPERHYPER, LPGCNGCN, LPGGATGAT
 from .ensemble.average_prediction import Average_Ensemble
 
 factory = {
-    'toynet': ToyNet,
     'gcn': GCNNet,
     'sage': SAGENet,
     'gat': GATNet,
     'gatv2': GATV2Net,
-    'hybrid-gcn': HybridGCN,
-    'hybrid-sage': HybridSAGE,
     'hyper-gcn': HyperGCN,
     'hyper-gat': HyperGAT,
     'ensemble': Average_Ensemble,
     'lp-gcn-hyper-gcn': LPGCNHyperGCN,
-    'catt-gcn-hyper-gcn': CATTGCNHyperGCN,
     'lp-gat-hyper-gcn': LPGATHyperGCN,
     'lp-gat-gcn': LPGGATGCN,
     'lp-gcn-gcn': LPGCNGCN,
     'lp-gat-gat': LPGGATGAT,
     'lp-hyper-hyper': LPHYPERHYPER,
 }
```

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/baseline.py` & `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/baseline.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/gat.py` & `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/gat.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/hybrid.py` & `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/hyper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,106 @@
 import yaml
 import torch
 import torch.nn.functional as F
 import torch.nn as nn
-from torch_geometric.nn import GCNConv, SAGEConv, HypergraphConv
-from .attention import Attention
+from torch_geometric.nn import HypergraphConv
 
-
-class HybridGCN(torch.nn.Module):
+"""
+for baseline method:
+# self.hyperGCN
+# x2 = hyperGCN(x,hyperedge_index)
+# x,x2
+# potential 2 impelmentations
+"""
+class HyperGCN(torch.nn.Module):
     def __init__(
             self, info, *args, **kwargs):
         super().__init__()
-        dim = 64
-        self.hyper1 = HypergraphConv(info["num_node_features"], dim)
-        self.conv1 = GCNConv(info["num_node_features"], dim)
-        self.attn1 = Attention(dim) # TODO: cross attention between q = hyper1(x) and k = conv1(x)
+        dim = 32
+        self.conv1 = HypergraphConv(info["num_node_features"], dim)
         self.is_regression = info["is_regression"]
         self.is_edge_pred = info["is_edge_pred"]
         if info["is_regression"]:
-            self.hyper2 = HypergraphConv(dim, dim)
-            self.conv2 = GCNConv(dim, dim)
-            self.attn2 = Attention(dim) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
+            self.conv2 = HypergraphConv(dim, dim, )
             self.head = nn.Linear(dim, 1)
         elif info["is_edge_pred"]:
-            self.hyper2 = HypergraphConv(dim, dim)
-            self.conv2 = GCNConv(dim, dim)
-            self.attn2 = Attention(dim) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
+            self.conv2 = HypergraphConv(dim, dim, )
         else:
-            self.conv2 = GCNConv(dim, info["num_classes"])
-            self.hyper2 = HypergraphConv(dim, info["num_classes"])
-            self.attn2 = Attention(info["num_classes"],head=1) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
+            self.conv2 = HypergraphConv(dim, info["num_classes"])
+
     def forward(self, data, *args, **kargs):
-        x, edge_index,hyperedge_index = data.x, data.edge_index, data.hyperedge_index
+        x, edge_index = data.x, data.hyperedge_index
         if self.is_edge_pred:
             edge_index = args[0][0] # the message passing edge index
-        x_gcn = F.relu(self.conv1(x, edge_index))
-        #print(f"!!!!!!x shape is:{x.shape}")
-        x_hyper = F.relu(self.hyper1(x, hyperedge_index))
-        x = self.attn1(x_gcn.unsqueeze(0), x_hyper.unsqueeze(0)).squeeze(0)
+        x = F.relu(self.conv1(x, edge_index))
         x = F.dropout(x, training=self.training)
-        x_gcn = self.conv2(x, edge_index)
-        x_hyper = self.hyper2(x_hyper, hyperedge_index)
-        x = self.attn2(x_gcn.unsqueeze(0), x_hyper.unsqueeze(0)).squeeze(0)
+        x = self.conv2(x, edge_index)
+
 
         if self.is_regression:
             x = self.head(x).squeeze()
         elif self.is_edge_pred:
             # args[1] is the edge_label_index
             edge_label_index = args[0][1]
             x = x[edge_label_index[0]]*x[edge_label_index[1]]
             x = torch.sum(x,-1)
         else:
             x = F.log_softmax(x, dim=1)
         return x
 
-class HybridSAGE(torch.nn.Module):
+
+class HyperGAT(torch.nn.Module):
     def __init__(
-            self, info, *args, **kwargs):
+            self, info, mixture_cls=None, load_config=None, *args, **kwargs):
         super().__init__()
         dim = 32
-        self.hyper1 = HypergraphConv(info["num_node_features"], dim)
-        self.conv1 = SAGEConv(info["num_node_features"], dim, normalize=False)
-        self.attn1 = Attention(dim) # TODO: cross attention between q = hyper1(x) and k = conv1(x)
+        heads = info["num_node_features"]//dim
         self.is_regression = info["is_regression"]
         self.is_edge_pred = info["is_edge_pred"]
-        if info["is_regression"]:
-            self.hyper2 = HypergraphConv(dim, dim)
-            self.conv2 = SAGEConv(dim, dim, normalize=False)
-            self.attn2 = Attention(dim) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
+        if self.is_regression:
+            self.conv2 = HypergraphConv(dim*heads, dim, use_attention=True)
             self.head = nn.Linear(dim, 1)
         elif info["is_edge_pred"]:
-            self.hyper2 = HypergraphConv(dim, dim)
-            self.conv2 = SAGEConv(dim, dim, normalize=False)
-            self.attn2 = Attention(dim) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
+            self.conv2 = HypergraphConv(dim*heads, dim, use_attention=True)
         else:
-            self.conv2 = SAGEConv(dim, info["num_classes"], normalize=False)
-            self.hyper2 = HypergraphConv(dim, info["num_classes"])
-            self.attn2 = Attention(info["num_classes"],head=1) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
+            self.conv2 = HypergraphConv(dim*heads, info["num_classes"], use_attention=True)
+
+        self.conv1 = HypergraphConv(
+            info["num_node_features"], dim, use_attention=True,heads=heads)
+
     def forward(self, data, *args, **kargs):
-        x, edge_index,hyperedge_index = data.x, data.edge_index, data.hyperedge_index
+        x, edge_index = data.x, data.hyperedge_index
         if self.is_edge_pred:
             edge_index = args[0][0] # the message passing edge index
-        x_sage = F.relu(self.conv1(x, edge_index))
-        x_hyper = F.relu(self.hyper1(x, hyperedge_index))
-        x = self.attn1(x_sage.unsqueeze(0), x_hyper.unsqueeze(0)).squeeze(0)
-        x = F.dropout(x, training=self.training)
-        x_sage = self.conv2(x, edge_index)
-        x_hyper = self.hyper2(x_hyper, hyperedge_index)
-        x = self.attn2(x_sage.unsqueeze(0), x_hyper.unsqueeze(0)).squeeze(0)
+        x = F.relu(self.conv1(x, edge_index,
+                              hyperedge_attr=self.hyperedge_representation(x, edge_index)))
+        x = F.dropout(x, p=0.5, training=self.training)
 
+        x = self.conv2(x, edge_index, hyperedge_attr=self.hyperedge_representation(x, edge_index))
         if self.is_regression:
             x = self.head(x).squeeze()
         elif self.is_edge_pred:
             # args[1] is the edge_label_index
             edge_label_index = args[0][1]
             x = x[edge_label_index[0]]*x[edge_label_index[1]]
             x = torch.sum(x,-1)
         else:
             x = F.log_softmax(x, dim=1)
         return x
+
+    def hyperedge_representation(self, x, hyperedge_index):
+        # Assuming x is a NumPy array, if not, convert it to a NumPy array
+        # Initialize a placeholder array with the length of the maximum hyperedge index + 1
+        max_hyperedge_index = torch.max(hyperedge_index[1])
+        hyperedge_representations = torch.zeros((max_hyperedge_index + 1, x.shape[1]),device=x.device)
+         # Use torch_scatter's scatter_add to accumulate the node values for each hyperedge
+        from torch_scatter import scatter_add
+        hyperedge_representations = scatter_add(src=x[hyperedge_index[0]], index=hyperedge_index[1], dim=0, out=hyperedge_representations)
+        """
+        # Iterate through hyperedge_index
+        for i in range(hyperedge_index.shape[1]):
+            source, target = hyperedge_index[:, i]
+
+            # Sum the node values for each hyperedge
+            hyperedge_representations[target] += x[source]
+        """
+        return hyperedge_representations
```

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/models/gnn/linearprobe.py` & `hybrid-graph-0.4/hg/hybrid_graph/models/gnn/linearprobe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import yaml
 import torch
 import torch.nn.functional as F
 import torch.nn as nn
 from torch_geometric.nn import GCNConv, HypergraphConv, GAT
 from .attention import Attention
 
-#GAT(dim, dim,num_layers=1 )
+
 class LPGCNHyperGCN(torch.nn.Module):
     def __init__(
             self, info, *args, **kwargs):
         super().__init__()
         dim = 64
         self.hyper1 = HypergraphConv(info["num_node_features"], dim)
         self.conv1 = GCNConv(info["num_node_features"], dim)
@@ -203,46 +203,8 @@
         x_hyper = self.hyper2(x_hyper, hyperedge_index)
         x = self.lp(torch.cat([x_gcn.unsqueeze(0),x_hyper.unsqueeze(0)],dim=2)).squeeze(0)
 
         if self.is_regression:
             x = self.head(x).squeeze()
         else:
             x = F.log_softmax(x, dim=1)
-        return x
-
-
-class CATTGCNHyperGCN(torch.nn.Module):
-    def __init__(
-            self, info, *args, **kwargs):
-        super().__init__()
-        dim = 64
-        self.hyper1 = HypergraphConv(info["num_node_features"], dim)
-        self.conv1 = GCNConv(info["num_node_features"], dim)
-        self.attn1con = Attention(dim)
-        self.attn1hyper = Attention(dim)
-        self.is_regression = info["is_regression"]
-        if info["is_regression"]:
-            self.hyper2 = HypergraphConv(dim, dim)
-            self.conv2 = GCNConv(dim, dim)
-            self.lp = nn.Linear(2*dim,dim) # TODO: cross attention between q = hyper2(x) and k = conv2(x)
-            self.head = nn.Linear(dim, 1)
-        else:
-            self.conv2 = GCNConv(dim, info["num_classes"])
-            self.hyper2 = HypergraphConv(dim, info["num_classes"])
-            self.lp = nn.Linear(2*info["num_classes"],info["num_classes"])
-    def forward(self, data, *args, **kargs):
-        x, edge_index,hyperedge_index = data.x, data.edge_index, data.hyperedge_index
-        x_gcn_temp = F.relu(self.conv1(x, edge_index))
-        x_hyper_temp = F.relu(self.hyper1(x, hyperedge_index))
-        x_gcn = self.attn1con(x_gcn_temp.unsqueeze(0), x_hyper_temp.unsqueeze(0)).squeeze(0)
-        x_hyper = self.attn1hyper(x_hyper_temp.unsqueeze(0), x_gcn_temp.unsqueeze(0)).squeeze(0)
-        x_gcn = F.dropout(x_gcn, training=self.training)
-        x_hyper = F.dropout(x_hyper, training=self.training)
-        x_gcn = self.conv2(x_gcn, edge_index)
-        x_hyper = self.hyper2(x_hyper, hyperedge_index)
-        x = self.lp(torch.cat([x_gcn.unsqueeze(0),x_hyper.unsqueeze(0)],dim=2)).squeeze(0)
-
-        if self.is_regression:
-            x = self.head(x).squeeze()
-        else:
-            x = F.log_softmax(x, dim=1)
         return x
```

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/sessions/plt_wrapper.py` & `hybrid-graph-0.4/hg/hybrid_graph/sessions/plt_wrapper.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/sessions/test.py` & `hybrid-graph-0.4/hg/hybrid_graph/sessions/test.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hg/hybrid_graph/sessions/train.py` & `hybrid-graph-0.4/hg/hybrid_graph/sessions/train.py`

 * *Files identical despite different names*

### Comparing `hybrid-graph-0.3/hybrid_graph.egg-info/PKG-INFO` & `hybrid-graph-0.4/hybrid_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: hybrid-graph
-Version: 0.3
+Version: 0.4
 Summary: A python package for accessing and Hybrid-graph Datasets and train-eval framework for GNNs
 Home-page: https://github.com/Zehui127/hybrid-graph-benchmark/
 Author: Xiangyu Zhao;Zehui Li
 Author-email: zehui.li22@imperial.ac.uk, x.zhao22@imperial.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align='center'>
-<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
+<img src="https://github.com/Zehui127/hybrid-graph-benchmark/blob/pre-release/docs/title.png?raw=true" style="width: 75%; height: auto;"/>
 </p>
 
 ------------------------------------------------------------------
 
 [![paper](https://img.shields.io/badge/Download-Raw%20Data-green)](https://zenodo.org/record/7982540)
 [![PyPI version](https://img.shields.io/pypi/v/hybrid-graph?color=purple)](https://pypi.org/project/hybrid-graph/)
-[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
 [![paper](https://img.shields.io/badge/Document-Website-purple)](https://zehui127.github.io/hybrid-graph-benchmark/)
+[![license](https://img.shields.io/github/license/Zehui127/hybrid-graph-benchmark)](LICENSE)
 <!-- [![paper](https://img.shields.io/badge/Paper-Open%20Review-orange)]() -->
 <!-- [![paper](https://img.shields.io/badge/Access-PyTorch%20Geometric-green)](https://pytorch-geometric.readthedocs.io/en/latest/index.html) -->
 <!-- ![]() -->
 
 This is a benchmark dataset for evaluating **hybrid-graph** (hypergraph and hierarchical graph) learning algorithms. It contains:
  - 23 real-world higer-order graphs from the domains of biology, social media, and wikipedia
  - Built-in functionalities for preprocessing hybrid-graphs
  - A framework to easily train and evaluate Graph Neural Networks
 <!-- ![](https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/img/architecture.png?raw=true) -->
-<img src="https://github.com/Zehui127/hypergraph-benchmarks/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
+<img src="https://github.com/Zehui127/hybrid-graph-benchmark/blob/pre-release/docs/architecture.png?raw=true" style="width: 75%; height: auto;">
 
 
 # Installation
 ## Requirements
 First, install the required PyTorch packages. You will need to know the version of CUDA you have installed, as well as the version of PyTorch you want to use. Replace `${TORCH}` and `${CUDA}` with these versions in the following commands:
 
 ```bash
```

### Comparing `hybrid-graph-0.3/hybrid_graph.egg-info/SOURCES.txt` & `hybrid-graph-0.4/hybrid_graph.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,18 @@
 hg/hybrid_graph/__init__.py
 hg/hybrid_graph/cli.py
 hg/hybrid_graph/io/__init__.py
 hg/hybrid_graph/io/factory.py
 hg/hybrid_graph/io/utils.py
 hg/hybrid_graph/models/__init__.py
 hg/hybrid_graph/models/gnn/__init__.py
-hg/hybrid_graph/models/gnn/attention.py
 hg/hybrid_graph/models/gnn/baseline.py
 hg/hybrid_graph/models/gnn/gat.py
-hg/hybrid_graph/models/gnn/hybrid.py
 hg/hybrid_graph/models/gnn/hyper.py
 hg/hybrid_graph/models/gnn/linearprobe.py
-hg/hybrid_graph/models/gnn/toynet.py
 hg/hybrid_graph/sessions/__init__.py
 hg/hybrid_graph/sessions/plt_wrapper.py
 hg/hybrid_graph/sessions/test.py
 hg/hybrid_graph/sessions/train.py
 hybrid_graph.egg-info/PKG-INFO
 hybrid_graph.egg-info/SOURCES.txt
 hybrid_graph.egg-info/dependency_links.txt
```

### Comparing `hybrid-graph-0.3/setup.py` & `hybrid-graph-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hybrid-graph",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     package_data={'hg': ['datasets/dataset_info.yaml']},
     install_requires=[
         'torch',
         'torch_scatter',
         'torch_sparse',
         'torch_geometric==2.2.0',
```

