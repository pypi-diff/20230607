# Comparing `tmp/torch_conduit-0.3.4.tar.gz` & `tmp/torch_conduit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_conduit-0.3.4.tar", max compression
+gzip compressed data, was "torch_conduit-0.3.5.tar", max compression
```

## Comparing `torch_conduit-0.3.4.tar` & `torch_conduit-0.3.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1081 2022-01-09 18:24:01.201254 torch_conduit-0.3.4/LICENSE
--rw-r--r--   0        0        0      408 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/README.md
--rw-r--r--   0        0        0       12 2022-12-18 12:46:23.375194 torch_conduit-0.3.4/conduit/__init__.py
--rw-r--r--   0        0        0     1329 2022-12-19 15:56:41.671401 torch_conduit-0.3.4/conduit/conf/configen.yaml
--rw-r--r--   0        0        0       51 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/__init__.py
--rw-r--r--   0        0        0      208 2022-12-19 15:56:41.671401 torch_conduit-0.3.4/conduit/data/constants.py
--rw-r--r--   0        0        0       20 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datamodules/__init__.py
--rw-r--r--   0        0        0       28 2022-12-18 12:46:23.247194 torch_conduit-0.3.4/conduit/data/datamodules/audio/__init__.py
--rw-r--r--   0        0        0     2558 2023-03-22 19:05:02.482581 torch_conduit-0.3.4/conduit/data/datamodules/audio/base.py
--rw-r--r--   0        0        0     2867 2023-05-04 16:42:34.589932 torch_conduit-0.3.4/conduit/data/datamodules/audio/ecoacoustics.py
--rw-r--r--   0        0        0    12126 2023-03-22 15:35:36.662964 torch_conduit-0.3.4/conduit/data/datamodules/base.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.255194 torch_conduit-0.3.4/conduit/data/datamodules/tabular/__init__.py
--rw-r--r--   0        0        0     1091 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datamodules/tabular/dummy.py
--rw-r--r--   0        0        0      186 2023-05-04 16:42:34.589932 torch_conduit-0.3.4/conduit/data/datamodules/vision/__init__.py
--rw-r--r--   0        0        0     3987 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datamodules/vision/base.py
--rw-r--r--   0        0        0     2678 2022-12-19 15:56:41.671401 torch_conduit-0.3.4/conduit/data/datamodules/vision/camelyon17.py
--rw-r--r--   0        0        0     2155 2022-12-19 15:56:41.671401 torch_conduit-0.3.4/conduit/data/datamodules/vision/celeba.py
--rw-r--r--   0        0        0     3430 2023-02-01 11:04:32.428283 torch_conduit-0.3.4/conduit/data/datamodules/vision/cmnist.py
--rw-r--r--   0        0        0     1145 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datamodules/vision/dummy.py
--rw-r--r--   0        0        0     1976 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/data/datamodules/vision/nico.py
--rw-r--r--   0        0        0     1580 2023-05-12 13:22:07.876897 torch_conduit-0.3.4/conduit/data/datamodules/vision/nico_plus_plus.py
--rw-r--r--   0        0        0     1647 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/data/datamodules/vision/pacs.py
--rw-r--r--   0        0        0     2337 2023-02-02 17:36:21.303492 torch_conduit-0.3.4/conduit/data/datamodules/vision/waterbirds.py
--rw-r--r--   0        0        0       65 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/__init__.py
--rw-r--r--   0        0        0       28 2022-12-18 12:46:23.295194 torch_conduit-0.3.4/conduit/data/datasets/audio/__init__.py
--rw-r--r--   0        0        0     2798 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/data/datasets/audio/base.py
--rw-r--r--   0        0        0    11284 2023-05-04 16:42:34.589932 torch_conduit-0.3.4/conduit/data/datasets/audio/ecoacoustics.py
--rw-r--r--   0        0        0    10725 2023-02-02 17:36:21.303492 torch_conduit-0.3.4/conduit/data/datasets/base.py
--rw-r--r--   0        0        0       41 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/tabular/__init__.py
--rw-r--r--   0        0        0     1811 2023-01-18 10:25:37.423919 torch_conduit-0.3.4/conduit/data/datasets/tabular/base.py
--rw-r--r--   0        0        0     1848 2023-05-13 18:40:52.769259 torch_conduit-0.3.4/conduit/data/datasets/tabular/dummy.py
--rw-r--r--   0        0        0    27787 2023-05-10 10:53:13.240908 torch_conduit-0.3.4/conduit/data/datasets/utils.py
--rw-r--r--   0        0        0      334 2023-05-04 16:42:34.589932 torch_conduit-0.3.4/conduit/data/datasets/vision/__init__.py
--rw-r--r--   0        0        0     4834 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/base.py
--rw-r--r--   0        0        0     6351 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/camelyon17.py
--rw-r--r--   0        0        0     5310 2023-02-25 16:39:35.362547 torch_conduit-0.3.4/conduit/data/datasets/vision/celeba.py
--rw-r--r--   0        0        0     9862 2023-04-24 19:49:50.515281 torch_conduit-0.3.4/conduit/data/datasets/vision/cmnist.py
--rw-r--r--   0        0        0     1131 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/dummy.py
--rw-r--r--   0        0        0     8944 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/fmow.py
--rw-r--r--   0        0        0    12403 2023-05-04 15:57:09.326105 torch_conduit-0.3.4/conduit/data/datasets/vision/isic.py
--rw-r--r--   0        0        0     7475 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/iwildcam.py
--rw-r--r--   0        0        0     7221 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/nico.py
--rw-r--r--   0        0        0     8274 2023-05-12 13:22:07.876897 torch_conduit-0.3.4/conduit/data/datasets/vision/nico_plus_plus.py
--rw-r--r--   0        0        0     7912 2023-02-01 11:04:32.432283 torch_conduit-0.3.4/conduit/data/datasets/vision/nih.py
--rw-r--r--   0        0        0     6291 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/pacs.py
--rw-r--r--   0        0        0     3917 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/ssrp.py
--rw-r--r--   0        0        0     3610 2023-02-01 11:04:32.432283 torch_conduit-0.3.4/conduit/data/datasets/vision/utils.py
--rw-r--r--   0        0        0       26 2023-02-02 17:36:21.303492 torch_conduit-0.3.4/conduit/data/datasets/vision/waterbirds/__init__.py
--rw-r--r--   0        0        0     5094 2023-02-02 17:36:21.303492 torch_conduit-0.3.4/conduit/data/datasets/vision/waterbirds/waterbirds.py
--rw-r--r--   0        0        0   156339 2023-02-02 17:36:21.303492 torch_conduit-0.3.4/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip
--rw-r--r--   0        0        0     2998 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/vision/wrappers.py
--rw-r--r--   0        0        0     5673 2023-01-19 16:12:52.451248 torch_conduit-0.3.4/conduit/data/datasets/wrappers.py
--rw-r--r--   0        0        0    18335 2023-05-04 16:42:34.589932 torch_conduit-0.3.4/conduit/data/structures.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.359194 torch_conduit-0.3.4/conduit/fair/__init__.py
--rw-r--r--   0        0        0       51 2022-12-18 12:46:23.343194 torch_conduit-0.3.4/conduit/fair/data/__init__.py
--rw-r--r--   0        0        0       68 2022-12-18 12:46:23.343194 torch_conduit-0.3.4/conduit/fair/data/datamodules/__init__.py
--rw-r--r--   0        0        0      214 2022-12-18 12:46:23.343194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/__init__.py
--rw-r--r--   0        0        0      692 2022-12-18 12:46:23.335194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/admissions.py
--rw-r--r--   0        0        0      814 2022-12-18 12:46:23.335194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/adult.py
--rw-r--r--   0        0        0     6015 2023-02-01 11:04:32.432283 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/base.py
--rw-r--r--   0        0        0      625 2022-12-18 12:46:23.327194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/compas.py
--rw-r--r--   0        0        0      645 2022-12-18 12:46:23.331194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/credit.py
--rw-r--r--   0        0        0      642 2022-12-18 12:46:23.323194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/crime.py
--rw-r--r--   0        0        0      606 2022-12-18 12:46:23.339194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/german.py
--rw-r--r--   0        0        0      608 2022-12-18 12:46:23.323194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/health.py
--rw-r--r--   0        0        0      573 2022-12-18 12:46:23.327194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/law.py
--rw-r--r--   0        0        0      579 2022-12-18 12:46:23.331194 torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/sqf.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.319194 torch_conduit-0.3.4/conduit/fair/data/datamodules/vision/__init__.py
--rw-r--r--   0        0        0       66 2022-12-18 12:46:23.355194 torch_conduit-0.3.4/conduit/fair/data/datasets/__init__.py
--rw-r--r--   0        0        0      974 2022-12-19 16:39:10.546686 torch_conduit-0.3.4/conduit/fair/data/datasets/dummy.py
--rw-r--r--   0        0        0     2336 2022-12-18 12:46:23.351194 torch_conduit-0.3.4/conduit/fair/data/datasets/ethicml.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.347194 torch_conduit-0.3.4/conduit/fair/data/datasets/vision/__init__.py
--rw-r--r--   0        0        0       20 2022-12-18 12:46:23.359194 torch_conduit-0.3.4/conduit/fair/losses/__init__.py
--rw-r--r--   0        0        0     1041 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/fair/losses/loss.py
--rw-r--r--   0        0        0     5992 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/hydra/conduit/data/datamodules/conf.py
--rw-r--r--   0        0        0     4195 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/hydra/conduit/data/datasets/conf.py
--rw-r--r--   0        0        0     6455 2022-12-19 15:18:44.170868 torch_conduit-0.3.4/conduit/hydra/conduit/fair/data/datamodules/conf.py
--rw-r--r--   0        0        0      457 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/hydra/conduit/models/self_supervised/loss/conf.py
--rw-r--r--   0        0        0      399 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/hydra/conduit/models/self_supervised/memory_bank/conf.py
--rw-r--r--   0        0        0      347 2022-12-18 12:46:23.375194 torch_conduit-0.3.4/conduit/logging.py
--rw-r--r--   0        0        0    21149 2023-05-12 19:05:48.407235 torch_conduit-0.3.4/conduit/metrics.py
--rw-r--r--   0        0        0       21 2022-12-18 12:46:23.383194 torch_conduit-0.3.4/conduit/models/__init__.py
--rw-r--r--   0        0        0    14963 2023-02-01 11:04:32.432283 torch_conduit-0.3.4/conduit/models/self_supervised/loss.py
--rw-r--r--   0        0        0     2386 2022-12-19 15:56:41.675401 torch_conduit-0.3.4/conduit/models/self_supervised/memory_bank.py
--rw-r--r--   0        0        0     1463 2023-04-17 21:49:37.066959 torch_conduit-0.3.4/conduit/models/utils.py
--rw-r--r--   0        0        0     9867 2023-04-17 20:52:30.804691 torch_conduit-0.3.4/conduit/progress.py
--rw-r--r--   0        0        0       64 2022-01-09 18:24:01.201254 torch_conduit-0.3.4/conduit/py.typed
--rw-r--r--   0        0        0      388 2023-04-17 21:49:37.066959 torch_conduit-0.3.4/conduit/structures.py
--rw-r--r--   0        0        0       23 2023-04-17 21:49:37.066959 torch_conduit-0.3.4/conduit/transforms/__init__.py
--rw-r--r--   0        0        0     3216 2022-12-18 12:46:23.371194 torch_conduit-0.3.4/conduit/transforms/audio.py
--rw-r--r--   0        0        0     2490 2023-02-01 11:04:32.432283 torch_conduit-0.3.4/conduit/transforms/fixmatch.py
--rw-r--r--   0        0        0     3271 2022-12-18 12:46:23.363194 torch_conduit-0.3.4/conduit/transforms/image.py
--rw-r--r--   0        0        0     8902 2023-02-01 11:04:32.432283 torch_conduit-0.3.4/conduit/transforms/multicrop.py
--rw-r--r--   0        0        0     6014 2023-01-18 10:25:37.427919 torch_conduit-0.3.4/conduit/transforms/tabular.py
--rw-r--r--   0        0        0     1606 2023-04-17 21:49:37.066959 torch_conduit-0.3.4/conduit/types.py
--rw-r--r--   0        0        0     5903 2023-05-13 18:40:56.885291 torch_conduit-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 torch_conduit-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-01-09 18:24:01.201254 torch_conduit-0.3.5/LICENSE
+-rw-r--r--   0        0        0      408 2023-01-19 16:12:52.451248 torch_conduit-0.3.5/README.md
+-rw-r--r--   0        0        0       12 2022-12-18 12:46:23.375194 torch_conduit-0.3.5/conduit/__init__.py
+-rw-r--r--   0        0        0     1329 2022-12-19 15:56:41.671401 torch_conduit-0.3.5/conduit/conf/configen.yaml
+-rw-r--r--   0        0        0       51 2023-01-19 16:12:52.451248 torch_conduit-0.3.5/conduit/data/__init__.py
+-rw-r--r--   0        0        0      208 2022-12-19 15:56:41.671401 torch_conduit-0.3.5/conduit/data/constants.py
+-rw-r--r--   0        0        0       20 2023-01-19 16:12:52.451248 torch_conduit-0.3.5/conduit/data/datamodules/__init__.py
+-rw-r--r--   0        0        0       28 2022-12-18 12:46:23.247194 torch_conduit-0.3.5/conduit/data/datamodules/audio/__init__.py
+-rw-r--r--   0        0        0     2649 2023-06-02 13:34:19.173733 torch_conduit-0.3.5/conduit/data/datamodules/audio/base.py
+-rw-r--r--   0        0        0     2955 2023-06-02 13:34:19.173733 torch_conduit-0.3.5/conduit/data/datamodules/audio/ecoacoustics.py
+-rw-r--r--   0        0        0    12273 2023-06-07 13:22:31.456823 torch_conduit-0.3.5/conduit/data/datamodules/base.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.255194 torch_conduit-0.3.5/conduit/data/datamodules/tabular/__init__.py
+-rw-r--r--   0        0        0     1178 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/tabular/dummy.py
+-rw-r--r--   0        0        0      186 2023-05-04 16:42:34.589932 torch_conduit-0.3.5/conduit/data/datamodules/vision/__init__.py
+-rw-r--r--   0        0        0     4075 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/base.py
+-rw-r--r--   0        0        0     2672 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/camelyon17.py
+-rw-r--r--   0        0        0     2153 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/celeba.py
+-rw-r--r--   0        0        0     3422 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/cmnist.py
+-rw-r--r--   0        0        0     1132 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/dummy.py
+-rw-r--r--   0        0        0     1976 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/nico.py
+-rw-r--r--   0        0        0     1578 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/nico_plus_plus.py
+-rw-r--r--   0        0        0     1647 2023-06-02 13:34:19.177733 torch_conduit-0.3.5/conduit/data/datamodules/vision/pacs.py
+-rw-r--r--   0        0        0     2331 2023-06-02 13:34:19.181733 torch_conduit-0.3.5/conduit/data/datamodules/vision/waterbirds.py
+-rw-r--r--   0        0        0       65 2023-01-19 16:12:52.451248 torch_conduit-0.3.5/conduit/data/datasets/__init__.py
+-rw-r--r--   0        0        0       28 2022-12-18 12:46:23.295194 torch_conduit-0.3.5/conduit/data/datasets/audio/__init__.py
+-rw-r--r--   0        0        0     3167 2023-06-07 13:22:31.456823 torch_conduit-0.3.5/conduit/data/datasets/audio/base.py
+-rw-r--r--   0        0        0    11362 2023-06-02 13:34:19.181733 torch_conduit-0.3.5/conduit/data/datasets/audio/ecoacoustics.py
+-rw-r--r--   0        0        0    11107 2023-06-07 13:22:31.456823 torch_conduit-0.3.5/conduit/data/datasets/base.py
+-rw-r--r--   0        0        0       41 2023-01-19 16:12:52.451248 torch_conduit-0.3.5/conduit/data/datasets/tabular/__init__.py
+-rw-r--r--   0        0        0     1837 2023-06-02 13:34:19.181733 torch_conduit-0.3.5/conduit/data/datasets/tabular/base.py
+-rw-r--r--   0        0        0     1848 2023-05-13 18:40:52.769259 torch_conduit-0.3.5/conduit/data/datasets/tabular/dummy.py
+-rw-r--r--   0        0        0    27817 2023-06-05 11:26:13.501056 torch_conduit-0.3.5/conduit/data/datasets/utils.py
+-rw-r--r--   0        0        0      334 2023-05-04 16:42:34.589932 torch_conduit-0.3.5/conduit/data/datasets/vision/__init__.py
+-rw-r--r--   0        0        0     5232 2023-06-07 13:22:31.456823 torch_conduit-0.3.5/conduit/data/datasets/vision/base.py
+-rw-r--r--   0        0        0     6350 2023-06-02 15:08:01.461330 torch_conduit-0.3.5/conduit/data/datasets/vision/camelyon17.py
+-rw-r--r--   0        0        0     5307 2023-06-02 15:08:01.461330 torch_conduit-0.3.5/conduit/data/datasets/vision/celeba.py
+-rw-r--r--   0        0        0     9870 2023-06-02 15:08:01.461330 torch_conduit-0.3.5/conduit/data/datasets/vision/cmnist.py
+-rw-r--r--   0        0        0     1173 2023-06-02 13:34:19.181733 torch_conduit-0.3.5/conduit/data/datasets/vision/dummy.py
+-rw-r--r--   0        0        0     8944 2023-06-02 13:34:19.181733 torch_conduit-0.3.5/conduit/data/datasets/vision/fmow.py
+-rw-r--r--   0        0        0    12421 2023-06-07 13:22:31.456823 torch_conduit-0.3.5/conduit/data/datasets/vision/isic.py
+-rw-r--r--   0        0        0     7475 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/data/datasets/vision/iwildcam.py
+-rw-r--r--   0        0        0     7221 2023-06-02 15:08:01.461330 torch_conduit-0.3.5/conduit/data/datasets/vision/nico.py
+-rw-r--r--   0        0        0     8275 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/data/datasets/vision/nico_plus_plus.py
+-rw-r--r--   0        0        0     7894 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/data/datasets/vision/nih.py
+-rw-r--r--   0        0        0     6355 2023-06-05 11:26:13.501056 torch_conduit-0.3.5/conduit/data/datasets/vision/pacs.py
+-rw-r--r--   0        0        0     3917 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/data/datasets/vision/ssrp.py
+-rw-r--r--   0        0        0     3610 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/data/datasets/vision/utils.py
+-rw-r--r--   0        0        0       26 2023-02-02 17:36:21.303492 torch_conduit-0.3.5/conduit/data/datasets/vision/waterbirds/__init__.py
+-rw-r--r--   0        0        0     5094 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/data/datasets/vision/waterbirds/waterbirds.py
+-rw-r--r--   0        0        0   156339 2023-02-02 17:36:21.303492 torch_conduit-0.3.5/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip
+-rw-r--r--   0        0        0     2998 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/data/datasets/vision/wrappers.py
+-rw-r--r--   0        0        0     5655 2023-06-05 11:26:13.501056 torch_conduit-0.3.5/conduit/data/datasets/wrappers.py
+-rw-r--r--   0        0        0    19096 2023-06-07 13:22:31.456823 torch_conduit-0.3.5/conduit/data/structures.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.359194 torch_conduit-0.3.5/conduit/fair/__init__.py
+-rw-r--r--   0        0        0       51 2022-12-18 12:46:23.343194 torch_conduit-0.3.5/conduit/fair/data/__init__.py
+-rw-r--r--   0        0        0       68 2022-12-18 12:46:23.343194 torch_conduit-0.3.5/conduit/fair/data/datamodules/__init__.py
+-rw-r--r--   0        0        0      214 2022-12-18 12:46:23.343194 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/__init__.py
+-rw-r--r--   0        0        0      668 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/admissions.py
+-rw-r--r--   0        0        0      790 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/adult.py
+-rw-r--r--   0        0        0     6096 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/base.py
+-rw-r--r--   0        0        0      601 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/compas.py
+-rw-r--r--   0        0        0      621 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/credit.py
+-rw-r--r--   0        0        0      618 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/crime.py
+-rw-r--r--   0        0        0      606 2022-12-18 12:46:23.339194 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/german.py
+-rw-r--r--   0        0        0      608 2022-12-18 12:46:23.323194 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/health.py
+-rw-r--r--   0        0        0      573 2022-12-18 12:46:23.327194 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/law.py
+-rw-r--r--   0        0        0      579 2022-12-18 12:46:23.331194 torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/sqf.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.319194 torch_conduit-0.3.5/conduit/fair/data/datamodules/vision/__init__.py
+-rw-r--r--   0        0        0       66 2022-12-18 12:46:23.355194 torch_conduit-0.3.5/conduit/fair/data/datasets/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-19 16:39:10.546686 torch_conduit-0.3.5/conduit/fair/data/datasets/dummy.py
+-rw-r--r--   0        0        0     2336 2022-12-18 12:46:23.351194 torch_conduit-0.3.5/conduit/fair/data/datasets/ethicml.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.347194 torch_conduit-0.3.5/conduit/fair/data/datasets/vision/__init__.py
+-rw-r--r--   0        0        0       20 2022-12-18 12:46:23.359194 torch_conduit-0.3.5/conduit/fair/losses/__init__.py
+-rw-r--r--   0        0        0     1042 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/fair/losses/loss.py
+-rw-r--r--   0        0        0     5992 2022-12-19 15:56:41.675401 torch_conduit-0.3.5/conduit/hydra/conduit/data/datamodules/conf.py
+-rw-r--r--   0        0        0     4195 2022-12-19 15:56:41.675401 torch_conduit-0.3.5/conduit/hydra/conduit/data/datasets/conf.py
+-rw-r--r--   0        0        0     6455 2022-12-19 15:18:44.170868 torch_conduit-0.3.5/conduit/hydra/conduit/fair/data/datamodules/conf.py
+-rw-r--r--   0        0        0      457 2022-12-19 15:56:41.675401 torch_conduit-0.3.5/conduit/hydra/conduit/models/self_supervised/loss/conf.py
+-rw-r--r--   0        0        0      399 2022-12-19 15:56:41.675401 torch_conduit-0.3.5/conduit/hydra/conduit/models/self_supervised/memory_bank/conf.py
+-rw-r--r--   0        0        0      347 2022-12-18 12:46:23.375194 torch_conduit-0.3.5/conduit/logging.py
+-rw-r--r--   0        0        0    21167 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/metrics.py
+-rw-r--r--   0        0        0       21 2022-12-18 12:46:23.383194 torch_conduit-0.3.5/conduit/models/__init__.py
+-rw-r--r--   0        0        0    15166 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/models/self_supervised/loss.py
+-rw-r--r--   0        0        0     2386 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/models/self_supervised/memory_bank.py
+-rw-r--r--   0        0        0     1463 2023-04-17 21:49:37.066958 torch_conduit-0.3.5/conduit/models/utils.py
+-rw-r--r--   0        0        0     9763 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/progress.py
+-rw-r--r--   0        0        0       64 2022-01-09 18:24:01.201254 torch_conduit-0.3.5/conduit/py.typed
+-rw-r--r--   0        0        0      388 2023-06-02 13:34:19.185733 torch_conduit-0.3.5/conduit/structures.py
+-rw-r--r--   0        0        0       23 2023-04-17 21:49:37.066958 torch_conduit-0.3.5/conduit/transforms/__init__.py
+-rw-r--r--   0        0        0     3216 2022-12-18 12:46:23.371194 torch_conduit-0.3.5/conduit/transforms/audio.py
+-rw-r--r--   0        0        0     2499 2023-06-02 15:08:01.465330 torch_conduit-0.3.5/conduit/transforms/fixmatch.py
+-rw-r--r--   0        0        0     3271 2022-12-18 12:46:23.363194 torch_conduit-0.3.5/conduit/transforms/image.py
+-rw-r--r--   0        0        0     8901 2023-06-05 11:26:13.501056 torch_conduit-0.3.5/conduit/transforms/multicrop.py
+-rw-r--r--   0        0        0     6089 2023-06-02 13:34:19.189733 torch_conduit-0.3.5/conduit/transforms/tabular.py
+-rw-r--r--   0        0        0     1606 2023-06-02 13:34:19.189733 torch_conduit-0.3.5/conduit/types.py
+-rw-r--r--   0        0        0     6688 2023-06-07 13:35:47.512656 torch_conduit-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2620 1970-01-01 00:00:00.000000 torch_conduit-0.3.5/PKG-INFO
```

### Comparing `torch_conduit-0.3.4/LICENSE` & `torch_conduit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/conf/configen.yaml` & `torch_conduit-0.3.5/conduit/conf/configen.yaml`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/audio/base.py` & `torch_conduit-0.3.5/conduit/data/datamodules/audio/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Base class for audio datasets."""
-from typing import Optional, TypeVar, final
+from abc import abstractmethod
+from typing import Optional, final
+from typing_extensions import override
 
 import attr
+from torch import Tensor
 import torchaudio.transforms as T  # type: ignore
-from typing_extensions import override
 
 from conduit.data.datamodules.base import CdtDataModule
+from conduit.data.datasets.audio.base import CdtAudioDataset
 from conduit.data.datasets.base import I
 from conduit.data.datasets.utils import AudioTform
-from conduit.data.datasets.wrappers import AudioTransformer, InstanceWeightedDataset
-from conduit.data.structures import SizedDataset
-from conduit.types import Stage
+from conduit.data.datasets.wrappers import AudioTransformer
+from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["CdtAudioDataModule"]
 
-D = TypeVar("D", bound=SizedDataset)
-
 
 @attr.define(kw_only=True)
-class CdtAudioDataModule(CdtDataModule[D, I]):
+class CdtAudioDataModule(CdtDataModule[AudioTransformer, I]):
     root: str = attr.field(kw_only=False)
     _train_transforms: Optional[AudioTform] = None
     _test_transforms: Optional[AudioTform] = None
 
     @property
     @final
     def train_transforms(self) -> AudioTform:
@@ -60,17 +60,19 @@
     def _default_train_transforms(self) -> T.Spectrogram:
         return T.Spectrogram()
 
     @property
     def _default_test_transforms(self) -> T.Spectrogram:
         return T.Spectrogram()
 
+    @abstractmethod
+    def _get_audio_splits(self) -> TrainValTestSplit[CdtAudioDataset[I, Tensor, Tensor]]:
+        raise NotImplementedError()
+
     @override
-    @final
-    def _setup(self, stage: Optional[Stage] = None) -> None:
-        train, val, test = self._get_splits()
-        train = AudioTransformer(train, transform=self.train_transforms)
-        if self.instance_weighting:
-            train = InstanceWeightedDataset(train)
-        self._train_data = train
-        self._val_data = AudioTransformer(val, transform=self.test_transforms)
-        self._test_data = AudioTransformer(test, transform=self.test_transforms)
+    def _get_splits(self) -> TrainValTestSplit[AudioTransformer]:
+        train, val, test = self._get_audio_splits()
+        return TrainValTestSplit(
+            train=AudioTransformer(train, transform=self.train_transforms),
+            val=AudioTransformer(val, transform=self.test_transforms),
+            test=AudioTransformer(test, transform=self.test_transforms),
+        )
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/audio/ecoacoustics.py` & `torch_conduit-0.3.5/conduit/data/datamodules/audio/ecoacoustics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Ecoacoustics data-module."""
 from typing import Any, List, Optional, Sequence
+from typing_extensions import override
 
 import attr
 from torch.utils.data import Sampler
-from typing_extensions import override
 
 from conduit.data.datasets.audio.ecoacoustics import Ecoacoustics, SoundscapeAttr
 from conduit.data.datasets.utils import AudioTform, CdtDataLoader
+from conduit.data.datasets.wrappers import AudioTransformer
 from conduit.data.structures import BinarySample, TrainValTestSplit
 from conduit.transforms.audio import Compose, Framing, LogMelSpectrogram
 
 from .base import CdtAudioDataModule
 
 __all__ = ["EcoacousticsDataModule"]
 
 
 @attr.define(kw_only=True)
-class EcoacousticsDataModule(CdtAudioDataModule[Ecoacoustics, BinarySample]):
+class EcoacousticsDataModule(CdtAudioDataModule[BinarySample]):
     """Data-module for the Ecoacoustics dataset."""
 
     segment_len: float = 15
     sample_rate: int = 48_000
     target_attrs: List[SoundscapeAttr]
 
     @staticmethod
     def _batch_converter(batch: BinarySample) -> BinarySample:
         return BinarySample(x=batch.x, y=batch.y)
 
     @override
     def make_dataloader(
         self,
-        ds: Ecoacoustics,
+        ds: AudioTransformer,
         *,
         batch_size: int,
         shuffle: bool = False,
         drop_last: bool = False,
         batch_sampler: Optional[Sampler[Sequence[int]]] = None,
     ) -> CdtDataLoader[BinarySample]:
         """Make DataLoader."""
@@ -61,24 +62,24 @@
 
     @property
     def _default_transform(self) -> Compose:
         return Compose([LogMelSpectrogram(), Framing()])
 
     @property
     @override
-    def _default_train_transforms(self) -> AudioTform:
+    def _default_train_transforms(self) -> AudioTform:  # type: ignore
         return self._default_transform
 
     @property
     @override
-    def _default_test_transforms(self) -> AudioTform:
+    def _default_test_transforms(self) -> AudioTform:  # type: ignore
         return self._default_transform
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[Ecoacoustics]:
+    def _get_audio_splits(self) -> TrainValTestSplit[Ecoacoustics]:
         all_data = Ecoacoustics(
             root=self.root,
             transform=None,  # Transform is applied in `CdtAudioDataModule._setup`
             segment_len=self.segment_len,
             target_attrs=self.target_attrs,
             sample_rate=self.sample_rate,
             download=False,
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/base.py` & `torch_conduit-0.3.5/conduit/data/datamodules/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 """Base class from which all data-modules in conduit inherit."""
 from abc import abstractmethod
 import logging
-from typing import Generic, Optional, Sequence, Tuple, TypeVar, cast, final
+from typing import Generic, Optional, Sequence, Tuple, TypeVar, Union, cast, final
+from typing_extensions import override
 
 import attr
 import pytorch_lightning as pl
 from ranzen.torch import SequentialBatchSampler, StratifiedBatchSampler, TrainingMode
 from ranzen.torch.data import num_batches_per_epoch
 import torch
 from torch.utils.data import Sampler
-from typing_extensions import override
 
 from conduit.data.datasets.base import CdtDataset
 from conduit.data.datasets.utils import (
     CdtDataLoader,
     extract_base_dataset,
     get_group_ids,
 )
 from conduit.data.datasets.wrappers import InstanceWeightedDataset
-from conduit.data.structures import (
-    Dataset,
-    NamedSample,
-    SizedDataset,
-    TrainValTestSplit,
-)
+from conduit.data.structures import Dataset, SampleBase, SizedDataset, TrainValTestSplit
 from conduit.logging import init_logger
 from conduit.types import Stage
 
 __all__ = ["CdtDataModule"]
 
 D = TypeVar("D", bound=SizedDataset)
-I = TypeVar("I", bound=NamedSample)
+I = TypeVar("I", bound=SampleBase, covariant=True)
 
 
 @attr.define(kw_only=True)
 class CdtDataModule(pl.LightningDataModule, Generic[D, I]):
     """Base DataModule for both Tabular and Vision data-modules.
 
     :param val_prop: Proportion of samples to designate as the validation split.
@@ -78,15 +73,15 @@
 
     _logger: Optional[logging.Logger] = attr.field(default=None, init=False)
 
     _train_data_base: Optional[Dataset] = attr.field(default=None, init=False)
     _val_data_base: Optional[Dataset] = attr.field(default=None, init=False)
     _test_data_base: Optional[Dataset] = attr.field(default=None, init=False)
 
-    _train_data: Optional[D] = attr.field(default=None, init=False)
+    _train_data: Union[None, D, InstanceWeightedDataset] = attr.field(default=None, init=False)
     _val_data: Optional[D] = attr.field(default=None, init=False)
     _test_data: Optional[D] = attr.field(default=None, init=False)
     _card_s: Optional[int] = attr.field(default=None, init=False)
     _card_y: Optional[int] = attr.field(default=None, init=False)
     _dim_s: Optional[torch.Size] = attr.field(default=None, init=False)
     _dim_y: Optional[torch.Size] = attr.field(default=None, init=False)
     _dim_x: Optional[Tuple[int, ...]] = attr.field(default=None, init=False)
@@ -196,37 +191,37 @@
         return self.make_dataloader(batch_size=self.eval_batch_size, ds=self.val_data)
 
     @override
     def test_dataloader(self) -> CdtDataLoader[I]:
         return self.make_dataloader(batch_size=self.eval_batch_size, ds=self.test_data)
 
     @property
-    def dim_x(self) -> Tuple[int, ...]:
+    def dim_x(self) -> Sequence[int]:
         """
         Returns the dimensions of the first input (x).
 
         :returns: Tuple containing the dimensions of the (first) input.
         """
         if self._dim_x is None:
             self._check_setup_called()
             input_size = tuple(self._train_data[0].x.shape)  # type: ignore
             self._dim_x = input_size
         return self._dim_x
 
-    def size(self) -> Tuple[int, ...]:
+    def size(self) -> Sequence[int]:
         """Alias for ``dim_x``.
 
         :returns: Tuple containing the dimensions of the (first) input.
         """
         return self.dim_x
 
     @final
     def _num_samples(self, dataset: D) -> int:
         if hasattr(dataset, "__len__"):
-            return len(dataset)
+            return len(dataset)  # type: ignore
         raise AttributeError(
             "Number of samples cannot be determined as dataset of type"
             f" '{dataset.__class__.__name__}' has no '__len__' attribute defined."
         )
 
     @property
     @final
@@ -309,14 +304,15 @@
         ...
 
     @property
     def is_set_up(self) -> bool:
         return self._train_data is not None
 
     def _setup(self, stage: Optional[Stage] = None) -> None:
+        train_data: Union[None, D, InstanceWeightedDataset]
         train_data, self._val_data, self._test_data = self._get_splits()
         if self.instance_weighting:
             train_data = InstanceWeightedDataset(train_data)
         self._train_data = train_data
 
     def _post_setup(self) -> None:
         # Make information (cardinality/dimensionality) about the dataset directly accessible through the data-module
@@ -328,12 +324,16 @@
         )
         self._test_data_base = extract_base_dataset(
             dataset=self.test_data, return_subset_indices=False
         )
 
     @override
     @final
-    def setup(self, stage: Optional[Stage] = None, force_reset: bool = False) -> None:
+    def setup(  # type: ignore
+        self,
+        stage: Optional[Stage] = None,
+        force_reset: bool = False,
+    ) -> None:
         # Only perform the setup if it hasn't already been done
         if force_reset or (not self.is_set_up):
             self._setup(stage=stage)
             self._post_setup()
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/tabular/dummy.py` & `torch_conduit-0.3.5/conduit/data/datamodules/tabular/dummy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Optional
+from typing_extensions import override
 
 import attr
-from typing_extensions import override
 
 from conduit.data import TrainValTestSplit
 from conduit.data.datamodules import CdtDataModule
 from conduit.data.datasets.tabular import RandomTabularDataset
+from conduit.data.structures import TernarySample
 
 
 @attr.define(kw_only=True)
-class DummyTabularDataModule(CdtDataModule):
+class DummyTabularDataModule(CdtDataModule[RandomTabularDataset, TernarySample]):
     num_samples: int
     num_disc_features: int
     num_cont_features: int
     seed: int = 8
     s_card: Optional[int] = None
     y_card: Optional[int] = None
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/base.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Base class for vision datasets."""
+from abc import abstractmethod
 from pathlib import Path
-from typing import List, Optional, TypeVar, Union
+from typing import List, Optional, Union, final
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 from albumentations.pytorch import ToTensorV2  # type: ignore
 import attr
-from typing_extensions import final, override
+from torch import Tensor
 
 from conduit.data.constants import IMAGENET_STATS
 from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datasets.base import I
 from conduit.data.datasets.vision import (
     AlbumentationsTform,
     ImageTform,
     ImageTransformer,
 )
-from conduit.data.datasets.wrappers import InstanceWeightedDataset
-from conduit.data.structures import ImageSize, MeanStd, SizedDataset
-from conduit.types import Stage
+from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.structures import ImageSize, MeanStd, TrainValTestSplit
 
 __all__ = ["CdtVisionDataModule"]
 
-D = TypeVar("D", bound=SizedDataset)
-
 
 @attr.define(kw_only=True)
-class CdtVisionDataModule(CdtDataModule[D, I]):
+class CdtVisionDataModule(CdtDataModule[ImageTransformer, I]):
     root: Union[str, Path] = attr.field(kw_only=False)
     _train_transforms: Optional[ImageTform] = None
     _test_transforms: Optional[ImageTform] = None
     norm_values: Optional[MeanStd] = attr.field(default=IMAGENET_STATS, init=False)
 
     @property
     @final
@@ -83,14 +82,15 @@
         """
         Returns the dimensions of the first input (x).
 
         :returns: ImageSize object containing the dimensions (C, H, W) of the (first) input.
         """
         return ImageSize(*super().dim_x)
 
+    @override
     def size(self) -> ImageSize:
         """Alias for ``dim_x``.
 
         :returns: ImageSize object containing the dimensions (C, H, W) of the (first) input.
         """
         return self.dim_x
 
@@ -98,16 +98,20 @@
     def _default_test_transforms(self) -> A.Compose:
         transform_ls: List[AlbumentationsTform] = [A.ToFloat()]
         if self.norm_values is not None:
             transform_ls.append(A.Normalize(mean=self.norm_values.mean, std=self.norm_values.std))
         transform_ls.append(ToTensorV2())
         return A.Compose(transform_ls)
 
+    @abstractmethod
+    def _get_image_splits(self) -> TrainValTestSplit[CdtVisionDataset[I, Tensor, Tensor]]:
+        raise NotImplementedError()
+
+    @final
     @override
-    def _setup(self, stage: Optional[Stage] = None) -> None:
-        train, val, test = self._get_splits()
-        train = ImageTransformer(train, transform=self.train_transforms)
-        if self.instance_weighting:
-            train = InstanceWeightedDataset(train)
-        self._train_data = train
-        self._val_data = ImageTransformer(val, transform=self.test_transforms)
-        self._test_data = ImageTransformer(test, transform=self.test_transforms)
+    def _get_splits(self) -> TrainValTestSplit[ImageTransformer]:
+        train, val, test = self._get_image_splits()
+        return TrainValTestSplit(
+            train=ImageTransformer(train, transform=self.train_transforms),
+            val=ImageTransformer(val, transform=self.test_transforms),
+            test=ImageTransformer(test, transform=self.test_transforms),
+        )
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/camelyon17.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/camelyon17.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Camelyon17 data-module."""
 from typing import Any
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 import attr
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.camelyon17 import (
     Camelyon17,
     Camelyon17Attr,
     Camelyon17Split,
     Camelyon17SplitScheme,
@@ -15,15 +15,15 @@
 )
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["Camelyon17DataModule"]
 
 
 @attr.define(kw_only=True)
-class Camelyon17DataModule(CdtVisionDataModule[Camelyon17, SampleType]):
+class Camelyon17DataModule(CdtVisionDataModule[SampleType]):
     """Data-module for the Camelyon17 dataset."""
 
     image_size: int = 96
     superclass: Camelyon17Attr = Camelyon17Attr.TUMOR
     subclass: Camelyon17Attr = Camelyon17Attr.CENTER
     use_predefined_splits: bool = False
     split_scheme: Camelyon17SplitScheme = Camelyon17SplitScheme.OFFICIAL
@@ -57,15 +57,15 @@
             ]
         )
         normalization = super()._default_train_transforms
 
         return A.Compose([base_transforms, normalization])
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[Camelyon17]:
+    def _get_image_splits(self) -> TrainValTestSplit[Camelyon17]:
         # Split the data according to the pre-defined split indices
         if self.use_predefined_splits:
             train_data, val_data, test_data = (
                 Camelyon17(root=self.root, split=split, split_scheme=self.split_scheme)
                 for split in Camelyon17Split
             )
         # Split the data randomly according to test- and val-prop
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/celeba.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/celeba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """CelebA data-module."""
 from typing import Any
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 import attr
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.celeba import (
     CelebA,
     CelebASplit,
     CelebAttr,
     SampleType,
 )
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["CelebADataModule"]
 
 
 @attr.define(kw_only=True)
-class CelebADataModule(CdtVisionDataModule[CelebA, SampleType]):
+class CelebADataModule(CdtVisionDataModule[SampleType]):
     """Data-module for the CelebA dataset."""
 
     image_size: int = 224
     superclass: CelebAttr = CelebAttr.SMILING
     subclass: CelebAttr = CelebAttr.MALE
     use_predefined_splits: bool = False
 
@@ -44,15 +44,15 @@
 
     @property
     @override
     def _default_test_transforms(self) -> A.Compose:
         return self._default_train_transforms
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[CelebA]:
+    def _get_image_splits(self) -> TrainValTestSplit[CelebA]:
         # Split the data according to the pre-defined split indices
         if self.use_predefined_splits:
             train_data, val_data, test_data = (
                 CelebA(root=self.root, superclass=self.superclass, transform=None, split=split)
                 for split in CelebASplit
             )
         # Split the data randomly according to test- and val-prop
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/cmnist.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/cmnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """ColoredMNIST data-module."""
 from functools import partial
 from typing import Any, Dict, List, Optional
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 from albumentations.pytorch.transforms import ToTensorV2  # type: ignore
 import attr
 import numpy as np
 from torchvision.datasets import MNIST  # type: ignore
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.cmnist import (
     ColoredMNIST,
     ColoredMNISTSplit,
     SampleType,
 )
 from conduit.data.structures import MeanStd, TrainValTestSplit
 
 __all__ = ["ColoredMNISTDataModule"]
 
 
 @attr.define(kw_only=True)
-class ColoredMNISTDataModule(CdtVisionDataModule[ColoredMNIST, SampleType]):
+class ColoredMNISTDataModule(CdtVisionDataModule[SampleType]):
     """Data-module for the ColoredMNIST dataset."""
 
     image_size: int = 32
     use_predefined_splits: bool = False
     # Colorization settings
     label_map: Optional[Dict[str, int]] = None
     colors: Optional[List[int]] = None
@@ -55,15 +55,15 @@
 
     @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         MNIST(root=str(self.root), download=True, train=True)
         MNIST(root=str(self.root), download=True, train=False)
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[ColoredMNIST]:
+    def _get_image_splits(self) -> TrainValTestSplit[ColoredMNIST]:
         # TODO: Add more sophisticated (e.g. biased) splits
         fact_func = partial(
             ColoredMNIST,
             root=self.root,
             background=self.background,
             black=self.black,
             greyscale=self.greyscale,
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/dummy.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Dummy data-module."""
-import attr
 from typing_extensions import override
 
+import attr
+
 from conduit.data import TrainValTestSplit
 from conduit.data.datamodules.vision import CdtVisionDataModule
 from conduit.data.datasets.vision.dummy import DummyVisionDataset, SampleType
 
 
 @attr.define(kw_only=True)
-class DummyVisionDataModule(CdtVisionDataModule[DummyVisionDataset, SampleType]):
+class DummyVisionDataModule(CdtVisionDataModule[SampleType]):
     num_samples: int = 1_000
     seed: int = 8
     root: str = ""
     height: int = 32
     width: int = 32
     channels: int = 3
     batch_size: int = 32
     s_card: int = 2
     y_card: int = 2
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[DummyVisionDataset]:
+    def _get_image_splits(self) -> TrainValTestSplit[DummyVisionDataset]:
         # Split the data randomly according to val- and test-prop
         data = DummyVisionDataset(
             channels=self.channels,
             height=self.height,
             width=self.width,
             num_samples=self.num_samples,
             s_card=self.s_card,
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/nico.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/nico.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """NICO data-module."""
 from typing import Any, Optional
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 import attr
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.utils import stratified_split
 from conduit.data.datasets.vision.nico import NICO, NicoSuperclass, SampleType
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["NICODataModule"]
 
 
 @attr.define(kw_only=True)
-class NICODataModule(CdtVisionDataModule[NICO, SampleType]):
+class NICODataModule(CdtVisionDataModule[SampleType]):
     """Data-module for the NICO dataset."""
 
     image_size: int = 224
     class_train_props: Optional[dict] = None
     superclass: NicoSuperclass = NicoSuperclass.ANIMALS
 
     @property
@@ -39,15 +39,15 @@
         return self._default_train_transforms
 
     @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         NICO(root=self.root, download=True)
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[NICO]:
+    def _get_image_splits(self) -> TrainValTestSplit[NICO]:
         all_data = NICO(root=self.root, superclass=self.superclass, transform=None)
         train_val_prop = 1 - self.test_prop
         train_val_data, test_data = stratified_split(
             all_data,
             default_train_prop=train_val_prop,
             train_props=self.class_train_props,
             seed=self.seed,
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/nico_plus_plus.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/nico_plus_plus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """NICO++ data-module."""
 from typing import Any, List, Optional
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 import attr
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision import NICOPP, NicoPPSplit, NicoPPTarget, SampleType
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["NICOPPDataModule"]
 
 
 @attr.define(kw_only=True)
-class NICOPPDataModule(CdtVisionDataModule[NICOPP, SampleType]):
+class NICOPPDataModule(CdtVisionDataModule[SampleType]):
     """Data-module for the NICO dataset."""
 
     image_size: int = 224
     superclasses: Optional[List[NicoPPTarget]] = None
 
     @property
     @override
@@ -37,14 +37,14 @@
         return self._default_train_transforms
 
     @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         pass
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[NICOPP]:
+    def _get_image_splits(self) -> TrainValTestSplit[NICOPP]:
         train_data, val_data, test_data = (
             NICOPP(root=self.root, superclasses=self.superclasses, transform=None, split=split)
             for split in NicoPPSplit
         )
 
         return TrainValTestSplit(train=train_data, val=val_data, test=test_data)
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/pacs.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/pacs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """PACS datamodule."""
 from typing import Any
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 import attr
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.pacs import PACS, SampleType
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["PACSDataModule"]
 
 
 @attr.define(kw_only=True)
-class PACSDataModule(CdtVisionDataModule[PACS, SampleType]):
+class PACSDataModule(CdtVisionDataModule[SampleType]):
     """PyTorch Lightning Datamodule for the PACS dataset."""
 
     image_size: int = 224
     target_domain: PACS.Domain = PACS.Domain.SKETCH
 
     @property
     @override
@@ -37,13 +37,13 @@
         return self._default_train_transforms
 
     @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         PACS(root=self.root, download=True)
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[PACS]:
+    def _get_image_splits(self) -> TrainValTestSplit[PACS]:
         all_data = PACS(root=self.root, domains=None, transform=None)
         train_val_data, test_data = all_data.domain_split(target_domains=self.target_domain)
         val_data, train_data = train_val_data.random_split(props=self.val_prop, seed=self.seed)
 
         return TrainValTestSplit(train=train_data, val=val_data, test=test_data)
```

