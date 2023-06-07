# Comparing `tmp/fastxtend-0.1.2.tar.gz` & `tmp/fastxtend-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastxtend-0.1.2.tar", last modified: Wed Mar 29 04:21:15 2023, max compression
+gzip compressed data, was "fastxtend-0.1.3.tar", last modified: Wed Jun  7 16:45:08 2023, max compression
```

## Comparing `fastxtend-0.1.2.tar` & `fastxtend-0.1.3.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/
--rw-r--r--   0 benja     (1000) benja     (1000)     1072 2023-01-10 05:21:20.000000 fastxtend-0.1.2/LICENSE
--rw-r--r--   0 benja     (1000) benja     (1000)     7335 2023-03-29 04:21:15.152789 fastxtend-0.1.2/PKG-INFO
--rw-r--r--   0 benja     (1000) benja     (1000)     6410 2023-03-29 04:16:58.000000 fastxtend-0.1.2/README.md
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.142789 fastxtend-0.1.2/fastxtend/
--rw-r--r--   0 benja     (1000) benja     (1000)       22 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)   187401 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/_modidx.py
--rw-r--r--   0 benja     (1000) benja     (1000)    14016 2022-09-18 15:27:45.000000 fastxtend-0.1.2/fastxtend/_nbdev.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/audio/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/audio/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)      493 2023-03-07 02:46:03.000000 fastxtend-0.1.2/fastxtend/audio/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)    30130 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/audio/augment.py
--rw-r--r--   0 benja     (1000) benja     (1000)     6870 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/audio/core.py
--rw-r--r--   0 benja     (1000) benja     (1000)    11546 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/audio/data.py
--rw-r--r--   0 benja     (1000) benja     (1000)     3500 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/audio/learner.py
--rw-r--r--   0 benja     (1000) benja     (1000)    11276 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/audio/mixup.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2728 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/basics.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/callback/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)      248 2023-03-07 02:46:03.000000 fastxtend-0.1.2/fastxtend/callback/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     1707 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/channelslast.py
--rw-r--r--   0 benja     (1000) benja     (1000)    10716 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/compiler.py
--rw-r--r--   0 benja     (1000) benja     (1000)    17890 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/cutmixup.py
--rw-r--r--   0 benja     (1000) benja     (1000)    10936 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/ema.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4583 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/lr_finder.py
--rw-r--r--   0 benja     (1000) benja     (1000)    22198 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/profiler.py
--rw-r--r--   0 benja     (1000) benja     (1000)    17099 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/progresize.py
--rw-r--r--   0 benja     (1000) benja     (1000)      160 2023-03-19 17:04:21.000000 fastxtend-0.1.2/fastxtend/callback/simpleprofiler.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2815 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/callback/tracker.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/data/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/data/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)       25 2022-06-06 01:55:48.000000 fastxtend-0.1.2/fastxtend/data/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2332 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/data/transforms.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/ffcv/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)      326 2023-03-28 02:14:44.000000 fastxtend-0.1.2/fastxtend/ffcv/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     6469 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/fields.py
--rw-r--r--   0 benja     (1000) benja     (1000)      148 2023-03-28 02:14:44.000000 fastxtend-0.1.2/fastxtend/ffcv/fx.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4885 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/inference.py
--rw-r--r--   0 benja     (1000) benja     (1000)    11128 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/loader.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4620 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/operations.py
--rw-r--r--   0 benja     (1000) benja     (1000)    35082 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/transforms.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2838 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/utils.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4310 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/ffcv/writer.py
--rw-r--r--   0 benja     (1000) benja     (1000)      837 2023-03-28 02:14:44.000000 fastxtend-0.1.2/fastxtend/imports.py
--rw-r--r--   0 benja     (1000) benja     (1000)     6746 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/losses.py
--rw-r--r--   0 benja     (1000) benja     (1000)    41980 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/metrics.py
--rw-r--r--   0 benja     (1000) benja     (1000)    12155 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/multiloss.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/optimizer/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/optimizer/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)    11769 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/optimizer/adan.py
--rw-r--r--   0 benja     (1000) benja     (1000)       93 2023-03-07 02:46:03.000000 fastxtend-0.1.2/fastxtend/optimizer/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)    15593 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/optimizer/foreach.py
--rw-r--r--   0 benja     (1000) benja     (1000)    18201 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/optimizer/fused.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4337 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/optimizer/lion.py
--rw-r--r--   0 benja     (1000) benja     (1000)    15094 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/optimizer/torchscript.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2987 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/patches.py
--rw-r--r--   0 benja     (1000) benja     (1000)     7538 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/schedulers.py
--rw-r--r--   0 benja     (1000) benja     (1000)     1554 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/test_utils.py
--rw-r--r--   0 benja     (1000) benja     (1000)      857 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/torch_core.py
--rw-r--r--   0 benja     (1000) benja     (1000)     2643 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/transform.py
--rw-r--r--   0 benja     (1000) benja     (1000)     3382 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/utils.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/vision/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)      324 2022-11-17 00:19:44.000000 fastxtend-0.1.2/fastxtend/vision/all.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/vision/augment/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/augment/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)       46 2022-08-02 17:05:20.000000 fastxtend-0.1.2/fastxtend/vision/augment/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     7734 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/augment/batch.py
--rw-r--r--   0 benja     (1000) benja     (1000)     6251 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/augment/itemtensor.py
--rw-r--r--   0 benja     (1000) benja     (1000)     1865 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/data.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend/vision/models/
--rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/models/__init__.py
--rw-r--r--   0 benja     (1000) benja     (1000)       78 2022-05-31 22:44:08.000000 fastxtend-0.1.2/fastxtend/vision/models/all.py
--rw-r--r--   0 benja     (1000) benja     (1000)     4796 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/models/attention_modules.py
--rw-r--r--   0 benja     (1000) benja     (1000)     1560 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/models/pooling.py
--rw-r--r--   0 benja     (1000) benja     (1000)    15564 2023-03-29 04:19:08.000000 fastxtend-0.1.2/fastxtend/vision/models/xresnet.py
-drwxr-xr-x   0 benja     (1000) benja     (1000)        0 2023-03-29 04:21:15.152789 fastxtend-0.1.2/fastxtend.egg-info/
--rw-r--r--   0 benja     (1000) benja     (1000)     7335 2023-03-29 04:21:15.000000 fastxtend-0.1.2/fastxtend.egg-info/PKG-INFO
--rw-r--r--   0 benja     (1000) benja     (1000)     2027 2023-03-29 04:21:15.000000 fastxtend-0.1.2/fastxtend.egg-info/SOURCES.txt
--rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-03-29 04:21:15.000000 fastxtend-0.1.2/fastxtend.egg-info/dependency_links.txt
--rw-r--r--   0 benja     (1000) benja     (1000)       40 2023-03-29 04:21:15.000000 fastxtend-0.1.2/fastxtend.egg-info/entry_points.txt
--rw-r--r--   0 benja     (1000) benja     (1000)        1 2022-06-01 06:44:50.000000 fastxtend-0.1.2/fastxtend.egg-info/not-zip-safe
--rw-r--r--   0 benja     (1000) benja     (1000)      569 2023-03-29 04:21:15.000000 fastxtend-0.1.2/fastxtend.egg-info/requires.txt
--rw-r--r--   0 benja     (1000) benja     (1000)       10 2023-03-29 04:21:15.000000 fastxtend-0.1.2/fastxtend.egg-info/top_level.txt
--rw-r--r--   0 benja     (1000) benja     (1000)       38 2023-03-29 04:21:15.152789 fastxtend-0.1.2/setup.cfg
--rw-r--r--   0 benja     (1000) benja     (1000)     3243 2023-03-28 02:14:45.000000 fastxtend-0.1.2/setup.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.373530 fastxtend-0.1.3/
+-rw-r--r--   0 benja     (1000) benja     (1000)     1072 2023-02-21 17:38:09.000000 fastxtend-0.1.3/LICENSE
+-rw-rw-r--   0 benja     (1000) benja     (1000)     7778 2023-06-07 16:45:08.373530 fastxtend-0.1.3/PKG-INFO
+-rw-rw-r--   0 benja     (1000) benja     (1000)     6853 2023-06-07 15:14:37.000000 fastxtend-0.1.3/README.md
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.361530 fastxtend-0.1.3/fastxtend/
+-rw-rw-r--   0 benja     (1000) benja     (1000)       22 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)   209914 2023-06-07 16:16:41.000000 fastxtend-0.1.3/fastxtend/_modidx.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend/audio/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/audio/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      493 2023-03-11 21:10:32.000000 fastxtend-0.1.3/fastxtend/audio/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    30135 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/augment.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     6870 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/core.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    11546 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/data.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     3500 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/learner.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    11276 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/audio/mixup.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     2728 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/basics.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend/callback/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/callback/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      248 2023-03-11 21:10:32.000000 fastxtend-0.1.3/fastxtend/callback/all.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     1707 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/channelslast.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    14473 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/compiler.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    17890 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/cutmixup.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    10936 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/ema.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4583 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/lr_finder.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    21973 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/profiler.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    17703 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/progresize.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      160 2023-03-20 20:46:25.000000 fastxtend-0.1.3/fastxtend/callback/simpleprofiler.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     2815 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/callback/tracker.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend/data/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/data/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)       25 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/data/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     2332 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/data/transforms.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/ffcv/
+-rw-rw-r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/ffcv/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      326 2023-03-27 07:41:32.000000 fastxtend-0.1.3/fastxtend/ffcv/all.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     3945 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/epoch_iterator.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     6469 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/fields.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      148 2023-03-27 07:41:32.000000 fastxtend-0.1.3/fastxtend/ffcv/fx.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4885 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/inference.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    12850 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/loader.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4556 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/operations.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    35082 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/transforms.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     2838 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/utils.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4310 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/ffcv/writer.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      837 2023-03-27 07:41:33.000000 fastxtend-0.1.3/fastxtend/imports.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     6746 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/losses.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    41980 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/metrics.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    12155 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/multiloss.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/optimizer/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/optimizer/__init__.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    11746 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/adan.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      163 2023-06-06 06:08:24.000000 fastxtend-0.1.3/fastxtend/optimizer/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    20144 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/eightbit.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    15451 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/foreach.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    22375 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/fused.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     5012 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/lion.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     9351 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/sophia.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     7601 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/stableadam.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)    15022 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/optimizer/torchscript.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     2987 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/patches.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     7538 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/schedulers.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     1993 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/test_utils.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)      857 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/torch_core.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     2643 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/transform.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     4545 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/utils.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/vision/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)      324 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/vision/all.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.369530 fastxtend-0.1.3/fastxtend/vision/augment/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/augment/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)       46 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/vision/augment/all.py
+-rw-rw-r--   0 benja     (1000) benja     (1000)     7734 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/vision/augment/batch.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     6251 2023-06-07 15:20:54.000000 fastxtend-0.1.3/fastxtend/vision/augment/itemtensor.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     1865 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/data.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.373530 fastxtend-0.1.3/fastxtend/vision/models/
+-rw-r--r--   0 benja     (1000) benja     (1000)        0 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/__init__.py
+-rw-r--r--   0 benja     (1000) benja     (1000)       78 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend/vision/models/all.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     4796 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/attention_modules.py
+-rw-r--r--   0 benja     (1000) benja     (1000)     1560 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/pooling.py
+-rw-r--r--   0 benja     (1000) benja     (1000)    15564 2023-06-07 15:20:55.000000 fastxtend-0.1.3/fastxtend/vision/models/xresnet.py
+drwxrwxr-x   0 benja     (1000) benja     (1000)        0 2023-06-07 16:45:08.365530 fastxtend-0.1.3/fastxtend.egg-info/
+-rw-r--r--   0 benja     (1000) benja     (1000)     7778 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/PKG-INFO
+-rw-r--r--   0 benja     (1000) benja     (1000)     2136 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/SOURCES.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/dependency_links.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)       40 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/entry_points.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)        1 2023-02-21 17:38:10.000000 fastxtend-0.1.3/fastxtend.egg-info/not-zip-safe
+-rw-r--r--   0 benja     (1000) benja     (1000)      611 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/requires.txt
+-rw-r--r--   0 benja     (1000) benja     (1000)       10 2023-06-07 16:45:08.000000 fastxtend-0.1.3/fastxtend.egg-info/top_level.txt
+-rw-rw-r--   0 benja     (1000) benja     (1000)       38 2023-06-07 16:45:08.373530 fastxtend-0.1.3/setup.cfg
+-rw-rw-r--   0 benja     (1000) benja     (1000)     3243 2023-03-27 07:41:33.000000 fastxtend-0.1.3/setup.py
```

### Comparing `fastxtend-0.1.2/LICENSE` & `fastxtend-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/PKG-INFO` & `fastxtend-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastxtend
-Version: 0.1.2
+Version: 0.1.3
 Summary: Train fastai models faster (and other useful tools)
 Home-page: https://github.com/warner-benjamin/fastxtend
 Author: Benjamin Warner
 Author-email: me@benjaminwarner.dev
 License: MIT License
 Project-URL: Documentation, https://fastxtend.benjaminwarner.dev/
 Keywords: fastai pytorch extensions
@@ -49,18 +49,23 @@
 
 ## Feature overview
 
 **Train Models Faster**
 
 - Drop in [fused optimizers](optimizer.fused.html), which are 21 to 293
   percent faster then fastai native optimizers.
+- Up to 75% optimizer memory savings with integrated
+  [bitsandbytes](https://github.com/TimDettmers/bitsandbytes) [8-bit
+  optimizers](optimizer.eightbit.html).
 - Increase GPU throughput and decrease training time with the
   [Progressive Resizing](callback.progresize.html) callback.
 - Use the highly optimized [FFCV DataLoader](ffcv.tutorial.html), fully
   integrated with fastai.
+- Integrated support for `torch.compile` via the
+  [Compile](callback.compiler.html) callbacks.
 
 **General Features**
 
 - Fused implementations of modern optimizers, such as
   [Adan](optimizer.adan.html) and [Lion](optimizer.lion.html).
 - Flexible [metrics](metrics.html) which can log on train, valid, or
   both. Backwards compatible with fastai metrics.
@@ -160,19 +165,20 @@
 ```
 
 To easily install prerequisites for all fastxtend features, use
 [Conda](https://docs.conda.io/en/latest) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html):
 
 ``` bash
-conda create -n fastxtend python=3.10 pytorch torchvision \
-torchaudio pytorch-cuda=11.8 cuda fastai nbdev pkg-config \
-libjpeg-turbo opencv tqdm terminaltables psutil numpy=1.23.5 \
-numba librosa=0.9.2 timm kornia rich typer wandb -c pytorch \
--c nvidia/label/cuda-11.8.0 -c fastai -c huggingface -c conda-forge
+conda create -n fastxtend python=3.10 "pytorch>=2.0.0" \
+torchvision torchaudio pytorch-cuda=11.8 cuda fastai nbdev \
+pkg-config libjpeg-turbo opencv tqdm terminaltables psutil \
+numpy numba librosa=0.9.2 timm kornia rich typer wandb \
+-c pytorch -c nvidia/label/cuda-11.8.0 -c fastai \
+-c huggingface -c conda-forge
 
 conda activate fastxtend
 ```
 
 replacing `pytorch-cuda=11.8` and `nvidia/label/cuda-11.8.0` with your
 preferred [supported version of
 Cuda](https://pytorch.org/get-started/locally). Then install fastxtend
@@ -232,7 +238,13 @@
 
 ``` python
 from fastxtend.callback import simpleprofiler
 
 learn = Learner(...).profile()
 learn.fit_one_cycle(2, 3e-3)
 ```
+
+## Benchmark
+
+To run the benchmark on your own machine, see the [example
+scripts](https://github.com/warner-benjamin/fastxtend/tree/main/examples)
+for details on how to replicate.
```

### Comparing `fastxtend-0.1.2/README.md` & `fastxtend-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,23 @@
 
 ## Feature overview
 
 **Train Models Faster**
 
 - Drop in [fused optimizers](optimizer.fused.html), which are 21 to 293
   percent faster then fastai native optimizers.
