# Comparing `tmp/jac_misc-1.4.0.9.tar.gz` & `tmp/jac_misc-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_misc-1.4.0.9.tar", last modified: Tue Feb 14 17:26:20 2023, max compression
+gzip compressed data, was "jac_misc-1.4.1.0.tar", last modified: Wed Jun  7 18:25:06 2023, max compression
```

## Comparing `jac_misc-1.4.0.9.tar` & `jac_misc-1.4.1.0.tar`

### file list

```diff
@@ -1,55 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.977539 jac_misc-1.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-14 17:26:20.977539 jac_misc-1.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.969539 jac_misc-1.4.0.9/jac_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.973539 jac_misc-1.4.0.9/jac_misc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/cluster/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.973539 jac_misc-1.4.0.9/jac_misc/cluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/cluster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/cluster/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.973539 jac_misc-1.4.0.9/jac_misc/example_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/example_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/example_module/example_module.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/example_module/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.973539 jac_misc-1.4.0.9/jac_misc/pdf_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/pdf_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/pdf_ext/pdf_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/pdf_ext/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.973539 jac_misc-1.4.0.9/jac_misc/pdf_ext/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/pdf_ext/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/pdf_ext/tests/test_pdf_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.977539 jac_misc-1.4.0.9/jac_misc/ph/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/ph.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.977539 jac_misc-1.4.0.9/jac_misc/ph/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/ph/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.977539 jac_misc-1.4.0.9/jac_misc/translator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/translator/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/jac_misc/translator/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:20.973539 jac_misc-1.4.0.9/jac_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-14 17:26:20.000000 jac_misc-1.4.0.9/jac_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-14 17:26:20.000000 jac_misc-1.4.0.9/jac_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:20.000000 jac_misc-1.4.0.9/jac_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-14 17:26:20.000000 jac_misc-1.4.0.9/jac_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-14 17:26:20.000000 jac_misc-1.4.0.9/jac_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:26:20.977539 jac_misc-1.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-14 17:25:58.000000 jac_misc-1.4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.556879 jac_misc-1.4.1.0/jac_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/cluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/cluster.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/example_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/example_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/example_module/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/example_module/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/openai/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/openai/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/pdf_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/pdf_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.564879 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/test_pdf_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.564879 jac_misc-1.4.1.0/jac_misc/ph/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/ph_train_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/run_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.564879 jac_misc-1.4.1.0/jac_misc/ph/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/jac_misc/translator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/translator/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/setup.py
```

### Comparing `jac_misc-1.4.0.9/jac_misc/cluster/cluster.py` & `jac_misc-1.4.1.0/jac_misc/cluster/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import umap
 import hdbscan
 
 import numpy as np
 
 import sklearn.cluster as cluster
 
-from jaseci.actions.live_actions import jaseci_action
-from jaseci.actions.remote_actions import launch_server
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.jsorc.remote_actions import launch_server
 from fastapi import HTTPException
 
 
 def get_umap_embedds(
     text_embeddings: list, n_neighbors=15, min_dist=0.1, n_components=2, random_state=42
 ):
     """
```

### Comparing `jac_misc-1.4.0.9/jac_misc/cluster/tests/test_cluster.py` & `jac_misc-1.4.1.0/jac_misc/cluster/tests/test_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 
 
 class TextClusterModule(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `jac_misc-1.4.0.9/jac_misc/pdf_ext/pdf_ext.py` & `jac_misc-1.4.1.0/jac_misc/pdf_ext/pdf_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import os
 import re
 import uuid
 
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from PyPDF2 import PdfFileReader
 from fastapi import HTTPException
 
 
 def download_pdf(url: str, filename: str):
     r"""method for downloading PDF from URL
     :param url: URL for the downloading a pdf file.
