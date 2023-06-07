# Comparing `tmp/lightning-fabric-2.0.2.tar.gz` & `tmp/lightning-fabric-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.0.2.tar", last modified: Mon Apr 24 13:57:44 2023, max compression
+gzip compressed data, was "lightning-fabric-2.0.3.tar", last modified: Wed Jun  7 17:11:24 2023, max compression
```

## Comparing `lightning-fabric-2.0.2.tar` & `lightning-fabric-2.0.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.321956 lightning-fabric-2.0.2/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/devel.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7917 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-24 13:57:43.000000 lightning-fabric-2.0.2/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-24 13:57:43.000000 lightning-fabric-2.0.2/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu_bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    37214 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-04-24 13:57:43.000000 lightning-fabric-2.0.2/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.017971 lightning-fabric-2.0.3/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.013971 lightning-fabric-2.0.3/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.017971 lightning-fabric-2.0.3/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.017971 lightning-fabric-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27286 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu_bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/version.info
```

### Comparing `lightning-fabric-2.0.2/.actions/assistant.py` & `lightning-fabric-2.0.3/.actions/assistant.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,15 +154,16 @@
 def load_readme_description(path_dir: str, homepage: str, version: str) -> str:
     """Load readme as decribtion.
 
     >>> load_readme_description(_PROJECT_ROOT, "", "")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
     '...PyTorch Lightning is just organized PyTorch...'
     """
     path_readme = os.path.join(path_dir, "README.md")
-    text = open(path_readme, encoding="utf-8").read()
+    with open(path_readme, encoding="utf-8") as fo:
+        text = fo.read()
 
     # drop images from readme
     text = text.replace(
         "![PT to PL](docs/source-pytorch/_static/images/general/pl_quick_start_full_compressed.gif)", ""
     )
 
     # https://github.com/Lightning-AI/lightning/raw/master/docs/source/_static/images/lightning_module/pt_to_pl.png
@@ -327,15 +328,15 @@
         fp_new = fp.replace(source_dir, target_dir)
         _, ext = os.path.splitext(fp)
         if ext in (".png", ".jpg", ".ico"):
             os.makedirs(dirname(fp_new), exist_ok=True)
             if not isfile(fp_new):
                 shutil.copy(fp, fp_new)
             continue
-        elif ext in (".pyc",):
+        if ext in (".pyc",):
             continue
         # Try to parse everything else
         with open(fp, encoding="utf-8") as fo:
             try:
                 lines = fo.readlines()
             except UnicodeDecodeError:
                 # a binary file, skip
@@ -390,16 +391,18 @@
             if req.name not in packages:
                 final.append(line)
         print(final)
         path.write_text("\n".join(final) + "\n")
 
     @staticmethod
     def _replace_min(fname: str) -> None:
-        req = open(fname, encoding="utf-8").read().replace(">=", "==")
-        open(fname, "w", encoding="utf-8").write(req)
+        with open(fname, encoding="utf-8") as fo:
+            req = fo.read().replace(">=", "==")
+        with open(fname, "w", encoding="utf-8") as fw:
+            fw.write(req)
 
     @staticmethod
     def replace_oldest_ver(requirement_fnames: Sequence[str] = REQUIREMENT_FILES_ALL) -> None:
         """Replace the min package version by fixed one."""
         for fname in requirement_fnames:
             AssistantCLI._replace_min(fname)
```

### Comparing `lightning-fabric-2.0.2/LICENSE` & `lightning-fabric-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/PKG-INFO` & `lightning-fabric-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.2
+Version: 2.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