+- Up to 75% optimizer memory savings with integrated
+  [bitsandbytes](https://github.com/TimDettmers/bitsandbytes) [8-bit
+  optimizers](optimizer.eightbit.html).
 - Increase GPU throughput and decrease training time with the
   [Progressive Resizing](callback.progresize.html) callback.
 - Use the highly optimized [FFCV DataLoader](ffcv.tutorial.html), fully
   integrated with fastai.
+- Integrated support for `torch.compile` via the
+  [Compile](callback.compiler.html) callbacks.
 
 **General Features**
 
 - Fused implementations of modern optimizers, such as
   [Adan](optimizer.adan.html) and [Lion](optimizer.lion.html).
 - Flexible [metrics](metrics.html) which can log on train, valid, or
   both. Backwards compatible with fastai metrics.
@@ -133,19 +138,20 @@
 ```
 
 To easily install prerequisites for all fastxtend features, use
 [Conda](https://docs.conda.io/en/latest) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html):
 
 ``` bash
-conda create -n fastxtend python=3.10 pytorch torchvision \
-torchaudio pytorch-cuda=11.8 cuda fastai nbdev pkg-config \
-libjpeg-turbo opencv tqdm terminaltables psutil numpy=1.23.5 \
-numba librosa=0.9.2 timm kornia rich typer wandb -c pytorch \
--c nvidia/label/cuda-11.8.0 -c fastai -c huggingface -c conda-forge
+conda create -n fastxtend python=3.10 "pytorch>=2.0.0" \
+torchvision torchaudio pytorch-cuda=11.8 cuda fastai nbdev \
+pkg-config libjpeg-turbo opencv tqdm terminaltables psutil \
+numpy numba librosa=0.9.2 timm kornia rich typer wandb \
+-c pytorch -c nvidia/label/cuda-11.8.0 -c fastai \
+-c huggingface -c conda-forge
 
 conda activate fastxtend
 ```
 
 replacing `pytorch-cuda=11.8` and `nvidia/label/cuda-11.8.0` with your
 preferred [supported version of
 Cuda](https://pytorch.org/get-started/locally). Then install fastxtend
@@ -205,7 +211,13 @@
 
 ``` python
 from fastxtend.callback import simpleprofiler
 
 learn = Learner(...).profile()
 learn.fit_one_cycle(2, 3e-3)
 ```
+
+## Benchmark
+
+To run the benchmark on your own machine, see the [example
+scripts](https://github.com/warner-benjamin/fastxtend/tree/main/examples)
+for details on how to replicate.
```

### Comparing `fastxtend-0.1.2/fastxtend/_modidx.py` & `fastxtend-0.1.3/fastxtend/_modidx.py`

 * *Files 8% similar despite different names*

```diff
@@ -296,14 +296,20 @@
                                                                                           'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.CompilerCallback': ( 'callback.compiler.html#compilercallback',
                                                                                                'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.CompilerCallback.__init__': ( 'callback.compiler.html#compilercallback.__init__',
                                                                                                         'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.CompilerCallback.before_fit': ( 'callback.compiler.html#compilercallback.before_fit',
                                                                                                           'fastxtend/callback/compiler.py'),
+                                             'fastxtend.callback.compiler.DynamoExplainCallback': ( 'callback.compiler.html#dynamoexplaincallback',
+                                                                                                    'fastxtend/callback/compiler.py'),
+                                             'fastxtend.callback.compiler.DynamoExplainCallback.__init__': ( 'callback.compiler.html#dynamoexplaincallback.__init__',
+                                                                                                             'fastxtend/callback/compiler.py'),
+                                             'fastxtend.callback.compiler.DynamoExplainCallback.before_fit': ( 'callback.compiler.html#dynamoexplaincallback.before_fit',
+                                                                                                               'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.Learner.compile': ( 'callback.compiler.html#learner.compile',
                                                                                               'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.Learner.export': ( 'callback.compiler.html#learner.export',
                                                                                              'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.Learner.fine_tune': ( 'callback.compiler.html#learner.fine_tune',
                                                                                                 'fastxtend/callback/compiler.py'),
                                              'fastxtend.callback.compiler.Learner.freeze_to': ( 'callback.compiler.html#learner.freeze_to',
@@ -470,14 +476,16 @@
                                                                                                                  'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback': ( 'callback.profiler.html#throughputpostcallback',
                                                                                                      'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.__init__': ( 'callback.profiler.html#throughputpostcallback.__init__',
                                                                                                               'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback._after_fit': ( 'callback.profiler.html#throughputpostcallback._after_fit',
                                                                                                                 'fastxtend/callback/profiler.py'),
+                                             'fastxtend.callback.profiler.ThroughputPostCallback._before_fit': ( 'callback.profiler.html#throughputpostcallback._before_fit',
+                                                                                                                 'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_batch': ( 'callback.profiler.html#throughputpostcallback.after_batch',
                                                                                                                  'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_epoch': ( 'callback.profiler.html#throughputpostcallback.after_epoch',
                                                                                                                  'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_fit': ( 'callback.profiler.html#throughputpostcallback.after_fit',
                                                                                                                'fastxtend/callback/profiler.py'),
                                              'fastxtend.callback.profiler.ThroughputPostCallback.after_train': ( 'callback.profiler.html#throughputpostcallback.after_train',
@@ -547,14 +555,26 @@
                                            'fastxtend.data.transforms.ParentSplitter': ( 'data.transforms.html#parentsplitter',
                                                                                          'fastxtend/data/transforms.py'),
                                            'fastxtend.data.transforms._greatgrandparent_idxs': ( 'data.transforms.html#_greatgrandparent_idxs',
                                                                                                  'fastxtend/data/transforms.py'),
                                            'fastxtend.data.transforms._parent_idxs': ( 'data.transforms.html#_parent_idxs',
                                                                                        'fastxtend/data/transforms.py')},
             'fastxtend.ffcv.all': {},
+            'fastxtend.ffcv.epoch_iterator': { 'fastxtend.ffcv.epoch_iterator.AsyncEpochIterator': ( 'ffcv.epoch_iterator.html#asyncepochiterator',
+                                                                                                     'fastxtend/ffcv/epoch_iterator.py'),
+                                               'fastxtend.ffcv.epoch_iterator.AsyncEpochIterator.__init__': ( 'ffcv.epoch_iterator.html#asyncepochiterator.__init__',
+                                                                                                              'fastxtend/ffcv/epoch_iterator.py'),
+                                               'fastxtend.ffcv.epoch_iterator.AsyncEpochIterator.close': ( 'ffcv.epoch_iterator.html#asyncepochiterator.close',
+                                                                                                           'fastxtend/ffcv/epoch_iterator.py'),
+                                               'fastxtend.ffcv.epoch_iterator.AsyncEpochIterator.run_pipeline': ( 'ffcv.epoch_iterator.html#asyncepochiterator.run_pipeline',
+                                                                                                                  'fastxtend/ffcv/epoch_iterator.py'),
+                                               'fastxtend.ffcv.epoch_iterator.EpochIterator': ( 'ffcv.epoch_iterator.html#epochiterator',
+                                                                                                'fastxtend/ffcv/epoch_iterator.py'),
+                                               'fastxtend.ffcv.epoch_iterator.EpochIterator.__init__': ( 'ffcv.epoch_iterator.html#epochiterator.__init__',
+                                                                                                         'fastxtend/ffcv/epoch_iterator.py')},
             'fastxtend.ffcv.fields': { 'fastxtend.ffcv.fields.RGBImageField': ( 'ffcv.fields.html#rgbimagefield',
                                                                                 'fastxtend/ffcv/fields.py'),
                                        'fastxtend.ffcv.fields.RGBImageField.__init__': ( 'ffcv.fields.html#rgbimagefield.__init__',
                                                                                          'fastxtend/ffcv/fields.py'),
                                        'fastxtend.ffcv.fields.RGBImageField.encode': ( 'ffcv.fields.html#rgbimagefield.encode',
                                                                                        'fastxtend/ffcv/fields.py'),
                                        'fastxtend.ffcv.fields.resizer': ('ffcv.fields.html#resizer', 'fastxtend/ffcv/fields.py')},
@@ -603,37 +623,40 @@
                                        'fastxtend.ffcv.loader.Loader': ('ffcv.loader.html#loader', 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.__init__': ( 'ffcv.loader.html#loader.__init__',
                                                                                   'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.__iter__': ( 'ffcv.loader.html#loader.__iter__',
                                                                                   'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._decode_batch': ( 'ffcv.loader.html#loader._decode_batch',
                                                                                        'fastxtend/ffcv/loader.py'),
-                                       'fastxtend.ffcv.loader.Loader._one_batch': ( 'ffcv.loader.html#loader._one_batch',
+                                       'fastxtend.ffcv.loader.Loader._iter': ('ffcv.loader.html#loader._iter', 'fastxtend/ffcv/loader.py'),
+                                       'fastxtend.ffcv.loader.Loader._n_batches': ( 'ffcv.loader.html#loader._n_batches',
                                                                                     'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._one_pass': ( 'ffcv.loader.html#loader._one_pass',
                                                                                    'fastxtend/ffcv/loader.py'),
+                                       'fastxtend.ffcv.loader.Loader._pipeline_device': ( 'ffcv.loader.html#loader._pipeline_device',
+                                                                                          'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._pre_show_batch': ( 'ffcv.loader.html#loader._pre_show_batch',
                                                                                          'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader._retain_dl': ( 'ffcv.loader.html#loader._retain_dl',
                                                                                     'fastxtend/ffcv/loader.py'),
-                                       'fastxtend.ffcv.loader.Loader.before_iter': ( 'ffcv.loader.html#loader.before_iter',
-                                                                                     'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.decode': ( 'ffcv.loader.html#loader.decode',
                                                                                 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.decode_batch': ( 'ffcv.loader.html#loader.decode_batch',
                                                                                       'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.device': ( 'ffcv.loader.html#loader.device',
                                                                                 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.n_inp': ('ffcv.loader.html#loader.n_inp', 'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.one_batch': ( 'ffcv.loader.html#loader.one_batch',
                                                                                    'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.show_batch': ( 'ffcv.loader.html#loader.show_batch',
                                                                                     'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.show_results': ( 'ffcv.loader.html#loader.show_results',
                                                                                       'fastxtend/ffcv/loader.py'),
+                                       'fastxtend.ffcv.loader.Loader.split_idx': ( 'ffcv.loader.html#loader.split_idx',
+                                                                                   'fastxtend/ffcv/loader.py'),
                                        'fastxtend.ffcv.loader.Loader.to': ('ffcv.loader.html#loader.to', 'fastxtend/ffcv/loader.py')},
             'fastxtend.ffcv.operations': { 'fastxtend.ffcv.operations.ToDevice': ( 'ffcv.operations.html#todevice',
                                                                                    'fastxtend/ffcv/operations.py'),
                                            'fastxtend.ffcv.operations.ToDevice.__init__': ( 'ffcv.operations.html#todevice.__init__',
                                                                                             'fastxtend/ffcv/operations.py'),
                                            'fastxtend.ffcv.operations.ToDevice.generate_code': ( 'ffcv.operations.html#todevice.generate_code',
                                                                                                  'fastxtend/ffcv/operations.py'),
@@ -1044,14 +1067,82 @@
                                                                                       'fastxtend/optimizer/adan.py'),
                                           'fastxtend.optimizer.adan.adan_setup': ( 'optimizer.adan.html#adan_setup',
                                                                                    'fastxtend/optimizer/adan.py'),
                                           'fastxtend.optimizer.adan.adan_step': ( 'optimizer.adan.html#adan_step',
                                                                                   'fastxtend/optimizer/adan.py'),
                                           'fastxtend.optimizer.adan.debias': ('optimizer.adan.html#debias', 'fastxtend/optimizer/adan.py')},
             'fastxtend.optimizer.all': {},
+            'fastxtend.optimizer.eightbit': { 'fastxtend.optimizer.eightbit.AdamW8bitOptimizer': ( 'optimizer.eightbit.html#adamw8bitoptimizer',
+                                                                                                   'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.AdamW8bitOptimizer.__init__': ( 'optimizer.eightbit.html#adamw8bitoptimizer.__init__',
+                                                                                                            'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBit1StateOptimizer': ( 'optimizer.eightbit.html#eightbit1stateoptimizer',
+                                                                                                        'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBit1StateOptimizer.__init__': ( 'optimizer.eightbit.html#eightbit1stateoptimizer.__init__',
+                                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBit1StateOptimizer.update_step': ( 'optimizer.eightbit.html#eightbit1stateoptimizer.update_step',
+                                                                                                                    'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBit2StateOptimizer': ( 'optimizer.eightbit.html#eightbit2stateoptimizer',
+                                                                                                        'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBit2StateOptimizer.__init__': ( 'optimizer.eightbit.html#eightbit2stateoptimizer.__init__',
+                                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBit2StateOptimizer.update_step': ( 'optimizer.eightbit.html#eightbit2stateoptimizer.update_step',
+                                                                                                                    'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitCommon': ( 'optimizer.eightbit.html#eightbitcommon',
+                                                                                               'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitCommon.step': ( 'optimizer.eightbit.html#eightbitcommon.step',
+                                                                                                    'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter': ( 'optimizer.eightbit.html#eightbitfastaiadapter',
+                                                                                                      'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter._set_hyper': ( 'optimizer.eightbit.html#eightbitfastaiadapter._set_hyper',
+                                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter._set_require_grad': ( 'optimizer.eightbit.html#eightbitfastaiadapter._set_require_grad',
+                                                                                                                        'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.clear_state': ( 'optimizer.eightbit.html#eightbitfastaiadapter.clear_state',
+                                                                                                                  'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.freeze': ( 'optimizer.eightbit.html#eightbitfastaiadapter.freeze',
+                                                                                                             'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.freeze_to': ( 'optimizer.eightbit.html#eightbitfastaiadapter.freeze_to',
+                                                                                                                'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.get_config': ( 'optimizer.eightbit.html#eightbitfastaiadapter.get_config',
+                                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.get_params': ( 'optimizer.eightbit.html#eightbitfastaiadapter.get_params',
+                                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.hypers': ( 'optimizer.eightbit.html#eightbitfastaiadapter.hypers',
+                                                                                                             'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.param_lists': ( 'optimizer.eightbit.html#eightbitfastaiadapter.param_lists',
+                                                                                                                  'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.set_hyper': ( 'optimizer.eightbit.html#eightbitfastaiadapter.set_hyper',
+                                                                                                                'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.set_hypers': ( 'optimizer.eightbit.html#eightbitfastaiadapter.set_hypers',
+                                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.EightBitFastaiAdapter.unfreeze': ( 'optimizer.eightbit.html#eightbitfastaiadapter.unfreeze',
+                                                                                                               'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.LAMB8bitOptimizer': ( 'optimizer.eightbit.html#lamb8bitoptimizer',
+                                                                                                  'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.LAMB8bitOptimizer.__init__': ( 'optimizer.eightbit.html#lamb8bitoptimizer.__init__',
+                                                                                                           'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.LARS8bitOptimizer': ( 'optimizer.eightbit.html#lars8bitoptimizer',
+                                                                                                  'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.LARS8bitOptimizer.__init__': ( 'optimizer.eightbit.html#lars8bitoptimizer.__init__',
+                                                                                                           'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.Lion8bitOptimizer': ( 'optimizer.eightbit.html#lion8bitoptimizer',
+                                                                                                  'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.Lion8bitOptimizer.__init__': ( 'optimizer.eightbit.html#lion8bitoptimizer.__init__',
+                                                                                                           'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.RMSProp8bitOptimizer': ( 'optimizer.eightbit.html#rmsprop8bitoptimizer',
+                                                                                                     'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.RMSProp8bitOptimizer.__init__': ( 'optimizer.eightbit.html#rmsprop8bitoptimizer.__init__',
+                                                                                                              'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.SGD8bitOptimizer': ( 'optimizer.eightbit.html#sgd8bitoptimizer',
+                                                                                                 'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit.SGD8bitOptimizer.__init__': ( 'optimizer.eightbit.html#sgd8bitoptimizer.__init__',
+                                                                                                          'fastxtend/optimizer/eightbit.py'),
+                                              'fastxtend.optimizer.eightbit._convert_params': ( 'optimizer.eightbit.html#_convert_params',
+                                                                                                'fastxtend/optimizer/eightbit.py')},
             'fastxtend.optimizer.foreach': { 'fastxtend.optimizer.foreach.AdamForEachOptimizer': ( 'optimizer.foreach.html#adamforeachoptimizer',
                                                                                                    'fastxtend/optimizer/foreach.py'),
                                              'fastxtend.optimizer.foreach.AdamForEachOptimizer.step': ( 'optimizer.foreach.html#adamforeachoptimizer.step',
                                                                                                         'fastxtend/optimizer/foreach.py'),
                                              'fastxtend.optimizer.foreach.ForEachOptimizer': ( 'optimizer.foreach.html#foreachoptimizer',
                                                                                                'fastxtend/optimizer/foreach.py'),
                                              'fastxtend.optimizer.foreach.ForEachOptimizer.__init__': ( 'optimizer.foreach.html#foreachoptimizer.__init__',
@@ -1124,14 +1215,72 @@
                                           'fastxtend.optimizer.lion.LionForEachOptimizer.step': ( 'optimizer.lion.html#lionforeachoptimizer.step',
                                                                                                   'fastxtend/optimizer/lion.py'),
                                           'fastxtend.optimizer.lion.lion': ('optimizer.lion.html#lion', 'fastxtend/optimizer/lion.py'),
                                           'fastxtend.optimizer.lion.lion_foreach_step': ( 'optimizer.lion.html#lion_foreach_step',
                                                                                           'fastxtend/optimizer/lion.py'),
                                           'fastxtend.optimizer.lion.lion_step': ( 'optimizer.lion.html#lion_step',
                                                                                   'fastxtend/optimizer/lion.py')},
+            'fastxtend.optimizer.sophia': { 'fastxtend.optimizer.sophia.Sophia': ( 'optimizer.sophia.html#sophia',
+                                                                                   'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaCallback': ( 'optimizer.sophia.html#sophiacallback',
+                                                                                           'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaCallback.__init__': ( 'optimizer.sophia.html#sophiacallback.__init__',
+                                                                                                    'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaCallback.after_step': ( 'optimizer.sophia.html#sophiacallback.after_step',
+                                                                                                      'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaCallback.before_fit': ( 'optimizer.sophia.html#sophiacallback.before_fit',
+                                                                                                      'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaCallback.before_loss': ( 'optimizer.sophia.html#sophiacallback.before_loss',
+                                                                                                       'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaCallback.before_step': ( 'optimizer.sophia.html#sophiacallback.before_step',
+                                                                                                       'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaForEachOptimizer': ( 'optimizer.sophia.html#sophiaforeachoptimizer',
+                                                                                                   'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaForEachOptimizer.__init__': ( 'optimizer.sophia.html#sophiaforeachoptimizer.__init__',
+                                                                                                            'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaForEachOptimizer.clear_state': ( 'optimizer.sophia.html#sophiaforeachoptimizer.clear_state',
+                                                                                                               'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaForEachOptimizer.step': ( 'optimizer.sophia.html#sophiaforeachoptimizer.step',
+                                                                                                        'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaForEachOptimizer.update_sophia_hypers': ( 'optimizer.sophia.html#sophiaforeachoptimizer.update_sophia_hypers',
+                                                                                                                        'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaHessian': ( 'optimizer.sophia.html#sophiahessian',
+                                                                                          'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaOptimizer': ( 'optimizer.sophia.html#sophiaoptimizer',
+                                                                                            'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaOptimizer.__init__': ( 'optimizer.sophia.html#sophiaoptimizer.__init__',
+                                                                                                     'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaOptimizer.clear_state': ( 'optimizer.sophia.html#sophiaoptimizer.clear_state',
+                                                                                                        'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaOptimizer.step': ( 'optimizer.sophia.html#sophiaoptimizer.step',
+                                                                                                 'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.SophiaOptimizer.update_sophia_hypers': ( 'optimizer.sophia.html#sophiaoptimizer.update_sophia_hypers',
+                                                                                                                 'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.sophia': ( 'optimizer.sophia.html#sophia',
+                                                                                   'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.sophia_foreach_step': ( 'optimizer.sophia.html#sophia_foreach_step',
+                                                                                                'fastxtend/optimizer/sophia.py'),
+                                            'fastxtend.optimizer.sophia.sophia_step': ( 'optimizer.sophia.html#sophia_step',
+                                                                                        'fastxtend/optimizer/sophia.py')},
+            'fastxtend.optimizer.stableadam': { 'fastxtend.optimizer.stableadam.StableAdam': ( 'optimizer.stableadam.html#stableadam',
+                                                                                               'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.StableAdamForEachOptimizer': ( 'optimizer.stableadam.html#stableadamforeachoptimizer',
+                                                                                                               'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.StableAdamForEachOptimizer.step': ( 'optimizer.stableadam.html#stableadamforeachoptimizer.step',
+                                                                                                                    'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.debias': ( 'optimizer.stableadam.html#debias',
+                                                                                           'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.stable_adam_foreach_step': ( 'optimizer.stableadam.html#stable_adam_foreach_step',
+                                                                                                             'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.stable_adam_jit_substep': ( 'optimizer.stableadam.html#stable_adam_jit_substep',
+                                                                                                            'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.stable_adam_step': ( 'optimizer.stableadam.html#stable_adam_step',
+                                                                                                     'fastxtend/optimizer/stableadam.py'),
+                                                'fastxtend.optimizer.stableadam.stableadam': ( 'optimizer.stableadam.html#stableadam',
+                                                                                               'fastxtend/optimizer/stableadam.py')},
             'fastxtend.optimizer.torchscript': { 'fastxtend.optimizer.torchscript.JitLookahead': ( 'optimizer.torchscript.html#jitlookahead',
                                                                                                    'fastxtend/optimizer/torchscript.py'),
                                                  'fastxtend.optimizer.torchscript.JitLookahead.__init__': ( 'optimizer.torchscript.html#jitlookahead.__init__',
                                                                                                             'fastxtend/optimizer/torchscript.py'),
                                                  'fastxtend.optimizer.torchscript.JitLookahead._init_state': ( 'optimizer.torchscript.html#jitlookahead._init_state',
                                                                                                                'fastxtend/optimizer/torchscript.py'),
                                                  'fastxtend.optimizer.torchscript.JitLookahead.clear_state': ( 'optimizer.torchscript.html#jitlookahead.clear_state',
@@ -1169,15 +1318,16 @@
             'fastxtend.patches': {},
             'fastxtend.schedulers': { 'fastxtend.schedulers.Learner.fit_cos_anneal': ( 'schedulers.html#learner.fit_cos_anneal',
                                                                                        'fastxtend/schedulers.py'),
                                       'fastxtend.schedulers.Learner.fit_flat_varied': ( 'schedulers.html#learner.fit_flat_varied',
                                                                                         'fastxtend/schedulers.py'),
                                       'fastxtend.schedulers.Learner.fit_flat_warmup': ( 'schedulers.html#learner.fit_flat_warmup',
                                                                                         'fastxtend/schedulers.py')},
-            'fastxtend.test_utils': {},
+            'fastxtend.test_utils': { 'fastxtend.test_utils.tst_param': ('test_utils.html#tst_param', 'fastxtend/test_utils.py'),
+                                      'fastxtend.test_utils.tst_params': ('test_utils.html#tst_params', 'fastxtend/test_utils.py')},
             'fastxtend.torch_core': { 'fastxtend.torch_core.TensorCategory': ('torch_core.html#tensorcategory', 'fastxtend/torch_core.py'),
                                       'fastxtend.torch_core.TensorCategory.show': ( 'torch_core.html#tensorcategory.show',
                                                                                     'fastxtend/torch_core.py'),
                                       'fastxtend.torch_core.TensorMultiCategory': ( 'torch_core.html#tensormulticategory',
                                                                                     'fastxtend/torch_core.py'),
                                       'fastxtend.torch_core.TensorMultiCategory.show': ( 'torch_core.html#tensormulticategory.show',
                                                                                          'fastxtend/torch_core.py')},
@@ -1189,15 +1339,17 @@
                                                                                           'fastxtend/transform.py'),
                                      'fastxtend.transform.BatchRandTransform._do_call': ( 'transform.html#batchrandtransform._do_call',
                                                                                           'fastxtend/transform.py'),
                                      'fastxtend.transform.BatchRandTransform._do_f': ( 'transform.html#batchrandtransform._do_f',
                                                                                        'fastxtend/transform.py'),
                                      'fastxtend.transform.BatchRandTransform.before_call': ( 'transform.html#batchrandtransform.before_call',
                                                                                              'fastxtend/transform.py')},
-            'fastxtend.utils': { 'fastxtend.utils.free_gpu_memory': ('utils.html#free_gpu_memory', 'fastxtend/utils.py'),
+            'fastxtend.utils': { 'fastxtend.utils.clean_ipython_hist': ('utils.html#clean_ipython_hist', 'fastxtend/utils.py'),
+                                 'fastxtend.utils.clean_traceback': ('utils.html#clean_traceback', 'fastxtend/utils.py'),
+                                 'fastxtend.utils.free_gpu_memory': ('utils.html#free_gpu_memory', 'fastxtend/utils.py'),
                                  'fastxtend.utils.less_random': ('utils.html#less_random', 'fastxtend/utils.py'),
                                  'fastxtend.utils.pil_to_numpy': ('utils.html#pil_to_numpy', 'fastxtend/utils.py'),
                                  'fastxtend.utils.scale_time': ('utils.html#scale_time', 'fastxtend/utils.py')},
             'fastxtend.vision.all': {},
             'fastxtend.vision.augment.all': {},
             'fastxtend.vision.augment.batch': { 'fastxtend.vision.augment.batch.ChannelDrop': ( 'vision.augment.batch.html#channeldrop',
                                                                                                 'fastxtend/vision/augment/batch.py'),
```