### Comparing `torch_conduit-0.3.4/conduit/data/datamodules/vision/waterbirds.py` & `torch_conduit-0.3.5/conduit/data/datamodules/vision/waterbirds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Waterbirds data-module."""
 from typing import Any
+from typing_extensions import override
 
 import albumentations as A  # type: ignore
 import attr
-from typing_extensions import override
 
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.waterbirds import Waterbirds
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["WaterbirdsDataModule"]
 
 
 @attr.define(kw_only=True)
-class WaterbirdsDataModule(CdtVisionDataModule[Waterbirds, Waterbirds.SampleType]):
+class WaterbirdsDataModule(CdtVisionDataModule[Waterbirds.SampleType]):
     """Data-module for the Waterbirds dataset."""
 
     image_size: int = 224
     use_predefined_splits: bool = False
 
     @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
@@ -41,15 +41,15 @@
 
     @property
     @override
     def _default_test_transforms(self) -> A.Compose:
         return self._default_train_transforms
 
     @override
-    def _get_splits(self) -> TrainValTestSplit[Waterbirds]:
+    def _get_image_splits(self) -> TrainValTestSplit[Waterbirds]:
         # Split the data according to the pre-defined split indices
         if self.use_predefined_splits:
             train_data, val_data, test_data = (
                 Waterbirds(root=self.root, split=split) for split in Waterbirds.Split
             )
         # Split the data randomly according to test- and val-prop
         else:
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/audio/base.py` & `torch_conduit-0.3.5/conduit/data/datasets/audio/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
-from typing import List, Optional, Union, overload
+from typing import List, Literal, Optional, Sequence, Union, overload
+from typing_extensions import override
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from torch import Tensor
 import torchaudio  # type: ignore