@@ -91,10 +91,10 @@
             return data
         raise HTTPException(status_code=400, detail=str("Invalid path"))
     else:
         raise HTTPException(status_code=400, detail=str("Missing params url/path"))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_misc-1.4.0.9/jac_misc/pdf_ext/tests/test_pdf_ext.py` & `jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/test_pdf_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 
 
 class PDFExtModule(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/config.yaml` & `jac_misc-1.4.1.0/jac_misc/ph/config.yaml`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/inference.py` & `jac_misc-1.4.1.0/jac_misc/ph/inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,14 +127,22 @@
         else:
             raise ImproperConnectionState("Inference Engine not found.")
 
     def train(self, uuid: str, config: Dict = None, auto_update=True) -> None:  # type: ignore
         if self.check(uuid):
             ph_config = self.ie_list[uuid].ph_config
             if config:
+                # If the training data is passed in, save it to a file first
+                dataset = config["Trainer"]["dataloader"]["args"].get("data_dict", None)
+                if dataset:
+                    data_loc = config["Trainer"]["dataloader"]["args"].get("data_dir")
+                    with open(data_loc, "w") as fout:
+                        json.dump(dataset, fout)
+                    del config["Trainer"]["dataloader"]["args"]["data_dict"]
+
                 deep_update(ph_config, config)
                 write_yaml(ph_config, f"heads/{uuid}/config.yaml")
             resume = (
                 f"heads/{uuid}/current.pth"
                 if os.path.exists(f"heads/{uuid}/current.pth")
                 else None
             )
```

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/ph.py` & `jac_misc-1.4.1.0/jac_misc/ph/ph.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 from typing import Any, Dict
 import warnings
 import os
 import traceback
 from fastapi import HTTPException
 import logging
 
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 
 from .utils.util import read_yaml, deep_update, save_custom_python
 from .inference import InferenceList
 
 warnings.filterwarnings("ignore")
 
 
 HEAD_NOT_FOUND = "No Active head found. Please create a head first using create_head."
 HEAD_LIST_NOT_FOUND = "No Active head list found. Use create_head_list first."
 
 
+@jaseci_action(act_group=["ph"], allow_remote=True)
 def setup():
     global il, list_config
     dirname = os.path.dirname(__file__)
     list_config = read_yaml(os.path.join(dirname, "config.yaml"))
     if os.path.exists("heads/config.yaml") and os.path.exists("heads/custom.py"):
         logging.warning("Found a heads list in the current directory. Loading it ...")
         il = InferenceList(config=read_yaml("heads/config.yaml"))
     else:
         logging.info("No heads list found. Run create_head_list to create one.")
         il = None
 
 
-setup()
-
 ### Start of PersonalizedHead Actions ###
 
 
 @jaseci_action(act_group=["ph"], allow_remote=True)
 def create_head_list(config: Dict = None, python: str = None) -> None:
     """
     Create a holder for all the heads
@@ -151,10 +150,10 @@
         raise HTTPException(status_code=500, detail=str(e))
 
 
 ### End of PersonalizedHead Actions ###
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/train.py` & `jac_misc-1.4.1.0/jac_misc/ph/train.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/base.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     def _resume_checkpoint(self, resume_path):
         """
         Resume from saved checkpoints
         :param resume_path: Checkpoint path to be resumed
         """
         resume_path = str(resume_path)
         self.logger.info("Loading checkpoint: {} ...".format(resume_path))
-        checkpoint = torch.load(resume_path)
+        checkpoint = torch.load(resume_path, map_location=torch.device("cpu"))
         self.start_epoch = checkpoint.get("epoch", 0) + 1
         self.epochs += checkpoint.get("epoch", 0)
         self.mnt_best = checkpoint.get("monitor_best", 0)
 
         # load architecture params from checkpoint.
         state_dict = checkpoint.get("state_dict", checkpoint)
         model_keys = list(self.model.state_dict().keys())
@@ -300,40 +300,43 @@
         model_config = self.config["Model"]
         self.infer_config = self.config["Inference"]
 
         self.model = getattr(model_module, model_config["type"])(
             **model_config.get("args", {})
         )
 
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
         # loading pretrained weights
         if self.infer_config["weights"]:
             if not os.path.exists(f"heads/{uuid}/current.pth"):
                 shutil.copyfile(
-                    self.infer_config["weights"], f"heads/{self.id}/current.pth"
+                    self.infer_config["weights"], f"heads/{uuid}/current.pth"
                 )
-                self.logger.info(
+                logger.info(
                     "Loading default checkpoint: {} ...".format(
                         self.infer_config["weights"]
                     )
                 )
 
-            checkpoint = torch.load(f"heads/{self.id}/current.pth")
+            checkpoint = torch.load(
+                f"heads/{uuid}/current.pth", map_location=torch.device("cpu")
+            )
             state_dict = checkpoint.get("state_dict", checkpoint)
             model_keys = list(self.model.state_dict().keys())
             if model_keys[0].startswith("model."):
                 new_state_dict = OrderedDict()
                 for k, v in state_dict.items():
                     name = "model." + k
                     new_state_dict[name] = v
                 state_dict = new_state_dict
             self.model.load_state_dict(state_dict)
             logger.info("Checkpoint loaded.")
 
         # Setting the device
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.model = self.model.to(self.device)
         self.model.eval()
 
         # Get Intermediate Activations
         self.out_activation_layer = self.infer_config.get("out_activation_layer", None)
         if self.out_activation_layer:
             self.activation = {}
@@ -354,15 +357,15 @@
     def preprocess(self, data: Any) -> Any:
         raise NotImplementedError
 
     def postprocess(self, data: Any) -> Any:
         raise NotImplementedError
 
     def load_weights(self, weights: str) -> None:
-        checkpoint = torch.load(weights)
+        checkpoint = torch.load(weights, map_location=torch.device("cpu"))
         state_dict = checkpoint.get("state_dict", checkpoint)
         self.model.load_state_dict(state_dict)
 
     def get_activation(self, name):
         def hook(model, input, output):
             self.activation[name] = output.detach()
```

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/dataloader.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/logger.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/logger.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/loss.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/loss.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/metric.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/metric.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/model.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/model.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/process.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/process.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/trainer.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/ph/utils/util.py` & `jac_misc-1.4.1.0/jac_misc/ph/utils/util.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.0.9/jac_misc/translator/translator.py` & `jac_misc-1.4.1.0/jac_misc/translator/translator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from transformers import MBartForConditionalGeneration, MBart50TokenizerFast
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from typing import Union, List
 from fastapi import HTTPException
 import traceback
-import torch
 
+model = None
+tokenizer = None
 
+
+@jaseci_action(act_group=["translator"], allow_remote=True)
 def setup():
+    global model, tokenizer, supported_languages
     model = MBartForConditionalGeneration.from_pretrained(
         "facebook/mbart-large-50-many-to-many-mmt"
     )
     tokenizer = MBart50TokenizerFast.from_pretrained(
         "facebook/mbart-large-50-many-to-many-mmt"
     )
-    return model, tokenizer
+    supported_languages = list(tokenizer.lang_code_to_id.keys())
 
 
-model, tokenizer = setup()
-supported_languages = list(tokenizer.lang_code_to_id.keys())
+setup()
 
 
 @jaseci_action(act_group=["translator"], allow_remote=True)
 def translate(text: Union[str, List[str]], src_lang: str, tgt_lang: str) -> List[str]:
     """
     Translate text from one language to another.
 
@@ -29,14 +32,15 @@
         text (Union[str, List[str]]): Text to translate.
         src_lang (str): Source language.
         tgt_lang (str): Target language.
 
     Returns:
         List[str]: Translated text.
     """
+    global model, tokenizer
     try:
         if src_lang not in supported_languages:
             raise ValueError(f"Unsupported source language: {src_lang}")
         if tgt_lang not in supported_languages:
             raise ValueError(f"Unsupported target language: {tgt_lang}")
 
         if isinstance(text, str):
```

### Comparing `jac_misc-1.4.0.9/jac_misc.egg-info/SOURCES.txt` & `jac_misc-1.4.1.0/jac_misc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,41 @@
 jac_misc.egg-info/requires.txt
 jac_misc.egg-info/top_level.txt
 jac_misc/cluster/__init__.py
 jac_misc/cluster/cluster.py
 jac_misc/cluster/requirements.txt
 jac_misc/cluster/tests/__init__.py
 jac_misc/cluster/tests/test_cluster.py
+jac_misc/cluster/tests/fixtures/__init__.py
+jac_misc/cluster/tests/fixtures/cluster.jac
 jac_misc/example_module/__init__.py
 jac_misc/example_module/example_module.py
 jac_misc/example_module/requirements.txt
+jac_misc/huggingface/__init__.py
+jac_misc/huggingface/huggingface.py
+jac_misc/huggingface/requirements.txt
+jac_misc/huggingface/utils.py
+jac_misc/openai/__init__.py
+jac_misc/openai/main.py
+jac_misc/openai/requirements.txt
 jac_misc/pdf_ext/__init__.py
 jac_misc/pdf_ext/pdf_ext.py
 jac_misc/pdf_ext/requirements.txt
 jac_misc/pdf_ext/tests/__init__.py
 jac_misc/pdf_ext/tests/test_pdf_ext.py
+jac_misc/pdf_ext/tests/fixtures/__init__.py
+jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac
 jac_misc/ph/__init__.py
 jac_misc/ph/config.yaml
+jac_misc/ph/custom.py
 jac_misc/ph/inference.py
 jac_misc/ph/ph.py
+jac_misc/ph/ph_train_data.json
 jac_misc/ph/requirements.txt
+jac_misc/ph/run_ph.py
 jac_misc/ph/train.py
 jac_misc/ph/utils/__init__.py
 jac_misc/ph/utils/base.py
 jac_misc/ph/utils/dataloader.py
 jac_misc/ph/utils/logger.py
 jac_misc/ph/utils/loss.py
 jac_misc/ph/utils/metric.py
```

### Comparing `jac_misc-1.4.0.9/setup.py` & `jac_misc-1.4.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from os.path import join
 
-MODULES = ["pdf_ext", "translator", "cluster", "ph"]
+MODULES = ["pdf_ext", "translator", "cluster", "ph", "openai", "huggingface"]
 
 
 def get_ver():
     with open(join("./jac_misc", "VERSION")) as version_file:
         return version_file.read().strip()
 
 
@@ -18,16 +18,20 @@
     return extras_requires
 
 
 setup(
     name="jac_misc",
     version=get_ver(),
     packages=find_packages(include=["jac_misc", "jac_misc.*"]),
-    install_requires=["jaseci", "pytest>=7.0.1,<7.1", "pytest-order>=1.0.1,<1.1"],
+    install_requires=[
+        f"jaseci=={get_ver()}",
+        "pytest>=7.0.1,<7.1",
+        "pytest-order>=1.0.1,<1.1",
+    ],
     extras_require=get_extras_requires(),
     package_data={
-        "": ["*.json", "*.cfg", "VERSION", "*.yaml", "requirements.txt"],
+        "": ["*.json", "*.cfg", "VERSION", "*.yaml", "requirements.txt", "*.jac"],
     },
     author="Jason Mars",
     author_email="jason@jaseci.org",
     url="https://github.com/Jaseci-Labs/jaseci/jaseci_ai_kit/jac_misc",
 )
```