### Comparing `fastxtend-0.1.2/fastxtend/audio/augment.py` & `fastxtend-0.1.3/fastxtend/audio/augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
         mv = random.randint(int(x.min), int(x.max)) if self.mask_value is None else self.mask_value
         if self.iid_masks and x.dim() == 4:
             return TAF.mask_along_axis_iid(x, mask_param, mv, 2)
         else:
             return TAF.mask_along_axis(x, mask_param, mv, 1)
 
 # %% ../../nbs/audio.03_augment.ipynb 69
-class AmplitudeToDBMode(Enum):
+class AmplitudeToDBMode(str, Enum):
     "All AmplitudeToDB modes as attributes to get tab-completion and typo-proofing",
     Power = 'power'
     Magnitude = 'magnitude'
 
 # %% ../../nbs/audio.03_augment.ipynb 70
 class AmplitudeToDB(DisplayedTransform):
     "Turn a `TensorSpec` or `TensorMelSpec` from the power/amplitude scale to the decibel scale"
```

### Comparing `fastxtend-0.1.2/fastxtend/audio/core.py` & `fastxtend-0.1.3/fastxtend/audio/core.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/audio/data.py` & `fastxtend-0.1.3/fastxtend/audio/data.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/audio/learner.py` & `fastxtend-0.1.3/fastxtend/audio/learner.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/audio/mixup.py` & `fastxtend-0.1.3/fastxtend/audio/mixup.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/basics.py` & `fastxtend-0.1.3/fastxtend/basics.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/callback/channelslast.py` & `fastxtend-0.1.3/fastxtend/callback/channelslast.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/callback/compiler.py` & `fastxtend-0.1.3/fastxtend/callback/compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,46 +14,53 @@
 import warnings
 
 from packaging.version import parse
 
 import torch._dynamo as dynamo
 from torch.serialization import FILE_LIKE
 
-from fastai.learner import Learner, save_model, join_path_file
-from fastai.callback.core import Callback, TrainEvalCallback
+from fastai.learner import Learner, save_model, join_path_file, _cast_tensor
 from fastai.callback import schedule
+from fastai.callback.core import Callback, TrainEvalCallback, CancelFitException
+from fastai.callback.fp16 import MixedPrecision
+
+try:
+    from fastxtend.ffcv.loader import Loader
+    FFCV = True
+except ImportError:
+    FFCV = False
 
 from ..imports import *
 
 # %% auto 0
-__all__ = ['CompileMode', 'MatMulPrecision', 'CompilerCallback', 'load_learner']
+__all__ = ['CompileMode', 'MatMulPrecision', 'CompilerCallback', 'DynamoExplainCallback', 'load_learner']
 
 # %% ../../nbs/callback.compiler.ipynb 6
 _torch_version = parse(torch.__version__)
-_torch_20  = parse('2.0')
-_torch_21  = parse('2.1')
+_torch_20 = parse('2.0')
+_torch_21 = parse('2.1')
 
 if _torch_version < _torch_20:
     warn('Imported `fastxtend.callback.compiler`, which requires a minimum of PyTorch 2.0 to work.')
 
 # %% ../../nbs/callback.compiler.ipynb 7
-class CompileMode(Enum):
+class CompileMode(str, Enum):
     "All valid `torch.compile` modes for tab-completion and typo-proofing"
     default        = 'default'
     reduceoverhead = 'reduce-overhead'
     maxautotune    = 'max-autotune'
 
 # %% ../../nbs/callback.compiler.ipynb 9
-class MatMulPrecision(Enum):
+class MatMulPrecision(str, Enum):
     "All valid `matmul_precision` modes for tab-completion and typo-proofing"
     highest = 'highest'
     high    = 'high'
     medium  = 'medium'
 