-from typing_extensions import override
 
 from conduit.data.datasets.base import CdtDataset, I, S, Y
 from conduit.data.datasets.utils import (
     AudioLoadingBackend,
     AudioTform,
     apply_audio_transform,
     infer_al_backend,
@@ -66,20 +66,32 @@
             return torchaudio.load(self.audio_dir / _filename)[0]  # type: ignore
 
         if isinstance(index, int):
             return _load(self.audio_dir / self.x[index])
         return torch.cat([_load(filepath) for filepath in self.x[index]], dim=0)
 
     @overload
-    def _sample_x(self, index: int, *, coerce_to_tensor: bool = ...) -> Tensor:
+    def _sample_x(self, index: int, *, coerce_to_tensor: Literal[True]) -> Tensor:
+        ...
+
+    @overload
+    def _sample_x(
+        self, index: Union[List[int], slice], *, coerce_to_tensor: Literal[True]
+    ) -> Union[Tensor, Sequence[Tensor]]:
         ...
 
     @overload
-    def _sample_x(self, index: List[int], *, coerce_to_tensor: bool = ...) -> List[Tensor]:
+    def _sample_x(self, index: int, *, coerce_to_tensor: Literal[False] = ...) -> Tensor:
+        ...
+
+    @overload
+    def _sample_x(
+        self, index: Union[List[int], slice], *, coerce_to_tensor: Literal[False] = ...
+    ) -> Union[Tensor, Sequence[Tensor]]:
         ...
 
     @override
     def _sample_x(
         self, index: IndexType, *, coerce_to_tensor: bool = False
-    ) -> Union[Tensor, List[Tensor]]:
+    ) -> Union[Tensor, Sequence[Tensor]]:
         waveform = self.load_sample(index)
         return apply_audio_transform(waveform, transform=None)
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/audio/ecoacoustics.py` & `torch_conduit-0.3.5/conduit/data/datasets/audio/ecoacoustics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,42 +6,43 @@
     Zenodo. https://doi.org/10.5281/zenodo.1255218
 """
 from enum import auto
 import math
 from pathlib import Path
 import shutil
 from typing import ClassVar, Final, List, Optional, Tuple, Union
+from typing_extensions import TypeAlias, override
 import zipfile
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_categorical_dtype, is_object_dtype
 from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
 import torchaudio  # type: ignore
 from tqdm import tqdm
-from typing_extensions import TypeAlias, override
 
 from conduit.data.datasets.audio.base import CdtAudioDataset
 from conduit.data.datasets.utils import AudioTform, UrlFileInfo, download_from_url
-from conduit.data.structures import TernarySample
+from conduit.data.structures import BinarySample
+from conduit.types import IndexType
 
 __all__ = ["Ecoacoustics", "SoundscapeAttr"]
 
 
 class SoundscapeAttr(StrEnum):
     HABITAT = auto()
     SITE = auto()
     TIME = auto()
     NN = "NN"
     N0 = "N0"
 
 
-SampleType: TypeAlias = TernarySample
+SampleType: TypeAlias = BinarySample
 
 
 class Ecoacoustics(CdtAudioDataset[SampleType, Tensor, Tensor]):
     """Dataset for audio data collected in various geographic locations."""
 
     _INDICES_DIR: ClassVar[str] = "AvianID_AcousticIndices"
     _METADATA_FILENAME: ClassVar[str] = "metadata.csv"
@@ -247,15 +248,16 @@
                 )
 
         pd.DataFrame(segment_filenames, columns=["fileName", "filePath"]).to_csv(
             processed_audio_dir / "filepaths.csv", index=False
         )
 
     @override
-    def load_sample(self, index: int) -> Tensor:
+    def load_sample(self, index: IndexType) -> Tensor:
+        assert isinstance(index, int)
         path = self.audio_dir / self.x[index]
 
         # get metadata first
         metadata = torchaudio.info(path)  # type: ignore
 
         # compute number of frames to take with the real sample rate
         num_frames_segment = int(
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/base.py` & `torch_conduit-0.3.5/conduit/data/datasets/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,26 +8,27 @@
     Sequence,
     TypeVar,
     Union,
     cast,
     final,
     overload,
 )
+from typing_extensions import Self, override
 
 import numpy as np
 import numpy.typing as npt
 from ranzen.misc import gcopy
 import torch
 from torch import Tensor
-from typing_extensions import Self, override
 
 from conduit.data.structures import (
     BinarySample,
     LoadedData,
     NamedSample,
+    SampleBase,
     SizedDataset,
     SubgroupSample,
     TargetData,
     TernarySample,
     UnloadedData,
 )
 from conduit.logging import init_logger
@@ -35,15 +36,15 @@
 from conduit.types import IndexType
 
 __all__ = ["CdtDataset", "I", "S", "X", "Y"]
 
 X = TypeVar("X", bound=UnloadedData)
 S = TypeVar("S", bound=Optional[Tensor])
 Y = TypeVar("Y", bound=Optional[Tensor])
-I = TypeVar("I", bound=NamedSample)
+I = TypeVar("I", bound=SampleBase, covariant=True)
 
 
 class CdtDataset(SizedDataset, Generic[I, X, Y, S]):
     _repr_indent: ClassVar[int] = 4
     _logger: Optional[logging.Logger] = None
 
     def __init__(
@@ -77,24 +78,36 @@
     @property
     def logger(self) -> logging.Logger:
         if self._logger is None:
             self._logger = init_logger(self.__class__.__name__)
         return self._logger
 
     @overload
-    def _sample_x(self, index: IndexType, *, coerce_to_tensor: Literal[True] = ...) -> Tensor:
+    def _sample_x(self, index: int, *, coerce_to_tensor: Literal[True]) -> Tensor:
+        ...
+
+    @overload
+    def _sample_x(
+        self, index: Union[List[int], slice], *, coerce_to_tensor: Literal[True]
+    ) -> Union[Tensor, Sequence[Tensor]]:
         ...
 
     @overload
-    def _sample_x(self, index: IndexType, *, coerce_to_tensor: Literal[False] = ...) -> LoadedData:
+    def _sample_x(self, index: int, *, coerce_to_tensor: Literal[False] = ...) -> LoadedData:
+        ...
+
+    @overload
+    def _sample_x(
+        self, index: Union[List[int], slice], *, coerce_to_tensor: Literal[False] = ...
+    ) -> Union[LoadedData, Sequence[LoadedData]]:
         ...
 
     def _sample_x(
         self, index: IndexType, *, coerce_to_tensor: bool = False
-    ) -> Union[LoadedData, Tensor]:
+    ) -> Union[LoadedData, Tensor, Sequence[LoadedData]]:
         x = self.x[index]
         if coerce_to_tensor and (not isinstance(x, Tensor)):
             x = torch.as_tensor(x)
         return x
 
     def _sample_s(self, index: IndexType) -> Optional[Tensor]:
         return None if self.s is None else self.s[index]
@@ -297,15 +310,15 @@
         if (superset.y is not None) and (other.y is not None):
             superset.y = torch.cat([superset.y, other.y], dim=0)
 
         if not inplace:
             return superset
 
     @override
-    def __getitem__(self: Self, index: IndexType) -> I:
+    def __getitem__(self: Self, index: int) -> I:
         x = self._sample_x(index, coerce_to_tensor=False)
         y = self._sample_y(index)
         s = self._sample_s(index)
         # Fetch the appropriate 'Sample' class
         if y is None:
             sample = NamedSample(x=x) if s is None else SubgroupSample(x=x, s=s)
         elif s is None:
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/tabular/base.py` & `torch_conduit-0.3.5/conduit/data/datasets/tabular/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from torch.functional import Tensor
 
-from conduit.data.datasets.base import CdtDataset
+from conduit.data.datasets.base import CdtDataset, I, S, Y
 from conduit.data.structures import TargetData
 from conduit.transforms.tabular import TabularTransform
 
 __all__ = ["CdtTabularDataset"]
 
 
-class CdtTabularDataset(CdtDataset):
+class CdtTabularDataset(CdtDataset[I, Tensor, Y, S]):
     x: Tensor
 
     def __init__(
         self,
         *,
         x: Union[Tensor, npt.NDArray[np.floating], npt.NDArray[np.integer]],
         y: Optional[TargetData] = None,
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/tabular/dummy.py` & `torch_conduit-0.3.5/conduit/data/datasets/tabular/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/utils.py` & `torch_conduit-0.3.5/conduit/data/datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Type,
     TypedDict,
     TypeVar,
     Union,
     cast,
     overload,
 )
+from typing_extensions import TypeAlias, TypeGuard, Unpack
 from zipfile import BadZipFile
 
 import numpy as np
 import numpy.typing as npt
 from ranzen.misc import gcopy
 from ranzen.torch.data import Subset, prop_random_split
 import torch
@@ -41,15 +42,14 @@
 from torch.utils.data.dataloader import DataLoader, _worker_init_fn_t
 from torch.utils.data.sampler import Sampler
 from torchvision.datasets.utils import (  # type: ignore
     _detect_file_type,
     download_url,
     extract_archive,
 )
-from typing_extensions import TypeAlias, TypeGuard, Unpack
 
 from conduit.data.datasets.base import CdtDataset
 from conduit.data.structures import (
     BinarySample,
     Dataset,
     LoadedData,
     NamedSample,
@@ -277,15 +277,15 @@
         subset = _subset_from_indices(_dataset=subset, _indices=indices)
 
     return subset
 
 
 def infer_sample_cls(
     sample: Union[List[LoadedData], Tuple[LoadedData, ...], Dict[str, LoadedData], LoadedData]
-) -> Type[NamedSample]:
+) -> Type[SampleBase]:
     """ "Attempt to infer the appropriate sample class based on the length of the input."""
     if not isinstance(sample, (list, tuple, dict)) or (len(sample) == 1):
         return NamedSample
     elif len(sample) == 2:
         return BinarySample
     elif len(sample) == 3:
         return TernarySample