### Comparing `lightning-fabric-2.0.2/README.md` & `lightning-fabric-2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
 [![PyPI Status](https://badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-lightning)
 [![PyPI Status](https://pepy.tech/badge/pytorch-lightning)](https://pepy.tech/project/pytorch-lightning)
-[![Conda](https://img.shields.io/conda/v/conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-lightning)
+[![Conda](https://img.shields.io/conda/v/conda-forge/lightning?label=conda&color=success)](https://anaconda.org/conda-forge/lightning)
 [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/pytorch_lightning)
 [![codecov](https://codecov.io/gh/Lightning-AI/lightning/branch/master/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/lightning)
 
-[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=stable)](https://lightning.ai/docs/pytorch/stable/)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/lightning-ai/lightning)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 
 <!--
 [![CodeFactor](https://www.codefactor.io/repository/github/Lightning-AI/lightning/badge)](https://www.codefactor.io/repository/github/Lightning-AI/lightning)
 -->
 
 </div>
@@ -486,15 +486,15 @@
 ______________________________________________________________________
 
 ## Community
 
 The lightning community is maintained by
 
 - [10+ core contributors](https://lightning.ai/docs/pytorch/latest/community/governance.html) who are all a mix of professional engineers, Research Scientists, and Ph.D. students from top AI labs.
-- 590+ active community contributors.
+- 800+ community contributors.
 
 Want to help us build Lightning and reduce boilerplate for thousands of researchers? [Learn how to make your first contribution here](https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html)
 
 Lightning is also part of the [PyTorch ecosystem](https://pytorch.org/ecosystem/) which requires projects to have solid testing, documentation and support.
 
 ### Asking for help
```

### Comparing `lightning-fabric-2.0.2/setup.py` & `lightning-fabric-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,19 @@
 
 
 @contextlib.contextmanager
 def _set_manifest_path(manifest_dir: str, aggregate: bool = False, mapping: Mapping = _PACKAGE_MAPPING) -> Generator:
     if aggregate:
         # aggregate all MANIFEST.in contents into a single temporary file
         manifest_path = _named_temporary_file(manifest_dir)
-        lines = ["include src/lightning/version.info\n", "include requirements/base.txt\n"]
+        lines = [
+            "include src/lightning/version.info\n",
+            "include src/lightning/py.typed\n",
+            "include requirements/base.txt\n",
+        ]
         # load manifest and aggregated all manifests
         for pkg in mapping.values():
             pkg_manifest = os.path.join(_PATH_SRC, pkg, "MANIFEST.in")
             if os.path.isfile(pkg_manifest):
                 with open(pkg_manifest) as fh:
                     lines.extend(fh.readlines())
         # convert lightning_foo to lightning/foo
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.0.3/src/lightning_fabric/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.3] - 2023-06-07
+
+- Added support for `Callback` registration through entry points ([#17756](https://github.com/Lightning-AI/lightning/pull/17756))
+- Add Fabric internal hooks ([#17759](https://github.com/Lightning-AI/lightning/pull/17759))
+
+### Changed
+
+- Made type hints public ([#17100](https://github.com/Lightning-AI/lightning/pull/17100))
+- Support compiling a module after it was set up by Fabric ([#17529](https://github.com/Lightning-AI/lightning/pull/17529))
+
+### Fixed
+
+- Fixed computing the next version folder in `CSVLogger` ([#17139](https://github.com/Lightning-AI/lightning/pull/17139))
+- Fixed inconsistent settings for FSDP Precision ([#17670](https://github.com/Lightning-AI/lightning/issues/17670))
+
+
 ## [2.0.2] - 2023-04-24
 
 ### Changed
 
 - Enable precision autocast for LightningModule step methods in Fabric ([#17439](https://github.com/Lightning-AI/lightning/pull/17439))
 
 ### Fixed
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/README.md` & `lightning-fabric-2.0.3/src/lightning_fabric/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/__setup__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     return _load_py_module("assistant", location)
 
 
 def _prepare_extras() -> Dict[str, Any]:
     assistant = _load_assistant()
     # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-extras
     # Define package extras. These are only installed if you specify them.
-    # From remote, use like `pip install pytorch-lightning[dev, docs]`
-    # From local copy of repo, use like `pip install ".[dev, docs]"`
+    # From remote, use like `pip install "lightning-fabric[dev, docs]"`
+    # From local copy of repo, use like `PACKAGE_NAME=fabric pip install ".[dev, docs]"`
     common_args = {"path_dir": _PATH_REQUIREMENTS, "unfreeze": "none" if _FREEZE_REQUIREMENTS else "all"}
     req_files = [Path(p) for p in glob.glob(os.path.join(_PATH_REQUIREMENTS, "*.txt"))]
     extras = {
         p.stem: assistant.load_requirements(file_name=p.name, **common_args)
         for p in req_files
-        if p.name not in ("docs.txt", "devel.txt", "base.txt")
+        if p.name not in ("docs.txt", "base.txt")
     }
     for req in parse_requirements(extras["strategies"]):
         extras[req.key] = [str(req)]
     extras["all"] = extras["strategies"] + extras["examples"]
     extras["dev"] = extras["all"] + extras["test"]
     return extras
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/accelerator.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import ABC, abstractmethod
-from typing import Any, Dict
+from typing import Any
 
 import torch
 
+from lightning_fabric.accelerators.registry import _AcceleratorRegistry
+
 
 class Accelerator(ABC):
     """The Accelerator base class.
 
     An Accelerator is meant to deal with one type of hardware.
 
     .. warning::  Writing your own accelerator is an :ref:`experimental <versioning:Experimental API>` feature.
@@ -50,9 +52,9 @@
 
     @staticmethod
     @abstractmethod
     def is_available() -> bool:
         """Detect if the hardware is available."""
 
     @classmethod
-    def register_accelerators(cls, accelerator_registry: Dict) -> None:
+    def register_accelerators(cls, accelerator_registry: _AcceleratorRegistry) -> None:
         pass
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Dict, List, Union
+from typing import List, Union
 
 import torch
 
 from lightning_fabric.accelerators.accelerator import Accelerator
+from lightning_fabric.accelerators.registry import _AcceleratorRegistry
 
 
 class CPUAccelerator(Accelerator):
     """Accelerator for CPU devices."""
 
     def setup_device(self, device: torch.device) -> None:
         """
@@ -32,16 +33,15 @@
 
     def teardown(self) -> None:
         pass
 
     @staticmethod
     def parse_devices(devices: Union[int, str, List[int]]) -> int:
         """Accelerator device parsing logic."""
-        devices = _parse_cpu_cores(devices)
-        return devices
+        return _parse_cpu_cores(devices)
 
     @staticmethod
     def get_parallel_devices(devices: Union[int, str, List[int]]) -> List[torch.device]:
         """Gets parallel devices for the Accelerator."""
         devices = _parse_cpu_cores(devices)
         return [torch.device("cpu")] * devices
 
@@ -52,15 +52,15 @@
 
     @staticmethod
     def is_available() -> bool:
         """CPU is always available for execution."""
         return True
 
     @classmethod
-    def register_accelerators(cls, accelerator_registry: Dict) -> None:
+    def register_accelerators(cls, accelerator_registry: _AcceleratorRegistry) -> None:
         accelerator_registry.register(
             "cpu",
             cls,
             description=cls.__class__.__name__,
         )
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cuda.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import warnings
 from contextlib import contextmanager
 from functools import lru_cache
-from typing import cast, Dict, Generator, List, Optional, Union
+from typing import cast, Generator, List, Optional, Union
 
 import torch
 from lightning_utilities.core.rank_zero import rank_zero_info
 
 from lightning_fabric.accelerators.accelerator import Accelerator
+from lightning_fabric.accelerators.registry import _AcceleratorRegistry
 from lightning_fabric.utilities.imports import _TORCH_GREATER_EQUAL_1_12, _TORCH_GREATER_EQUAL_2_0
 
 
 class CUDAAccelerator(Accelerator):
     """Accelerator for NVIDIA CUDA devices."""
 
     def setup_device(self, device: torch.device) -> None:
@@ -59,15 +60,15 @@
         return num_cuda_devices()
 
     @staticmethod
     def is_available() -> bool:
         return num_cuda_devices() > 0
 
     @classmethod
-    def register_accelerators(cls, accelerator_registry: Dict) -> None:
+    def register_accelerators(cls, accelerator_registry: _AcceleratorRegistry) -> None:
         accelerator_registry.register(
             "cuda",
             cls,
             description=cls.__class__.__name__,
         )
 
 
@@ -327,17 +328,15 @@
             raw_cnt = _raw_device_count_nvml()
             if raw_cnt <= 0:
                 return raw_cnt
             # Trim the list up to a maximum available device
             for idx, val in enumerate(visible_devices):
                 if cast(int, val) >= raw_cnt:
                     return idx
-    except OSError:
-        return -1
-    except AttributeError:
+    except (OSError, AttributeError):
         return -1
     return len(visible_devices)
 
 
 def _check_cuda_matmul_precision(device: torch.device) -> None:
     if not _TORCH_GREATER_EQUAL_1_12:
         # before 1.12, tf32 was used by default
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/mps.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import platform
 from functools import lru_cache
-from typing import Dict, List, Optional, Union
+from typing import List, Optional, Union
 
 import torch
 
 from lightning_fabric.accelerators.accelerator import Accelerator
+from lightning_fabric.accelerators.registry import _AcceleratorRegistry
 from lightning_fabric.utilities.imports import _TORCH_GREATER_EQUAL_1_12
 
 
 class MPSAccelerator(Accelerator):
     """Accelerator for Metal Apple Silicon GPU devices.
 
     .. warning::  Use of this accelerator beyond import and instantiation is experimental.
@@ -40,16 +41,15 @@
         pass
 
     @staticmethod
     def parse_devices(devices: Union[int, str, List[int]]) -> Optional[List[int]]:
         """Accelerator device parsing logic."""
         from lightning_fabric.utilities.device_parser import _parse_gpu_ids
 
-        parsed_devices = _parse_gpu_ids(devices, include_mps=True)
-        return parsed_devices
+        return _parse_gpu_ids(devices, include_mps=True)
 
     @staticmethod
     def get_parallel_devices(devices: Union[int, str, List[int]]) -> List[torch.device]:
         """Gets parallel devices for the Accelerator."""
         parsed_devices = MPSAccelerator.parse_devices(devices)
         assert parsed_devices is not None
         return [torch.device("mps", i) for i in range(len(parsed_devices))]
@@ -65,15 +65,15 @@
         """MPS is only available for certain torch builds starting at torch>=1.12, and is only enabled on a machine
         with the ARM-based Apple Silicon processors."""
         return (
             _TORCH_GREATER_EQUAL_1_12 and torch.backends.mps.is_available() and platform.processor() in ("arm", "arm64")
         )
 
     @classmethod
-    def register_accelerators(cls, accelerator_registry: Dict) -> None:
+    def register_accelerators(cls, accelerator_registry: _AcceleratorRegistry) -> None:
         accelerator_registry.register(
             "mps",
             cls,
             description=cls.__class__.__name__,
         )
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import importlib
 from inspect import getmembers, isclass
 from typing import Any, Callable, Dict, List, Optional
 
-from lightning_fabric.accelerators.accelerator import Accelerator
 from lightning_fabric.utilities.exceptions import MisconfigurationException
 from lightning_fabric.utilities.registry import _is_register_method_overridden
 
 
 class _AcceleratorRegistry(dict):
     """This class is a Registry that stores information about the Accelerators.
 
@@ -110,10 +109,12 @@
 
     def __str__(self) -> str:
         return "Registered Accelerators: {}".format(", ".join(self.available_accelerators()))
 
 
 def call_register_accelerators(registry: _AcceleratorRegistry, base_module: str) -> None:
     module = importlib.import_module(base_module)
+    from lightning_fabric.accelerators.accelerator import Accelerator
+
     for _, mod in getmembers(module, isclass):
         if issubclass(mod, Accelerator) and _is_register_method_overridden(mod, Accelerator, "register_accelerators"):
             mod.register_accelerators(registry)
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/tpu.py` & `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/tpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,15 @@
     if devices in (1, 8, None):
         return True
 
     # allow picking 1 of 8 indexes
     if isinstance(devices, (list, tuple, set)):
         has_1_tpu_idx = len(devices) == 1
         is_valid_tpu_idx = 1 <= list(devices)[0] <= 8
-
-        is_valid_tpu_core_choice = has_1_tpu_idx and is_valid_tpu_idx
-        return is_valid_tpu_core_choice
+        return has_1_tpu_idx and is_valid_tpu_idx
 
     return False
 
 
 def _parse_tpu_devices_str(devices: str) -> Union[int, List[int]]:
     if devices in ("1", "8"):
         return int(devices)
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/cli.py` & `lightning-fabric-2.0.3/src/lightning_fabric/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,18 +158,15 @@
     return len(parsed_devices) if parsed_devices is not None else 0
 
 
 def _torchrun_launch(args: Namespace, script_args: List[str]) -> None:
     """This will invoke `torchrun` programmatically to launch the given script in new processes."""
     import torch.distributed.run as torchrun
 
-    if args.strategy == "dp":
-        num_processes = 1
-    else:
-        num_processes = _get_num_processes(args.accelerator, args.devices)
+    num_processes = 1 if args.strategy == "dp" else _get_num_processes(args.accelerator, args.devices)
 
     torchrun_args = [
         f"--nproc_per_node={num_processes}",
         f"--nnodes={args.num_nodes}",
         f"--node_rank={args.node_rank}",
         f"--master_addr={args.main_address}",
         f"--master_port={args.main_port}",
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/connector.py` & `lightning-fabric-2.0.3/src/lightning_fabric/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         accelerator: Union[str, Accelerator] = "auto",
         strategy: Union[str, Strategy] = "auto",
         devices: Union[List[int], str, int] = "auto",
         num_nodes: int = 1,
         precision: _PRECISION_INPUT = "32-true",
         plugins: Optional[Union[_PLUGIN_INPUT, List[_PLUGIN_INPUT]]] = None,
     ) -> None:
-
         # These arguments can be set through environment variables set by the CLI
         accelerator = self._argument_from_env("accelerator", accelerator, default="auto")
         strategy = self._argument_from_env("strategy", strategy, default="auto")
         devices = self._argument_from_env("devices", devices, default="auto")
         num_nodes = self._argument_from_env("num_nodes", num_nodes, default=1)
         precision = self._argument_from_env("precision", precision, default="32-true")
 
@@ -254,50 +253,45 @@
         # handle the case when the user passes in a strategy instance which has an accelerator, precision,
         # checkpoint io or cluster env set up
         # TODO: improve the error messages below
         if isinstance(self._strategy_flag, Strategy):
             if self._strategy_flag._accelerator:
                 if self._accelerator_flag != "auto":
                     raise ValueError("accelerator set through both strategy class and accelerator flag, choose one")
-                else:
-                    self._accelerator_flag = self._strategy_flag._accelerator
+                self._accelerator_flag = self._strategy_flag._accelerator
             if self._strategy_flag._precision:
                 # [RFC] handle precision plugin set up conflict?
                 if self._precision_instance:
                     raise ValueError("precision set through both strategy class and plugins, choose one")
-                else:
-                    self._precision_instance = self._strategy_flag._precision
+                self._precision_instance = self._strategy_flag._precision
             if self._strategy_flag._checkpoint_io:
                 if self.checkpoint_io:
                     raise ValueError("checkpoint_io set through both strategy class and plugins, choose one")
-                else:
-                    self.checkpoint_io = self._strategy_flag._checkpoint_io
+                self.checkpoint_io = self._strategy_flag._checkpoint_io
             if getattr(self._strategy_flag, "cluster_environment", None):
                 if self._cluster_environment_flag:
                     raise ValueError("cluster_environment set through both strategy class and plugins, choose one")
-                else:
-                    self._cluster_environment_flag = getattr(self._strategy_flag, "cluster_environment")
+                self._cluster_environment_flag = getattr(self._strategy_flag, "cluster_environment")
 
-            if hasattr(self._strategy_flag, "parallel_devices"):
-                if self._strategy_flag.parallel_devices:
-                    if self._strategy_flag.parallel_devices[0].type == "cpu":
-                        if self._accelerator_flag and self._accelerator_flag not in ("auto", "cpu"):
-                            raise ValueError(
-                                f"CPU parallel_devices set through {self._strategy_flag.__class__.__name__} class,"
-                                f" but accelerator set to {self._accelerator_flag}, please choose one device type"
-                            )
-                        self._accelerator_flag = "cpu"
-                    if self._strategy_flag.parallel_devices[0].type == "cuda":
-                        if self._accelerator_flag and self._accelerator_flag not in ("auto", "cuda", "gpu"):
-                            raise ValueError(
-                                f"GPU parallel_devices set through {self._strategy_flag.__class__.__name__} class,"
-                                f" but accelerator set to {self._accelerator_flag}, please choose one device type"
-                            )
-                        self._accelerator_flag = "cuda"
-                    self._parallel_devices = self._strategy_flag.parallel_devices
+            if hasattr(self._strategy_flag, "parallel_devices") and self._strategy_flag.parallel_devices:
+                if self._strategy_flag.parallel_devices[0].type == "cpu":
+                    if self._accelerator_flag and self._accelerator_flag not in ("auto", "cpu"):
+                        raise ValueError(
+                            f"CPU parallel_devices set through {self._strategy_flag.__class__.__name__} class,"
+                            f" but accelerator set to {self._accelerator_flag}, please choose one device type"
+                        )
+                    self._accelerator_flag = "cpu"
+                if self._strategy_flag.parallel_devices[0].type == "cuda":
+                    if self._accelerator_flag and self._accelerator_flag not in ("auto", "cuda", "gpu"):
+                        raise ValueError(
+                            f"GPU parallel_devices set through {self._strategy_flag.__class__.__name__} class,"
+                            f" but accelerator set to {self._accelerator_flag}, please choose one device type"
+                        )
+                    self._accelerator_flag = "cuda"
+                self._parallel_devices = self._strategy_flag.parallel_devices
 
     def _check_device_config_and_set_final_flags(self, devices: Union[List[int], str, int], num_nodes: int) -> None:
         self._num_nodes_flag = int(num_nodes) if num_nodes is not None else 1
         self._devices_flag = devices
 
         if self._devices_flag in ([], 0, "0"):
             accelerator_name = (
@@ -373,17 +367,16 @@
                 return env_type()
         return LightningEnvironment()
 
     def _choose_strategy(self) -> Union[Strategy, str]:
         if self._accelerator_flag == "tpu":
             if self._parallel_devices and len(self._parallel_devices) > 1:
                 return "xla"
-            else:
-                # TODO: lazy initialized device, then here could be self._strategy_flag = "single_tpu_device"
-                return SingleTPUStrategy(device=self._parallel_devices[0])  # type: ignore
+            # TODO: lazy initialized device, then here could be self._strategy_flag = "single_tpu_device"
+            return SingleTPUStrategy(device=self._parallel_devices[0])  # type: ignore
         if self._num_nodes_flag > 1:
             return "ddp"
         if len(self._parallel_devices) <= 1:
             # TODO: Change this once gpu accelerator was renamed to cuda accelerator
             if isinstance(self._accelerator_flag, (CUDAAccelerator, MPSAccelerator)) or (
                 isinstance(self._accelerator_flag, str) and self._accelerator_flag in ("cuda", "gpu", "mps")
             ):
@@ -434,15 +427,15 @@
         self._validate_precision_choice()
         if isinstance(self._precision_instance, Precision):
             return self._precision_instance
 
         if isinstance(self.accelerator, TPUAccelerator):
             if self._precision_input == "32-true":
                 return TPUPrecision()
-            elif self._precision_input in ("16-mixed", "bf16-mixed"):
+            if self._precision_input in ("16-mixed", "bf16-mixed"):
                 if self._precision_input == "16-mixed":
                     rank_zero_warn(
                         "You passed `Fabric(accelerator='tpu', precision='16-mixed')` but AMP with fp16"
                         " is not supported with TPUs. Using `precision='bf16-mixed'` instead."
                     )
                 return TPUBf16Precision()
         if isinstance(self.strategy, DeepSpeedStrategy):
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/fabric.py` & `lightning-fabric-2.0.3/src/lightning_fabric/fabric.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,25 @@
 from lightning_fabric.utilities.data import (
     _auto_add_worker_init_fn,
     _replace_dunder_methods,
     _update_dataloader,
     has_iterable_dataset,
 )
 from lightning_fabric.utilities.distributed import DistributedSamplerWrapper
+from lightning_fabric.utilities.registry import _load_external_callbacks
 from lightning_fabric.utilities.seed import seed_everything
 from lightning_fabric.utilities.types import ReduceOp
 from lightning_fabric.utilities.warnings import PossibleUserWarning
-from lightning_fabric.wrappers import _FabricDataLoader, _FabricModule, _FabricOptimizer, _unwrap_objects
+from lightning_fabric.wrappers import (
+    _FabricDataLoader,
+    _FabricModule,
+    _FabricOptimizer,
+    _unwrap_compiled,
+    _unwrap_objects,
+)
 
 
 class Fabric:
     """Fabric accelerates your PyTorch training or inference code with minimal changes required.
 
     - Automatic placement of models and data onto the device.
     - Automatic support for mixed and double precision (smaller memory footprint).
@@ -95,16 +102,15 @@
             num_nodes=num_nodes,
             precision=precision,
             plugins=plugins,
         )
         self._strategy: Strategy = self._connector.strategy
         self._accelerator: Accelerator = self._connector.accelerator
         self._precision: Precision = self._strategy.precision
-        callbacks = callbacks if callbacks is not None else []
-        self._callbacks = callbacks if isinstance(callbacks, list) else [callbacks]
+        self._callbacks = self._configure_callbacks(callbacks)
         loggers = loggers if loggers is not None else []
         self._loggers = loggers if isinstance(loggers, list) else [loggers]
         self._models_setup: int = 0
 
         self._prepare_run_method()
         if _is_using_cli():
             # when the CLI is used to launch the script, we need to set up the environment (init processes) here so
@@ -202,22 +208,27 @@
             module = self._strategy.setup_module(module)
 
         module = _FabricModule(module, self._precision, original_module=original_module)
 
         # Update the _DeviceDtypeModuleMixin's device parameter
         module.to(self.device if move_to_device else next(module.parameters(), torch.tensor(0)).device)
 
-        optimizers = [_FabricOptimizer(optimizer=optimizer, strategy=self._strategy) for optimizer in optimizers]
+        optimizers = [
+            _FabricOptimizer(optimizer=optimizer, strategy=self._strategy, callbacks=self._callbacks)
+            for optimizer in optimizers
+        ]
 
         self._models_setup += 1
 
         if hasattr(original_module, "_fabric"):  # this is probably a LightningModule
             original_module._fabric = self  # type: ignore[assignment]
             original_module._fabric_optimizers = optimizers  # type: ignore[assignment]
 
+        self.call("on_after_setup", fabric=self, module=module)
+
         if optimizers:
             # join both types in a tuple for API convenience
             return (module, *optimizers)
         return module
 
     def setup_module(self, module: nn.Module, move_to_device: bool = True) -> _FabricModule:
         """Set up a model for accelerated training or inference.
@@ -266,15 +277,18 @@
             *optimizers: One or more optmizers to set up.
 
         Returns:
             The wrapped optimizer(s).
         """
         self._validate_setup_optimizers(optimizers)
         optimizers = [self._strategy.setup_optimizer(optimizer) for optimizer in optimizers]
-        optimizers = [_FabricOptimizer(optimizer=optimizer, strategy=self._strategy) for optimizer in optimizers]
+        optimizers = [
+            _FabricOptimizer(optimizer=optimizer, strategy=self._strategy, callbacks=self._callbacks)
+            for optimizer in optimizers
+        ]
         return optimizers[0] if len(optimizers) == 1 else tuple(optimizers)
 
     def setup_dataloaders(
         self, *dataloaders: DataLoader, use_distributed_sampler: bool = True, move_to_device: bool = True
     ) -> Union[DataLoader, List[DataLoader]]:
         """Set up one or multiple dataloaders for accelerated training. If you need different settings for each
         dataloader, call this method individually for each one.
@@ -390,15 +404,15 @@
             raise ValueError(
                 "Only one of `clip_val` or `max_norm` can be set as this specifies the underlying clipping algorithm!"
             )
 
         if clip_val is not None:
             self.strategy.clip_gradients_value(_unwrap_objects(module), _unwrap_objects(optimizer), clip_val=clip_val)
             return None
-        elif max_norm is not None:
+        if max_norm is not None:
             return self.strategy.clip_gradients_norm(
                 _unwrap_objects(module),
                 _unwrap_objects(optimizer),
                 max_norm=max_norm,
                 norm_type=norm_type,
                 error_if_nonfinite=error_if_nonfinite,
             )
@@ -538,15 +552,15 @@
         Both the model's `.forward()` and the `self.backward()` call need to run under this context.
 
         Args:
             module: The module for which to control the gradient synchronization.
             enabled: Whether the context manager is enabled or not. ``True`` means skip the sync, ``False`` means do not
                 skip.
         """
-
+        module = _unwrap_compiled(module)
         if not isinstance(module, _FabricModule):
             raise TypeError(
                 "You need to set up the model first before you can call `self.no_backward_sync()`:"
                 " `model = self.setup(model, ...)`"
             )
         if not enabled or isinstance(self._strategy, SingleDeviceStrategy):
             context = nullcontext()
@@ -725,16 +739,15 @@
             workers = True
         return seed_everything(seed=seed, workers=workers)
 
     def _run_impl(self, run_method: Callable, *args: Any, **kwargs: Any) -> Any:
         run_method = partial(self._run_with_setup, run_method)
         if self._strategy.launcher is not None:
             return self._strategy.launcher.launch(run_method, *args, **kwargs)
-        else:
-            return run_method(*args, **kwargs)
+        return run_method(*args, **kwargs)
 
     def _run_with_setup(self, run_function: Callable, *args: Any, **kwargs: Any) -> Any:
         self._strategy.setup_environment()
         # apply sharded context to prevent OOM
         with self.sharded_model(), _replace_dunder_methods(DataLoader, "dataset"), _replace_dunder_methods(
             BatchSampler
         ):
@@ -829,14 +842,21 @@
 
         if any(isinstance(dl, _FabricDataLoader) for dl in dataloaders):
             raise ValueError("A dataloader should be passed only once to the `setup_dataloaders` method.")
 
         if any(not isinstance(dl, DataLoader) for dl in dataloaders):
             raise TypeError("Only PyTorch DataLoader are currently supported in `setup_dataloaders`.")
 
+    @staticmethod
+    def _configure_callbacks(callbacks: Optional[Union[List[Any], Any]]) -> List[Any]:
+        callbacks = callbacks if callbacks is not None else []
+        callbacks = callbacks if isinstance(callbacks, list) else [callbacks]
+        callbacks.extend(_load_external_callbacks("lightning_fabric.callbacks_factory"))
+        return callbacks
+
 
 def _is_using_cli() -> bool:
     return bool(int(os.environ.get("LT_CLI_USED", "0")))
 
 
 def _do_nothing(*_: Any) -> None:
     pass
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.0.3/src/lightning_fabric/loggers/csv_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 from lightning_fabric.utilities.rank_zero import rank_zero_only, rank_zero_warn
 from lightning_fabric.utilities.types import _PATH
 
 log = logging.getLogger(__name__)
 
 
 class CSVLogger(Logger):
-    r"""
-    Log to the local file system in CSV format.
+    r"""Log to the local file system in CSV format.
 
     Logs are saved to ``os.path.join(root_dir, name, version)``.
 
     Args:
         root_dir: The root directory in which all your experiments with different names and versions will be stored.
         name: Experiment name. Defaults to ``'lightning_logs'``.
         version: Experiment version. If version is not specified the logger inspects the save
@@ -102,16 +101,15 @@
         """The log directory for this run.
 
         By default, it is named ``'version_${self.version}'`` but it can be overridden by passing a string value for the
         constructor's version parameter instead of ``None`` or an int.
         """
         # create a pseudo standard path
         version = self.version if isinstance(self.version, str) else f"version_{self.version}"
-        log_dir = os.path.join(self.root_dir, self.name, version)
-        return log_dir
+        return os.path.join(self.root_dir, self.name, version)
 
     @property
     @rank_zero_experiment
     def experiment(self) -> "_ExperimentWriter":
         """Actual ExperimentWriter object. To use ExperimentWriter features anywhere in your code, do the
         following.
 
@@ -154,28 +152,28 @@
         root_dir = self.root_dir
 
         if not self._fs.isdir(root_dir):
             log.warning("Missing logger folder: %s", root_dir)
             return 0
 
         existing_versions = []
-        for d in self._fs.listdir(root_dir, detail=False):
-            name = d[len(root_dir) + 1 :]  # removes parent directories
-            if self._fs.isdir(d) and name.startswith("version_"):
+        for d in self._fs.listdir(root_dir):
+            full_path = d["name"]
+            name = os.path.basename(full_path)
+            if self._fs.isdir(full_path) and name.startswith("version_"):
                 existing_versions.append(int(name.split("_")[1]))
 
         if len(existing_versions) == 0:
             return 0
 
         return max(existing_versions) + 1
 
 
 class _ExperimentWriter:
-    r"""
-    Experiment writer for CSVLogger.
+    r"""Experiment writer for CSVLogger.
 
     Args:
         log_dir: Directory for the experiment logs
     """
 
     NAME_METRICS_FILE = "metrics.csv"
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.0.3/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.0.3/src/lightning_fabric/loggers/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     if _TENSORBOARD_AVAILABLE:
         from torch.utils.tensorboard import SummaryWriter
     else:
         from tensorboardX import SummaryWriter  # type: ignore[no-redef]
 
 
 class TensorBoardLogger(Logger):
-    r"""
-    Log to local file system in `TensorBoard <https://www.tensorflow.org/tensorboard>`_ format.
+    r"""Log to local file system in `TensorBoard <https://www.tensorflow.org/tensorboard>`_ format.
 
     Implemented using :class:`~tensorboardX.SummaryWriter`. Logs are saved to
     ``os.path.join(root_dir, name, version)``. This is the recommended logger in Lightning Fabric.
 
     Args:
         root_dir: The root directory in which all your experiments with different names and versions will be stored.
         name: Experiment name. Defaults to ``'lightning_logs'``. If it is the empty string then no per-experiment
@@ -198,16 +197,17 @@
             if isinstance(v, dict):
                 self.experiment.add_scalars(k, v, step)
             else:
                 try:
                     self.experiment.add_scalar(k, v, step)
                 # TODO(fabric): specify the possible exception
                 except Exception as ex:
-                    m = f"\n you tried to log {v} which is currently not supported. Try a dict or a scalar/tensor."
-                    raise ValueError(m) from ex
+                    raise ValueError(
+                        f"\n you tried to log {v} which is currently not supported. Try a dict or a scalar/tensor."
+                    ) from ex
 
     @rank_zero_only
     def log_hyperparams(
         self, params: Union[Dict[str, Any], Namespace], metrics: Optional[Dict[str, Any]] = None
     ) -> None:
         """Record hyperparameters. TensorBoard logs with and without saved hyperparameters are incompatible, the
         hyperparameters are then not displayed in the TensorBoard. Please delete or move the previously saved logs
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,16 +169,17 @@
             )
 
     @staticmethod
     def _validate_srun_variables() -> None:
         """Checks for conflicting or incorrectly set variables set through `srun` and raises a useful error
         message.
 
-        Right now, we only check for the most common user errors. See `the srun docs
-        <https://slurm.schedmd.com/srun.html>`_ for a complete list of supported srun variables.
+        Right now, we only check for the most common user errors. See
+        `the srun docs <https://slurm.schedmd.com/srun.html>`_
+        for a complete list of supported srun variables.
         """
         ntasks = int(os.environ.get("SLURM_NTASKS", "1"))
         if ntasks > 1 and "SLURM_NTASKS_PER_NODE" not in os.environ:
             raise RuntimeError(
                 f"You set `--ntasks={ntasks}` in your SLURM bash script, but this variable is not supported."
                 f" HINT: Use `--ntasks-per-node={ntasks}` instead."
             )
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,17 +44,24 @@
         )
 
     @property
     def mixed_precision_config(self) -> "TorchMixedPrecision":
         from torch.distributed.fsdp.fully_sharded_data_parallel import MixedPrecision as TorchMixedPrecision
 
         if self.precision == "16-mixed":
-            dtype = torch.float16
+            param_dtype = torch.float32
+            reduce_dtype = buffer_dtype = torch.float16
         elif self.precision == "bf16-mixed":
-            dtype = torch.bfloat16
+            param_dtype = torch.float32
+            reduce_dtype = buffer_dtype = torch.bfloat16
+        elif self.precision == "16-true":
+            param_dtype = reduce_dtype = buffer_dtype = torch.float16
+        elif self.precision == "bf16-true":
+            param_dtype = reduce_dtype = buffer_dtype = torch.bfloat16
         else:
             raise ValueError(f"Was unable to infer precision type, received {self.precision!r}.")
+
         return TorchMixedPrecision(
-            param_dtype=dtype,
-            reduce_dtype=dtype,
-            buffer_dtype=dtype,
+            param_dtype=param_dtype,
+            reduce_dtype=reduce_dtype,
+            buffer_dtype=buffer_dtype,
         )
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,11 +21,10 @@
     """Precision plugin for TPU integration."""
 
     def optimizer_step(
         self,
         optimizer: Optimizable,
         **kwargs: Any,
     ) -> Any:
-
         import torch_xla.core.xla_model as xm
 
         return xm.optimizer_step(optimizer, optimizer_args=kwargs)
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu_bf16.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu_bf16.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/ddp.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from lightning_fabric.plugins.collectives.torch_collective import default_pg_timeout
 from lightning_fabric.plugins.environments.cluster_environment import ClusterEnvironment
 from lightning_fabric.plugins.io.checkpoint_io import CheckpointIO
 from lightning_fabric.plugins.precision import Precision
 from lightning_fabric.strategies.launchers.multiprocessing import _MultiProcessingLauncher
 from lightning_fabric.strategies.launchers.subprocess_script import _SubprocessScriptLauncher
 from lightning_fabric.strategies.parallel import ParallelStrategy
+from lightning_fabric.strategies.registry import _StrategyRegistry
 from lightning_fabric.strategies.strategy import _BackwardSyncControl, TBroadcast
 from lightning_fabric.utilities.distributed import (
     _distributed_available,
     _get_default_process_group_backend_for_device,
     _init_dist_connection,
     _sync_ddp_if_available,
 )
@@ -130,15 +131,15 @@
             reduce_op: the reduction operation. Defaults to 'mean'/'avg'.
                 Can also be a string 'sum' to calculate the sum during reduction.
 
         Return:
             reduced value, except when the input was not a tensor the output remains is unchanged
         """
         if isinstance(tensor, Tensor):
-            tensor = _sync_ddp_if_available(tensor, group, reduce_op=reduce_op)
+            return _sync_ddp_if_available(tensor, group, reduce_op=reduce_op)
         return tensor
 
     def barrier(self, *args: Any, **kwargs: Any) -> None:
         if not _distributed_available():
             return
         if torch.distributed.get_backend() == "nccl":
             torch.distributed.barrier(device_ids=self._determine_ddp_device_ids())
@@ -156,15 +157,15 @@
 
     def get_module_state_dict(self, module: Module) -> Dict[str, Union[Any, Tensor]]:
         if isinstance(module, DistributedDataParallel):
             module = module.module
         return super().get_module_state_dict(module)
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         entries = (
             ("ddp", "popen"),
             ("ddp_spawn", "spawn"),
             ("ddp_fork", "fork"),
             ("ddp_notebook", "fork"),
         )
         for name, start_method in entries:
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,22 @@
 from torch.nn import Module
 from torch.optim import Optimizer
 
 from lightning_fabric.accelerators import Accelerator, CUDAAccelerator
 from lightning_fabric.plugins.environments.cluster_environment import ClusterEnvironment
 from lightning_fabric.plugins.precision import Precision
 from lightning_fabric.strategies.ddp import DDPStrategy
+from lightning_fabric.strategies.registry import _StrategyRegistry
 from lightning_fabric.strategies.strategy import _Sharded
 from lightning_fabric.utilities.distributed import log
-from lightning_fabric.utilities.imports import _TORCH_GREATER_EQUAL_2_0
 from lightning_fabric.utilities.rank_zero import rank_zero_info, rank_zero_only, rank_zero_warn
 from lightning_fabric.utilities.seed import reset_seed
 from lightning_fabric.utilities.types import _PATH
 
-_DEEPSPEED_AVAILABLE = (
-    # DeepSpeed fails under 0.8.2 with torch 2.0: https://github.com/microsoft/DeepSpeed/pull/2863
-    RequirementCache("deepspeed>=0.8.2")
-    or (
-        not _TORCH_GREATER_EQUAL_2_0
-        and RequirementCache("deepspeed")
-        # check packaging because of https://github.com/microsoft/DeepSpeed/pull/2771
-        # remove the packaging check when min version is >=0.8.1
-        and RequirementCache("packaging>=20.0")
-    )
-)
+_DEEPSPEED_AVAILABLE = RequirementCache("deepspeed")
 if TYPE_CHECKING and _DEEPSPEED_AVAILABLE:
     import deepspeed
 
 
 # TODO(fabric): Links in the docstrings to PL-specific deepspeed user docs need to be replaced.
 class DeepSpeedStrategy(DDPStrategy, _Sharded):
     DEEPSPEED_ENV_VAR = "PL_DEEPSPEED_CONFIG_PATH"
@@ -401,15 +391,15 @@
         engines = _get_deepspeed_engines_from_state(state)
         if len(engines) == 0:
             raise ValueError(
                 "Could not find a DeepSpeed model in the provided checkpoint state. Please provide the model as"
                 " part of the state like so: `save_checkpoint(..., state={'model': model, ...})`. Make sure"
                 " you set up the model (and optimizers if any) through the strategy before saving the checkpoint."
             )
-        elif len(engines) > 1:
+        if len(engines) > 1:
             raise ValueError(
                 "Found multiple DeepSpeed engine modules in the given state. Saving checkpoints with DeepSpeed is"
                 " currently limited to a single model per checkpoint. To save multiple models, call the"
                 " save method for each model separately with a different path."
             )
         engine = engines[0]
 
@@ -464,15 +454,15 @@
         engines = _get_deepspeed_engines_from_state(state)
         if len(engines) == 0:
             raise ValueError(
                 "Could not find a DeepSpeed model in the provided checkpoint state. Please provide the model as"
                 " part of the state like so: `load_checkpoint(..., state={'model': model, ...})`. Make sure"
                 " you set up the model (and optimizers if any) through the strategy before loading the checkpoint."
             )
-        elif len(engines) > 1:
+        if len(engines) > 1:
             raise ValueError(
                 "Found multiple DeepSpeed engine modules in the given state. Saving and loading checkpoints"
                 " with DeepSpeed is currently limited to a single model per checkpoint. To load multiple model"
                 " states, call the load method for each model checkpoint separately."
             )
         engine = engines[0]
         optimzer_state_requested = bool(len([item for item in state.values() if isinstance(item, Optimizer)]))
@@ -514,15 +504,15 @@
     ) -> None:
         raise NotImplementedError(
             "DeepSpeed handles gradient clipping automatically within the optimizer. "
             "Make sure to set the `gradient_clipping` value in your Config."
         )
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         strategy_registry.register("deepspeed", cls, description="Default DeepSpeed Strategy")
         strategy_registry.register("deepspeed_stage_1", cls, description="DeepSpeed with ZeRO Stage 1 enabled", stage=1)
         strategy_registry.register("deepspeed_stage_2", cls, description="DeepSpeed with ZeRO Stage 2 enabled", stage=2)
         strategy_registry.register(
             "deepspeed_stage_2_offload",
             cls,
             description="DeepSpeed ZeRO Stage 2 and CPU Offload",
@@ -780,16 +770,15 @@
         return config
 
 
 def _get_deepspeed_engines_from_state(state: Dict[str, Any]) -> List["deepspeed.DeepSpeedEngine"]:
     from deepspeed import DeepSpeedEngine
 
     modules = chain(*(module.modules() for module in state.values() if isinstance(module, Module)))
-    engines = [engine for engine in modules if isinstance(engine, DeepSpeedEngine)]
-    return engines
+    return [engine for engine in modules if isinstance(engine, DeepSpeedEngine)]
 
 
 def _validate_state_keys(state: Dict[str, Any]) -> None:
     # DeepSpeed merges the client state into its internal engine state when saving, but it does not check for
     # colliding keys from the user. We explicitly check it here:
     deepspeed_internal_keys = {
         "module",
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/dp.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from torch import Tensor
 from torch.nn import DataParallel, Module
 
 from lightning_fabric.accelerators import Accelerator
 from lightning_fabric.plugins.io.checkpoint_io import CheckpointIO
 from lightning_fabric.plugins.precision import Precision
 from lightning_fabric.strategies.parallel import ParallelStrategy
+from lightning_fabric.strategies.registry import _StrategyRegistry
 from lightning_fabric.strategies.strategy import TBroadcast, TReduce
 from lightning_fabric.utilities.apply_func import apply_to_collection
 from lightning_fabric.utilities.distributed import ReduceOp
 
 
 class DataParallelStrategy(ParallelStrategy):
     """Implements data-parallel training in a single process, i.e., the model gets replicated to each device and
@@ -85,9 +86,9 @@
 
     def get_module_state_dict(self, module: Module) -> Dict[str, Union[Any, Tensor]]:
         if isinstance(module, DataParallel):
             module = module.module
         return super().get_module_state_dict(module)
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         strategy_registry.register("dp", cls, description=cls.__class__.__name__)
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/fsdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from lightning_fabric.accelerators import Accelerator
 from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment, Precision
 from lightning_fabric.plugins.collectives.torch_collective import default_pg_timeout
 from lightning_fabric.plugins.precision.fsdp import FSDPPrecision
 from lightning_fabric.strategies.launchers.subprocess_script import _SubprocessScriptLauncher
 from lightning_fabric.strategies.parallel import ParallelStrategy
+from lightning_fabric.strategies.registry import _StrategyRegistry
 from lightning_fabric.strategies.strategy import _BackwardSyncControl, _Sharded, TBroadcast
 from lightning_fabric.utilities.distributed import (
     _distributed_available,
     _get_default_process_group_backend_for_device,
     _init_dist_connection,
     _sync_ddp_if_available,
 )
@@ -140,14 +141,15 @@
 
     @property
     def mixed_precision_config(self) -> Optional["MixedPrecision"]:
         if self.mixed_precision:
             return self.mixed_precision
         if isinstance(self.precision, FSDPPrecision):
             return self.precision.mixed_precision_config
+        return None
 
     def _configure_launcher(self) -> None:
         assert self.cluster_environment is not None
         if not self.cluster_environment.creates_processes_externally:
             self._launcher = _SubprocessScriptLauncher(self.cluster_environment, self.num_processes, self.num_nodes)
 
     def setup_environment(self) -> None:
@@ -228,15 +230,15 @@
         ):
             yield
 
     def all_reduce(
         self, tensor: Tensor, group: Optional[Any] = None, reduce_op: Optional[Union[ReduceOp, str]] = "mean"
     ) -> Tensor:
         if isinstance(tensor, Tensor):
-            tensor = _sync_ddp_if_available(tensor, group, reduce_op=reduce_op)
+            return _sync_ddp_if_available(tensor, group, reduce_op=reduce_op)
         return tensor
 
     def barrier(self, *args: Any, **kwargs: Any) -> None:
         if not _distributed_available():
             return
         if torch.distributed.get_backend() == "nccl":
             torch.distributed.barrier(device_ids=[self.root_device.index])
@@ -270,15 +272,15 @@
 
         raise NotImplementedError(
             "FSDP currently does not support to clip gradients by value. "
             "Consider clipping by norm instead or choose another strategy!"
         )
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         if not _TORCH_GREATER_EQUAL_1_12 or not torch.distributed.is_available():
             return
 
         strategy_registry.register(
             "fsdp",
             cls,
             description="Fully Sharded Data Parallel (FSDP) training",
@@ -347,11 +349,11 @@
     return cpu_offload if isinstance(cpu_offload, CPUOffload) else CPUOffload(offload_params=bool(cpu_offload))
 
 
 def _optimizer_has_flat_params(optimizer: Optimizer) -> bool:
     _FSDP_FLATTENED = "_fsdp_flattened"
     if _TORCH_GREATER_EQUAL_1_13:
         return any(getattr(param, _FSDP_FLATTENED, False) for param in optimizer.param_groups[0]["params"])
-    else:
-        from torch.distributed.fsdp import FlatParameter
 
-        return any(isinstance(param, FlatParameter) for param in optimizer.param_groups[0]["params"])
+    from torch.distributed.fsdp import FlatParameter
+
+    return any(isinstance(param, FlatParameter) for param in optimizer.param_groups[0]["params"])
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/base.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import ABC, abstractmethod
 from typing import Any, Callable
 
 
 class _Launcher(ABC):
-    r"""
-    Abstract base class for all Launchers.
+    r"""Abstract base class for all Launchers.
 
     Launchers are responsible for the creation and instrumentation of new processes so that the
     :class:`~lightning_fabric.strategies.strategy.Strategy` can set up communication between all them.
 
     Subclass this class and override any of the relevant methods to provide a custom implementation depending on
     cluster environment, hardware, strategy, etc.
     """
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import ABC, abstractmethod
 from typing import Any, Callable
 
 
 class _Launcher(ABC):
-    r"""
-    Abstract base class for all Launchers.
+    r"""Abstract base class for all Launchers.
 
     Launchers are responsible for the creation and instrumentation of new processes so that the
     :class:`~lightning_fabric.strategies.strategy.Strategy` can set up communication between all them.
 
     Subclass this class and override any of the relevant methods to provide a custom implementation depending on
     cluster environment, hardware, strategy, etc.
     """
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,15 @@
 
 
 def _basic_subprocess_cmd() -> Sequence[str]:
     import __main__  # local import to avoid https://github.com/Lightning-AI/lightning/issues/15218
 
     if __main__.__spec__ is None:  # pragma: no-cover
         return [sys.executable, os.path.abspath(sys.argv[0])] + sys.argv[1:]
-    else:
-        return [sys.executable, "-m", __main__.__spec__.name] + sys.argv[1:]
+    return [sys.executable, "-m", __main__.__spec__.name] + sys.argv[1:]
 
 
 def _hydra_subprocess_cmd(local_rank: int) -> Tuple[Sequence[str], str]:
     import __main__  # local import to avoid https://github.com/Lightning-AI/lightning/issues/15218
     from hydra.utils import get_original_cwd, to_absolute_path
 
     # when user is using hydra find the absolute path
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from lightning_fabric.utilities.apply_func import move_data_to_device
 
 if TYPE_CHECKING:
     from lightning_fabric.strategies import XLAStrategy
 
 
 class _XLALauncher(_Launcher):
-    r"""Launches processes that run a given function in parallel on XLA supported hardware, and joins them all at the
-    end.
+    r"""Launches processes that run a given function in parallel on XLA supported hardware, and joins them all at
+    the end.
 
     The main process in which this launcher is invoked creates N so-called worker processes (using the
     `torch_xla` :func:`xmp.spawn`) that run the given function.
     Worker processes have a rank that ranges from 0 to N - 1.
 
     Note:
         - This launcher requires all objects to be pickleable.
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import importlib
 from inspect import getmembers, isclass
 from typing import Any, Callable, Dict, List, Optional
 
-from lightning_fabric.strategies.strategy import Strategy
 from lightning_fabric.utilities.registry import _is_register_method_overridden
 
 
 class _StrategyRegistry(dict):
     """This class is a Registry that stores information about the Training Strategies.
 
     The Strategies are mapped to strings. These strings are names that identify
@@ -78,15 +77,15 @@
             return strategy
 
         if strategy is not None:
             return do_register(strategy)
 
         return do_register
 
-    def get(self, name: str, default: Optional[Strategy] = None) -> Strategy:  # type: ignore[override]
+    def get(self, name: str, default: Optional[Any] = None) -> Any:
         """Calls the registered strategy with the required parameters and returns the strategy object.
 
         Args:
             name (str): the name that identifies a strategy, e.g. "deepspeed_stage_3"
         """
         if name in self:
             data = self[name]
@@ -109,10 +108,12 @@
 
     def __str__(self) -> str:
         return "Registered Strategies: {}".format(", ".join(self.keys()))
 
 
 def _call_register_strategies(registry: _StrategyRegistry, base_module: str) -> None:
     module = importlib.import_module(base_module)
+    from lightning_fabric.strategies.strategy import Strategy
+
     for _, mod in getmembers(module, isclass):
         if issubclass(mod, Strategy) and _is_register_method_overridden(mod, Strategy, "register_strategies"):
             mod.register_strategies(registry)
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_tpu.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from torch.utils.data import DataLoader
 
 from lightning_fabric.accelerators import Accelerator
 from lightning_fabric.plugins.io.checkpoint_io import CheckpointIO
 from lightning_fabric.plugins.io.torch_io import TorchCheckpointIO
 from lightning_fabric.plugins.precision import Precision
 from lightning_fabric.strategies.launchers.launcher import _Launcher
+from lightning_fabric.strategies.registry import _StrategyRegistry
 from lightning_fabric.utilities.apply_func import move_data_to_device
 from lightning_fabric.utilities.types import _PATH, _Stateful, Optimizable, ReduceOp
 
 TBroadcast = TypeVar("TBroadcast")
 TReduce = TypeVar("TReduce")
 
 log = logging.getLogger(__name__)
@@ -272,15 +273,15 @@
             raise KeyError(
                 f"The requested state contains a key '{invalid_keys[0]}' that does not exist in the loaded checkpoint."
             )
 
         for name, obj in state.copy().items():
             if name not in checkpoint:
                 continue
-            elif isinstance(obj, _Stateful):
+            if isinstance(obj, _Stateful):
                 if isinstance(obj, Module):
                     # TODO(fabric): Make strict loading configurable
                     obj.load_state_dict(checkpoint.pop(name), strict=True)
                 else:
                     obj.load_state_dict(checkpoint.pop(name))
             else:
                 state[name] = checkpoint.pop(name)
@@ -323,15 +324,15 @@
     def clip_gradients_value(self, module: torch.nn.Module, optimizer: Optimizer, clip_val: Union[float, int]) -> None:
         """Clip gradients by value."""
         self.precision.unscale_gradients(optimizer)
         parameters = self.precision.main_params(optimizer)
         return torch.nn.utils.clip_grad_value_(parameters, clip_value=clip_val)
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict[str, Any]) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         pass
 
     def _err_msg_joint_setup_required(self) -> str:
         return (
             f"The `{type(self).__name__}` does not support setting up the module and optimizer(s) independently."
             " Please call `setup_module_and_optimizers(model, [optimizer, ...])` to jointly set them up."
         )
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.0.3/src/lightning_fabric/strategies/xla.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from lightning_fabric.accelerators import Accelerator
 from lightning_fabric.accelerators.tpu import _XLA_AVAILABLE
 from lightning_fabric.plugins.environments import XLAEnvironment
 from lightning_fabric.plugins.io.checkpoint_io import CheckpointIO
 from lightning_fabric.plugins.io.xla import XLACheckpointIO
 from lightning_fabric.plugins.precision import Precision
-from lightning_fabric.strategies import ParallelStrategy
+from lightning_fabric.strategies import _StrategyRegistry, ParallelStrategy
 from lightning_fabric.strategies.launchers.xla import _XLALauncher
 from lightning_fabric.strategies.strategy import TBroadcast
 from lightning_fabric.utilities.data import has_len
 from lightning_fabric.utilities.rank_zero import rank_zero_only
 from lightning_fabric.utilities.types import _PATH, ReduceOp
 
 if TYPE_CHECKING and _XLA_AVAILABLE:
@@ -171,16 +171,15 @@
         torch.save(obj, buffer)
         data = bytearray(buffer.getbuffer())
         data_tensor = torch.tensor(data, device=self.root_device, dtype=torch.float)
         import torch_xla.core.xla_model as xm
 
         data = xm.all_gather(data_tensor)
         buffer = io.BytesIO(data.cpu().byte().numpy())
-        obj = torch.load(buffer)
-        return obj
+        return torch.load(buffer)
 
     def save_checkpoint(
         self, path: _PATH, state: Dict[str, Union[Module, Optimizer, Any]], storage_options: Optional[Any] = None
     ) -> None:
         """Save model, optimizer, and other state as a checkpoint file.
 
         Args:
@@ -199,15 +198,15 @@
         Args:
             filepath: Path to checkpoint
         """
         if self.local_rank == 0:
             self.checkpoint_io.remove_checkpoint(filepath)
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         strategy_registry.register("xla", cls, description=cls.__class__.__name__)
 
     def _set_world_ranks(self) -> None:
         if self.cluster_environment is None:
             return
         rank_zero_only.rank = self.cluster_environment.global_rank()
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/apply_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     Return:
         the same collection but with all contained tensors residing on the new device.
 
     See Also:
         - :meth:`torch.Tensor.to`
         - :class:`torch.device`
     """
-
     if isinstance(device, str):
         device = torch.device(device)
 
     def batch_to(data: Any) -> Any:
         kwargs = {}
         # Don't issue non-blocking transfers to CPU
         # Same with MPS due to a race condition bug: https://github.com/pytorch/pytorch/issues/83015
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,15 @@
 
 class _WrapAttrTag(LightningEnum):
     SET = "set"
     DEL = "del"
 
     def __call__(self, *args: Any) -> None:
         fn: Union[Callable[[object, str], None], Callable[[object, str, Any], None]]
-        if self == self.SET:
-            fn = setattr
-        else:
-            fn = delattr
+        fn = setattr if self == self.SET else delattr
         return fn(*args)
 
 
 def has_iterable_dataset(dataloader: object) -> bool:
     return hasattr(dataloader, "dataset") and isinstance(dataloader.dataset, IterableDataset)
 
 
@@ -72,16 +69,15 @@
             " to avoid having duplicate data."
         )
     return length is not None
 
 
 def _update_dataloader(dataloader: DataLoader, sampler: Union[Sampler, Iterable]) -> DataLoader:
     dl_args, dl_kwargs = _get_dataloader_init_args_and_kwargs(dataloader, sampler)
-    dataloader = _reinstantiate_wrapped_cls(dataloader, *dl_args, **dl_kwargs)
-    return dataloader
+    return _reinstantiate_wrapped_cls(dataloader, *dl_args, **dl_kwargs)
 
 
 def _get_dataloader_init_args_and_kwargs(
     dataloader: DataLoader,
     sampler: Union[Sampler, Iterable],
     disallow_batch_sampler: bool = False,
 ) -> Tuple[Tuple[Any], Dict[str, Any]]:
@@ -217,29 +213,29 @@
             else:
                 try:
                     batch_sampler = batch_sampler_cls(
                         sampler,
                         batch_size=batch_sampler.batch_size,
                         drop_last=batch_sampler.drop_last,
                     )
-                except TypeError as e:
+                except TypeError as ex:
                     import re
 
-                    match = re.match(r".*__init__\(\) (got multiple values)|(missing \d required)", str(e))
+                    match = re.match(r".*__init__\(\) (got multiple values)|(missing \d required)", str(ex))
                     if not match:
                         # an unexpected `TypeError`, continue failure
                         raise
 
                     # There could either be too few or too many arguments. Customizing the message based on this doesn't
                     # make much sense since our MisconfigurationException is going to be raised from the original one.
                     raise TypeError(
                         "We tried to re-instantiate your custom batch sampler and failed. "
                         "To mitigate this, either follow the API of `BatchSampler` or instantiate "
                         "your custom batch sampler inside `*_dataloader` hooks of your module."
-                    ) from e
+                    ) from ex
 
             return {
                 "sampler": None,
                 "shuffle": False,
                 "batch_sampler": batch_sampler,
                 "batch_size": 1,
                 "drop_last": False,
@@ -256,32 +252,32 @@
 
 
 def _reinstantiate_wrapped_cls(orig_object: Any, *args: Any, explicit_cls: Optional[Type] = None, **kwargs: Any) -> Any:
     constructor = type(orig_object) if explicit_cls is None else explicit_cls
 
     try:
         result = constructor(*args, **kwargs)
-    except TypeError as e:
+    except TypeError as ex:
         # improve exception message due to an incorrect implementation of the `DataLoader` where multiple subclass
         # `__init__` arguments map to one `DataLoader.__init__` argument
         import re
 
-        match = re.match(r".*__init__\(\) got multiple values .* '(\w+)'", str(e))
+        match = re.match(r".*__init__\(\) got multiple values .* '(\w+)'", str(ex))
         if not match:
             # an unexpected `TypeError`, continue failure
             raise
         argument = match.groups()[0]
         message = (
             f"The {constructor.__name__} implementation has an error where more than one `__init__` argument"
             f" can be passed to its parent's `{argument}=...` `__init__` argument. This is likely caused by allowing"
             f" passing both a custom argument that will map to the `{argument}` argument as well as `**kwargs`."
             f" `kwargs` should be filtered to make sure they don't contain the `{argument}` key."
             " This argument was automatically passed to your object by PyTorch Lightning."
         )
-        raise MisconfigurationException(message) from e
+        raise MisconfigurationException(message) from ex
 
     attrs_record = getattr(orig_object, "__pl_attrs_record", [])
     for args, fn in attrs_record:
         fn(result, *args)
 
     return result
 
@@ -405,15 +401,15 @@
     Returns a tuple indicating success of the operation and modified saved args and kwargs
     """
 
     if replace_key in arg_names:
         replace_index = arg_names.index(replace_key)
         args = args[:replace_index] + (replace_value,) + args[replace_index + 1 :]
         return True, args, kwargs
-    elif replace_key in kwargs or replace_key in default_kwargs:
+    if replace_key in kwargs or replace_key in default_kwargs:
         kwargs[replace_key] = replace_value
         return True, args, kwargs
 
     return False, args, kwargs
 
 
 def _set_sampler_epoch(dataloader: object, epoch: int) -> None:
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
     if not isinstance(gpus, list):
         raise TypeError("GPUs should be a list")
 
     assert len(gpus) > 0, "GPUs should be a non-empty list"
 
     # set root gpu
-    root_gpu = gpus[0]
-
-    return root_gpu
+    return gpus[0]
 
 
 def _parse_gpu_ids(
     gpus: Optional[Union[int, str, List[int]]],
     include_cuda: bool = False,
     include_mps: bool = False,
 ) -> Optional[List[int]]:
@@ -189,13 +187,13 @@
         MisconfigurationException:
             If ``device_ids`` of GPU/TPUs aren't ``int``, ``str``, sequence of ``int`` or ``None``
     """
     msg = "Device IDs (GPU/TPU) must be an int, a string, a sequence of ints or None, but you passed"
 
     if device_ids is None:
         return
-    elif isinstance(device_ids, (MutableSequence, tuple)):
+    if isinstance(device_ids, (MutableSequence, tuple)):
         for id_ in device_ids:
             if type(id_) is not int:
                 raise MisconfigurationException(f"{msg} a sequence of {type(id_).__name__}.")
     elif type(device_ids) not in (int, str):
         raise MisconfigurationException(f"{msg} {type(device_ids).__name__}.")
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,7 +26,10 @@
 _IS_INTERACTIVE = hasattr(sys, "ps1") or bool(sys.flags.interactive)
 
 _TORCH_GREATER_EQUAL_1_12 = compare_version("torch", operator.ge, "1.12.0")
 _TORCH_GREATER_EQUAL_1_13 = compare_version("torch", operator.ge, "1.13.0")
 _TORCH_GREATER_EQUAL_2_0 = compare_version("torch", operator.ge, "2.0.0", use_base_version=True)
 _TORCH_GREATER_EQUAL_2_1 = compare_version("torch", operator.ge, "2.1.0", use_base_version=True)
 _TORCH_EQUAL_2_0 = _TORCH_GREATER_EQUAL_2_0 and not _TORCH_GREATER_EQUAL_2_1
+
+_PYTHON_GREATER_EQUAL_3_8_0 = (sys.version_info.major, sys.version_info.minor) >= (3, 8)
+_PYTHON_GREATER_EQUAL_3_10_0 = (sys.version_info.major, sys.version_info.minor) >= (3, 10)
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         'float': 0.3,
         'int': 1,
         'layer': "<class 'torch.nn.modules.batchnorm.BatchNorm1d'>",
         'list': '[1, 2, 3]',
         'namespace': 'Namespace(foo=3)',
         'string': 'abc'}
     """
-    for k in params.keys():
+    for k in params:
         # convert relevant np scalars to python types first (instead of str)
         if isinstance(params[k], (np.bool_, np.integer, np.floating)):
             params[k] = params[k].item()
         elif type(params[k]) not in [bool, int, float, str, Tensor]:
             params[k] = str(params[k])
     return params
 
@@ -133,11 +133,10 @@
         metrics: Dictionary with metric names as keys and measured quantities as values
         prefix: Prefix to insert before each key
         separator: Separates prefix and original key name
 
     Returns:
         Dictionary with prefix and separator inserted before each key
     """
-    if prefix:
-        metrics = {f"{prefix}{separator}{k}": v for k, v in metrics.items()}
-
-    return metrics
+    if not prefix:
+        return metrics
+    return {f"{prefix}{separator}{k}": v for k, v in metrics.items()}
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/rank_zero.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Utilities that can be used for calling functions on a particular rank."""
 import logging
 import os
 from typing import Optional
 
 import lightning_utilities.core.rank_zero as rank_zero_module
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/seed.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     os.environ["PL_SEED_WORKERS"] = f"{int(workers)}"
 
     return seed
 
 
 def _select_seed_randomly(min_seed_value: int = min_seed_value, max_seed_value: int = max_seed_value) -> int:
-    return random.randint(min_seed_value, max_seed_value)
+    return random.randint(min_seed_value, max_seed_value)  # noqa: S311
 
 
 def reset_seed() -> None:
     """Reset the seed to the value that :func:`lightning_fabric.utilities.seed.seed_everything` previously set.
 
     If :func:`lightning_fabric.utilities.seed.seed_everything` is unused, this function will do nothing.
     """
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.0.3/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.0.3/src/lightning_fabric/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
-from typing import Any, Callable, Dict, Generator, Iterator, Mapping, Optional, overload, TypeVar, Union
+from typing import Any, Callable, Dict, Generator, Iterator, List, Mapping, Optional, overload, TypeVar, Union
 
 import torch
 from lightning_utilities import WarningCache
 from lightning_utilities.core.apply_func import apply_to_collection
 from torch import nn as nn
 from torch import Tensor
 from torch.nn.modules.module import _IncompatibleKeys
@@ -24,41 +24,41 @@
 from torch.utils.data import DataLoader
 
 from lightning_fabric.plugins import Precision
 from lightning_fabric.strategies import Strategy
 from lightning_fabric.utilities import move_data_to_device
 from lightning_fabric.utilities.data import _set_sampler_epoch
 from lightning_fabric.utilities.device_dtype_mixin import _DeviceDtypeModuleMixin
+from lightning_fabric.utilities.imports import _TORCH_GREATER_EQUAL_2_0
 from lightning_fabric.utilities.types import Optimizable
 from lightning_fabric.utilities.warnings import PossibleUserWarning
 
 warning_cache = WarningCache()
 T_destination = TypeVar("T_destination", bound=Dict[str, Any])
 _LIGHTNING_MODULE_STEP_METHODS = ("training_step", "validation_step", "test_step", "predict_step")
 
 
 class _FabricOptimizer:
-    def __init__(self, optimizer: Optimizer, strategy: Strategy) -> None:
+    def __init__(self, optimizer: Optimizer, strategy: Strategy, callbacks: Optional[List[Callable]] = None) -> None:
         """FabricOptimizer is a thin wrapper around the :class:`~torch.optim.Optimizer` that delegates the
         optimizer step calls to the strategy plugin.
 
         The underlying wrapped optimizer object can be accessed via the property :attr:`optimizer`.
 
         Args:
             optimizer: The optimizer to wrap
             strategy: Reference to the strategy for handling the optimizer step
         """
         # `__del__` is skipped in case the optimizer has implemented custom destructor logic which we would
         # not want to call on destruction of the `_FabricOptimizer
-        self.__dict__ = {
-            k: v for k, v in optimizer.__dict__.items() if k not in ("state_dict", "step", "zero_grad", "__del__")
-        }
+        self.__dict__ = {k: v for k, v in optimizer.__dict__.items() if k not in ("state_dict", "step", "__del__")}
         self.__class__ = type("Fabric" + optimizer.__class__.__name__, (self.__class__, optimizer.__class__), {})
         self._optimizer = optimizer
         self._strategy = strategy
+        self._callbacks = callbacks or []
 
     @property
     def optimizer(self) -> Optimizer:
         return self._optimizer
 
     def state_dict(self) -> Dict[str, Tensor]:
         return self._strategy.get_optimizer_state(self.optimizer)
@@ -66,22 +66,23 @@
     def step(self, closure: Optional[Callable] = None) -> Any:
         kwargs = {"closure": closure} if closure is not None else {}
         if hasattr(self._strategy, "model") and isinstance(self._strategy.model, Optimizable):
             # only DeepSpeed defines this
             optimizer = self._strategy.model
         else:
             optimizer = self.optimizer
-        return self._strategy.optimizer_step(
+        output = self._strategy.optimizer_step(
             optimizer,
             **kwargs,
         )
-
-    def zero_grad(self, **kwargs: Any) -> None:
-        kwargs = _process_optimizer_zero_grad_kwargs(self.optimizer, kwargs)
-        self.optimizer.zero_grad(**kwargs)
+        for callback in self._callbacks:
+            hook = getattr(callback, "on_after_optimizer_step", None)
+            if callable(hook):
+                hook(strategy=self._strategy, optimizer=optimizer)
+        return output
 
 
 class _FabricModule(_DeviceDtypeModuleMixin):
     def __init__(
         self, forward_module: nn.Module, precision: Precision, original_module: Optional[nn.Module] = None
     ) -> None:
         """The FabricModule is a thin wrapper around the :class:`torch.nn.Module` and handles precision / autocast
@@ -216,40 +217,54 @@
         if self._device is None:
             yield from iter(self._dataloader)
         else:
             for item in self._dataloader:
                 yield move_data_to_device(item, self._device)
 
 
-def _process_optimizer_zero_grad_kwargs(optimizer: Optimizer, kwargs: Dict[str, Any]) -> Dict[str, Any]:
-    if "set_to_none" in kwargs and "set_grads_to_None" in inspect.signature(optimizer.zero_grad).parameters:
-        # Some optimizers out there, for example DeepSpeedZeroOptimizer, use a different name than PyTorch
-        kwargs["set_grads_to_None"] = kwargs.pop("set_to_none")
-    return kwargs
-
-
 def _unwrap_objects(collection: Any) -> Any:
     def _unwrap(
         obj: Union[_FabricModule, _FabricOptimizer, _FabricDataLoader]
     ) -> Union[nn.Module, Optimizer, DataLoader]:
-        if isinstance(obj, _FabricModule):
-            return obj._forward_module
+        if isinstance(unwrapped := _unwrap_compiled(obj), _FabricModule):
+            return unwrapped._forward_module
         if isinstance(obj, _FabricOptimizer):
             return obj.optimizer
         if isinstance(obj, _FabricDataLoader):
             return obj._dataloader
         return obj
 
-    return apply_to_collection(collection, dtype=(_FabricModule, _FabricOptimizer, _FabricDataLoader), function=_unwrap)
+    types = [_FabricModule, _FabricOptimizer, _FabricDataLoader]
+    if _TORCH_GREATER_EQUAL_2_0:
+        from torch._dynamo import OptimizedModule
+
+        types.append(OptimizedModule)
+
+    return apply_to_collection(collection, dtype=tuple(types), function=_unwrap)
+
+
+def _unwrap_compiled(obj: Any) -> Any:
+    """Removes the :class:`torch._dynamo.OptimizedModule` around the object if it is wrapped.
+
+    Use this function before instance checks against e.g. :class:`_FabricModule`.
+    """
+    if not _TORCH_GREATER_EQUAL_2_0:
+        return obj
+    from torch._dynamo import OptimizedModule
+
+    if isinstance(obj, OptimizedModule):
+        return obj._orig_mod
+    return obj
 
 
 def is_wrapped(obj: object) -> bool:
     """Checks if an object was set up by Fabric.
 
     A :class:`~torch.nn.Module` may be wrapped by a :class:`_FabricModule`, a :class:`~torch.optim.Optimizer`
     may be wrapped by a :class:`_FabricOptimizer`, or a :class:`~torch.utils.data.DataLoader` may be wrapped by
     :class:`_FabricDataLoader`.
 
     Args:
         obj: The object to test.
     """
+    obj = _unwrap_compiled(obj)
     return isinstance(obj, (_FabricModule, _FabricOptimizer, _FabricDataLoader))
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.0.3/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.2
+Version: 2.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.0.3/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 .actions/assistant.py
 requirements/fabric/base.txt
-requirements/fabric/devel.txt
 requirements/fabric/docs.txt
 requirements/fabric/examples.txt
 requirements/fabric/strategies.txt
 requirements/fabric/test.txt
 src/version.info
 src/lightning_fabric/CHANGELOG.md
 src/lightning_fabric/MANIFEST.in
@@ -16,14 +15,15 @@
 src/lightning_fabric/__about__.py
 src/lightning_fabric/__init__.py
 src/lightning_fabric/__setup__.py
 src/lightning_fabric/__version__.py
 src/lightning_fabric/cli.py
 src/lightning_fabric/connector.py
 src/lightning_fabric/fabric.py
+src/lightning_fabric/py.typed
 src/lightning_fabric/version.info
 src/lightning_fabric/wrappers.py
 src/lightning_fabric.egg-info/PKG-INFO
 src/lightning_fabric.egg-info/SOURCES.txt
 src/lightning_fabric.egg-info/dependency_links.txt
 src/lightning_fabric.egg-info/not-zip-safe
 src/lightning_fabric.egg-info/requires.txt
```

### Comparing `lightning-fabric-2.0.2/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.0.3/src/lightning_fabric.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 torch>=1.11.0
 fsspec[http]>2021.06.0
 packaging>=17.1
 typing-extensions>=4.0.0
 lightning-utilities>=0.7.0
 
 [all]
-torchvision>=0.10.0
+torchvision>=0.12.0
 torchmetrics>=0.10.0
 lightning-utilities>=0.8.0
 
 [all:platform_system != "Windows"]
-deepspeed>=0.6.0
+deepspeed>=0.8.2
 
 [deepspeed]
 
 [deepspeed:platform_system != "Windows"]
-deepspeed>=0.6.0
+deepspeed>=0.8.2
 
 [dev]
-torchvision>=0.10.0
+torchvision>=0.12.0
 torchmetrics>=0.10.0
 lightning-utilities>=0.8.0
-coverage==6.5.0
-pytest==7.2.0
+coverage==7.2.5
+pytest==7.3.1
 pytest-cov==4.0.0
 pytest-rerunfailures==10.3
 click==8.1.3
 tensorboardX>=2.2
 
 [dev:platform_system != "Windows"]
-deepspeed>=0.6.0
+deepspeed>=0.8.2
 
 [examples]
-torchvision>=0.10.0
+torchvision>=0.12.0
 torchmetrics>=0.10.0
 lightning-utilities>=0.8.0
 
 [strategies]
 
 [strategies:platform_system != "Windows"]
-deepspeed>=0.6.0
+deepspeed>=0.8.2
 
 [test]
-coverage==6.5.0
-pytest==7.2.0
+coverage==7.2.5
+pytest==7.3.1
 pytest-cov==4.0.0
 pytest-rerunfailures==10.3
 click==8.1.3
 tensorboardX>=2.2
```