-# %% ../../nbs/callback.compiler.ipynb 10
+# %% ../../nbs/callback.compiler.ipynb 11
 class CompilerCallback(Callback):
     "An experimental callback for `torch.compile` (beta) and fastai"
     order = TrainEvalCallback.order + 1 # Compiling needs to occur on the GPU, but before distributed training starts
 
     def __init__(self,
         fullgraph:bool=False, # Prevent breaking model into subgraphs
         dynamic:bool=False, # Use dynamic shape tracing
@@ -73,85 +80,160 @@
         store_attr(but='recompile')
         self._recompile = recompile
 
     def before_fit(self):
         if _torch_version < _torch_20:
             self.run = False
             warn("Attempting to use `CompilerCallback` without PyTorch 2.0 or greater. Disabling.")
+            return
 
         if torch.cuda.get_device_capability() >= (8, 0) and torch.get_float32_matmul_precision() != self.matmul_precision:
             if self.verbose and self.matmul_precision!='highest':
                 print(f"Your GPU has modern tensor cores, automatically enabling by setting `torch.set_float32_matmul_precision('{self.matmul_precision}')`")
             torch.set_float32_matmul_precision(self.matmul_precision)
 
-        if hasattr(self.learn, 'lr_finder'):
-            self.run = False
-            return
-
         if hasattr(self.learn, 'progressive_resize') and _torch_version < _torch_21:
             warn("Using `ProgressiveResize` and `torch.compile` at the same time will result in a new compile every size change.")
         msg = ""
         if self.dynamic:
             msg += "Using `torch.compile` with dynamic shapes is under active development and might fail\n"
         if self.mode == 'max-autotune':
             msg += "Using `torch.compile` with `mode='max-autotune'` is under active development and might fail\n"
         if msg != "":
             msg += "See https://pytorch.org/docs/master/compile/index.html#troubleshooting-and-gotchas for more details"
             warn(msg)
         if self.mode == 'reduce-overhead':
             warn("Using `torch.compile` & fastai with `mode='reduce-overhead'` currently doesn't appear to train.")
-            
+
         if self._recompile and isinstance(self.learn.model, dynamo.OptimizedModule):
-            if self.verbose: 
+            if self.verbose:
                 print("Recompiling model")
             dynamo.reset()
             self.learn.model = self.learn.model._orig_mod
         self._recompile = False
-        
+
         if not isinstance(self.learn.model, dynamo.OptimizedModule):
-            self.learn.model = torch.compile(self.learn.model, fullgraph=self.fullgraph, 
-                                             dynamic=self.dynamic, backend=self.backend, 
+            self.learn.model = torch.compile(self.learn.model, fullgraph=self.fullgraph,
+                                             dynamic=self.dynamic, backend=self.backend,
                                              mode=self.mode, options=self.options)
 
-# %% ../../nbs/callback.compiler.ipynb 13
+# %% ../../nbs/callback.compiler.ipynb 14
+class DynamoExplainCallback(Callback):
+    "An experimental callback to find graph breaks with `torch.compile` (beta)"
+    order = MixedPrecision.order+1 # DynamoExplain occurs on the GPU before any training starts
+
+    def __init__(self,
+        print_results:bool=True, # Print enabled `torch._dynamo.explain` output(s)
+        explanation:bool=True, # Print the `explanation` output
+        out_guards:bool=False, # Print the `out_guards` output
+        graphs:bool=False, # Print the `graphs` output
+        ops_per_graph:bool=False, # Print the `ops_per_graph` output
+        break_reasons:bool=False, # Print the `break_reasons` output
+        explanation_verbose:bool=False, # Print the `explanation_verbose` output
+    ):
+        self.print_results = print_results
+        self.print_explanation = explanation
+        self.print_out_guards = out_guards
+        self.print_graphs = graphs
+        self.print_ops_per_graph = ops_per_graph
+        self.print_break_reasons = break_reasons
+        self.print_explanation_verbose = explanation_verbose
+
+    def before_fit(self):
+        if _torch_version < _torch_20:
+            self.run = False
+            warn("Attempting to use `DynamoExplainCallback` without PyTorch 2.0 or greater. Canceling training.")
+            raise CancelFitException()
+
+        self.explanation, self.out_guards, self.graphs, self.ops_per_graph, self.break_reasons, self.explanation_verbose = '','','','','',''
+        states = get_random_states()
+        try:
+            if FFCV and isinstance(self.dls.train, Loader) and self.dls.train.async_tfms:
+                # With `async_tfms`, `Loader` needs to initialize all `Loader.batches_ahead` Cuda streams
+                # for the training dataloader. Since FFCV doesn't support seeded transforms and the reset
+                # random state only seeds the dataset order, this shouldn't effect training outcome.
+                b = self.dls.train.one_batch(batches_ahead=True)
+            else:
+                b = self.dls.valid.one_batch()
+            i = getattr(self.dls, 'n_inp', 1 if len(b)==1 else len(b)-1)
+            self.learn.xb, self.learn.yb = b[:i], b[i:]
+
+            if hasattr(self.learn, 'mixed_precision'):
+                self.learn.mixed_precision.autocast.__enter__()
+
+            self.explanation, self.out_guards, self.graphs, self.ops_per_graph, self.break_reasons, self.explanation_verbose \
+                = dynamo.explain(self.learn.model, *_cast_tensor(self.learn.xb))
+
+            if hasattr(self.learn, 'mixed_precision'):
+                self.learn.mixed_precision.autocast.__exit__(None, None, None)
+
+            self.learn.opt.zero_grad()
+        finally:
+            set_random_states(**states)
+
+        if self.print_results:
+            print('\nDynamo Explain Report')
+            if self.print_explanation:
+                print('\nExplanation:\n')
+                print(self.explanation)
+            if self.print_out_guards:
+                print('\nOut Guards:\n')
+                print(self.out_guards)
+            if self.print_graphs:
+                print('\nGraphs:\n')
+                print(self.graphs)
+            if self.print_ops_per_graph:
+                print('\nOperations per Graph:\n')
+                print(self.ops_per_graph)
+            if self.print_break_reasons:
+                print('\nBreak Reasons:\n')
+                print(self.break_reasons)
+            if self.print_explanation_verbose:
+                print('\nVerbose Explanation:\n')
+                print(self.explanation_verbose)
+            print('\n')
+
+        raise CancelFitException()
+
+# %% ../../nbs/callback.compiler.ipynb 17
 @patch
 def compile(self:Learner,
     fullgraph:bool=False, # Prevent breaking model into subgraphs
     backend:str|Callable='inductor', # `torch.compile` backend to use
     mode:str|CompileMode|None=None, # `torch.compile` mode to use
     options:Dict[str, Union[str,int,bool]]|None=None, # Extra options to pass to compile backend
     matmul_precision:str|MatMulPrecision='high', # Set Ampere and newer TF32 matmul precision
     recompile:bool=False, # Force a compiled model to recompile. Use when freezing/unfreezing a compiled model.
     verbose:bool=True, # Verbose output
 ):
     "Set `Learner` to compile model using `torch.compile`."
     return self.add_cb(CompilerCallback(fullgraph=fullgraph, backend=backend,
-                                        mode=mode, options=options, 
-                                        matmul_precision=matmul_precision, 
+                                        mode=mode, options=options,
+                                        matmul_precision=matmul_precision,
                                         recompile=recompile, verbose=verbose))
 
-# %% ../../nbs/callback.compiler.ipynb 17
+# %% ../../nbs/callback.compiler.ipynb 21
 @patch
 @delegates(save_model)
-def save(self:Learner, 
+def save(self:Learner,
     file:FILE_LIKE, # Save file name, path, bytes, or IO
     save_compiled:bool=False, # Save compiled model
     **kwargs
 ):
     "Save model and optimizer state (if `with_opt`) to `self.path/self.model_dir/file`"
     file = join_path_file(file, self.path/self.model_dir, ext='.pth')
     if _torch_version >= _torch_20 and isinstance(self.model, dynamo.OptimizedModule) and not save_compiled:
         save_model(file, self.model._orig_mod, getattr(self,'opt',None), **kwargs)
     else:
         save_model(file, self.model, getattr(self,'opt',None), **kwargs)
     return file
 
-# %% ../../nbs/callback.compiler.ipynb 19
+# %% ../../nbs/callback.compiler.ipynb 23
 @patch
-def export(self:Learner, 
+def export(self:Learner,
     fname:FILE_LIKE='export.pkl', # Learner export file name, path, bytes, or IO
     pickle_module:Any=pickle, # Module used for pickling metadata and objects
     pickle_protocol:int=2 # Pickle protocol used
 ):
     "Export the content of `self` without the items and the optimizer state for inference"
     if rank_distrib(): return # don't export if child proc
     self._end_cleanup()
@@ -166,66 +248,66 @@
         # To avoid the warning that come from PyTorch about model not being checked
         warnings.simplefilter("ignore")
         torch.save(self, self.path/fname, pickle_module=pickle_module, pickle_protocol=pickle_protocol)
     self.create_opt()
     if state is not None: self.opt.load_state_dict(state)
     self.dls = old_dbunch
 
-# %% ../../nbs/callback.compiler.ipynb 21
+# %% ../../nbs/callback.compiler.ipynb 25
 def load_learner(
     fname:FILE_LIKE, # File name, path, bytes, or IO
     cpu:bool=True, # Load model to CPU
     pickle_module=pickle # Module used for unpickling metadata and objects
 ):
     "Load a `Learner` object in `fname`, by default putting it on the `cpu`"
     distrib_barrier()
     map_loc = 'cpu' if cpu else default_device()
     try: res = torch.load(fname, map_location=map_loc, pickle_module=pickle_module)
-    except AttributeError as e: 
+    except AttributeError as e:
         e.args = [f"Custom classes or functions exported with your `Learner` not available in namespace.\Re-declare/import before loading:\n\t{e.args[0]}"]
         raise
-    if cpu: 
+    if cpu:
         res.dls.cpu()
         if hasattr(res, 'channels_last'): res = res.to_contiguous(to_fp32=True)
         elif hasattr(res, 'mixed_precision'): res = res.to_fp32()
         elif hasattr(res, 'non_native_mixed_precision'): res = res.to_non_native_fp32()
         if hasattr(res, 'compiler'): res = res.remove_cb(CompilerCallback)
     return res
 
-# %% ../../nbs/callback.compiler.ipynb 24
+# %% ../../nbs/callback.compiler.ipynb 28
 @patch
 def freeze_to(self:Learner, n:int):
     "Freeze parameter groups up to `n`"
-    if self.opt is None: 
+    if self.opt is None:
         self.create_opt()
     self.opt.freeze_to(n)
     self.opt.clear_state()
     if _torch_version >= _torch_20 and isinstance(self.model, dynamo.OptimizedModule):
         if hasattr(self, 'compiler'):
             self.compiler._recompile = True
         else:
             warn("Freezing or unfreezing a compiled model isn't supported."\
                  "\nThe model must be recompiled to take effect."\
                  "\nPass `CompilerCallback(..., recompile=True)` to `Learner.cbs`"\
                  "\nor call `torch._dynamo.reset() and recompile model.")
 
-# %% ../../nbs/callback.compiler.ipynb 27
+# %% ../../nbs/callback.compiler.ipynb 31
 @patch
 @delegates(Learner.fit_one_cycle)
-def fine_tune(self:Learner, 
+def fine_tune(self:Learner,
     epochs:int, # Number of unfrozen epochs to train
     base_lr:float=2e-3, # Base learning rate, model head unfrozen learning rate
     freeze_epochs:int=1, # Number of frozen epochs to train
-    lr_mult:Numeric=100, # Model stem unfrozen learning rate: `base_lr/lr_mult``
+    lr_mult:Numeric=100, # Model stem unfrozen learning rate: `base_lr/lr_mult`
     pct_start:float=0.3, # Start unfrozen learning rate cosine annealing
     div:Numeric=5.0, # Initial unfrozen learning rate: `base_lr/div`
     freeze_compile:bool=False, # pct_start for unfrozen fit_one_cycle
     **kwargs
 ):
     "Fine tune with `Learner.freeze` for `freeze_epochs`, then with `Learner.unfreeze` for `epochs`, using discriminative LR."
     self.freeze()
     if _torch_version >= _torch_20 and hasattr(self, 'compiler') and not freeze_compile:
-            self.compiler.run = isinstance(self.model, dynamo.OptimizedModule)
+        self.compiler.run = isinstance(self.model, dynamo.OptimizedModule)
     self.fit_one_cycle(freeze_epochs, slice(base_lr), pct_start=0.99, **kwargs)
     base_lr /= 2
     self.unfreeze()
     self.fit_one_cycle(epochs, slice(base_lr/lr_mult, base_lr), pct_start=pct_start, div=div, **kwargs)
```

### Comparing `fastxtend-0.1.2/fastxtend/callback/cutmixup.py` & `fastxtend-0.1.3/fastxtend/callback/cutmixup.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/callback/ema.py` & `fastxtend-0.1.3/fastxtend/callback/ema.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/callback/lr_finder.py` & `fastxtend-0.1.3/fastxtend/callback/lr_finder.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/callback/profiler.py` & `fastxtend-0.1.3/fastxtend/callback/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,23 +264,26 @@
 class ThroughputPostCallback(Callback):
     "Required pair with `ThroughputCallback` to profile training performance. Removes itself after training is over."
     order,remove_on_fetch = Recorder.order-1,True
     def __init__(self):
         self._log_full = False
         self._phase, self._train, self._valid = _phase, _train_short, _train_short
 
-    def before_fit(self):
-        self.profiler = self.learn.throughput
+    def _before_fit(self):
         self.has_logger = self.profiler.has_logger
         self._start_train_logging, self._start_valid_logging = False, False
         self.n_train_batches = len(self.dls.train)
         self.n_valid_batches = len(self.dls.valid)
         self._rolling_average = self.profiler._rolling_average
         self._iter = -self.profiler._drop
 
+    def before_fit(self):
+        self.profiler = self.learn.throughput
+        self._before_fit()
+
     def after_train(self):
         self.profiler._raw_values['train'].append(time.perf_counter() - self.profiler._train_start)
 
     def after_validate(self):
         self.profiler._raw_values['valid'].append(time.perf_counter() - self.profiler._validate_start)
 
     def after_batch(self):
@@ -350,19 +353,15 @@
     order,remove_on_fetch = Recorder.order-1,True
     def __init__(self):
         self._log_full = True
         self._phase, self._train, self._valid = _phase, _train_full, _valid_full
 
     def before_fit(self):
         self.profiler = self.learn.simple_profiler
-        self._start_logging = self.profiler._rolling_average + self.profiler._drop
-        self.has_logger = self.profiler.has_logger
-        self._start_train_logging, self._start_valid_logging = False, False
-        self.n_train_batches = len(self.dls.train)
-        self.n_valid_batches = len(self.dls.valid)
+        self._before_fit()
 
     def after_pred(self):
         if self.training:
             self.profiler._raw_values['train_forward'].append(time.perf_counter() - self.profiler._train_batch_start)
             self.profiler._train_loss_start = time.perf_counter()
         else:
             self.profiler._raw_values['valid_predict'].append(time.perf_counter() - self.profiler._valid_batch_start)
@@ -378,15 +377,15 @@
         self.profiler._raw_values['train_opt_step'].append(time.perf_counter() - self.profiler._step_start)
         self.profiler._zero_start = time.perf_counter()
 
     def after_fit(self):
         self._after_fit([SimpleProfilerCallback, SimpleProfilerPostCallback])
 
 # %% ../../nbs/callback.profiler.ipynb 28
-class ProfileMode(Enum):
+class ProfileMode(str, Enum):
     "Profile enum for `Learner.profile`"
     Throughput = 'throughput'
     Simple     = 'simple'
 
 # %% ../../nbs/callback.profiler.ipynb 29
 @patch
 def profile(self:Learner,
```

### Comparing `fastxtend-0.1.2/fastxtend/callback/progresize.py` & `fastxtend-0.1.3/fastxtend/callback/progresize.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 from fastcore.transform import Pipeline
 
 from fastai.callback.core import Callback
 from fastai.callback.fp16 import MixedPrecision
 from fastai.learner import _cast_tensor
 from fastai.vision.augment import AffineCoordTfm, RandomResizedCropGPU
 
+try:
+    from fastxtend.ffcv.loader import Loader
+    FFCV = True
+except ImportError:
+    FFCV = False
+
 from ..imports import *
 
 # %% auto 0
 __all__ = ['IncreaseMode', 'ProgressiveResize']
 
 # %% ../../nbs/callback.progresize.ipynb 4
 _resize_augs = (AffineCoordTfm, RandomResizedCropGPU)
@@ -39,38 +45,38 @@
 # %% ../../nbs/callback.progresize.ipynb 7
 def _evenly_divisible(final_size, current_size, increase_by, steps):
     increase_by = tensor(increase_by)
     return (((final_size-current_size) % increase_by).sum() == 0) and (((final_size-current_size) - (increase_by*steps)).sum() == 0)
 
 # %% ../../nbs/callback.progresize.ipynb 8
 def _batch_subset(b, subset):
-    if isinstance(b, tuple): 
+    if isinstance(b, tuple):
         return tuple(_batch_subset(b_, subset) for b_ in b)
-    elif isinstance(b, Tensor): 
+    elif isinstance(b, Tensor):
         return retain_types(b[:subset], b)
-    else: 
+    else:
         raise ValueError(f'Unexpected type {b}')
 
 # %% ../../nbs/callback.progresize.ipynb 10
-class IncreaseMode(Enum):
+class IncreaseMode(str, Enum):
     "Increase mode for `ProgressiveResize`"
     Epoch = 'epoch'
     Batch = 'batch'
 
 # %% ../../nbs/callback.progresize.ipynb 11
 class ProgressiveResize(Callback):
     "Progressively increase the size of input images during training. Starting from `initial_size` and ending at the valid image size or `final_size`."
     order = MixedPrecision.order+1 # Needs to run after MixedPrecision
     def __init__(self,
         initial_size:float|tuple[int,int]=0.5, # Staring size to increase from. Image shape must be square
         start:Numeric=0.5, # Earliest upsizing epoch in percent of training time or epoch (index 0)
         finish:Numeric=0.75, # Last upsizing epoch in percent of training time or epoch (index 0)
         increase_by:int=4, # Progressively increase image size by `increase_by`, or minimum increase per upsizing epoch
-        increase_mode:IncreaseMode=IncreaseMode.Batch, # Increase image size by training percent or before an epoch starts
-        resize_mode:str='bilinear', # PyTorch interpolate mode string for upsizing. Resets to existing fastai DataLoader mode at `final_size`.
+        increase_mode:IncreaseMode=IncreaseMode.Batch, # Increase image size anytime during training or only before an epoch starts
+        resize_mode:str='bilinear', # PyTorch interpolate mode string for upsizing. Resets to existing fastai DataLoader mode at `final_size`
         resize_valid:bool=True, # Apply progressive resizing to valid dataset
         final_size:tuple[int,int]|None=None, # Final image size. Set if using a non-fastai DataLoaders, automatically detected from fastai DataLoader with batch_tfms
         add_resize:bool=False, # Add a separate resize step. Use for non-fastai DataLoaders or fastai DataLoader without batch_tfms
         resize_targ:bool=False, # Applies the separate resize step to targets
         preallocate_bs:int|None=None, # Preallocation batch size. Set if the valid DataLoader has a larger batch size than the train DataLoader.
         empty_cache:bool=False, # Call `torch.cuda.empty_cache()` before a resizing epoch. May prevent Cuda & Magma errors. Don't use with multiple GPUs
         verbose:bool=True, # Print a summary of the progressive resizing schedule
@@ -95,15 +101,21 @@
         self.increase_by = tensor(self.increase_by)
         self.resize_batch = self.increase_mode == IncreaseMode.Batch
 
         # Dry run at full resolution to pre-allocate memory
         # See https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html#pre-allocate-memory-in-case-of-variable-input-length
         states = get_random_states()
         try:
-            b = self.dls.valid.one_batch()
+            if FFCV and isinstance(self.dls.train, Loader) and self.dls.train.async_tfms:
+                # With `async_tfms`, `Loader` needs to initialize all `Loader.batches_ahead` Cuda streams
+                # for the training dataloader. Since FFCV doesn't support seeded transforms and the reset
+                # random state only seeds the dataset order, this shouldn't effect training outcome.
+                b = self.dls.train.one_batch(batches_ahead=True)
+            else:
+                b = self.dls.valid.one_batch()
             i = getattr(self.dls, 'n_inp', 1 if len(b)==1 else len(b)-1)
             if isinstance(self.preallocate_bs, int):
                 b = _batch_subset(b, self.preallocate_bs)
             self.learn.xb, self.learn.yb = b[:i], b[i:]
 
             if hasattr(self.learn, 'mixed_precision'):
                 self.learn.mixed_precision.autocast.__enter__()
```

### Comparing `fastxtend-0.1.2/fastxtend/callback/tracker.py` & `fastxtend-0.1.3/fastxtend/callback/tracker.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/data/transforms.py` & `fastxtend-0.1.3/fastxtend/data/transforms.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/fields.py` & `fastxtend-0.1.3/fastxtend/ffcv/fields.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/inference.py` & `fastxtend-0.1.3/fastxtend/ffcv/inference.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/loader.py` & `fastxtend-0.1.3/fastxtend/ffcv/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 # %% ../../nbs/ffcv.loader.ipynb 1
 # Contains code from:
 # fastai - Apache License 2.0 - Copyright (c) 2023 fast.ai
 
 # %% ../../nbs/ffcv.loader.ipynb 4
 from __future__ import annotations
 
-from typing import Mapping, Sequence
 from pathlib import Path
+from typing import Mapping, Sequence
 
 import numpy as np
 
 from ffcv.fields.base import Field
 from ffcv.loader.loader import Loader as _Loader
 from ffcv.loader.loader import OrderOption, ORDER_TYPE, DEFAULT_OS_CACHE, ORDER_MAP
+from ffcv.pipeline.compiler import Compiler
 from ffcv.pipeline.operation import Operation
 from ffcv.transforms.ops import ToDevice as _ToDevice
 
 from fastcore.basics import GetAttr, detuplify, Inf
 from fastcore.dispatch import retain_types, explode_types
 from fastcore.meta import funcs_kwargs
 from fastcore.transform import Pipeline
 
-from fastai.data.core import show_batch, show_results, DataLoaders
+from fastai.data.core import show_batch, show_results
 
+from .epoch_iterator import EpochIterator, AsyncEpochIterator
 from ..imports import *
 
 # %% auto 0
 __all__ = ['Loader', 'OrderOption']
 
 # %% ../../nbs/ffcv.loader.ipynb 5
 _all_ = ['OrderOption']
@@ -64,32 +66,41 @@
         order:ORDER_TYPE=OrderOption.SEQUENTIAL, # Dataset traversal order, one of: `SEQEUNTIAL`, `RANDOM`, `QUASI_RANDOM`
         distributed:bool=False, # Emulates the behavior of PyTorch's DistributedSampler for distributed training
         seed:int|None=None, # Random seed for batch ordering
         indices:Sequence[int]|None=None, # Subset dataset by returning only these indices
         pipelines:Mapping[str, Sequence[Operation|nn.Module]]={}, # Dictionary defining for each field the sequence of Decoders and transforms to apply
         custom_fields:Mapping[str, Field]={}, # Dictonary informing `Loader` of the types associated to fields that are using a custom type
         drop_last:bool|None=None, # Drop non-full batch in each epoch. Defaults to True if order is `SEQEUNTIAL`
-        batches_ahead:int=3, # Number of batches prepared in advance; balances latency and memory
+        batches_ahead:int=2, # Number of batches prepared in advance; balances latency and memory
         recompile:bool=False, # Recompile at every epoch. Required if FFCV augmentations change during training
         device:str|int|torch.device|None=None, # Device to place batch. Defaults to fastai's `default_device`
+        async_tfms:bool=False, # Asynchronously run `batch_tfms` before batch is drawn.
         n_inp:int|None=None, # Number of inputs to the model. Defaults to pipelines length minus 1
         split_idx:int|None=None, # Apply batch transform(s) to training (0) or validation (1) set. Defaults to valid if order is `SEQEUNTIAL`
         do_setup:bool=True, # Run `setup()` for batch transform(s)
         **kwargs
     ):
         if 'batch_tfms' in kwargs:
             if 'after_batch' not in kwargs:
                 kwargs['after_batch'] = kwargs.pop('batch_tfms')
             else:
                 raise ValueError('Cannot pass both `after_batch` and `batch_tfms` to `FFCVDataLoader`')
 
-        kwargs['after_batch'] = Pipeline(kwargs.get('after_batch', None))
+        if split_idx is None:
+            self._split_idx = int(order==OrderOption.SEQUENTIAL)
+        else:
+            self._split_idx = split_idx
+
+        kwargs['after_batch'] = Pipeline(kwargs.get('after_batch', None), split_idx=self._split_idx)
         if do_setup:
             kwargs['after_batch'].setup(self)
 
+        self.async_tfms = async_tfms and len(kwargs['after_batch'].fs) > 0
+        self.cuda_streams = None
+
         if drop_last is None:
             drop_last != order==OrderOption.SEQUENTIAL
 
         _Loader.__init__(self,
             fname=str(Path(fname)),
             batch_size=batch_size,
             num_workers=num_workers,
@@ -107,19 +118,14 @@
         BaseDL.__init__(self, **kwargs)
 
         if device is None:
             self.device = default_device()
         else:
             self.device = device
 
-        if split_idx is None:
-            self.split_idx = int(order==OrderOption.SEQUENTIAL)
-        else:
-            self.split_idx = split_idx
-
         if n_inp is None:
             self._n_inp = len(pipelines) - 1
         else:
             self._n_inp = n_inp
 
         for name in ['item_tfms', 'after_item', 'before_batch']:
             if name in kwargs:
@@ -130,18 +136,18 @@
                           f"initialize the fastxtend `Loader` pipeline with FFCV transforms."
                 else:
                     msg = f"fastxtend's `Loader` will not call any {name} methods. " \
                           f"{name} are for use with a fastai DataLoader."
                 warn(msg)
 
 
-    def one_batch(self):
-        "Return one processed batch of input(s) and target(s)"
-        for b in self._one_batch():
-            # need to return the yield from _one_batch so `Loader` can reset to iterate the entire epoch
+    def one_batch(self, batches_ahead:bool=False):
+        "Return one processed batch of input(s) and target(s), optionally loading `batches_ahead`"
+        for b in self._n_batches(self.batches_ahead + 2 if batches_ahead else 1):
+            # need to return the yield from _n_batches so `Loader` can reset to iterate the entire epoch
             pass
         return b
 
     def show_batch(self,
         b=None, # Batch to show
         max_n:int=9, # Maximum number of items to show
         ctxs=None, # List of `ctx` objects to show data. Could be matplotlib axis, DataFrame etc
@@ -189,54 +195,86 @@
         return self._n_inp
 
     @property
     def device(self):
         return self._device
 
     @device.setter
-    def device(self, device):
+    def device(self, device:int|str|torch.device):
+        # parse device
         device, *_ = torch._C._nn._parse_to(device=device)
         self._device = device
         # Device setter for FFCV Pipeline
         for p in self.pipeline_specs.values():
             for t in p.transforms:
                 if isinstance(t, _ToDevice):
                     t.device = device
-        # Device setter for fastai batch_tfms
+        # Device setter for Loader.batch_tfms
         if hasattr(self.after_batch, 'fs'):
-            for tfm in self.after_batch.fs:
-                if hasattr(tfm, 'to') and callable(tfm.to): 
-                    tfm.to(device)
-                else:
-                    for a in L(getattr(tfm, 'parameters', None)):
-                        setattr(tfm, a, getattr(tfm, a).to(device))
+            self._pipeline_device(self.after_batch.fs)
 
     def to(self, device:int|str|torch.device):
         "Sets `self.device=device`."
         self.device = device
         return self
 
-    def before_iter(self):
-        super().before_iter()
-        f = getattr(self, 'after_batch')
-        if isinstance(f,Pipeline):
-            f.split_idx=self.split_idx
+    @property
+    def split_idx(self):
+        return self._split_idx
+
+    @split_idx.setter
+    def split_idx(self, split_idx:int):
+        "Sets fastai batch transforms to train (split_idx=0) or valid (split_idx=1)"
+        self._split_idx = split_idx
+        if isinstance(self.after_batch, Pipeline):
+            self.after_batch.split_idx = split_idx
 
     def decode(self, b):
         "Decode batch `b`"
         return to_cpu(self.after_batch.decode(self._retain_dl(b)))
 
     def decode_batch(self, b, max_n:int=9):
         "Decode up to `max_n` input(s) from batch `b`"
         return self._decode_batch(self.decode(b), max_n)
 
+    def _pipeline_device(self, pipe):
+        "Device setter for fastai pipeline"
+        for tfm in pipe:
+            if hasattr(tfm, 'to') and callable(tfm.to):
+                tfm.to(self.device, non_blocking=True)
+            else:
+                for a in L(getattr(tfm, 'parameters', None)):
+                    setattr(tfm, a, getattr(tfm, a).to(self.device, non_blocking=True))
+
+    def _iter(self):
+        Compiler.set_num_threads(self.num_workers)
+        order = self.next_traversal_order()
+        selected_order = order[:len(self) * self.batch_size]
+        self.next_epoch += 1
+
+        # Compile at the first epoch
+        if self.code is None or self.recompile:
+            self.generate_code()
+
+        # Asynchronous transforms require using the same Cuda streams for the entire run
+        if self.cuda_streams is None:
+            self.cuda_streams = [(torch.cuda.Stream() if torch.cuda.is_available() else None)
+                                  for _ in range(self.batches_ahead + 2)]
+        if self.async_tfms:
+            return AsyncEpochIterator(self, selected_order, self.after_batch)
+        else:
+            return EpochIterator(self, selected_order)
+
     def __iter__(self):
         self.before_iter()
-        for b in super().__iter__():
-            yield self.after_batch(b)
+        if self.async_tfms:
+            yield from self._iter()
+        else:
+            for b in self._iter():
+                yield self.after_batch(b)
         self.after_iter()
         if hasattr(self, 'it'):
             del(self.it)
 
     def _one_pass(self, b=None):
         if b is None:
             b = self.one_batch()
@@ -256,28 +294,28 @@
         if hasattr(b, 'show'):
             return b,None,None
         its = self._decode_batch(b, max_n)
         if not is_listy(b):
             b,its = [b],L((o,) for o in its)
         return detuplify(b[:self.n_inp]),detuplify(b[self.n_inp:]),its
 
-    def _one_batch(self):
+    def _n_batches(self, num_batches:int=1):
         orig_traversal_order = self.traversal_order
         orig_indices = self.indices
         orig_drop_last = self.drop_last
 
         # Set Loader to only return one batch per epoch
         if self._args['order'] == OrderOption.SEQUENTIAL:
-            self.indices = np.arange(0, self.batch_size)
+            self.indices = np.arange(0, self.batch_size*num_batches)
         else:
-            self.indices = np.random.random_integers(0, self.reader.num_samples, self.batch_size)
+            self.indices = np.random.random_integers(0, self.reader.num_samples, self.batch_size*num_batches)
         self.traversal_order = ORDER_MAP[OrderOption.SEQUENTIAL](self)
         self.drop_last = False
 
-        # yield one batch
-        yield next(self.__iter__())
+        # yield num_batches
+        yield from self.__iter__()
 
         # Reset Loader state to its original status
         self.next_epoch -= 1
         self.indices = orig_indices
         self.drop_last = orig_drop_last
         self.traversal_order = orig_traversal_order
```

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/operations.py` & `fastxtend-0.1.3/fastxtend/ffcv/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 # %% ../../nbs/ffcv.operations.ipynb 1
 # Contains code from:
 # FFCV - Apache License 2.0 - Copyright (c) 2022 FFCV Team
 
 # %% ../../nbs/ffcv.operations.ipynb 4
 from __future__ import annotations
 
-from abc import ABCMeta
 from typing import Callable, Optional, Tuple
 from dataclasses import replace
 
 import torch
 import numpy as np
 
 from fastcore.dispatch import retain_meta
-from fastcore.transform import _TfmMeta
 
 from fastai.data.transforms import IntToFloatTensor as _IntToFloatTensor
 
 from ffcv.pipeline.allocation_query import AllocationQuery
 from ffcv.pipeline.operation import Operation
 from ffcv.pipeline.state import State
 from ffcv.transforms.ops import ToDevice as _ToDevice
```

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/transforms.py` & `fastxtend-0.1.3/fastxtend/ffcv/transforms.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/utils.py` & `fastxtend-0.1.3/fastxtend/ffcv/utils.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/ffcv/writer.py` & `fastxtend-0.1.3/fastxtend/ffcv/writer.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/imports.py` & `fastxtend-0.1.3/fastxtend/imports.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/losses.py` & `fastxtend-0.1.3/fastxtend/losses.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/metrics.py` & `fastxtend-0.1.3/fastxtend/metrics.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/multiloss.py` & `fastxtend-0.1.3/fastxtend/multiloss.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/optimizer/adan.py` & `fastxtend-0.1.3/fastxtend/optimizer/adan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/optimizer.adan.ipynb.
 
 # %% ../../nbs/optimizer.adan.ipynb 1
 # Memory and operations reduction ported from the official Adan implementation
 # https://github.com/sail-sg/Adan - Apache License 2.0 - Copyright 2022 Xingyu Xie et al
 
-# %% ../../nbs/optimizer.adan.ipynb 3
+# %% ../../nbs/optimizer.adan.ipynb 4
 from __future__ import annotations
 from typing import Optional, Dict
 
 import numpy as np
 
 from fastai.optimizer import Optimizer
 
@@ -205,15 +205,15 @@
     @torch.no_grad()
     def step(self, closure=None):
         if closure is not None: raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             pl, gl, grad_avg, diff_avg, sqr_avg, prior_grad, steps, do_wd = [], [], [], [], [], [], [], []
 
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
 
                     if 'step' not in state:
                         state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                         state['diff_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                         state['sqr_avg']  = torch.zeros_like(p, memory_format=torch.preserve_format)
                         if self.paper_init:
@@ -231,15 +231,15 @@
                     prior_grad.append(state['prior_grad'])
                     do_wd.append(state.get('do_wd', True))
                     steps.append(state['step'])
 
             self.opt_step(p=pl, grad=gl, grad_avg=grad_avg, diff_avg=diff_avg, sqr_avg=sqr_avg,
                           prior_grad=prior_grad, steps=np.array(steps, dtype=np.int32), do_wd=np.array(do_wd, dtype=bool), **hyper)
 
-# %% ../../nbs/optimizer.adan.ipynb 16
+# %% ../../nbs/optimizer.adan.ipynb 15
 def Adan(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     beta1:float=0.98, # Gradient moving average (β1) coefficient
     beta2:float=0.92, # Gradient difference moving average (β2) coefficient
     beta3:float=0.99, # Gradient squared moving average (β3) coefficient
     eps:float=1e-8, # Added for numerical stability
@@ -255,26 +255,26 @@
     elif jit:
         cb = partial(adan_jit_step, paper_init=paper_init)
         return JitOptimizer(params, cb, lr=lr, beta1=beta1, beta2=beta2, beta3=beta3, eps=eps, wd=wd)
     else:
         cbs = [partial(adan_setup, paper_init=paper_init), adan_step]
         return Optimizer(params, cbs, lr=lr, beta1=beta1, beta2=beta2, beta3=beta3, eps=eps, wd=wd)
 
-# %% ../../nbs/optimizer.adan.ipynb 17
+# %% ../../nbs/optimizer.adan.ipynb 16
 def adan(
     beta1:float=0.98, # Gradient moving average (β1) coefficient
     beta2:float=0.92, # Gradient difference moving average (β2) coefficient
     beta3:float=0.99, # Gradient squared moving average (β3) coefficient
     eps:float=1e-8, # Added for numerical stability
     wd:float=0.02, # True weight decay
     paper_init:bool=False, # Initialize prior gradient with current gradient per paper, or zeroes
     foreach:bool=False, # Use fused ForEach implementation
     jit:bool=False # Use fused TorchScript implementation
 ) -> Optimizer|AdanForEachOptimizer|JitOptimizer:
     "Partial function for the Adan optimizer with fused ForEach and TorchScript implementations"
     return partialler(Adan, beta1=beta1, beta2=beta2, beta3=beta3, eps=eps, wd=wd,
                       paper_init=paper_init, foreach=foreach, jit=jit)
 
-# %% ../../nbs/optimizer.adan.ipynb 19
+# %% ../../nbs/optimizer.adan.ipynb 18
 def AdanLargeBatchLR(bs:int) -> float:
     "Square root rule for scaling `Adan` learning rate for large-batch training"
     return math.sqrt(bs/256)*6.25e-3
```

### Comparing `fastxtend-0.1.2/fastxtend/optimizer/foreach.py` & `fastxtend-0.1.3/fastxtend/optimizer/foreach.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,22 +65,22 @@
     def step(self, closure=None):
         if closure is not None:
             raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             pl, gl, grad_avg, ones, do_wd = [], [], [], [], []
 
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
 
                     if 'setup' not in state:
                         if hyper['mom'] != 0:
                             state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                         if not self.decouple_wd:
-                            state['ones'] = torch.ones_like(p, memory_format=torch.preserve_format)
+                            state['ones'] = torch.ones(1, dtype=p.dtype, device=p.device)
                         state['setup'] = True
 
                     pl.append(p)
                     gl.append(p.grad)
                     grad_avg.append(state.get('grad_avg', None))
                     ones.append(state.get('ones', None))
                     do_wd.append(state.get('do_wd', True))
@@ -129,22 +129,22 @@
     def step(self, closure=None):
         if closure is not None:
             raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             pl, gl, grad_avg, sqr_avg, ones, steps, do_wd = [], [], [], [], [], [], []
 
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
 
                     if 'step' not in state:
                         state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                         state['sqr_avg']  = torch.zeros_like(p, memory_format=torch.preserve_format)
                         if not self.decouple_wd:
-                            state['ones'] = torch.ones_like(p, memory_format=torch.preserve_format)
+                            state['ones'] = torch.ones(1, dtype=p.dtype, device=p.device)
                         state['step'] = 0
 
                     state['step'] += 1
                     pl.append(p)
                     gl.append(p.grad)
                     grad_avg.append(state['grad_avg'])
                     sqr_avg.append(state['sqr_avg'])
@@ -206,21 +206,21 @@
     def step(self, closure=None):
         if closure is not None:
             raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             pl, gl, grad_avg, sqr_avg, steps, ones, do_wd = [], [], [], [], [], [], []
 
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
 
                     if 'step' not in state:
                         state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                         state['sqr_avg']  = torch.zeros_like(p, memory_format=torch.preserve_format)
-                        state['ones']     = torch.ones_like(p, memory_format=torch.preserve_format)
+                        state['ones']     = torch.ones(1, dtype=p.dtype, device=p.device)
                         state['step']     = 0
 
                     state['step'] += 1
                     pl.append(p)
                     gl.append(p.grad)
                     grad_avg.append(state['grad_avg'])
                     sqr_avg.append(state['sqr_avg'])
@@ -230,17 +230,15 @@
 
             self.opt_step(p=pl, g=gl, grad_avg=grad_avg, sqr_avg=sqr_avg, ones=ones,
                           steps=np.array(steps, dtype=np.int32), do_wd=np.array(do_wd, dtype=bool),
                           decouple_wd=self.decouple_wd, **hyper)
 
 # %% ../../nbs/optimizer.foreach.ipynb 35
 @torch.jit.script
-def lamb_jit_substep(p:Tensor, lstep:Tensor, lr:float):
-    r1 = p.pow(2).mean().sqrt()
-    r2 = lstep.pow(2).mean().sqrt()
+def lamb_jit_substep(r1:Tensor, r2:Tensor, lr:float):
     if r1 == 0 or r2 == 0:
         return -lr
     else:
         return -lr*min(r1/r2, 10.)
 
 # %% ../../nbs/optimizer.foreach.ipynb 36
 def lamb_foreach_step(p:list[Tensor], g:list[Tensor], grad_avg:list[Tensor], sqr_avg:list[Tensor], ones:list[Tensor],
@@ -271,16 +269,18 @@
     debias2 = np.sqrt(1 - sqr_mom**steps)
 
     debias2 = torch._foreach_div(torch._foreach_sqrt(sqr_avg), debias2.tolist())
     torch._foreach_add_(debias2, eps)
     lstep = torch._foreach_div(grad_avg, debias1.tolist())
     torch._foreach_div_(lstep, debias2)
 
-    # there are no implementations for foreach_pow, foreach_mean, or foreach_where/if methods
-    q = [lamb_jit_substep(pi, ls, lr) for pi, ls in zip(p, lstep)]
+    r1s = torch._foreach_norm(p, 2)
+    r2s = torch._foreach_norm(lstep, 2)
+    # there are no implementations for foreach_where/if methods so use a loop
+    q = [lamb_jit_substep(r1, r2, lr) for r1, r2 in zip(r1s, r2s)]
 
     # cannot use scalers with foreach_add & multiple tensors, so divide by one with foreach_addcdiv
     torch._foreach_addcdiv_(p, lstep, ones, scalars=q)
 
 # %% ../../nbs/optimizer.foreach.ipynb 37
 class LambForEachOptimizer(RAdamForEachOptimizer):
     "An `ForEachOptimizer` with a modified step for `lamb_foreach_step`"
@@ -314,21 +314,21 @@
     def step(self, closure=None):
         self.count += 1
         if closure is not None:
             raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             pl, gl, grad_avg, sqr_avg, slow_p, steps, ones, do_wd = [], [], [], [], [], [], [], []
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
 
                     if 'step' not in state:
                         state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                         state['sqr_avg']  = torch.zeros_like(p, memory_format=torch.preserve_format)
-                        state['ones']     = torch.ones_like(p, memory_format=torch.preserve_format)
+                        state['ones']     = torch.ones(1, dtype=p.dtype, device=p.device)
                         state['slow_p']   = p.data.clone()
                         state['step']     = 0
 
                     state['step'] += 1
                     pl.append(p)
                     gl.append(p.grad)
                     grad_avg.append(state['grad_avg'])
```

### Comparing `fastxtend-0.1.2/fastxtend/optimizer/fused.py` & `fastxtend-0.1.3/fastxtend/optimizer/fused.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,124 +19,174 @@
                                              lamb_jit_step, JitLookahead, ranger_jit_step)
 
 from .foreach import (SGDForEachOptimizer, sgd_foreach_step, AdamForEachOptimizer,
                                          adam_foreach_step, RAdamForEachOptimizer, radam_foreach_step,
                                          LambForEachOptimizer, lamb_foreach_step, RangerForEachOptimizer,
                                          ranger_foreach_step)
 
+try:
+    from fastxtend.optimizer.eightbit import (SGD8bitOptimizer, RMSProp8bitOptimizer, AdamW8bitOptimizer,
+                                              LARS8bitOptimizer, LAMB8bitOptimizer)
+    EIGHTBIT = True
+except ImportError:
+    EIGHTBIT = False
+
 from ..imports import *
 
 # %% auto 0
 __all__ = ['SGD', 'sgd', 'RMSProp', 'rmsprop', 'Adam', 'adam', 'RAdam', 'radam', 'QHAdam', 'qhadam', 'Larc', 'larc', 'Lamb',
            'lamb', 'Ranger', 'ranger']
 
-# %% ../../nbs/optimizer.fused.ipynb 9
+# %% ../../nbs/optimizer.fused.ipynb 8
 def SGD(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0., # Gradient moving average (β1) coefficient
     wd:float=0., # Optional weight decay (true or L2)
     decouple_wd:bool=True, # Apply true weight decay (SGDW) or L2 regularization (SGD)
     foreach:bool=False, # Use fused ForEach implementation
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|SGDForEachOptimizer|JitOptimizer:
-    "A fastai SGD/SGDW optimizer with fused ForEach and TorchScript implementations"
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|SGDForEachOptimizer|JitOptimizer|SGD8bitOptimizer:
+    "A fastai SGD/SGDW optimizer with fused ForEach, TorchScript, & 8-bit implementations"
     if foreach:
-        return SGDForEachOptimizer(params, sgd_foreach_step, lr=lr, mom=mom, wd=wd, decouple_wd=decouple_wd)
+        return SGDForEachOptimizer(params, sgd_foreach_step, lr=lr, mom=mom,
+                                   wd=wd, decouple_wd=decouple_wd)
     elif jit:
-        return JitOptimizer(params, sgd_jit_step, lr=lr, mom=mom, wd=wd, decouple_wd=decouple_wd)
+        return JitOptimizer(params, sgd_jit_step, lr=lr, mom=mom, wd=wd,
+                            decouple_wd=decouple_wd)
+    elif eightbit:
+        if EIGHTBIT:
+            if decouple_wd and wd > 0:
+                raise NotImplementedError(f'8-bit SGD only supports L2 weight decay: {decouple_wd=}')
+            return SGD8bitOptimizer(params, lr=lr, mom=mom, wd=wd, **eightbitargs)
+        else:
+            raise ImportError(f'{eightbit=}. bitsandbytes package not found. Run `pip install bitsandbytes`.')
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         if mom != 0: cbs.append(average_grad)
         cbs.append(sgd_step if mom==0 else momentum_step)
         return Optimizer(params, cbs, lr=lr, mom=mom, wd=wd)
 
-# %% ../../nbs/optimizer.fused.ipynb 10
+# %% ../../nbs/optimizer.fused.ipynb 9
 def sgd(
     mom:float=0., # Gradient moving average (β1) coefficient
     wd:float=0., # Optional weight decay (true or L2)
     decouple_wd:bool=True, # Apply true weight decay (SGDW) or L2 regularization (SGD)
     foreach:bool=False, # Use fused ForEach implementation
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|SGDForEachOptimizer|JitOptimizer:
-    "Partial function for the SGD/SGDW optimizer with fused ForEach and TorchScript implementations"
-    return partialler(SGD, mom=mom, wd=wd, decouple_wd=decouple_wd, jit=jit, foreach=foreach)
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|SGDForEachOptimizer|JitOptimizer|SGD8bitOptimizer:
+    "Partial function for the SGD/SGDW optimizer with fused ForEach, TorchScript, & 8-bit implementations"
+    return partialler(SGD, mom=mom, wd=wd, decouple_wd=decouple_wd, jit=jit,
+                      foreach=foreach, eightbit=eightbit, **eightbitargs)
 
-# %% ../../nbs/optimizer.fused.ipynb 13
+# %% ../../nbs/optimizer.fused.ipynb 12
 def RMSProp(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0., # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-8, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|JitOptimizer:
-    "A fastai RMSProp/RMSPropW optimizer with a fused TorchScript implementation"
+    decouple_wd:bool=True, # Apply true weight decay or L2 regularization. Ignored if `eightbit=True`
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|JitOptimizer|RMSProp8bitOptimizer:
+    "A fastai RMSProp/RMSPropW optimizer with fused TorchScript and 8-bit implementations"
     if jit:
         return JitOptimizer(params, rmsprop_jit_step, lr=lr, mom=mom, sqr_mom=sqr_mom,
                             eps=eps, wd=wd, decouple_wd=decouple_wd)
+    elif eightbit:
+        if EIGHTBIT:
+            if decouple_wd and wd > 0:
+                raise NotImplementedError(f'8-bit RMSProp only supports L2 weight decay: {decouple_wd=}')
+            if mom > 0:
+                raise NotImplementedError(f'8-bit RMSProp does not use momentum: {mom=}')
+            return RMSProp8bitOptimizer(params, lr=lr, sqr_mom=sqr_mom,
+                                        eps=eps, wd=wd, **eightbitargs)
+        else:
+            raise ImportError(f'{eightbit=}. bitsandbytes package not found. Run `pip install bitsandbytes`.')
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         cbs += ([average_sqr_grad] if mom==0. else [average_grad, average_sqr_grad])
         cbs.append(rms_prop_step)
         return Optimizer(params, cbs, lr=lr, mom=mom, sqr_mom=sqr_mom, wd=wd, eps=eps)
 
-# %% ../../nbs/optimizer.fused.ipynb 14
+# %% ../../nbs/optimizer.fused.ipynb 13
 def rmsprop(
     mom:float=0., # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-8, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
     decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|JitOptimizer:
-    "Partial function for the RMSProp/RMSPropW optimizer with a fused TorchScript implementation"
-    return partialler(RMSProp, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd, decouple_wd=decouple_wd, jit=jit)
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|JitOptimizer|RMSProp8bitOptimizer:
+    "Partial function for the RMSProp/RMSPropW optimizer with fused TorchScript and 8-bit implementations"
+    return partialler(RMSProp, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd,
+                      decouple_wd=decouple_wd, jit=jit, eightbit=eightbit,
+                      **eightbitargs)
 
-# %% ../../nbs/optimizer.fused.ipynb 17
+# %% ../../nbs/optimizer.fused.ipynb 16
 def Adam(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0.9, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-5, # Added for numerical stability
     wd:float=0.01, # Optional weight decay (true or L2)
     decouple_wd:bool=True, # Apply true weight decay (AdamW) or L2 regularization (Adam)
     foreach:bool=False, # Use fused ForEach implementation
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|AdamForEachOptimizer|JitOptimizer:
-    "A fastai Adam/AdamW optimizer with fused ForEach and TorchScript implementations"
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|AdamForEachOptimizer|JitOptimizer|AdamW8bitOptimizer:
+    "A fastai Adam/AdamW optimizer with fused ForEach, TorchScript, & 8-bit implementations"
     if foreach:
         return AdamForEachOptimizer(params, adam_foreach_step, lr=lr, mom=mom,
                                     sqr_mom=sqr_mom, eps=eps, wd=wd, decouple_wd=decouple_wd)
     elif jit:
         return JitOptimizer(params, adam_jit_step, lr=lr, mom=mom, sqr_mom=sqr_mom,
                             eps=eps, wd=wd, decouple_wd=decouple_wd)
+    elif eightbit:
+        if EIGHTBIT:
+            if not decouple_wd and wd > 0:
+                raise NotImplementedError(f'8-bit AdamW only supports true weight decay: {decouple_wd=}')
+            return AdamW8bitOptimizer('adam', params, lr=lr, mom=mom, sqr_mom=sqr_mom,
+                                           eps=eps, wd=wd, **eightbitargs)
+        else:
+            raise ImportError(f'{eightbit=}. bitsandbytes package not found. Run `pip install bitsandbytes`.')
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         cbs += [partial(average_grad, dampening=True), average_sqr_grad, step_stat, adam_step]
         return Optimizer(params, cbs, lr=lr, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd)
 
-# %% ../../nbs/optimizer.fused.ipynb 18
+# %% ../../nbs/optimizer.fused.ipynb 17
 def adam(
     mom:float=0.9, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-5, # Added for numerical stability
     wd:float=0.01, # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
+    decouple_wd:bool=True, # Apply true weight decay (AdamW) or L2 regularization (Adam)
     foreach:bool=False, # Use fused ForEach implementation
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|AdamForEachOptimizer|JitOptimizer:
-    "Partial function for the Adam/AdamW optimizer with fused ForEach and TorchScript implementations"
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|AdamForEachOptimizer|JitOptimizer|AdamW8bitOptimizer:
+    "Partial function for the Adam/AdamW optimizer with fused ForEach, TorchScript, & 8-bit implementations"
     return partialler(Adam, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd,
-                      decouple_wd=decouple_wd, foreach=foreach, jit=jit)
+                      decouple_wd=decouple_wd, foreach=foreach, jit=jit,
+                      eightbit=eightbit, **eightbitargs)
 
-# %% ../../nbs/optimizer.fused.ipynb 21
+# %% ../../nbs/optimizer.fused.ipynb 20
 def RAdam(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0.9, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-5, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
@@ -155,30 +205,30 @@
         return JitOptimizer(params, radam_jit_step, lr=lr, mom=mom, sqr_mom=sqr_mom, eps=eps,
                             wd=wd, decouple_wd=decouple_wd)
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         cbs += [partial(average_grad, dampening=True), average_sqr_grad, step_stat, radam_step]
         return Optimizer(params, cbs, lr=lr, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd, beta=beta)
 
-# %% ../../nbs/optimizer.fused.ipynb 22
+# %% ../../nbs/optimizer.fused.ipynb 21
 def radam(
     mom:float=0.9, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-5, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
     beta:float=0., # Set to enable SAdam with native fastai RAdam
-    decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
+    decouple_wd:bool=True, # Apply true weight decay (RAdamW) or L2 regularization (RAdam)
     foreach:bool=False, # Use fused ForEach implementation
     jit:bool=False # Use fused TorchScript implementation
 ) -> Optimizer|RAdamForEachOptimizer|JitOptimizer:
     "Partial function for the RAdam/RAdamW optimizer with fused ForEach and TorchScript implementations"
     return partialler(RAdam, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd, beta=beta,
                       decouple_wd=decouple_wd, foreach=foreach, jit=jit)
 
-# %% ../../nbs/optimizer.fused.ipynb 25
+# %% ../../nbs/optimizer.fused.ipynb 24
 def QHAdam(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0.999, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.999, # Gradient squared moving average (β2) coefficient
     nu_1:float=0.7, # QH immediate discount factor
     nu_2:float=1.0, # QH momentum discount factor
@@ -192,105 +242,131 @@
         return JitOptimizer(params, qhadam_jit_step, lr=lr, nu_1=nu_1, nu_2=nu_2, mom=mom,
                             sqr_mom=sqr_mom, eps=eps, wd=wd, decouple_wd=decouple_wd)
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         cbs += [partial(average_grad, dampening=True), average_sqr_grad, step_stat, qhadam_step]
         return Optimizer(params, cbs, lr=lr, nu_1=nu_1, nu_2=nu_2, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd)
 
-# %% ../../nbs/optimizer.fused.ipynb 26
+# %% ../../nbs/optimizer.fused.ipynb 25
 def qhadam(
     mom:float=0.999, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.999, # Gradient squared moving average (β2) coefficient
     nu_1:float=0.7, # QH immediate discount factor
     nu_2:float=1.0, # QH momentum discount factor
     eps:float=1e-8, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
+    decouple_wd:bool=True, # Apply true weight decay (QHAdamW) or L2 regularization (QHAdam)
     jit:bool=False # Use fused TorchScript implementation
 ) -> Optimizer|JitOptimizer:
     "Partial function for the QHAdam/QHAdamW optimizer with a fused TorchScript implementation"
     return partialler(QHAdam, mom=mom, sqr_mom=sqr_mom, nu_1=nu_1, nu_2=nu_2, eps=eps,
                       wd=wd, decouple_wd=decouple_wd, jit=jit)
 
-# %% ../../nbs/optimizer.fused.ipynb 29
+# %% ../../nbs/optimizer.fused.ipynb 28
 def Larc(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0.9, # Gradient moving average (β1) coefficient
     clip:bool=True, # LARC if clip=True, LARS if clip=False
     trust_coeff:float=0.02, # Trust coeffiecnet for calculating layerwise LR
     eps:float=1e-8, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay or L2 regularization
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|JitOptimizer:
-    "A fastai LARC/LARS optimizer with a fused TorchScript implementation"
+    decouple_wd:bool=True, # Apply true weight decay or L2 regularization. Ignored if `eightbit=True`
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation. Only supports LARS: `clip=False`
+    **eightbitargs
+) -> Optimizer|JitOptimizer|LARS8bitOptimizer:
+    "A fastai LARC/LARS optimizer with fused TorchScript & 8-bit implementations"
     if jit:
         cb = partial(larc_jit_step, clip=clip)
         return JitOptimizer(params, cb, lr=lr, mom=mom, trust_coeff=trust_coeff,
                             eps=eps, wd=wd, decouple_wd=decouple_wd)
+    elif eightbit:
+        if EIGHTBIT:
+            if clip:
+                raise NotImplementedError(f'{eightbit=} only supports the LARS optimizer. Set `clip=False`.')
+            if decouple_wd and wd > 0:
+                raise NotImplementedError(f'8-bit LARS only supports L2 weight decay: {decouple_wd=}')
+            return LARS8bitOptimizer(params, lr=lr, mom=mom, wd=wd, trust_coeff=trust_coeff, **eightbitargs)
+        else:
+            raise ImportError(f'{eightbit=}. bitsandbytes package not found. Run `pip install bitsandbytes`.')
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         if mom!=0.: cbs.append(average_grad)
         cbs += [partial(larc_layer_lr, clip=clip), larc_step]
         return Optimizer(params, cbs, lr=lr, mom=mom, trust_coeff=trust_coeff, eps=eps, wd=wd)
 
-# %% ../../nbs/optimizer.fused.ipynb 30
+# %% ../../nbs/optimizer.fused.ipynb 29
 def larc(
     mom:float=0.9, # Gradient moving average (β1) coefficient
     clip:bool=True, # LARC if clip=True, LARS if clip=False
     trust_coeff:float=0.02, # Trust coeffiecnet for calculating layerwise LR
     eps:float=1e-8, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|JitOptimizer:
-    "Partial function for the LARC/LARS optimizer with a fused TorchScript implementation"
+    decouple_wd:bool=True, # Apply true weight decay or L2 regularization
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation. Only supports LARS
+    **eightbitargs
+) -> Optimizer|JitOptimizer|LARS8bitOptimizer:
+    "Partial function for the LARC/LARS optimizer with fused TorchScript & 8-bit implementations"
     return partialler(Larc, mom=mom, clip=clip, eps=eps, trust_coeff=trust_coeff,
                       wd=wd, decouple_wd=decouple_wd, jit=jit)
 
-# %% ../../nbs/optimizer.fused.ipynb 33
+# %% ../../nbs/optimizer.fused.ipynb 32
 def Lamb(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0.9, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-5, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay or L2 regularization
+    decouple_wd:bool=True, # Apply true weight decay or L2 regularization. Ignored if `eightbit=True`
     foreach:bool=False, # Use fused ForEach implementation
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|LambForEachOptimizer|JitOptimizer:
-    "A fastai LAMB optimizer with fused ForEach and TorchScript implementations"
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation. Only supports true weight decay
+    **eightbitargs
+) -> Optimizer|LambForEachOptimizer|JitOptimizer|LAMB8bitOptimizer:
+    "A fastai LAMB optimizer with fused ForEach, TorchScript, & 8-bit implementations"
     if foreach:
         return LambForEachOptimizer(params, lamb_foreach_step, lr=lr, mom=mom, sqr_mom=sqr_mom,
                                     eps=eps, wd=wd, decouple_wd=decouple_wd)
-    if jit:
+    elif jit:
         return JitOptimizer(params, lamb_jit_step, lr=lr, mom=mom, sqr_mom=sqr_mom,
                             eps=eps, wd=wd, decouple_wd=decouple_wd)
+    elif eightbit:
+        if EIGHTBIT:
+            if not decouple_wd and wd > 0:
+                raise NotImplementedError(f'8-bit LAMB only supports true weight decay: {decouple_wd=}')
+            return LAMB8bitOptimizer(params, lr=lr, mom=mom, sqr_mom=sqr_mom,
+                                     eps=eps, wd=wd, **eightbitargs)
+        else:
+            raise ImportError(f'{eightbit=}. bitsandbytes package not found. Run `pip install bitsandbytes`.')
     else:
         cbs = [weight_decay] if decouple_wd else [l2_reg]
         cbs += [partial(average_grad, dampening=True), average_sqr_grad, step_stat, lamb_step]
         return Optimizer(params, cbs, lr=lr, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd)
 
-# %% ../../nbs/optimizer.fused.ipynb 34
+# %% ../../nbs/optimizer.fused.ipynb 33
 def lamb(
     mom:float=0.9, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-5, # Added for numerical stability
     wd:float=0., # Optional weight decay (true or L2)
-    decouple_wd:bool=True, # Apply true weight decay (RMSPropW) or L2 regularization (RMSProp)
+    decouple_wd:bool=True, # Apply true weight decay or L2 regularization
     foreach:bool=False, # Use fused ForEach implementation
-    jit:bool=False # Use fused TorchScript implementation
-) -> Optimizer|LambForEachOptimizer|JitOptimizer:
-    "Partial function for the LAMB optimizer with fused ForEach and TorchScript implementations"
+    jit:bool=False, # Use fused TorchScript implementation
+    eightbit:bool=False, # Use fused 8-bit implementation. Only supports true weight decay
+    **eightbitargs
+) -> Optimizer|LambForEachOptimizer|JitOptimizer|LAMB8bitOptimizer:
+    "Partial function for the LAMB optimizer with fused ForEach, TorchScript, & 8-bit implementations"
     return partialler(Lamb, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd,
-                      decouple_wd=decouple_wd, foreach=foreach, jit=jit)
+                      decouple_wd=decouple_wd, foreach=foreach, jit=jit,
+                      eightbit=eightbit, **eightbitargs)
 
-# %% ../../nbs/optimizer.fused.ipynb 37
+# %% ../../nbs/optimizer.fused.ipynb 36
 def Ranger(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     mom:float=0.95, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-6, # Added for numerical stability
     wd:float=0.01, # Optional weight decay (true or L2)
@@ -308,15 +384,15 @@
         return JitLookahead(params, ranger_jit_step, lr=lr, mom=mom, sqr_mom=sqr_mom, eps=eps,
                             wd=wd, k=k, alpha=alpha, decouple_wd=decouple_wd)
     else:
         return Lookahead(RAdam(params, lr=lr, mom=mom, sqr_mom=sqr_mom, eps=eps, wd=wd,
                                decouple_wd=decouple_wd),
                          k=k, alpha=alpha)
 
-# %% ../../nbs/optimizer.fused.ipynb 38
+# %% ../../nbs/optimizer.fused.ipynb 37
 def ranger(
     mom:float=0.95, # Gradient moving average (β1) coefficient
     sqr_mom:float=0.99, # Gradient squared moving average (β2) coefficient
     eps:float=1e-6, # Added for numerical stability
     wd:float=0.01, # Optional weight decay (true or L2)
     k:int=6, # How often to conduct Lookahead step
     alpha:float=0.5, # Slow weight moving average coefficient
```

### Comparing `fastxtend-0.1.2/fastxtend/optimizer/lion.py` & `fastxtend-0.1.3/fastxtend/optimizer/lion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/optimizer.lion.ipynb.
 
 # %% ../../nbs/optimizer.lion.ipynb 1
 # Lion implementation based on the paper's code release
 # https://github.com/google/automl/tree/master/lion - Apache License 2.0 - Copyright 2020 Google Research
 
-# %% ../../nbs/optimizer.lion.ipynb 3
+# %% ../../nbs/optimizer.lion.ipynb 4
 from __future__ import annotations
 
 import numpy as np
 
 from fastai.optimizer import Optimizer
 
 from .foreach import ForEachOptimizer
+
+try:
+    from fastxtend.optimizer.eightbit import Lion8bitOptimizer
+    EIGHTBIT = True
+except ImportError:
+    EIGHTBIT = False
+
 from ..imports import *
 
 # %% auto 0
 __all__ = ['Lion', 'lion']
 
 # %% ../../nbs/optimizer.lion.ipynb 6
 def lion_step(p:Tensor, lr:float, wd:float, beta1:float, beta2:float,
@@ -72,45 +79,56 @@
     @torch.no_grad()
     def step(self, closure=None):
         if closure is not None: raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             pl, gl, grad_avg, do_wd = [], [], [], []
 
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
 
                     if 'grad_avg' not in state:
                         state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
 
                     pl.append(p)
                     gl.append(p.grad)
                     grad_avg.append(state['grad_avg'])
                     do_wd.append(state.get('do_wd', True))
 
             self.opt_step(p=pl, g=gl, grad_avg=grad_avg, do_wd=np.array(do_wd, dtype=bool), **hyper)
 
-# %% ../../nbs/optimizer.lion.ipynb 12
+# %% ../../nbs/optimizer.lion.ipynb 11
 def Lion(
     params:Listified[Tensor], # Model parameters or parameter groups
     lr:float, # Default learning rate
     beta1:float=0.9, # Update gradient moving average (β1) coefficient
     beta2:float=0.99, # Gradient moving average (β2) coefficient
     wd:float=0.1, # True weight decay
     foreach:bool=False, # Use fused ForEach implementation
-) -> Optimizer|LionForEachOptimizer:
-    "A fastai Lion optimizer with a fused ForEach implementation"
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|LionForEachOptimizer|Lion8bitOptimizer:
+    "A fastai Lion optimizer with fused ForEach and 8-bit implementations"
     if foreach:
         return LionForEachOptimizer(params, lion_foreach_step, lr=lr,
                                     beta1=beta1, beta2=beta2, wd=wd)
+    elif eightbit:
+        if EIGHTBIT:
+            return Lion8bitOptimizer(params, lr=lr, beta1=beta1,
+                                     beta2=beta2, wd=wd, **eightbitargs)
+        else:
+            raise ImportError(f'{eightbit=}. bitsandbytes package not found. Run `pip install bitsandbytes`')
     else:
         return Optimizer(params, [lion_step], lr=lr, beta1=beta1, beta2=beta2, wd=wd)
 
-# %% ../../nbs/optimizer.lion.ipynb 13
+# %% ../../nbs/optimizer.lion.ipynb 12
 def lion(
     beta1:float=0.9, # Update gradient moving average (β1) coefficient
     beta2:float=0.99, # Gradient moving average (β2) coefficient
     wd:float=0.1, # True weight decay
     foreach:bool=False, # Use fused ForEach implementation
-) -> Optimizer|LionForEachOptimizer:
-    "Partial function for the Lion optimizer with a fused ForEach implementation"
-    return partialler(Lion, beta1=beta1, beta2=beta2, wd=wd, foreach=foreach)
+    eightbit:bool=False, # Use fused 8-bit implementation
+    **eightbitargs
+) -> Optimizer|LionForEachOptimizer|Lion8bitOptimizer:
+    "Partial function for the Lion optimizer with fused ForEach and 8-bit implementations"
+    return partialler(Lion, beta1=beta1, beta2=beta2, wd=wd, foreach=foreach,
+                      eightbit=eightbit, **eightbitargs)
```

### Comparing `fastxtend-0.1.2/fastxtend/optimizer/torchscript.py` & `fastxtend-0.1.3/fastxtend/optimizer/torchscript.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     @torch.no_grad()
     def step(self, closure=None):
         if closure is not None:
             raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     state = self.state[p]
                     _update(state, self.opt_step(p=p, g=p.grad, decouple_wd=self.decouple_wd, **{**state, **hyper}))
 
 # %% ../../nbs/optimizer.torchscript.ipynb 13
 @torch.jit.script
 def sgd_jit_step(p:Tensor, g:Tensor, decouple_wd:bool, lr:float, wd:float, mom:float,
                  grad_avg:Optional[Tensor]=None, do_wd:bool=True, force_train:Optional[bool]=None):
@@ -320,17 +320,17 @@
     # average_sqr_grad
     sqr_avg = sqr_avg.mul(sqr_mom).addcmul(grad, grad, value=1-sqr_mom)
 
     # lamb_step
     debias1 = 1-mom**step
     debias2 = 1-sqr_mom**step
 
-    r1 = param.pow(2).mean().sqrt()
+    r1 = param.norm(2)
     lstep = (grad_avg/debias1) / ((sqr_avg/debias2).sqrt()+eps)
-    r2 = lstep.pow(2).mean().sqrt()
+    r2 = lstep.norm(2)
 
     if r1 == 0 or r2 == 0:
         param = param.add(lstep, alpha=-lr)
     else:
         q = min(r1/r2, 10.)
         param = param.add(lstep, alpha=-lr*q)
 
@@ -353,15 +353,15 @@
 
     @torch.no_grad()
     def step(self, closure=None):
         self.count += 1
         if closure is not None: raise NotImplementedError("fastai optimizers currently do not support closure")
         for pg, hyper in zip(self.param_lists, self.hypers):
             for p in pg:
-                if hasattr(p, 'grad') and p.grad is not None:
+                if p.grad is not None:
                     _update(self.state[p], self.opt_step(p, p.grad, decouple_wd=self.decouple_wd, **{**self.state[p], **hyper}, count=self.count))
 
     def clear_state(self):
         super().clear_state()
         self._init_state()
 
     def state_dict(self):
```

### Comparing `fastxtend-0.1.2/fastxtend/patches.py` & `fastxtend-0.1.3/fastxtend/patches.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/schedulers.py` & `fastxtend-0.1.3/fastxtend/schedulers.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/test_utils.py` & `fastxtend-0.1.3/fastxtend/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/test_utils.ipynb.
 
 # %% auto 0
-__all__ = ['TEST_AUDIO', 'TEST_IMAGE', 'test_fail', 'test', 'nequals', 'test_eq', 'test_eq_type', 'test_ne', 'is_close',
-           'test_close', 'test_is', 'test_shuffled', 'test_stdout', 'test_warns', 'test_fig_exists',
-           'ExceptionExpected', 'exception', 'synth_dbunch', 'RegModel', 'synth_learner', 'VerboseCallback', 'get_env',
-           'try_import', 'nvidia_smi', 'nvidia_mem', 'test_show_install', 'less_random']
+__all__ = ['TEST_AUDIO', 'TEST_IMAGE', 'tst_param', 'tst_params', 'test_fail', 'test', 'nequals', 'test_eq', 'test_eq_type',
+           'test_ne', 'is_close', 'test_close', 'test_is', 'test_shuffled', 'test_stdout', 'test_warns',
+           'test_fig_exists', 'ExceptionExpected', 'exception', 'synth_dbunch', 'RegModel', 'synth_learner',
+           'VerboseCallback', 'get_env', 'try_import', 'nvidia_smi', 'nvidia_mem', 'test_show_install', 'less_random']
 
 # %% ../nbs/test_utils.ipynb 2
-from fastcore.test import (test_fail, test, nequals, test_eq, test_eq_type, test_ne, 
-                           is_close, test_close, test_is, test_shuffled, test_stdout, 
+from fastcore.test import (test_fail, test, nequals, test_eq, test_eq_type, test_ne,
+                           is_close, test_close, test_is, test_shuffled, test_stdout,
                            test_warns, TEST_IMAGE, test_fig_exists, ExceptionExpected, exception)
 
+from fastcore.foundation import L
+from fastai.torch_core import tensor
 from fastai.test_utils import synth_dbunch, synth_learner, RegModel, VerboseCallback, get_env, try_import, nvidia_smi, nvidia_mem
 from fastai.test_utils import show_install as test_show_install
 from .utils import less_random
 
 # %% ../nbs/test_utils.ipynb 4
 _all_ = ['test_fail', 'test', 'nequals', 'test_eq', 'test_eq_type', 'test_ne', 'is_close', 'test_close', 'test_is', 'test_shuffled', 'test_stdout', 'test_warns', 'TEST_IMAGE', 'test_fig_exists', 'ExceptionExpected', 'exception',  'synth_dbunch', 'RegModel', 'synth_learner', 'VerboseCallback', 'get_env', 'try_import', 'nvidia_smi', 'nvidia_mem', 'test_show_install', 'less_random']
 
 # %% ../nbs/test_utils.ipynb 5
 TEST_AUDIO = 'audio/whistle.wav'
 TEST_IMAGE = 'images/puppy.jpg'
+
+# %% ../nbs/test_utils.ipynb 7
+def tst_param(val, grad=None):
+    "Create a tensor with `val` and a gradient of `grad` for testing"
+    res = tensor([val]).float()
+    res.grad = tensor([val/10 if grad is None else grad]).float()
+    return res
+
+# %% ../nbs/test_utils.ipynb 8
+def tst_params():
+    r = L.range(4)
+    return r.map(tst_param)
```

### Comparing `fastxtend-0.1.2/fastxtend/torch_core.py` & `fastxtend-0.1.3/fastxtend/torch_core.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/transform.py` & `fastxtend-0.1.3/fastxtend/transform.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/utils.py` & `fastxtend-0.1.3/fastxtend/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,70 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/utils.ipynb.
 
 # %% ../nbs/utils.ipynb 1
 # Contains code from:
 # fastai - Apache License 2.0 - Copyright (c) 2023 fast.ai
+# miniai - Apache License 2.0 - Copyright (c) 2023 fast.ai
+# ipython - BSD 3-Clause License - Copyright (c) 2008-Present IPython Development Team; 2001-2007 Fernando Perez; 2001 Janko Hauser; 2001 Nathaniel Gray
 # mish-cuda - MIT License - Copyright (c) 2019 thomasbrandon https://github.com/thomasbrandon/mish-cuda
 
 # %% ../nbs/utils.ipynb 3
 from __future__ import annotations
 
-import torch, random, gc
+import torch, random, gc, sys, traceback
 import numpy as np
 import PIL.Image as Image
 
 from fastcore.foundation import contextmanager
 
 from fastai.learner import Learner
 from fastai.data.core import DataLoaders
 from fastai.callback.core import set_random_states, get_random_states
 
 # %% auto 0
 __all__ = ['free_gpu_memory', 'less_random', 'scale_time', 'pil_to_numpy']
 
 # %% ../nbs/utils.ipynb 4
+def clean_ipython_hist():
+    # Code in this function mainly copied from IPython source
+    if not 'get_ipython' in globals():
+        return
+    ip = get_ipython()
+    user_ns = ip.user_ns
+    ip.displayhook.flush()
+    pc = ip.displayhook.prompt_count + 1
+    for n in range(1, pc):
+        user_ns.pop('_i'+repr(n),None)
+    user_ns.update(dict(_i='',_ii='',_iii=''))
+    hm = ip.history_manager
+    hm.input_hist_parsed[:] = [''] * pc
+    hm.input_hist_raw[:] = [''] * pc
+    hm._i = hm._ii = hm._iii = hm._i00 = ''
+
+# %% ../nbs/utils.ipynb 5
+def clean_traceback():
+    # h/t Piotr Czapla
+    if hasattr(sys, 'last_traceback'):
+        traceback.clear_frames(sys.last_traceback)
+        delattr(sys, 'last_traceback')
+    if hasattr(sys, 'last_type'):
+        delattr(sys, 'last_type')
+    if hasattr(sys, 'last_value'):
+        delattr(sys, 'last_value')
+
+# %% ../nbs/utils.ipynb 6
 def free_gpu_memory(learn:Learner, dls:DataLoaders=None):
     "Frees GPU memory using `gc.collect` and `torch.cuda.empty_cache`"
     learn.dls, learn, dls = None, None, None
+    clean_traceback()
+    clean_ipython_hist()
     gc.collect()
     torch.cuda.empty_cache()
 
-# %% ../nbs/utils.ipynb 5
+# %% ../nbs/utils.ipynb 7
 @contextmanager
 def less_random(
     seed:int=42, # Seed for `random`, `torch`, and `numpy`
     deterministic:bool|None=None, # Set `torch.backends.cudnn.deterministic` if not None
     benchmark:bool|None=None # Set `torch.backends.cudnn.benchmark` if not None
 ):
     """
@@ -56,27 +88,27 @@
         torch.backends.cudnn.benchmark = benchmark
 
     try:
         yield # we are managing global variables
     finally:
         set_random_states(**states)
 
-# %% ../nbs/utils.ipynb 7
+# %% ../nbs/utils.ipynb 9
 # modified from https://github.com/thomasbrandon/mish-cuda/blob/master/test/perftest.py
 def scale_time(val:float, spec:str="#0.4G"):
     "Scale fractional second `time` values and return formatted to `spec`"
     if val == 0:
         return '-'
     PREFIXES = np.array([c for c in u"yzafpnµm kMGTPEZY"])
     exp = np.int8(np.log10(np.abs(val)) // 3 * 3 * np.sign(val))
     val /= 10.**exp
     prefix = PREFIXES[exp//3 + len(PREFIXES)//2]
     return f"{val:{spec}}{prefix}s"
 
-# %% ../nbs/utils.ipynb 8
+# %% ../nbs/utils.ipynb 10
 # From https://uploadcare.com/blog/fast-import-of-pillow-images-to-numpy-opencv-arrays/
 # Up to 2.5 times faster with the same functionality and a smaller number of allocations than numpy.asarray(img)
 def pil_to_numpy(img:Image.Image) -> np.ndarray:
     "Fast conversion of Pillow `Image` to NumPy NDArray"
     img.load()
     # unpack data
     enc = Image._getencoder(img.mode, 'raw', img.mode)
```

### Comparing `fastxtend-0.1.2/fastxtend/vision/augment/batch.py` & `fastxtend-0.1.3/fastxtend/vision/augment/batch.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/vision/augment/itemtensor.py` & `fastxtend-0.1.3/fastxtend/vision/augment/itemtensor.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/vision/data.py` & `fastxtend-0.1.3/fastxtend/vision/data.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/vision/models/attention_modules.py` & `fastxtend-0.1.3/fastxtend/vision/models/attention_modules.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/vision/models/pooling.py` & `fastxtend-0.1.3/fastxtend/vision/models/pooling.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend/vision/models/xresnet.py` & `fastxtend-0.1.3/fastxtend/vision/models/xresnet.py`

 * *Files identical despite different names*

### Comparing `fastxtend-0.1.2/fastxtend.egg-info/PKG-INFO` & `fastxtend-0.1.3/fastxtend.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastxtend
-Version: 0.1.2
+Version: 0.1.3
 Summary: Train fastai models faster (and other useful tools)
 Home-page: https://github.com/warner-benjamin/fastxtend
 Author: Benjamin Warner
 Author-email: me@benjaminwarner.dev
 License: MIT License
 Project-URL: Documentation, https://fastxtend.benjaminwarner.dev/
 Keywords: fastai pytorch extensions
@@ -49,18 +49,23 @@
 
 ## Feature overview
 
 **Train Models Faster**
 
 - Drop in [fused optimizers](optimizer.fused.html), which are 21 to 293
   percent faster then fastai native optimizers.
+- Up to 75% optimizer memory savings with integrated
+  [bitsandbytes](https://github.com/TimDettmers/bitsandbytes) [8-bit
+  optimizers](optimizer.eightbit.html).
 - Increase GPU throughput and decrease training time with the
   [Progressive Resizing](callback.progresize.html) callback.
 - Use the highly optimized [FFCV DataLoader](ffcv.tutorial.html), fully
   integrated with fastai.
+- Integrated support for `torch.compile` via the
+  [Compile](callback.compiler.html) callbacks.
 
 **General Features**
 
 - Fused implementations of modern optimizers, such as
   [Adan](optimizer.adan.html) and [Lion](optimizer.lion.html).
 - Flexible [metrics](metrics.html) which can log on train, valid, or
   both. Backwards compatible with fastai metrics.
@@ -160,19 +165,20 @@
 ```
 
 To easily install prerequisites for all fastxtend features, use
 [Conda](https://docs.conda.io/en/latest) or
 [Miniconda](https://docs.conda.io/en/latest/miniconda.html):
 
 ``` bash
-conda create -n fastxtend python=3.10 pytorch torchvision \
-torchaudio pytorch-cuda=11.8 cuda fastai nbdev pkg-config \
-libjpeg-turbo opencv tqdm terminaltables psutil numpy=1.23.5 \
-numba librosa=0.9.2 timm kornia rich typer wandb -c pytorch \
--c nvidia/label/cuda-11.8.0 -c fastai -c huggingface -c conda-forge
+conda create -n fastxtend python=3.10 "pytorch>=2.0.0" \
+torchvision torchaudio pytorch-cuda=11.8 cuda fastai nbdev \
+pkg-config libjpeg-turbo opencv tqdm terminaltables psutil \
+numpy numba librosa=0.9.2 timm kornia rich typer wandb \
+-c pytorch -c nvidia/label/cuda-11.8.0 -c fastai \
+-c huggingface -c conda-forge
 
 conda activate fastxtend
 ```
 
 replacing `pytorch-cuda=11.8` and `nvidia/label/cuda-11.8.0` with your
 preferred [supported version of
 Cuda](https://pytorch.org/get-started/locally). Then install fastxtend
@@ -232,7 +238,13 @@
 
 ``` python
 from fastxtend.callback import simpleprofiler
 
 learn = Learner(...).profile()
 learn.fit_one_cycle(2, 3e-3)
 ```
+
+## Benchmark
+
+To run the benchmark on your own machine, see the [example
+scripts](https://github.com/warner-benjamin/fastxtend/tree/main/examples)
+for details on how to replicate.
```

### Comparing `fastxtend-0.1.2/fastxtend.egg-info/SOURCES.txt` & `fastxtend-0.1.3/fastxtend.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 setup.py
 fastxtend/__init__.py
 fastxtend/_modidx.py
-fastxtend/_nbdev.py
 fastxtend/basics.py
 fastxtend/imports.py
 fastxtend/losses.py
 fastxtend/metrics.py
 fastxtend/multiloss.py
 fastxtend/patches.py
 fastxtend/schedulers.py
@@ -41,28 +40,32 @@
 fastxtend/callback/simpleprofiler.py
 fastxtend/callback/tracker.py
 fastxtend/data/__init__.py
 fastxtend/data/all.py
 fastxtend/data/transforms.py
 fastxtend/ffcv/__init__.py
 fastxtend/ffcv/all.py
+fastxtend/ffcv/epoch_iterator.py
 fastxtend/ffcv/fields.py
 fastxtend/ffcv/fx.py
 fastxtend/ffcv/inference.py
 fastxtend/ffcv/loader.py
 fastxtend/ffcv/operations.py
 fastxtend/ffcv/transforms.py
 fastxtend/ffcv/utils.py
 fastxtend/ffcv/writer.py
 fastxtend/optimizer/__init__.py
 fastxtend/optimizer/adan.py
 fastxtend/optimizer/all.py
+fastxtend/optimizer/eightbit.py
 fastxtend/optimizer/foreach.py
 fastxtend/optimizer/fused.py
 fastxtend/optimizer/lion.py
+fastxtend/optimizer/sophia.py
+fastxtend/optimizer/stableadam.py
 fastxtend/optimizer/torchscript.py
 fastxtend/vision/__init__.py
 fastxtend/vision/all.py
 fastxtend/vision/data.py
 fastxtend/vision/augment/__init__.py
 fastxtend/vision/augment/all.py
 fastxtend/vision/augment/batch.py
```

### Comparing `fastxtend-0.1.2/setup.py` & `fastxtend-0.1.3/setup.py`

 * *Files identical despite different names*