@@ -381,15 +381,15 @@
                 raise ValueError(
                     f"batch of type '{type(collated_batch)}' could not be automatically cast to a "
                     "'Sample' instance. Batch must be of type 'dict', 'tuple', or 'list'."
                 )
         return collated_batch
 
 
-I = TypeVar("I", bound=NamedSample)
+I = TypeVar("I", bound=SampleBase, covariant=True)
 
 
 class _DataLoaderKwargs(TypedDict, total=False):
     """Dictionary of keyword arguments used to avoid specifying the default values."""
 
     batch_size: Optional[int]
     shuffle: bool
@@ -738,17 +738,17 @@
     thresholds[1:] += id_counts.cumsum(0)[:-1].unsqueeze(-1)
 
     train_test_inds = sort_inds.tensor_split(thresholds.flatten()[:-1], dim=0)
     train_inds = perm_inds[torch.cat(train_test_inds[0::2])]
     test_inds = perm_inds[torch.cat(train_test_inds[1::2])]
 
     if as_indices:
-        return TrainTestSplit(train=train_inds.tolist(), test=test_inds.tolist())
+        return TrainTestSplit[List[int]](train=train_inds.tolist(), test=test_inds.tolist())
 
     train_data = make_subset(dataset=dataset, indices=train_inds)
     test_data = make_subset(dataset=dataset, indices=test_inds)
 
-    return TrainTestSplit(train=train_data, test=test_data)
+    return TrainTestSplit[PCD](train=train_data, test=test_data)
 
 
 def is_tensor_list(ls: List[Any]) -> TypeGuard[List[Tensor]]:
     return isinstance(ls[0], Tensor)
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/base.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from functools import reduce
 import operator
 from pathlib import Path
-from typing import List, Optional, Sequence, Union, cast, overload
+from typing import List, Literal, Optional, Sequence, Union, cast, overload
+from typing_extensions import Self, TypeAlias, override
 
 import numpy as np
 import numpy.typing as npt
 from ranzen.types import Addable
 import torch
 from torch import Tensor
-from typing_extensions import Self, TypeAlias, override
 
 from conduit.data.datasets.base import CdtDataset, I, S, Y
 from conduit.data.datasets.vision.utils import (
     ImageLoadingBackend,
     ImageTform,
     RawImage,
     apply_image_transform,
@@ -21,15 +21,15 @@
     load_image,
 )
 from conduit.data.structures import TargetData
 from conduit.types import IndexType
 
 __all__ = ["CdtVisionDataset"]
 
-ItemType: TypeAlias = Union[RawImage, Tensor, Sequence[RawImage], Sequence[Tensor]]
+ItemType: TypeAlias = Union[RawImage, Tensor]
 
 
 class CdtVisionDataset(CdtDataset[I, npt.NDArray[np.string_], Y, S]):
     def __init__(
         self,
         *,
         x: npt.NDArray[np.string_],
@@ -65,38 +65,52 @@
         return '\n'.join(lines)
 
     def _load_image(self, index: IndexType) -> RawImage:
         filepath = cast(str, self.x[index])
         return load_image(self.image_dir / filepath, backend=self._il_backend)
 
     @overload
-    def _sample_x(self, index: int, *, coerce_to_tensor: bool = ...) -> ItemType:
+    def _sample_x(self, index: int, *, coerce_to_tensor: Literal[True]) -> Tensor:
+        ...
+
+    @overload
+    def _sample_x(
+        self, index: Union[List[int], slice], *, coerce_to_tensor: Literal[True]
+    ) -> Union[Tensor, Sequence[Tensor]]:
         ...
 
     @overload
-    def _sample_x(self, index: List[int], *, coerce_to_tensor: bool = ...) -> List[ItemType]:
+    def _sample_x(self, index: int, *, coerce_to_tensor: Literal[False] = ...) -> ItemType:
+        ...
+
+    @overload
+    def _sample_x(
+        self, index: Union[List[int], slice], *, coerce_to_tensor: Literal[False] = ...
+    ) -> Union[ItemType, Sequence[ItemType]]:
         ...
 
     @override
     def _sample_x(
         self, index: IndexType, *, coerce_to_tensor: bool = False
-    ) -> Union[ItemType, List[ItemType]]:
+    ) -> Union[ItemType, Sequence[ItemType]]:
         if isinstance(index, slice):
             index = list(range(len(self)))[index]
         if isinstance(index, list):
-            sample_ls = [self._sample_x(index=i, coerce_to_tensor=coerce_to_tensor) for i in index]
+            sample_ls: List[ItemType] = [
+                self._sample_x(index=i, coerce_to_tensor=coerce_to_tensor)  # type: ignore
+                for i in index
+            ]
             elem = sample_ls[0]
             if isinstance(elem, Addable):
                 summed = reduce(operator.add, sample_ls)
                 return cast(ItemType, summed)
             if isinstance(elem, Tensor):
-                sample_ls = cast(List[Tensor], sample_ls)
-                return torch.stack(sample_ls, dim=0)
+                return torch.stack(cast(List[Tensor], sample_ls), dim=0)
             elif isinstance(sample_ls[0], np.ndarray):
-                return np.stack(sample_ls, axis=0)
+                return np.stack(cast(List[np.ndarray], sample_ls), axis=0)
             return sample_ls
 
         image = self._load_image(index)
         image = apply_image_transform(image=image, transform=self.transform)
         if coerce_to_tensor and (not isinstance(image, Tensor)):
             if isinstance(image, Sequence):
                 image = [img_to_tensor(subimage) for subimage in image]
@@ -104,14 +118,15 @@
                 image = img_to_tensor(image)
         return image
 
     @override
     def subset(
         self,
         indices: Union[List[int], npt.NDArray[np.uint64], Tensor, slice],
+        *,
         deep: bool = False,
         transform: Optional[ImageTform] = None,
     ) -> Self:
         """Create a subset of the dataset from the given indices.
 
         :param indices: The sample-indices from which to create the subset. In the case of being a
             numpy array or tensor, said array or tensor must be 0- or 1-dimensional.
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/camelyon17.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/camelyon17.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum, auto
 from pathlib import Path
 from typing import ClassVar, Optional, Union
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen.decorators import parsable
 from ranzen.misc import StrEnum
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets import UrlFileInfo, download_from_url
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
 
@@ -19,15 +19,15 @@
 
 
 class Camelyon17SplitScheme(StrEnum):
     OFFICIAL = auto()
     """Oficial split."""
 
     MIXED_TO_TEST = auto()
-    """ 
+    """
     For the mixed-to-test setting, slide 23 (corresponding to patient 042, node 3 in the
     original dataset) is moved from the test set to the training set
     """
 
 
 class Camelyon17Split(Enum):
     TRAIN = 0
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/celeba.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/celeba.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """CelebA Dataset."""
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, List, Optional, Union
+from typing_extensions import TypeAlias
 
 import numpy as np
 import pandas as pd
 from ranzen import parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
 
@@ -140,15 +140,15 @@
             )
             skiprows = (splits != self.split.value).nonzero()[0] + 2
         attrs = pd.read_csv(
             self._base_dir / "list_attr_celeba.txt",
             delim_whitespace=True,
             header=1,
             usecols=[self.superclass.value, self.subclass.value],
-            skiprows=skiprows,  # pyright: ignore
+            skiprows=skiprows,  # type: ignore
         )
 
         x = np.array(attrs.index)
         s_unmapped = torch.as_tensor(attrs[self.subclass.value].to_numpy())
         y_unmapped = torch.as_tensor(attrs[self.superclass.value].to_numpy())
         # map from {-1, 1} to {0, 1}
         s_binary = torch.div(s_unmapped + 1, 2, rounding_mode='floor')
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/cmnist.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/cmnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ColoredMNIST Dataset."""
 from enum import auto
 from pathlib import Path
 from typing import ClassVar, Dict, List, Optional, Tuple, Union, cast
+from typing_extensions import TypeAlias, override
 
-from PIL import Image
 import numpy as np
 import numpy.typing as npt
+from PIL import Image
 from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
 from torchvision.datasets import MNIST  # type: ignore
-from typing_extensions import TypeAlias, override
 
 from conduit.data.structures import TernarySample
-from conduit.types import NDArrayR
+from conduit.types import IndexType, NDArrayR
 
 from .base import CdtVisionDataset
 from .utils import ImageTform, RawImage
 
 __all__ = ["ColoredMNIST", "ColoredMNISTSplit", "MNISTColorizer"]
 
 
@@ -141,43 +141,43 @@
         return images_colorized
 
 
 def _filter_data_by_labels(
     data: Tensor,
     *,
     targets: Tensor,
-    label_map: Dict[str, int],
+    label_map: Dict[int, int],
 ) -> Tuple[Tensor, Tensor]:
     final_mask = torch.zeros_like(targets).bool()
     for old_label, new_label in label_map.items():
-        mask = targets == int(old_label)
+        mask = targets == old_label
         targets[mask] = new_label
         final_mask |= mask
     return data[final_mask], targets[final_mask]
 
 
 class ColoredMNISTSplit(StrEnum):
     TRAIN = auto()
     TEST = auto()
 
 
 SampleType: TypeAlias = TernarySample
 
 
 class ColoredMNIST(CdtVisionDataset[SampleType, Tensor, Tensor]):
-    x: npt.NDArray[np.floating]
+    x: npt.NDArray[np.uint8]
 
     @parsable
     def __init__(
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         transform: Optional[ImageTform] = None,
-        label_map: Optional[Dict[str, int]] = None,
+        label_map: Optional[Dict[int, int]] = None,
         colors: Optional[List[int]] = None,
         num_colors: int = 10,
         scale: float = 0.2,
         correlation: Optional[float] = None,
         binarize: bool = False,
         greyscale: bool = False,
         background: bool = False,
@@ -204,15 +204,15 @@
             raise ValueError(
                 "Strength of correlation between colour and targets must be between 0 and 1."
             )
         self.correlation = correlation
 
         if isinstance(self.split, ColoredMNISTSplit):
             base_dataset = MNIST(
-                root=str(root), download=download, train=self.split is ColoredMNISTSplit.train
+                root=str(root), download=download, train=self.split is ColoredMNISTSplit.TRAIN
             )
             x = base_dataset.data
             y = base_dataset.targets
         else:
             x_ls, y_ls = [], []
             for _split in ColoredMNISTSplit:
                 base_dataset = MNIST(
@@ -261,12 +261,12 @@
         x_colorized = colorizer(images=x, labels=s)
         # Convert to HWC format for compatibility with transforms
         x_colorized = x_colorized.movedim(1, -1).numpy().astype(np.uint8)
 
         super().__init__(x=x_colorized, y=y, s=s, transform=transform, image_dir=root)
 
     @override
-    def _load_image(self, index: int) -> RawImage:
+    def _load_image(self, index: IndexType) -> RawImage:
         image = self.x[index]
         if self._il_backend == "pillow":
-            image = Image.fromarray(image)
+            return Image.fromarray(image)
         return image
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/dummy.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/dummy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional
+from typing_extensions import TypeAlias, override
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias, override
 
 from conduit.data.structures import TernarySample
+from conduit.types import IndexType
 
 from .base import CdtVisionDataset
 
 SampleType: TypeAlias = TernarySample
 
 
 class DummyVisionDataset(CdtVisionDataset[SampleType, Tensor, Tensor]):
@@ -28,11 +29,11 @@
         self.width = width
         s = torch.randint(s_card, (num_samples,)) if s_card is not None else None
         y = torch.randint(y_card, (num_samples,)) if y_card is not None else None
         x = np.array([""] * num_samples)
         super().__init__(x=x, s=s, y=y, image_dir="")
 
     @override
-    def _load_image(self, index: int) -> npt.NDArray[np.uint8]:
+    def _load_image(self, index: IndexType) -> npt.NDArray[np.uint8]:
         return np.random.randint(
             0, 256, size=(self.height, self.width, self.channels), dtype="uint8"
         )
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/fmow.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/fmow.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import auto
 from pathlib import Path
 from typing import ClassVar, Optional, Union
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets.utils import UrlFileInfo, download_from_url
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/isic.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/isic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from __future__ import annotations
 from enum import auto
 from itertools import islice
 import os
 from pathlib import Path
 import shutil
 from typing import ClassVar, Iterable, Iterator, List, Optional, TypeVar, Union
+from typing_extensions import TypeAlias
 import zipfile
 
-from PIL import Image
 import pandas as pd
+from PIL import Image
 from ranzen import StrEnum, flatten_dict
 from ranzen.decorators import parsable
 import requests
 import torch
 from torch import Tensor
 from tqdm import tqdm
-from typing_extensions import TypeAlias
 
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
 
 __all__ = ["IsicAttr", "ISIC"]
@@ -169,16 +169,16 @@
                 args = ""
                 args += template_start
                 args += template_sep.join(block)
                 args += template_end
                 req = requests.get(f"{self._REST_API_URL}/image/download{args}", stream=True)
                 req.raise_for_status()
                 image_path = raw_image_dir / f"{i}.zip"
-                with open(image_path, "wb") as f:
-                    shutil.copyfileobj(req.raw, f)
+                with image_path.open("wb") as f:
+                    shutil.copyfileobj(req.raw, f)  # pyright: ignore
                 del req
                 pbar.update()
 
     def _preprocess_isic_metadata(self) -> None:
         """Preprocesses the raw ISIC metadata."""
         self._processed_dir.mkdir(exist_ok=True)
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/iwildcam.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/iwildcam.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import ClassVar, Optional, Union
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets.utils import UrlFileInfo, download_from_url
 from conduit.data.structures import SubgroupSample, TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/nico.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/nico.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """NICO Dataset."""
 from enum import auto
 from pathlib import Path
 from typing import ClassVar, List, Optional, Union, cast
+from typing_extensions import TypeAlias
 
-from PIL import Image, UnidentifiedImageError
 import pandas as pd
+from PIL import Image, UnidentifiedImageError
 from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets.utils import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/nico_plus_plus.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/nico_plus_plus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """NICO Dataset."""
 from enum import Enum, auto
 from functools import cached_property
 import json
 from pathlib import Path
 import random
 from typing import ClassVar, Dict, List, Literal, Optional, Sequence, Set, Tuple, Union
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
 
 __all__ = ["NICOPP", "NicoPPTarget", "NicoPPAttr", "NicoPPSplit"]
@@ -185,15 +185,15 @@
         if not (self._base_dir / "dg_label_id_mapping.json").exists():
             return False
         return True
 
     def _extract_metadata(self) -> None:
         self.logger.info("Generating metadata for NICO++...")
         attributes = ["autumn", "dim", "grass", "outdoor", "rock", "water"]  # 6 attrs, 60 labels
-        meta = json.load(open(self._base_dir / "dg_label_id_mapping.json", "r"))
+        meta = json.load((self._base_dir / "dg_label_id_mapping.json").open("r"))
 
         def _make_balanced_testset(
             df: pd.DataFrame, *, seed: int, num_samples_val_test: int
         ) -> pd.DataFrame:
             # each group has a test set size of (2/3 * num_samples_val_test) and a val set size of
             # (1/3 * num_samples_val_test); if total samples in original group < num_samples_val_test,
             # val/test will still be split by 1:2, but no training samples remained
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/nih.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/nih.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, Optional, Union, cast
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen import parsable, str_to_enum
 from sklearn.preprocessing import MultiLabelBinarizer
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
 
 __all__ = ["NIHChestXRays", "NIHSplit", "NIHSubgroup", "NIHTarget"]
@@ -93,15 +93,15 @@
         self,
         root: Union[Path, str],
         *,
         target: Optional[Union[NIHTarget, str]] = NIHTarget.FINDING,
         subgroup: Union[NIHSubgroup, str] = NIHSubgroup.GENDER,
         split: Optional[Union[NIHSplit, str]] = None,
         transform: Optional[ImageTform] = None,
-        num_quantiles: Optional[float] = 4,
+        num_quantiles: Optional[int] = 4,
         download: bool = True,
     ) -> None:
         """
         :param root: Root directory of the dataset.
         :param target: Attribute to set as the target attribute ('y').
         :param subgroup: Attribute to set as the subgroup attribute ('s').
         :param split: Which predefined split of the dataset to use. If ``None`` then the full
@@ -157,15 +157,15 @@
             s_pd = cast(pd.Series, pd.qcut(s_pd, q=num_quantiles))
         s_pd_le = s_pd.factorize()[0]
         s = torch.as_tensor(s_pd_le, dtype=torch.long)
 
         findings_str = self.metadata["Finding Labels"].str.split("|")
         self.encoder = MultiLabelBinarizer().fit(findings_str)
         findings_ml = pd.DataFrame(
-            self.encoder.transform(findings_str), columns=self.encoder.classes_  # type: ignore
+            self.encoder.transform(findings_str), columns=self.encoder.classes_
         )
         self.metadata = pd.concat((self.metadata, findings_ml), axis=1)
         if self.target is None:
             findings_ml.drop("No Finding", axis=1, inplace=True)
         else:
             findings_ml = findings_ml[self.target.value]
             if self.target is NIHTarget.FINDING:
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/pacs.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/pacs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """PACS Dataset."""
 from enum import auto
 from pathlib import Path
 from typing import ClassVar, List, Optional, Union
+from typing_extensions import Self, TypeAlias
 
 import numpy as np
 import pandas as pd
 from ranzen import StrEnum, parsable, str_to_enum
 import torch
 from torch import Tensor
-from typing_extensions import Self, TypeAlias
 
 from conduit.data.datasets.utils import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample, TrainTestSplit
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
 
@@ -55,14 +55,15 @@
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         transform: Optional[ImageTform] = None,
         domains: Optional[Union[Domain, str, List[Union[str, Domain]]]] = None,
     ) -> None:
+        self.domains: Union[None, PacsDomain, List[PacsDomain]]
         if isinstance(domains, str):
             self.domains = PacsDomain(domains)
         elif isinstance(domains, list):
             domains_ = [PacsDomain(elem) for elem in domains]
             self.domains = domains_
         else:
             self.domains = domains
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/ssrp.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/ssrp.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """SSRP Dataset."""
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, List, Optional, Union, cast
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen import parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets.utils import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample
 
 from .base import CdtVisionDataset
 from .utils import ImageTform
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/utils.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Utils for vision datasets."""
 from pathlib import Path
 from typing import Any, Callable, Literal, Optional, Union, get_args, overload
+from typing_extensions import TypeAlias
 
-from PIL import Image
 import albumentations as A  # type: ignore
 import cv2
 import numpy as np
 import numpy.typing as npt
+from PIL import Image
 import torch
 from torch import Tensor
 from torchvision.transforms import functional as TF  # type: ignore
-from typing_extensions import TypeAlias
 
 from conduit.data.structures import RawImage
 
 __all__ = [
     "AlbumentationsTform",
     "ImageLoadingBackend",
     "ImageTform",
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/waterbirds/waterbirds.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/waterbirds/waterbirds.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, Optional, Union
+from typing_extensions import TypeAlias
 
 import pandas as pd
 from ranzen import parsable
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
 
 from conduit.data.datasets.utils import UrlFileInfo, download_from_url
 from conduit.data.datasets.vision import CdtVisionDataset, ImageTform
 from conduit.data.structures import TernarySample
 
 __all__ = [
     "Waterbirds",
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip` & `torch_conduit-0.3.5/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/vision/wrappers.py` & `torch_conduit-0.3.5/conduit/data/datasets/vision/wrappers.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import replace
 from typing import Any, Optional, Tuple, Union
+from typing_extensions import override
 
-from PIL import Image
 import numpy as np
+from PIL import Image
 import torch
 from torch import Tensor
-from typing_extensions import override
 
 from conduit.data.datasets.utils import extract_base_dataset
 from conduit.data.datasets.vision.base import CdtVisionDataset
 from conduit.data.datasets.vision.utils import ImageTform, apply_image_transform
 from conduit.data.structures import Dataset, DatasetWrapper, RawImage, SampleBase
 
 __all__ = [
```

### Comparing `torch_conduit-0.3.4/conduit/data/datasets/wrappers.py` & `torch_conduit-0.3.5/conduit/data/datasets/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Dataset wrappers."""
 from dataclasses import is_dataclass, replace
 from typing import Any, Optional, Tuple, Union
+from typing_extensions import override
 
 from torch import Tensor
-from typing_extensions import override
 
 from conduit.data.datasets.utils import (
     AudioTform,
     apply_audio_transform,
     compute_instance_weights,
 )
 from conduit.data.structures import (
     BinarySample,
     BinarySampleIW,
     Dataset,
     DatasetWrapper,
-    NamedSample,
     SampleBase,
     SubgroupSample,
     TernarySample,
     TernarySampleIW,
     _BinarySampleMixin,
     shallow_asdict,
 )
@@ -123,15 +122,15 @@
     """Wrapper endowing datasets with instance-weights."""
 
     def __init__(self, dataset: Dataset) -> None:
         self.dataset = dataset
         self.iw = compute_instance_weights(dataset)
 
     @override
-    def __getitem__(self, index: int) -> Union[NamedSample, Tuple[Any, ...]]:
+    def __getitem__(self, index: int) -> Union[SampleBase, Tuple[Any, ...]]:
         sample = self.dataset[index]
         iw = self.iw[index]
         if isinstance(sample, (BinarySample, SubgroupSample, TernarySample)):
             return sample.add_field(iw=iw)
         elif isinstance(sample, tuple):
             if len(sample) == 2:
                 x, y = sample
```

### Comparing `torch_conduit-0.3.4/conduit/data/structures.py` & `torch_conduit-0.3.5/conduit/data/structures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Data structures."""
 from __future__ import annotations
 from abc import abstractmethod
+from collections.abc import Sequence
 from dataclasses import asdict, dataclass, field, fields, is_dataclass
 from typing import (
     Any,
     Dict,
     Generic,
     Iterable,
     Iterator,
@@ -14,24 +15,24 @@
     Tuple,
     TypeVar,
     Union,
     cast,
     overload,
     runtime_checkable,
 )
+from typing_extensions import Self, TypeAlias, override
 
-from PIL import Image
 import attr
 import numpy as np
 import numpy.typing as npt
+from PIL import Image
 from ranzen.misc import gcopy, reduce_add
 from ranzen.types import Addable
 import torch
 from torch import Tensor
-from typing_extensions import Self, TypeAlias, override
 
 from conduit.types import IndexType, Sized
 
 __all__ = [
     "BinarySample",
     "BinarySampleIW",
     "Dataset",
@@ -55,14 +56,49 @@
     "TrainValTestSplit",
     "UnloadedData",
     "concatenate_inputs",
     "shallow_asdict",
     "shallow_astuple",
 ]
 
+
+@runtime_checkable
+class InputContainer(Sized, Addable, Protocol):
+    @classmethod
+    def fromiter(cls, sequence: Iterable[Self]) -> Self:
+        """
+        Collates a sequence of container instances into a single instance.
+
+        :param sequence: Sequence of containers to be collated.
+
+        :returns: A collated container.
+        """
+        return reduce_add(sequence)
+
+    @override
+    def __len__(self) -> int:
+        """Total number of samples in the container."""
+        ...
+
+    @override
+    def __add__(self, other: Self) -> Self:
+        ...
+
+    def to(
+        self,
+        device: Optional[Union[torch.device, str]],
+        *,
+        non_blocking: bool = False,
+    ) -> Self:
+        for name, value in shallow_asdict(self).items():
+            if isinstance(value, (Tensor, InputContainer)):
+                setattr(self, name, value.to(device, non_blocking=non_blocking))
+        return self
+
+
 RawImage: TypeAlias = Union[npt.NDArray[np.integer], Image.Image]
 UnloadedData: TypeAlias = Union[
     npt.NDArray[np.floating],
     npt.NDArray[np.integer],
     npt.NDArray[np.string_],
     Tensor,
 ]
@@ -74,15 +110,15 @@
     npt.NDArray[np.string_],
     Dict[str, Tensor],
     Dict[str, Image.Image],
     Dict[str, npt.NDArray[np.floating]],
     Dict[str, npt.NDArray[np.integer]],
     Dict[str, npt.NDArray[np.string_]],
     List[Image.Image],
-    "InputContainer[X_co]",
+    InputContainer,
 ]
 IndexabledData: TypeAlias = Union[
     Tensor,
     npt.NDArray[np.floating],
     npt.NDArray[np.integer],
     npt.NDArray[np.string_],
 ]
@@ -126,50 +162,16 @@
                 x1[key] = concatenate_inputs(x1[key], value, is_batched=is_batched)  # type: ignore
             else:
                 x1[key] = value  # type: ignore
             return x1
     return x1 + x2  # type: ignore
 
 
-@runtime_checkable
-class InputContainer(Sized, Addable, Protocol[X_co]):
-    @classmethod
-    def fromiter(cls, sequence: Iterable[Self]) -> Self:
-        """
-        Collates a sequence of container instances into a single instance.
-
-        :param sequence: Sequence of containers to be collated.
-
-        :returns: A collated container.
-        """
-        return reduce_add(sequence)
-
-    @override
-    def __len__(self) -> int:
-        """Total number of samples in the container."""
-        ...
-
-    @override
-    def __add__(self, other: Self) -> Self:
-        ...
-
-    def to(
-        self,
-        device: Optional[Union[torch.device, str]],
-        *,
-        non_blocking: bool = False,
-    ) -> Self:
-        for name, value in shallow_asdict(self).items():
-            if isinstance(value, (Tensor, InputContainer)):
-                setattr(self, name, value.to(device, non_blocking=non_blocking))
-        return self
-
-
 @dataclass
-class MultiCropOutput(InputContainer[Tensor]):
+class MultiCropOutput(InputContainer):
     global_crops: List[Tensor]
     local_crops: List[Tensor] = field(default_factory=list)
 
     @property
     def all_crops(self) -> List[Tensor]:
         return self.global_crops + self.local_crops
 
@@ -200,36 +202,36 @@
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         copy.global_crops = copy.global_crops + other.global_crops
         copy.local_crops = copy.local_crops + other.local_crops
         return copy
 
 
-IS = TypeVar("IS", bound="SampleBase[IndexabledData]")
-
-
 @dataclass
-class SampleBase(InputContainer[X]):
+class SampleBase(InputContainer, Generic[X]):
     x: X
 
     @override
     def __len__(self) -> int:
         return len(self.__dataclass_fields__)
 
     @abstractmethod
-    def __iter__(self) -> Iterator[X]:
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
         ...
 
     @override
     def __add__(self, other: Self) -> Self:
+        return self._get_copy(other, is_batched=True)
+
+    def _get_copy(self, other: Self, is_batched: bool) -> Self:
         copy = gcopy(self, deep=False)
-        copy.x = concatenate_inputs(copy.x, other.x, is_batched=True)
+        copy.x = concatenate_inputs(copy.x, other.x, is_batched=is_batched)
         return copy
 
-    def astuple(self, deep: bool = False) -> Tuple[X]:
+    def astuple(self, deep: bool = False) -> Tuple[Union[X, Tensor], ...]:
         tuple_ = tuple(iter(self))
         if deep:
             tuple_ = gcopy(tuple_, deep=True)
         return tuple_
 
     def asdict(self, deep: bool = False) -> Dict[str, X]:
         if deep:
@@ -237,272 +239,284 @@
         return shallow_asdict(self)
 
     def __getitem__(self: "SampleBase[XI]", index: IndexType) -> "SampleBase[XI]":
         return gcopy(self, deep=False, x=self.x[index])
 
 
 @dataclass
-class NamedSample(SampleBase[X]):
-    @overload
-    def add_field(self, *, y: None = ..., s: None = ..., iw: None = ...) -> Self:
-        ...
+class _BinarySampleMixin:
+    y: Tensor
 
-    @overload
-    def add_field(self, *, y: Tensor = ..., s: None = ..., iw: None = ...) -> "BinarySample":
-        ...
+    def _add_to_y(self, other: Self) -> None:
+        self.y = torch.cat([self.y, other.y], dim=0)
 
-    @overload
-    def add_field(self, *, y: Tensor = ..., s: None = ..., iw: Tensor = ...) -> "BinarySampleIW":
-        ...
 
-    @overload
-    def add_field(self, *, y: Tensor = ..., s: Tensor = ..., iw: None = ...) -> "TernarySample":
-        ...
+@dataclass
+class _SubgroupSampleMixin:
+    s: Tensor
 
-    @overload
-    def add_field(self, *, y: Tensor = ..., s: Tensor = ..., iw: Tensor = ...) -> "TernarySampleIW":
-        ...
+    def _add_to_s(self, other: Self) -> None:
+        self.s = torch.cat([self.s, other.s], dim=0)
 
-    def add_field(
-        self, y: Optional[Tensor] = None, s: Optional[Tensor] = None, iw: Optional[Tensor] = None
-    ) -> Union[Self, "BinarySample", "BinarySampleIW", "TernarySample", "TernarySampleIW"]:
-        if y is not None:
-            if s is not None:
-                if iw is not None:
-                    return TernarySampleIW(x=self.x, s=s, y=y, iw=iw)
-                return TernarySample(x=self.x, s=s, y=y)
-            if iw is not None:
-                return BinarySampleIW(x=self.x, y=y, iw=iw)
-            return BinarySample(x=self.x, y=y)
-        return self
 
-    @override
-    def __iter__(self) -> Iterator[X]:
-        yield self.x
+@dataclass
+class _IwMixin:
+    iw: Tensor
 
-    @override
-    def __getitem__(self: "NamedSample[XI]", index: IndexType) -> "NamedSample[XI]":
-        return gcopy(self, deep=False, x=self.x[index])
+    def _add_to_iw(self, other: Self) -> None:
+        self.iw = torch.cat([self.iw, other.iw], dim=0)
 
 
 @dataclass
-class _BinarySampleMixin:
-    y: Tensor
-
+class TernarySampleIW(_IwMixin, _BinarySampleMixin, _SubgroupSampleMixin, SampleBase[X]):
+    def add_field(self) -> Self:
+        return self
 
-@dataclass
-class _SubgroupSampleMixin:
-    s: Tensor
+    @override
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
+        yield from (self.x, self.y, self.s, self.iw)
 
+    @override
+    def __add__(self, other: Self) -> Self:
+        copy = self._get_copy(other, is_batched=len(self.y) > 1)
+        copy._add_to_y(other)
+        copy._add_to_s(other)
+        copy._add_to_iw(other)
+        return copy
 
-@dataclass
-class BinarySample(NamedSample[X], _BinarySampleMixin):
-    @overload
-    def add_field(self, *, s: None = ..., iw: None = ...) -> Self:
-        ...
+    @override
+    def __getitem__(self: "TernarySampleIW[XI]", index: IndexType) -> "TernarySampleIW[XI]":
+        return gcopy(
+            self, deep=False, x=self.x[index], y=self.y[index], s=self.s[index], iw=self.iw[index]
+        )
 
-    @overload
-    def add_field(self, *, s: None = ..., iw: Tensor = ...) -> "BinarySampleIW":
-        ...
 
+@dataclass
+class TernarySample(_BinarySampleMixin, _SubgroupSampleMixin, SampleBase[X]):
     @overload
-    def add_field(self, *, s: Tensor = ..., iw: None = ...) -> "TernarySample":
+    def add_field(self, iw: None = ...) -> Self:
         ...
 
     @overload
-    def add_field(self, *, s: Tensor = ..., iw: Tensor = ...) -> "TernarySampleIW":
+    def add_field(self, iw: Tensor) -> TernarySampleIW:
         ...
 
-    def add_field(
-        self, *, s: Optional[Tensor] = None, iw: Optional[Tensor] = None
-    ) -> Union[Self, "BinarySampleIW", "TernarySample", "TernarySampleIW"]:
-        if s is not None:
-            if iw is not None:
-                return TernarySampleIW(x=self.x, s=s, y=self.y, iw=iw)
-            return TernarySample(x=self.x, s=s, y=self.y)
+    def add_field(self, iw: Optional[Tensor] = None) -> Union[Self, TernarySampleIW]:
         if iw is not None:
-            return BinarySampleIW(x=self.x, y=self.y, iw=iw)
+            return TernarySampleIW(x=self.x, s=self.s, y=self.y, iw=iw)
         return self
 
     @override
-    def __iter__(self) -> Iterator[LoadedData]:  # type: ignore
-        yield from (self.x, self.y)
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
+        yield from (self.x, self.y, self.s)
 
     @override
     def __add__(self, other: Self) -> Self:
-        copy = gcopy(self, deep=False)
-        copy.y = torch.cat([copy.y, other.y], dim=0)
-        copy.x = concatenate_inputs(copy.x, other.x, is_batched=len(copy.y) > 1)
+        copy = self._get_copy(other, is_batched=len(self.y) > 1)
+        copy._add_to_y(other)
+        copy._add_to_s(other)
         return copy
 
     @override
-    def __getitem__(self: "BinarySample[XI]", index: IndexType) -> "BinarySample[XI]":
-        return gcopy(self, deep=False, x=self.x[index], y=self.y[index])
+    def __getitem__(self: "TernarySample[XI]", index: IndexType) -> "TernarySample[XI]":
+        return gcopy(self, deep=False, x=self.x[index], y=self.y[index], s=self.s[index])
 
 
 @dataclass
-class SubgroupSample(NamedSample[X], _SubgroupSampleMixin):
-    @overload
-    def add_field(self, *, y: None = ..., iw: None = ...) -> Self:
-        ...
-
+class BinarySampleIW(_IwMixin, _BinarySampleMixin, SampleBase[X]):
     @overload
-    def add_field(self, *, y: None = ..., iw: Tensor = ...) -> "SubgroupSampleIW":
-        ...
-
-    @overload
-    def add_field(self, *, y: Tensor = ..., iw: None = ...) -> "TernarySample":
+    def add_field(self, s: None = ...) -> Self:
         ...
 
     @overload
-    def add_field(self, *, y: Tensor = ..., iw: Tensor = ...) -> "TernarySampleIW":
+    def add_field(self, s: Tensor) -> TernarySampleIW:
         ...
 
-    def add_field(
-        self, *, y: Optional[Tensor] = None, iw: Optional[Tensor] = None
-    ) -> Union[Self, "SubgroupSampleIW", "TernarySample", "TernarySampleIW"]:
-        if y is not None:
-            if iw is not None:
-                return TernarySampleIW(x=self.x, s=self.s, y=y, iw=iw)
-            return TernarySample(x=self.x, s=self.s, y=y)
-        if iw is not None:
-            return SubgroupSampleIW(x=self.x, s=self.s, iw=iw)
+    def add_field(self, s: Optional[Tensor] = None) -> Union[Self, TernarySampleIW]:
+        if s is not None:
+            return TernarySampleIW(x=self.x, s=s, y=self.y, iw=self.iw)
         return self
 
     @override
-    def __iter__(self) -> Iterator[LoadedData]:  # type: ignore
-        yield from (self.x, self.s)
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
+        yield from (self.x, self.y, self.iw)
 
     @override
     def __add__(self, other: Self) -> Self:
-        copy = gcopy(self, deep=False)
-        copy.s = torch.cat([copy.s, other.s], dim=0)
-        copy.x = concatenate_inputs(copy.x, other.x, is_batched=len(copy.s) > 1)
+        copy = self._get_copy(other, is_batched=len(self.y) > 1)
+        copy._add_to_y(other)
+        copy._add_to_iw(other)
         return copy
 
     @override
-    def __getitem__(self: "SubgroupSample[XI]", index: IndexType) -> "SubgroupSample[XI]":
-        return gcopy(self, deep=False, x=self.x[index], s=self.s[index])
+    def __getitem__(self: "BinarySampleIW[XI]", index: IndexType) -> "BinarySampleIW[XI]":
+        return gcopy(self, deep=False, x=self.x[index], y=self.y[index], iw=self.iw[index])
 
 
 @dataclass
-class _IwMixin:
-    iw: Tensor
+class BinarySample(_BinarySampleMixin, SampleBase[X]):
+    @overload
+    def add_field(self, *, s: None = ..., iw: None = ...) -> Self:
+        ...
 
+    @overload
+    def add_field(self, *, s: None = ..., iw: Tensor) -> BinarySampleIW:
+        ...
 
-@dataclass
-class BinarySampleIW(BinarySample[X], _BinarySampleMixin, _IwMixin):
     @overload
-    def add_field(self, s: None = ...) -> Self:
+    def add_field(self, *, s: Tensor, iw: None = ...) -> TernarySample:
         ...
 
     @overload
-    def add_field(self, s: Tensor = ...) -> "TernarySampleIW":
+    def add_field(self, *, s: Tensor, iw: Tensor) -> TernarySampleIW:
         ...
 
-    def add_field(self, s: Optional[Tensor] = None) -> Union[Self, "TernarySampleIW"]:
+    def add_field(
+        self, *, s: Optional[Tensor] = None, iw: Optional[Tensor] = None
+    ) -> Union[Self, BinarySampleIW, TernarySample, TernarySampleIW]:
         if s is not None:
-            return TernarySampleIW(x=self.x, s=s, y=self.y, iw=self.iw)
+            if iw is not None:
+                return TernarySampleIW(x=self.x, s=s, y=self.y, iw=iw)
+            return TernarySample(x=self.x, s=s, y=self.y)
+        if iw is not None:
+            return BinarySampleIW(x=self.x, y=self.y, iw=iw)
         return self
 
     @override
-    def __iter__(self) -> Iterator[LoadedData]:
-        yield from (self.x, self.y, self.iw)
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
+        yield from (self.x, self.y)
 
     @override
     def __add__(self, other: Self) -> Self:
-        copy = super().__add__(other)
-        copy.iw = torch.cat([copy.iw, other.iw], dim=0)
+        copy = self._get_copy(other, is_batched=len(self.y) > 1)
+        copy._add_to_y(other)
         return copy
 
     @override
-    def __getitem__(self: "BinarySampleIW[XI]", index: IndexType) -> "BinarySampleIW[XI]":
-        return gcopy(self, deep=False, x=self.x[index], y=self.y[index], iw=self.iw[index])
+    def __getitem__(self: "BinarySample[XI]", index: IndexType) -> "BinarySample[XI]":
+        return gcopy(self, deep=False, x=self.x[index], y=self.y[index])
 
 
 @dataclass
-class SubgroupSampleIW(SubgroupSample[X], _IwMixin):
+class SubgroupSampleIW(SampleBase[X], _SubgroupSampleMixin, _IwMixin):
     @overload
     def add_field(self, y: None = ...) -> Self:
         ...
 
     @overload
-    def add_field(self, y: Tensor = ...) -> "TernarySampleIW":
+    def add_field(self, y: Tensor) -> TernarySampleIW:
         ...
 
-    def add_field(self, y: Optional[Tensor] = None) -> Union[Self, "TernarySampleIW"]:
+    def add_field(self, y: Optional[Tensor] = None) -> Union[Self, TernarySampleIW]:
         if y is not None:
             return TernarySampleIW(x=self.x, s=self.s, y=y, iw=self.iw)
         return self
 
     @override
-    def __iter__(self) -> Iterator[LoadedData]:
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
         yield from (self.x, self.s, self.iw)
 
     @override
     def __add__(self, other: Self) -> Self:
-        copy = super().__add__(other)
-        copy.iw = torch.cat([copy.iw, other.iw], dim=0)
+        copy = self._get_copy(other, is_batched=len(self.s) > 1)
+        copy._add_to_s(other)
+        copy._add_to_iw(other)
         return copy
 
     @override
     def __getitem__(self: "SubgroupSampleIW[XI]", index: IndexType) -> "SubgroupSampleIW[XI]":
         return gcopy(self, deep=False, x=self.x[index], s=self.s[index], iw=self.iw[index])
 
 
 @dataclass
-class TernarySample(BinarySample[X], _SubgroupSampleMixin):
+class SubgroupSample(_SubgroupSampleMixin, SampleBase[X]):
     @overload
-    def add_field(self, iw: None = ...) -> Self:
+    def add_field(self, *, y: None = ..., iw: None = ...) -> Self:
+        ...
+
+    @overload
+    def add_field(self, *, y: None = ..., iw: Tensor) -> SubgroupSampleIW:
         ...
 
     @overload
-    def add_field(self, iw: Tensor) -> Self:
+    def add_field(self, *, y: Tensor, iw: None = ...) -> TernarySample:
         ...
 
-    def add_field(self, iw: Optional[Tensor] = None) -> Union[Self, "TernarySampleIW"]:
+    @overload
+    def add_field(self, *, y: Tensor, iw: Tensor) -> TernarySampleIW:
+        ...
+
+    def add_field(
+        self, *, y: Optional[Tensor] = None, iw: Optional[Tensor] = None
+    ) -> Union[Self, SubgroupSampleIW, TernarySample, TernarySampleIW]:
+        if y is not None:
+            if iw is not None:
+                return TernarySampleIW(x=self.x, s=self.s, y=y, iw=iw)
+            return TernarySample(x=self.x, s=self.s, y=y)
         if iw is not None:
-            return TernarySampleIW(x=self.x, s=self.s, y=self.y, iw=iw)
+            return SubgroupSampleIW(x=self.x, s=self.s, iw=iw)
         return self
 
     @override
-    def __iter__(self) -> Iterator[LoadedData]:
-        yield from (self.x, self.y, self.s)
+    def __iter__(self) -> Iterator[Union[X, Tensor]]:
+        yield from (self.x, self.s)
 
     @override
     def __add__(self, other: Self) -> Self:
-        copy = super().__add__(other)
-        copy.s = torch.cat([copy.s, other.s], dim=0)
+        copy = self._get_copy(other, is_batched=len(self.s) > 1)
+        copy._add_to_s(other)
         return copy
 
     @override
-    def __getitem__(self: "TernarySample[XI]", index: IndexType) -> "TernarySample[XI]":
-        return gcopy(self, deep=False, x=self.x[index], y=self.y[index], s=self.s[index])
+    def __getitem__(self: "SubgroupSample[XI]", index: IndexType) -> "SubgroupSample[XI]":
+        return gcopy(self, deep=False, x=self.x[index], s=self.s[index])
 
 
 @dataclass
-class TernarySampleIW(TernarySample[X], _IwMixin):
-    def add_field(self) -> Self:
-        return self
+class NamedSample(SampleBase[X]):
+    @overload
+    def add_field(self, *, y: None = ..., s: None = ..., iw: None = ...) -> Self:
+        ...
 
-    @override
-    def __iter__(self) -> Iterator[LoadedData]:
-        yield from (self.x, self.y, self.s, self.iw)
+    @overload
+    def add_field(self, *, y: Tensor, s: None = ..., iw: None = ...) -> BinarySample:
+        ...
+
+    @overload
+    def add_field(self, *, y: Tensor, s: None = ..., iw: Tensor) -> BinarySampleIW:
+        ...
+
+    @overload
+    def add_field(self, *, y: Tensor, s: Tensor, iw: None = ...) -> TernarySample:
+        ...
+
+    @overload
+    def add_field(self, *, y: Tensor, s: Tensor, iw: Tensor) -> TernarySampleIW:
+        ...
+
+    def add_field(
+        self, *, y: Optional[Tensor] = None, s: Optional[Tensor] = None, iw: Optional[Tensor] = None
+    ) -> Union[Self, BinarySample, BinarySampleIW, TernarySample, TernarySampleIW]:
+        if y is not None:
+            if s is not None:
+                if iw is not None:
+                    return TernarySampleIW(x=self.x, s=s, y=y, iw=iw)
+                return TernarySample(x=self.x, s=s, y=y)
+            if iw is not None:
+                return BinarySampleIW(x=self.x, y=y, iw=iw)
+            return BinarySample(x=self.x, y=y)
+        return self
 
     @override
-    def __add__(self, other: Self) -> Self:
-        copy = super().__add__(other)
-        copy.iw = torch.cat([copy.iw, other.iw], dim=0)
-        return copy
+    def __iter__(self) -> Iterator[X]:
+        yield self.x
 
     @override
-    def __getitem__(self: "TernarySampleIW[XI]", index: IndexType) -> "TernarySampleIW[XI]":
-        return gcopy(
-            self, deep=False, x=self.x[index], y=self.y[index], s=self.s[index], iw=self.iw[index]
-        )
+    def __getitem__(self: "NamedSample[XI]", index: IndexType) -> "NamedSample[XI]":
+        return gcopy(self, deep=False, x=self.x[index])
 
 
 def shallow_astuple(dataclass: object) -> Tuple[Any, ...]:
     """dataclasses.astuple() but without the deep-copying/recursion." """
     if not is_dataclass(dataclass):
         raise TypeError("shallow_astuple() should be called on dataclass instances")
     return tuple(getattr(dataclass, field.name) for field in fields(dataclass))
@@ -512,15 +526,15 @@
     """dataclasses.asdict() but without the deep-copying/recursion." """
     if not is_dataclass(dataclass):
         raise TypeError("shallow_asdict() should be called on dataclass instances")
     return {field.name: getattr(dataclass, field.name) for field in fields(dataclass)}
 
 
 @attr.define
-class ImageSize:
+class ImageSize(Sequence):
     c: int
     h: int
     w: int
 
     def __mul__(self, other: Union[Self, float]) -> Self:
         copy = gcopy(self, deep=False)
         if isinstance(other, float):
@@ -532,14 +546,28 @@
             copy.h *= other.h
             copy.w *= other.w
         return copy
 
     def __iter__(self) -> Iterator[int]:
         yield from (self.c, self.h, self.w)
 
+    @overload
+    def __getitem__(self, index: int) -> int:
+        ...
+
+    @overload
+    def __getitem__(self, index: slice) -> Sequence[int]:
+        ...
+
+    def __getitem__(self, index: Union[int, slice]) -> Union[int, Sequence[int]]:
+        return (self.c, self.h, self.w)[index]
+
+    def __len__(self) -> int:
+        return 3
+
     @property
     def numel(self) -> int:
         return sum(iter(self))
 
 
 @attr.define(kw_only=True)
 class MeanStd:
@@ -581,15 +609,15 @@
 @runtime_checkable
 class SizedDataset(Dataset[R_co], Sized, Protocol):
     @override
     def __getitem__(self, index: int) -> R_co:
         ...
 
     @override
-    def __len__(self) -> Optional[int]:
+    def __len__(self) -> Optional[int]:  # type: ignore
         ...
 
 
 X2 = TypeVar("X2", bound=UnloadedData)
 Y = TypeVar("Y", Tensor, None)
 S = TypeVar("S", Tensor, None)
 
@@ -603,29 +631,29 @@
     def __getitem__(self, index: int) -> R_co:
         ...
 
     def __len__(self) -> int:
         ...
 
 
-D = TypeVar("D", bound=Union[Dataset, Tensor, List[int]])
+D = TypeVar("D", bound=Union[Dataset, Tensor, List[int]], covariant=True)
 
 
 @runtime_checkable
 class DatasetWrapper(SizedDataset[R_co], Protocol):
     dataset: Dataset
 
     @override
     def __getitem__(self, index: int) -> R_co:
         ...
 
     @override
     def __len__(self) -> Optional[int]:
         if isinstance(self.dataset, SizedDataset):
-            return len(self.dataset)
+            return len(self.dataset)  # type: ignore
         return None
 
 
 @attr.define(kw_only=True)
 class TrainTestSplit(Generic[D]):
     train: D
     test: D
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/admissions.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/admissions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Admissions Dataset."""
 import attr
-from ethicml.data import Admissions
+from ethicml.data import Admissions, Dataset
 from ethicml.data import AdmissionsSplits as AdmissionsSens
-from ethicml.data import Dataset
 
 from conduit.fair.data.datamodules.tabular.base import EthicMlDataModule
 
 __all__ = ["AdmissionsDataModule", "AdmissionsSens"]
 
 
 @attr.define(kw_only=True)
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/adult.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/adult.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Adult Income Dataset."""
 import attr
-from ethicml.data import Adult
+from ethicml.data import Adult, Dataset
 from ethicml.data import AdultSplits as AdultSens
-from ethicml.data import Dataset
 
 from conduit.fair.data.datamodules.tabular.base import EthicMlDataModule
 
 __all__ = ["AdultDataModule", "AdultSens"]
 
 
 @attr.define(kw_only=True)
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/base.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Tabular data-module."""
 from abc import abstractmethod
-from typing import Dict, List, Optional, Union, cast
+from typing import Dict, List, Optional, Union, cast, final
+from typing_extensions import override
 
 import attr
 import ethicml as em
 from ethicml.data import Dataset, FeatureOrder
 from sklearn.preprocessing import StandardScaler
-from typing_extensions import final, override
+from torch import Tensor
 
 from conduit.data.datamodules import CdtDataModule
-from conduit.data.structures import TrainValTestSplit
+from conduit.data.structures import TernarySample, TrainValTestSplit
 from conduit.fair.data.datasets import DataTupleDataset
 
 __all__ = ["EthicMlDataModule"]
 
 
 @attr.define(kw_only=True)
-class EthicMlDataModule(CdtDataModule):
+class EthicMlDataModule(CdtDataModule[DataTupleDataset, TernarySample[Tensor]]):
     """Base data-module for tabular datasets."""
 
     scaler: em.ScalerType = attr.field(factory=StandardScaler)
     invert_s: bool = False
     _datatuple: Optional[em.DataTuple] = attr.field(default=None, init=False)
     _train_datatuple: Optional[em.DataTuple] = attr.field(default=None, init=False)
     _val_datatuple: Optional[em.DataTuple] = attr.field(default=None, init=False)
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/compas.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/compas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """COMPAS Dataset."""
 import attr
-from ethicml.data import Compas
+from ethicml.data import Compas, Dataset
 from ethicml.data import CompasSplits as CompasSens
-from ethicml.data import Dataset
 
 from conduit.fair.data.datamodules.tabular.base import EthicMlDataModule
 
 __all__ = ["CompasDataModule", "CompasSens"]
 
 
 @attr.define(kw_only=True)
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/credit.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/credit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Credit Dataset."""
 import attr
-from ethicml.data import Credit
+from ethicml.data import Credit, Dataset
 from ethicml.data import CreditSplits as CreditSens
-from ethicml.data import Dataset
 
 from conduit.fair.data.datamodules.tabular.base import EthicMlDataModule
 
 __all__ = ["CreditDataModule", "CreditSens"]
 
 
 @attr.define(kw_only=True)
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/crime.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/crime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Crime Dataset."""
 import attr
-from ethicml.data import Crime
+from ethicml.data import Crime, Dataset
 from ethicml.data import CrimeSplits as CrimeSens
-from ethicml.data import Dataset
 
 from conduit.fair.data.datamodules.tabular.base import EthicMlDataModule
 
 __all__ = ["CrimeDataModule", "CrimeSens"]
 
 
 @attr.define(kw_only=True)
```

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/german.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/german.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/health.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/health.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/law.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/law.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datamodules/tabular/sqf.py` & `torch_conduit-0.3.5/conduit/fair/data/datamodules/tabular/sqf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datasets/dummy.py` & `torch_conduit-0.3.5/conduit/fair/data/datasets/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/fair/data/datasets/ethicml.py` & `torch_conduit-0.3.5/conduit/fair/data/datasets/ethicml.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/fair/losses/loss.py` & `torch_conduit-0.3.5/conduit/fair/losses/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from torch import Tensor, nn
 from typing_extensions import override
 
+from torch import Tensor, nn
+
 from conduit.types import Loss
 
 __all__ = ["OnlineReweightingLoss"]
 
 
 class OnlineReweightingLoss(nn.Module):
     """Wrapper that computes a loss balanced by intersectional group size."""
```

### Comparing `torch_conduit-0.3.4/conduit/hydra/conduit/data/datamodules/conf.py` & `torch_conduit-0.3.5/conduit/hydra/conduit/data/datamodules/conf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/hydra/conduit/data/datasets/conf.py` & `torch_conduit-0.3.5/conduit/hydra/conduit/data/datasets/conf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/hydra/conduit/fair/data/datamodules/conf.py` & `torch_conduit-0.3.5/conduit/hydra/conduit/fair/data/datamodules/conf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/metrics.py` & `torch_conduit-0.3.5/conduit/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     :returns: The score(s) as determined by the :attr:`comparator` and :attr:`aggregator`.
 
     :raises ValueError: If ``y_pred``, ``y_true``, and ``s`` do not match in size at dimension 0
         (the 'batch' dimension).
     """
     y_pred = y_pred.squeeze()
     y_true = y_true.squeeze()
-    index_set = None
+    index_set: Optional[Tensor] = None
 
     if group_ids:
         group_ids_ls = list(group_ids)
         first_elem = group_ids_ls.pop().clone().squeeze()
         index_set = first_elem.unique(return_inverse=True)[1]
 
         for elem in group_ids_ls:
```

### Comparing `torch_conduit-0.3.4/conduit/models/self_supervised/loss.py` & `torch_conduit-0.3.5/conduit/models/self_supervised/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from enum import Enum
-from typing import Callable, Optional, TypeVar, Union, cast
+from typing import Callable, Optional, Protocol, TypeVar, Union, cast
+from typing_extensions import Self
 
 import torch
 from torch import Tensor
 from torch.autograd.function import Function, NestedIOFunction
 import torch.distributed
 import torch.nn as nn
 import torch.nn.functional as F
-from typing_extensions import Self
 
 __all__ = [
     "DecoupledContrastiveLoss",
     "SupConReduction",
     "decoupled_contrastive_loss",
     "moco_v2_loss",
     "simclr_loss",
     "soft_supcon_loss",
     "supcon_loss",
 ]
 
 
+class _BatchStore(Protocol):
+    batch_size: int
+
+
 class _Synchronize(Function):
     @staticmethod
-    def forward(ctx: NestedIOFunction, tensor: Tensor) -> Tensor:
-        ctx.batch_size = tensor.shape[0]
+    def forward(ctx: NestedIOFunction, tensor: Tensor) -> Tensor:  # type: ignore
+        context = cast(_BatchStore, ctx)
+        context.batch_size = tensor.shape[0]
 
         gathered_tensor = [
             torch.zeros_like(tensor) for _ in range(torch.distributed.get_world_size())
         ]
 
         torch.distributed.all_gather(gathered_tensor, tensor)
         gathered_tensor = torch.cat(gathered_tensor, dim=0)
 
         return gathered_tensor
 
     @staticmethod
-    def backward(ctx: NestedIOFunction, grad_output: Tensor) -> Tensor:
+    def backward(ctx: NestedIOFunction, grad_output: Tensor) -> Tensor:  # type: ignore
+        context = cast(_BatchStore, ctx)
         grad_input = grad_output.clone()
         torch.distributed.all_reduce(grad_input, op=torch.distributed.ReduceOp.SUM, async_op=False)
-        idx_from = torch.distributed.get_rank() * ctx.batch_size
-        idx_to = (torch.distributed.get_rank() + 1) * ctx.batch_size
+        idx_from = torch.distributed.get_rank() * context.batch_size
+        idx_to = (torch.distributed.get_rank() + 1) * context.batch_size
         return grad_input[idx_from:idx_to]
 
 
 def maybe_synchronize(input: Tensor) -> Tensor:
     if torch.distributed.is_available() and torch.distributed.is_initialized():
-        return _Synchronize.apply(input)
+        return _Synchronize.apply(input)  # type: ignore
     return input
 
 
 def logsumexp(
     input: Tensor, *, dim: int, keepdim: bool = False, keep_mask: Optional[Tensor] = None
 ) -> Tensor:
     """Numerically stable implementation of logsumexp that allows for masked summation."""
```

### Comparing `torch_conduit-0.3.4/conduit/models/self_supervised/memory_bank.py` & `torch_conduit-0.3.5/conduit/models/self_supervised/memory_bank.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Type
+from typing_extensions import Self, override
 
 import torch
 from torch import Tensor, nn
 import torch.nn.functional as F
-from typing_extensions import Self, override
 
 from conduit.types import Indexable, IndexType, Sized
 
 __all__ = ["MemoryBank"]
 
 
 @torch.no_grad()
```

### Comparing `torch_conduit-0.3.4/conduit/models/utils.py` & `torch_conduit-0.3.5/conduit/models/utils.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/progress.py` & `torch_conduit-0.3.5/conduit/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from enum import Enum
 from typing import Any, Callable, Dict, Optional, Union, cast
+from typing_extensions import TypeAlias, override
 
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks.progress.rich_progress import (
     BatchesProcessedColumn,
     CustomBarColumn,
     CustomTimeColumn,
     ProcessingSpeedColumn,
@@ -12,15 +13,14 @@
     RichProgressBarTheme,
 )
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from rich.console import RenderableType
 from rich.progress import Task, TaskID, TextColumn
 from rich.table import Column
 from rich.text import Text
-from typing_extensions import TypeAlias, override
 
 __all__ = ["CdtProgressBar", "ProgressBarTheme"]
 
 
 class _FixedLengthProcessionSpeed(ProcessingSpeedColumn):
     """Renders processing speed for the progress bar with fixes length"""
 
@@ -106,15 +106,15 @@
             theme=theme,
             console_kwargs=console_kwargs,
         )
         self.predict_progress_bar_id = None
         self._predict_description = predict_description
 
     @override
-    def configure_columns(self, *args: Any, **kwargs: Any) -> list:  # pyright: ignore
+    def configure_columns(self, *args: Any, **kwargs: Any) -> list:
         return [
             TextColumn(
                 "[progress.description]{task.description}",
                 table_column=Column(
                     no_wrap=True,
                     min_width=9,  # prevents blinking during validation, length of `Validation `
                 ),
@@ -143,32 +143,35 @@
         the training dataloader is of infinite size.
         """
         if self.trainer.max_steps >= 0:
             return self.trainer.max_steps
         return self.trainer.num_training_batches
 
     @override
-    def _add_task(
+    def _add_task(  # type: ignore
         self, total_batches: float, description: str, visible: bool = True
     ) -> Optional[TaskID]:
         if self.progress is not None:
             return self.progress.add_task(
                 f"[{self.theme.description}]{description}", total=total_batches, visible=visible
             )
 
     @override
-    def _update(self, progress_bar_id: int, current: int, visible: bool = True) -> None:
+    def _update(
+        self, progress_bar_id: Optional[TaskID], current: int, visible: bool = True
+    ) -> None:
         if self.progress is not None and self.is_enabled:
+            assert progress_bar_id is not None
             total = self.progress.tasks[progress_bar_id].total
             if not self._should_update(current, total):  # type: ignore
                 return
 
             leftover = current % self.refresh_rate
             advance = leftover if (current == total and leftover != 0) else self.refresh_rate
-            self.progress.update(TaskID(progress_bar_id), advance=advance, visible=visible)
+            self.progress.update(progress_bar_id, advance=advance, visible=visible)
             self.refresh()
 
     @override
     def _get_train_description(self, current_epoch: Optional[int]) -> str:
         train_description = f"Training"
         if current_epoch is not None:
             train_description += f" (Epoch: {current_epoch})"
@@ -191,15 +194,15 @@
     def _progress_bar_id(self, value: Optional[TaskID]) -> None:
         if hasattr(self, "train_progress_bar_id"):
             self.train_progress_bar_id = value
         if hasattr(self, "main_progress_bar_id"):
             self.main_progress_bar_id = value
 
     @override
-    def on_train_epoch_start(self, trainer: pl.Trainer, pl_module) -> None:  # pyright: ignore
+    def on_train_epoch_start(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         total_train_batches = self.total_train_batches
         total_val_batches = self.total_val_batches
         if total_train_batches != float("inf"):
             # val can be checked multiple times per epoch
             val_checks_per_epoch = total_train_batches // trainer.val_check_batch
             total_val_batches = total_val_batches * val_checks_per_epoch
 
@@ -220,22 +223,22 @@
             )
         self.refresh()
 
     @override
     def on_validation_batch_end(
         self,
         trainer: pl.Trainer,
-        pl_module: pl.LightningModule,  # pyright: ignore
-        outputs: Optional[STEP_OUTPUT],  # pyright: ignore
-        batch: Any,  # pyright: ignore
+        pl_module: pl.LightningModule,
+        outputs: Optional[STEP_OUTPUT],
+        batch: Any,
         batch_idx: int,
-        dataloader_idx: int = 0,  # pyright: ignore
+        dataloader_idx: int = 0,
     ) -> None:
         if trainer.sanity_checking:
-            self._update(self.val_sanity_progress_bar_id, batch_idx + 1)  # type: ignore
+            self._update(self.val_sanity_progress_bar_id, batch_idx + 1)
         elif self.val_progress_bar_id is not None:
             # check to see if we should update the main training progress bar
             self._update(self.val_progress_bar_id, batch_idx + 1)
         self.refresh()
 
     @property
     def predict_description(self) -> str:
@@ -244,18 +247,18 @@
     @predict_description.setter
     def predict_description(self, value: str) -> None:
         self._predict_description = value
 
     @override
     def on_predict_batch_start(
         self,
-        trainer: pl.Trainer,  # pyright: ignore
-        pl_module: pl.LightningModule,  # pyright: ignore
-        batch: Any,  # pyright: ignore
-        batch_idx: int,  # pyright: ignore
+        trainer: pl.Trainer,
+        pl_module: pl.LightningModule,
+        batch: Any,
+        batch_idx: int,
         dataloader_idx: int = 0,
     ) -> None:
         if self.has_dataloader_changed(dataloader_idx):
             if (self.predict_progress_bar_id is not None) and (self.progress is not None):
                 self.progress.update(TaskID(self.predict_progress_bar_id), advance=0, visible=False)
             self.predict_progress_bar_id = self._add_task(
                 self.total_predict_batches_current_dataloader, self.predict_description
```

### Comparing `torch_conduit-0.3.4/conduit/transforms/audio.py` & `torch_conduit-0.3.5/conduit/transforms/audio.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/transforms/fixmatch.py` & `torch_conduit-0.3.5/conduit/transforms/fixmatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from dataclasses import dataclass
 from typing import Callable, Generic, List, Optional, TypeVar, Union
+from typing_extensions import Self, override
 
-from PIL import Image
 import numpy as np
+from PIL import Image
 from ranzen.misc import gcopy
 from torch import Tensor
-from typing_extensions import Self, override
 
 from conduit.data.datasets.vision.utils import ImageTform, apply_image_transform
 from conduit.data.structures import InputContainer, RawImage, concatenate_inputs
 
 __all__ = [
     "FixMatchPair",
     "FixMatchTransform",
 ]
 
 X = TypeVar("X", bound=Union[Tensor, RawImage, List[Image.Image]])
 
 
 @dataclass
-class FixMatchPair(InputContainer[X]):
+class FixMatchPair(InputContainer, Generic[X]):
     strong: X
     weak: X
 
     @override
     def __len__(self) -> int:
         if isinstance(self.strong, Image.Image):
             return 1
```

### Comparing `torch_conduit-0.3.4/conduit/transforms/image.py` & `torch_conduit-0.3.5/conduit/transforms/image.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.4/conduit/transforms/multicrop.py` & `torch_conduit-0.3.5/conduit/transforms/multicrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Generic, List, Optional, Sequence, Tuple, TypeVar, Union, overload
+from typing_extensions import Self, override
 
 from ranzen.misc import gcopy
 import torch
 from torch import Tensor
 import torchvision.transforms as T  # type: ignore
 import torchvision.transforms.functional as TF  # type: ignore
-from typing_extensions import Self, override
 
 from conduit.data.constants import IMAGENET_STATS
 from conduit.data.datasets.vision.utils import (
     ImageTform,
     PillowTform,
     apply_image_transform,
     img_to_tensor,
@@ -28,15 +28,15 @@
     "MultiCropOutput",
     "MultiCropTransform",
     "MultiViewPair",
 ]
 
 
 @dataclass
-class MultiViewPair(InputContainer[Tensor]):
+class MultiViewPair(InputContainer):
     v1: Tensor
     v2: Tensor
 
     def __post_init__(self) -> None:
         if self.v1.size() != self.v2.size():
             raise AttributeError("'v1' and 'v2' must have the same shape.")
 
@@ -52,14 +52,15 @@
         copy.v2 = concatenate_inputs(copy.v2, other.v2, is_batched=is_batched)
 
         return copy
 
     def size(self) -> torch.Size:
         return self.v1.size()
 
+    @property
     def shape(self) -> torch.Size:
         return self.v1.shape
 
     def merge(self) -> Tensor:
         is_batched = self.v1.ndim == 4
         return concatenate_inputs(self.v1, self.v2, is_batched=is_batched)
 
@@ -73,15 +74,15 @@
 
     @property
     def num_sources(self) -> int:
         return len(self)
 
 
 @dataclass
-class MultiCropOutput(InputContainer[MultiViewPair]):
+class MultiCropOutput(InputContainer):
     global_views: MultiViewPair
     local_views: Tensor
 
     @property
     def num_sources(self) -> int:
         """The number of samples from which the views were generated."""
         return len(self.global_views)
@@ -98,24 +99,24 @@
 
     @property
     def num_crops(self) -> int:
         return self.num_global_crops + self.num_local_crops
 
     @property
     def global_crop_size(self) -> Tuple[int, int, int]:
-        return self.global_views.shape[1:]  # type: ignore
+        return self.global_views.shape[1:]
 
     @property
     def local_crop_size(self) -> Tuple[int, int, int]:
         if self.local_views is None:
             raise AttributeError("Cannot retrieve the local-crop size as 'local_' is 'None'.")
         return self.local_views.shape[1:]
 
     @property
-    def shape(self):
+    def shape(self) -> torch.Size:
         """Shape of the global crops."""
         return self.global_views.shape
 
     def astuple(self) -> Tuple[Tensor, Tensor]:
         return (self.global_views.merge(), self.local_views)
 
     @property
@@ -168,15 +169,15 @@
             raise AttributeError(
                 " 'local_crops' must be a positive integer if 'local_transform' is defined."
             )
         self.local_transform = local_transform
         self.local_crops_number = local_crops_number
 
     @staticmethod
-    def _apply_transform(image: RawImage, transform: ImageTform):
+    def _apply_transform(image: RawImage, transform: ImageTform) -> Tensor:
         view = apply_image_transform(image, transform=transform)
         if not isinstance(view, Tensor):
             view = img_to_tensor(view)
         return view
 
     @overload
     def __call__(self: "MultiCropTransform[ImageTform]", image: RawImage) -> MultiCropOutput:
```

### Comparing `torch_conduit-0.3.4/conduit/transforms/tabular.py` & `torch_conduit-0.3.5/conduit/transforms/tabular.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 import math
 from typing import ClassVar, List, Union, final
+from typing_extensions import override
 
 import torch
 from torch import Tensor
-from typing_extensions import override
 
 __all__ = [
     "TabularTransform",
     "MinMaxNormalize",
     "QuantileNormalize",
     "TabularNormalize",
     "ZScoreNormalize",
 ]
 
 
-class TabularTransform:
+class TabularTransform(ABC):
     """PLaceholder base class."""
 
+    @abstractmethod
     def __call__(self, data: Tensor) -> Tensor:
-        ...
+        raise NotImplementedError()
 
 
 class TabularNormalize(TabularTransform):
     _EPS: ClassVar[float] = torch.finfo(torch.float32).eps
 
     def __init__(
         self, inplace: bool = False, indices: Union[slice, List[int]] = slice(None)
@@ -88,14 +89,15 @@
         return data
 
     @final
     def __call__(self, data: Tensor) -> Tensor:
         return self.transform(data)
 
 
+@final
 class ZScoreNormalize(TabularNormalize):
     mean: Tensor
     std: Tensor
 
     @override
     def _fit(self, data: Tensor) -> None:
         self.std, self.mean = torch.std_mean(data, dim=0, keepdim=True, unbiased=True)
@@ -109,14 +111,15 @@
     @override
     def _transform(self, data: Tensor) -> Tensor:
         data -= self.mean
         data /= self.std.clamp_min(self._EPS)
         return data
 
 
+@final
 class QuantileNormalize(TabularNormalize):
     iqr: Tensor
     median: Tensor
 
     def __init__(self, q_min: float = 0.25, q_max: float = 0.75, inplace: bool = False) -> None:
         super().__init__(inplace=inplace)
         if not (0 <= q_min <= 1):
@@ -157,14 +160,15 @@
     @override
     def _transform(self, data: Tensor) -> Tensor:
         data -= self.median
         data /= self.iqr.clamp_min(self._EPS)
         return data
 
 
+@final
 class MinMaxNormalize(TabularNormalize):
     orig_max: Tensor
     orig_min: Tensor
     orig_range: Tensor
 
     def __init__(self, new_min: float = 0.0, new_max: float = 1.0, inplace: bool = False) -> None:
         super().__init__(inplace=inplace)
```

### Comparing `torch_conduit-0.3.4/conduit/types.py` & `torch_conduit-0.3.5/conduit/types.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from enum import auto
 from typing import Any, Dict, List, Mapping, Protocol, TypeVar, Union, runtime_checkable
+from typing_extensions import TypeAlias
 
 import numpy as np
 import numpy.typing as npt
 from ranzen import StrEnum
 from ranzen.torch.loss import ReductionType
 from torch import Tensor
 from torch.optim.lr_scheduler import CosineAnnealingWarmRestarts, ExponentialLR, StepLR
 from torchmetrics import Metric
-from typing_extensions import TypeAlias
 
 __all__ = [
     "IndexType",
     "Indexable",
     "LRScheduler",
     "Loss",
     "MetricDict",
```

### Comparing `torch_conduit-0.3.4/pyproject.toml` & `torch_conduit-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-conduit"
-version = "0.3.4"
+version = "0.3.5"
 description = "Lightweight framework for dataloading with PyTorch and channeling the power of PyTorch Lightning"
 authors = ["PAL <info@predictive-analytics-lab.com>"]
 license = "Apache License 2.0"
 packages = [
   { include = "conduit" },
 ]
 include=["conduit/py.typed"]
@@ -25,14 +25,20 @@
 attrs = ">=21.2.0"
 numpy = "^1.22.3"
 pandas = ">=1.3.3,<3.0"
 python = ">=3.8.0,<3.12"
 ranzen = {version = ">=2.0.0"}
 scikit-learn = "^1.2.0"
 typing-extensions = ">=4.4.0"
+filelock = "*"
+jinja2 = "*"
+networkx = "*"
+sympy = "*"
+pillow = ">=5.3.0,!=8.3.*"
+requests = "*"
 
 # NOTE: the following has to be kept in sync with the groups below
 # download
 gdown = {version = "^3.13.0", optional = true}
 kaggle = {version = "^1.5.12", optional = true}
 # image
 albumentations = {version = "^1.0.0", optional = true}
@@ -86,16 +92,15 @@
     "rich",  # logging
     "ethicml",  # fair
 ]
 
 [[tool.poetry.source]]
 name = "torchcpu"
 url = "https://download.pytorch.org/whl/cpu"
-default = false
-secondary = true
+priority = "explicit"
 
 [tool.poetry.group.torch]
 optional = true
 
 [tool.poetry.group.torch.dependencies]
 pytorch-lightning = "^2.0.1.post0"
 torch = { version = "*", source = "torchcpu", markers = "sys_platform == 'linux'" }
@@ -138,37 +143,66 @@
     | dist
     | conduit/hydra
   )/
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
-[tool.isort]
-known_third_party = ["PIL", "albumentations", "attr", "cv2", "ethicml", "hydra", "numpy", "omegaconf", "pandas", "pytest", "pytorch_lightning", "ranzen", "requests", "rich", "sklearn", "torch", "torchaudio", "torchmetrics", "torchvision", "tqdm", "typing_extensions"]
-known_future_library = []
-extra_standard_library = ["dataclasses", "__future__", "typing_extensions"]
-line_length = 88
-profile = "black"
-force_sort_within_sections = "True"
+[tool.ruff]
+line-length = 88  # for import sorting
+select = [
+    "E", # pycodestyle
+    "F", # pyflakes
+    "I", # isort
+    # "N", # naming
+    "PLC", # pylint convention
+    "PLE", # pylint error
+    # "PLR", # pylint refactor
+    "PLW", # pylint warning
+    "PTH", # use-pathlib
+    # "UP", # pyupgrade
+    "W",
+]
+ignore = [
+    "E501", # line length
+    "E721", # `isinstance()` vs `type() == type()`
+    "E741", # ambiguous variable name
+    "F541", # f-string without placeholder
+    "PLW2901", # overwriting loop variable
+]
+target-version = "py38"
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F403"]
+
+[tool.ruff.isort]
+known-third-party = ["PIL", "albumentations", "attr", "cv2", "ethicml", "hydra", "numpy", "omegaconf", "pandas", "pytest", "pytorch_lightning", "ranzen", "requests", "rich", "sklearn", "torch", "torchaudio", "torchmetrics", "torchvision", "tqdm"]
+extra-standard-library = ["typing_extensions"]
+no-lines-before = ["future", "standard-library"]
+force-sort-within-sections = true
+split-on-trailing-comma = false
 classes = ["MISSING", "NICO", "PACS", "SSRP", "ISIC"]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonVersion = "3.8"
 reportMissingTypeArgument = "none"
 reportCallInDefaultInitializer = "warning"
 reportPropertyTypeMismatch = "none"
 reportUninitializedInstanceVariable = "warning"
 reportPrivateUsage = "none"
+reportUnnecessaryTypeIgnoreComment = "warning"
+reportUnnecessaryIsInstance = "warning"
+reportUnnecessaryCast = "warning"
+reportUnnecessaryComparison = "warning"
 # these errors are a bit annoying
 reportUnknownMemberType = "none"
 reportUnknownVariableType = "none"
 reportUnknownParameterType = "none"
 reportUnknownArgumentType = "none"
-reportUnnecessaryTypeIgnoreComment = "warning"
 ignore = ["conduit/hydra/**"]
 
 [tool.mypy]
 python_version = "3.8"
 no_implicit_optional = true
 allow_redefinition = true
 strict_equality = true
```

### Comparing `torch_conduit-0.3.4/PKG-INFO` & `torch_conduit-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: torch-conduit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Lightweight framework for dataloading with PyTorch and channeling the power of PyTorch Lightning
 Home-page: https://github.com/wearepal/conduit
 License: Apache-2.0
 Keywords: typing,python,pytorch,datasets,pytorch-lightning,lightning-bolts
 Author: PAL
 Author-email: info@predictive-analytics-lab.com
 Requires-Python: >=3.8.0,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: audio
 Provides-Extra: download
 Provides-Extra: fair
 Provides-Extra: hydra
 Provides-Extra: image
 Provides-Extra: logging
 Requires-Dist: albumentations (>=1.0.0,<2.0.0) ; extra == "image" or extra == "all"
 Requires-Dist: attrs (>=21.2.0)
 Requires-Dist: ethicml[data] (>=1.2.1,<2.0.0) ; extra == "fair" or extra == "all"
+Requires-Dist: filelock
 Requires-Dist: gdown (>=3.13.0,<4.0.0) ; extra == "download" or extra == "all"
 Requires-Dist: hydra-core (>=1.1.1,<2.0.0) ; extra == "hydra" or extra == "all"
+Requires-Dist: jinja2
 Requires-Dist: kaggle (>=1.5.12,<2.0.0) ; extra == "download" or extra == "all"
+Requires-Dist: networkx
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.5.3,<5.0.0) ; extra == "image" or extra == "all"
 Requires-Dist: pandas (>=1.3.3,<3.0)
+Requires-Dist: pillow (>=5.3.0,!=8.3.*)
 Requires-Dist: ranzen (>=2.0.0)
+Requires-Dist: requests
 Requires-Dist: rich (>=12.5.1,<13.0.0) ; extra == "logging" or extra == "all"
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: soundfile ; (platform_system == "Windows") and (extra == "audio" or extra == "all")
 Requires-Dist: sox ; (platform_system == "Linux" or platform_system == "macOS") and (extra == "audio" or extra == "all")
+Requires-Dist: sympy
 Requires-Dist: typing-extensions (>=4.4.0)
 Project-URL: Repository, https://github.com/wearepal/conduit
 Description-Content-Type: text/markdown
 
 # conduit :electron:
 
 Al lightweight framework for channeling the power of PyTorch Lightning.
```

