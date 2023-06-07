# Comparing `tmp/a2-0.3.7.tar.gz` & `tmp/a2-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2-0.3.7.tar", max compression
+gzip compressed data, was "a2-0.3.8.tar", max compression
```

## Comparing `a2-0.3.7.tar` & `a2-0.3.8.tar`

### file list

```diff
@@ -1,56 +1,1961 @@
--rw-r--r--   0        0        0     3941 2023-06-06 16:39:04.054525 a2-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.7/src/a2/__init__.py
--rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.7/src/a2/cli/__init__.py
--rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.7/src/a2/cli/cli_plotting/__init__.py
--rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.7/src/a2/cli/cli_plotting/plot.py
--rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.7/src/a2/cli/cli_plotting/single_plots.py
--rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.7/src/a2/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.7/src/a2/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.7/src/a2/data/emoji/__init__.py
--rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.7/src/a2/data/emoji/emoji_df.csv
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.7/src/a2/data/vocabularies/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.7/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
--rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.7/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
--rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.7/src/a2/dataset/__init__.py
--rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.7/src/a2/dataset/emojis.py
--rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.3.7/src/a2/dataset/load_dataset.py
--rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.7/src/a2/dataset/radar.py
--rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.7/src/a2/dataset/stations.py
--rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.7/src/a2/dataset/tweets.py
--rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.7/src/a2/dataset/units.py
--rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.3.7/src/a2/dataset/utils_dataset.py
--rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.7/src/a2/plotting/__init__.py
--rw-r--r--   0        0        0     8164 2023-05-12 12:06:36.401113 a2-0.3.7/src/a2/plotting/analysis.py
--rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.7/src/a2/plotting/axes_utils.py
--rw-r--r--   0        0        0    30638 2023-05-16 11:22:03.945363 a2-0.3.7/src/a2/plotting/histograms.py
--rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.7/src/a2/plotting/parallel_plotting.py
--rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.7/src/a2/plotting/timeseries.py
--rw-r--r--   0        0        0    16218 2023-05-12 12:06:36.401113 a2-0.3.7/src/a2/plotting/utils_plotting.py
--rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.7/src/a2/plotting/weather_maps.py
--rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.7/src/a2/preprocess/__init__.py
--rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.7/src/a2/preprocess/embedding.py
--rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/preprocess/normalize_text.py
--rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.3.7/src/a2/training/__init__.py
--rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.3.7/src/a2/training/benchmarks.py
--rw-r--r--   0        0        0     2863 2023-06-06 15:14:17.260894 a2-0.3.7/src/a2/training/dataset_hugging.py
--rw-r--r--   0        0        0     4213 2023-06-06 15:45:58.319253 a2-0.3.7/src/a2/training/evaluate_hugging.py
--rw-r--r--   0        0        0     4563 2023-06-06 15:48:04.766178 a2-0.3.7/src/a2/training/tracking.py
--rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.3.7/src/a2/training/tracking_hugging.py
--rw-r--r--   0        0        0     6390 2023-05-12 12:06:13.512505 a2-0.3.7/src/a2/training/training_deep500.py
--rw-r--r--   0        0        0    11299 2023-06-06 14:58:39.420340 a2-0.3.7/src/a2/training/training_hugging.py
--rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/training/training_performance.py
--rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.7/src/a2/training/utils_training.py
--rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.7/src/a2/twitter/__init__.py
--rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.7/src/a2/twitter/downloader.py
--rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.3.7/src/a2/twitter/locations.py
--rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.7/src/a2/twitter/twitter_api.py
--rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.3.7/src/a2/utils/__init__.py
--rw-r--r--   0        0        0     8662 2023-06-06 16:36:35.562037 a2-0.3.7/src/a2/utils/argparse.py
--rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.3.7/src/a2/utils/checks.py
--rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.7/src/a2/utils/constants.py
--rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.3.7/src/a2/utils/file_handling.py
--rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/utils/strings.py
--rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.3.7/src/a2/utils/testing.py
--rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.7/src/a2/utils/times.py
--rw-r--r--   0        0        0     6088 2023-05-12 12:06:36.405113 a2-0.3.7/src/a2/utils/utils.py
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 a2-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     3941 2023-06-07 07:45:20.025969 a2-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.8/src/a2/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.8/src/a2/cli/__init__.py
+-rw-r--r--   0        0        0      200 2023-01-13 09:53:11.940626 a2-0.3.8/src/a2/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      297 2023-01-13 09:40:55.677429 a2-0.3.8/src/a2/cli/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.8/src/a2/cli/cli_plotting/__init__.py
+-rw-r--r--   0        0        0      203 2023-01-13 09:53:11.952627 a2-0.3.8/src/a2/cli/cli_plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      359 2023-01-13 09:53:14.892690 a2-0.3.8/src/a2/cli/cli_plotting/__pycache__/plot.cpython-310.pyc
+-rw-r--r--   0        0        0     2101 2023-02-16 10:12:23.148895 a2-0.3.8/src/a2/cli/cli_plotting/__pycache__/single_plots.cpython-310.pyc
+-rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.8/src/a2/cli/cli_plotting/plot.py
+-rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.8/src/a2/cli/cli_plotting/single_plots.py
+-rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.8/src/a2/cli/main.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.8/src/a2/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.8/src/a2/data/emoji/__init__.py
+-rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.8/src/a2/data/emoji/emoji_df.csv
+-rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0023_fe0f_20e3.png
+-rw-r--r--   0        0        0     1221 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/002a_fe0f_20e3.png
+-rw-r--r--   0        0        0     1065 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0030_fe0f_20e3.png
+-rw-r--r--   0        0        0      989 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0031_fe0f_20e3.png
+-rw-r--r--   0        0        0     1043 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0032_fe0f_20e3.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0033_fe0f_20e3.png
+-rw-r--r--   0        0        0     1077 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0034_fe0f_20e3.png
+-rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0035_fe0f_20e3.png
+-rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0036_fe0f_20e3.png
+-rw-r--r--   0        0        0      985 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0037_fe0f_20e3.png
+-rw-r--r--   0        0        0     1120 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0038_fe0f_20e3.png
+-rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/0039_fe0f_20e3.png
+-rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/00a9.png
+-rw-r--r--   0        0        0     1091 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/00ae.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f004.png
+-rw-r--r--   0        0        0     1141 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f0cf.png
+-rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f170.png
+-rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f171.png
+-rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f17e.png
+-rw-r--r--   0        0        0     1075 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f17f.png
+-rw-r--r--   0        0        0     1342 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f18e.png
+-rw-r--r--   0        0        0     1352 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f191.png
+-rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f192.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f193.png
+-rw-r--r--   0        0        0     1150 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f194.png
+-rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f195.png
+-rw-r--r--   0        0        0     1194 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f196.png
+-rw-r--r--   0        0        0     1264 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f197.png
+-rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f198.png
+-rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f199.png
+-rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f19a.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1e8.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1e9.png
+-rw-r--r--   0        0        0     1245 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1ea.png
+-rw-r--r--   0        0        0     1346 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1eb.png
+-rw-r--r--   0        0        0     1555 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1ec.png
+-rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1ee.png
+-rw-r--r--   0        0        0     1206 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f1.png
+-rw-r--r--   0        0        0     1444 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f2.png
+-rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f4.png
+-rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f6.png
+-rw-r--r--   0        0        0     1193 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f7.png
+-rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f8.png
+-rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1f9.png
+-rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1fa.png
+-rw-r--r--   0        0        0     1379 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1fc.png
+-rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1fd.png
+-rw-r--r--   0        0        0     1592 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e6_1f1ff.png
+-rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1e6.png
+-rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1e7.png
+-rw-r--r--   0        0        0      935 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1e9.png
+-rw-r--r--   0        0        0      998 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1ea.png
+-rw-r--r--   0        0        0     1253 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1eb.png
+-rw-r--r--   0        0        0     1348 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1ec.png
+-rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1ed.png
+-rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1ee.png
+-rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1ef.png
+-rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f1.png
+-rw-r--r--   0        0        0     2553 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f2.png
+-rw-r--r--   0        0        0     2134 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f3.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f4.png
+-rw-r--r--   0        0        0     1467 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f6.png
+-rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f7.png
+-rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f8.png
+-rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1f9.png
+-rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1fb.png
+-rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1fc.png
+-rw-r--r--   0        0        0     1417 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1fe.png
+-rw-r--r--   0        0        0     2195 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e7_1f1ff.png
+-rw-r--r--   0        0        0     1263 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1e6.png
+-rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1e8.png
+-rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1e9.png
+-rw-r--r--   0        0        0     1831 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1eb.png
+-rw-r--r--   0        0        0     1460 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1ec.png
+-rw-r--r--   0        0        0      879 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1ed.png
+-rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1ee.png
+-rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f0.png
+-rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f1.png
+-rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f2.png
+-rw-r--r--   0        0        0     1055 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f3.png
+-rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f4.png
+-rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f5.png
+-rw-r--r--   0        0        0     1521 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1f7.png
+-rw-r--r--   0        0        0     1609 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1fa.png
+-rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1fb.png
+-rw-r--r--   0        0        0     1215 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1fc.png
+-rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1fd.png
+-rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1fe.png
+-rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e8_1f1ff.png
+-rw-r--r--   0        0        0     1280 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1ea.png
+-rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1ec.png
+-rw-r--r--   0        0        0     1331 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1ef.png
+-rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1f0.png
+-rw-r--r--   0        0        0     2283 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1f2.png
+-rw-r--r--   0        0        0     1737 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1f4.png
+-rw-r--r--   0        0        0     1324 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1e9_1f1ff.png
+-rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1e6.png
+-rw-r--r--   0        0        0     1976 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1e8.png
+-rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1ea.png
+-rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1ec.png
+-rw-r--r--   0        0        0     1270 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1ed.png
+-rw-r--r--   0        0        0     1719 2022-11-18 15:36:28.436585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1f7.png
+-rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1f8.png
+-rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1f9.png
+-rw-r--r--   0        0        0      969 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ea_1f1fa.png
+-rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1eb_1f1ee.png
+-rw-r--r--   0        0        0     2421 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1eb_1f1ef.png
+-rw-r--r--   0        0        0     2067 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1eb_1f1f0.png
+-rw-r--r--   0        0        0     1005 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1eb_1f1f2.png
+-rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1eb_1f1f4.png
+-rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1eb_1f1f7.png
+-rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1e6.png
+-rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1e7.png
+-rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1e9.png
+-rw-r--r--   0        0        0     1583 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1ea.png
+-rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1eb.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1ec.png
+-rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1ed.png
+-rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1ee.png
+-rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f1.png
+-rw-r--r--   0        0        0     1570 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f2.png
+-rw-r--r--   0        0        0     1023 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f3.png
+-rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f5.png
+-rw-r--r--   0        0        0     1641 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f6.png
+-rw-r--r--   0        0        0     1677 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f7.png
+-rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f8.png
+-rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1f9.png
+-rw-r--r--   0        0        0     1354 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1fa.png
+-rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1fc.png
+-rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ec_1f1fe.png
+-rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ed_1f1f0.png
+-rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ed_1f1f2.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ed_1f1f3.png
+-rw-r--r--   0        0        0     1843 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ed_1f1f7.png
+-rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ed_1f1f9.png
+-rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ed_1f1fa.png
+-rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1e8.png
+-rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1e9.png
+-rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1ea.png
+-rw-r--r--   0        0        0     1453 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f1.png
+-rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f2.png
+-rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f3.png
+-rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f4.png
+-rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f6.png
+-rw-r--r--   0        0        0     1566 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f7.png
+-rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f8.png
+-rw-r--r--   0        0        0      995 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ee_1f1f9.png
+-rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ef_1f1ea.png
+-rw-r--r--   0        0        0     1536 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ef_1f1f2.png
+-rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ef_1f1f4.png
+-rw-r--r--   0        0        0     1019 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ef_1f1f5.png
+-rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1ea.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1ec.png
+-rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1ed.png
+-rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1ee.png
+-rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1f2.png
+-rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1f3.png
+-rw-r--r--   0        0        0     1552 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1f5.png
+-rw-r--r--   0        0        0     1531 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1f7.png
+-rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1fc.png
+-rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1fe.png
+-rw-r--r--   0        0        0     1473 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f0_1f1ff.png
+-rw-r--r--   0        0        0     1229 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1e6.png
+-rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1e7.png
+-rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1e8.png
+-rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1ee.png
+-rw-r--r--   0        0        0     1483 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1f0.png
+-rw-r--r--   0        0        0     1995 2022-11-18 15:36:28.440585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1f7.png
+-rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1f8.png
+-rw-r--r--   0        0        0     1333 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1f9.png
+-rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1fa.png
+-rw-r--r--   0        0        0     1056 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1fb.png
+-rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f1_1f1fe.png
+-rw-r--r--   0        0        0     1158 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1e6.png
+-rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1e8.png
+-rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1e9.png
+-rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1ea.png
+-rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1eb.png
+-rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1ec.png
+-rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1ed.png
+-rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f0.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f1.png
+-rw-r--r--   0        0        0     1574 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f2.png
+-rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f3.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f4.png
+-rw-r--r--   0        0        0     1791 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f5.png
+-rw-r--r--   0        0        0     1505 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f6.png
+-rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f7.png
+-rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f8.png
+-rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1f9.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1fa.png
+-rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1fb.png
+-rw-r--r--   0        0        0     1364 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1fc.png
+-rw-r--r--   0        0        0     1311 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1fd.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1fe.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f2_1f1ff.png
+-rw-r--r--   0        0        0     1835 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1e6.png
+-rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1e8.png
+-rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1ea.png
+-rw-r--r--   0        0        0     1149 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1eb.png
+-rw-r--r--   0        0        0      881 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1ec.png
+-rw-r--r--   0        0        0     1377 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1ee.png
+-rw-r--r--   0        0        0     1234 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1f1.png
+-rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1f4.png
+-rw-r--r--   0        0        0      999 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1f5.png
+-rw-r--r--   0        0        0     1148 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1f7.png
+-rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1fa.png
+-rw-r--r--   0        0        0     1683 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f3_1f1ff.png
+-rw-r--r--   0        0        0     1419 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f4_1f1f2.png
+-rw-r--r--   0        0        0     1550 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1e6.png
+-rw-r--r--   0        0        0      977 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1ea.png
+-rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1eb.png
+-rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1ec.png
+-rw-r--r--   0        0        0     1695 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1ed.png
+-rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f0.png
+-rw-r--r--   0        0        0     1040 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f1.png
+-rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f2.png
+-rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f3.png
+-rw-r--r--   0        0        0     1622 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f7.png
+-rw-r--r--   0        0        0     1211 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f8.png
+-rw-r--r--   0        0        0     1590 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1f9.png
+-rw-r--r--   0        0        0     1022 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1fc.png
+-rw-r--r--   0        0        0     1607 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f5_1f1fe.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f6_1f1e6.png
+-rw-r--r--   0        0        0     1792 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f7_1f1ea.png
+-rw-r--r--   0        0        0      954 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f7_1f1f4.png
+-rw-r--r--   0        0        0     1872 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f7_1f1f8.png
+-rw-r--r--   0        0        0     1298 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f7_1f1fa.png
+-rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f7_1f1fc.png
+-rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1e6.png
+-rw-r--r--   0        0        0     1729 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1e7.png
+-rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1e8.png
+-rw-r--r--   0        0        0     1203 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1e9.png
+-rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1ea.png
+-rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1ec.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1ed.png
+-rw-r--r--   0        0        0     1613 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1ee.png
+-rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1ef.png
+-rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f0.png
+-rw-r--r--   0        0        0     1411 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f1.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.444585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f2.png
+-rw-r--r--   0        0        0     1228 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f3.png
+-rw-r--r--   0        0        0      884 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f4.png
+-rw-r--r--   0        0        0     1557 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f7.png
+-rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f8.png
+-rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1f9.png
+-rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1fb.png
+-rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1fd.png
+-rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1fe.png
+-rw-r--r--   0        0        0     2344 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f8_1f1ff.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1e6.png
+-rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1e8.png
+-rw-r--r--   0        0        0      968 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1e9.png
+-rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1eb.png
+-rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1ec.png
+-rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1ed.png
+-rw-r--r--   0        0        0     1440 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1ef.png
+-rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f0.png
+-rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f1.png
+-rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f2.png
+-rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f3.png
+-rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f4.png
+-rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f7.png
+-rw-r--r--   0        0        0     1448 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1f9.png
+-rw-r--r--   0        0        0     2227 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1fb.png
+-rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1fc.png
+-rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1f9_1f1ff.png
+-rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1e6.png
+-rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1ec.png
+-rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1f2.png
+-rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1f3.png
+-rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1f8.png
+-rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1fe.png
+-rw-r--r--   0        0        0     1743 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fa_1f1ff.png
+-rw-r--r--   0        0        0     1197 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1e6.png
+-rw-r--r--   0        0        0     1337 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1e8.png
+-rw-r--r--   0        0        0     1580 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1ea.png
+-rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1ec.png
+-rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1ee.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1f3.png
+-rw-r--r--   0        0        0     1594 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fb_1f1fa.png
+-rw-r--r--   0        0        0     1319 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fc_1f1eb.png
+-rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fc_1f1f8.png
+-rw-r--r--   0        0        0     1128 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fd_1f1f0.png
+-rw-r--r--   0        0        0     1184 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fe_1f1ea.png
+-rw-r--r--   0        0        0     1649 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1fe_1f1f9.png
+-rw-r--r--   0        0        0     2075 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ff_1f1e6.png
+-rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ff_1f1f2.png
+-rw-r--r--   0        0        0     2394 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f1ff_1f1fc.png
+-rw-r--r--   0        0        0     1081 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f201.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f202.png
+-rw-r--r--   0        0        0     1478 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f21a.png
+-rw-r--r--   0        0        0     1514 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f22f.png
+-rw-r--r--   0        0        0     1682 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f232.png
+-rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f233.png
+-rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f234.png
+-rw-r--r--   0        0        0     1667 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f235.png
+-rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f236.png
+-rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f237.png
+-rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f238.png
+-rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f239.png
+-rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f23a.png
+-rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f250.png
+-rw-r--r--   0        0        0     1181 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f251.png
+-rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f300.png
+-rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f301.png
+-rw-r--r--   0        0        0     1753 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f302.png
+-rw-r--r--   0        0        0     2162 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f303.png
+-rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f304.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f305.png
+-rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f306.png
+-rw-r--r--   0        0        0     2397 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f307.png
+-rw-r--r--   0        0        0     3358 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f308.png
+-rw-r--r--   0        0        0     1972 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f309.png
+-rw-r--r--   0        0        0     2761 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f30a.png
+-rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f30b.png
+-rw-r--r--   0        0        0     1639 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f30c.png
+-rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f30d.png
+-rw-r--r--   0        0        0     3347 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f30e.png
+-rw-r--r--   0        0        0     3956 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f30f.png
+-rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f310.png
+-rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f311.png
+-rw-r--r--   0        0        0     2102 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f312.png
+-rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f313.png
+-rw-r--r--   0        0        0     2310 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f314.png
+-rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f315.png
+-rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f316.png
+-rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f317.png
+-rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f318.png
+-rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f319.png
+-rw-r--r--   0        0        0     1551 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f31a.png
+-rw-r--r--   0        0        0     1589 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f31b.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f31c.png
+-rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f31d.png
+-rw-r--r--   0        0        0     3537 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f31e.png
+-rw-r--r--   0        0        0     1898 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f31f.png
+-rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f320.png
+-rw-r--r--   0        0        0     1925 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f321.png
+-rw-r--r--   0        0        0     1971 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f324.png
+-rw-r--r--   0        0        0     1326 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f325.png
+-rw-r--r--   0        0        0     2070 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f326.png
+-rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f327.png
+-rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f328.png
+-rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f329.png
+-rw-r--r--   0        0        0     2338 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f32a.png
+-rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f32b.png
+-rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f32c.png
+-rw-r--r--   0        0        0     2143 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f32d.png
+-rw-r--r--   0        0        0     3164 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f32e.png
+-rw-r--r--   0        0        0     2846 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f32f.png
+-rw-r--r--   0        0        0     2278 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f330.png
+-rw-r--r--   0        0        0     1332 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f331.png
+-rw-r--r--   0        0        0     2597 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f332.png
+-rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f333.png
+-rw-r--r--   0        0        0     3072 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f334.png
+-rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f335.png
+-rw-r--r--   0        0        0     1845 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f336.png
+-rw-r--r--   0        0        0     3135 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f337.png
+-rw-r--r--   0        0        0     3604 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f338.png
+-rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f339.png
+-rw-r--r--   0        0        0     3826 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f33a.png
+-rw-r--r--   0        0        0     2868 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f33b.png
+-rw-r--r--   0        0        0     2956 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f33c.png
+-rw-r--r--   0        0        0     3578 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f33d.png
+-rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f33e.png
+-rw-r--r--   0        0        0     2049 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f33f.png
+-rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f340.png
+-rw-r--r--   0        0        0     2961 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f341.png
+-rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f342.png
+-rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f343.png
+-rw-r--r--   0        0        0     2132 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f344.png
+-rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f345.png
+-rw-r--r--   0        0        0     1652 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f346.png
+-rw-r--r--   0        0        0     3397 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f347.png
+-rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f348.png
+-rw-r--r--   0        0        0     1901 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f349.png
+-rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f34a.png
+-rw-r--r--   0        0        0     2346 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f34b.png
+-rw-r--r--   0        0        0     2330 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f34c.png
+-rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f34d.png
+-rw-r--r--   0        0        0     2045 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f34e.png
+-rw-r--r--   0        0        0     1960 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f34f.png
+-rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f350.png
+-rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f351.png
+-rw-r--r--   0        0        0     2440 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f352.png
+-rw-r--r--   0        0        0     3080 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f353.png
+-rw-r--r--   0        0        0     3804 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f354.png
+-rw-r--r--   0        0        0     2094 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f355.png
+-rw-r--r--   0        0        0     2512 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f356.png
+-rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f357.png
+-rw-r--r--   0        0        0     2273 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f358.png
+-rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f359.png
+-rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f35a.png
+-rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f35b.png
+-rw-r--r--   0        0        0     3130 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f35c.png
+-rw-r--r--   0        0        0     2982 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f35d.png
+-rw-r--r--   0        0        0     1849 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f35e.png
+-rw-r--r--   0        0        0     2730 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f35f.png
+-rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f360.png
+-rw-r--r--   0        0        0     2058 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f361.png
+-rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f362.png
+-rw-r--r--   0        0        0     2825 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f363.png
+-rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f364.png
+-rw-r--r--   0        0        0     1761 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f365.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f366.png
+-rw-r--r--   0        0        0     2335 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f367.png
+-rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f368.png
+-rw-r--r--   0        0        0     4358 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f369.png
+-rw-r--r--   0        0        0     2375 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f36a.png
+-rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f36b.png
+-rw-r--r--   0        0        0     2528 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f36c.png
+-rw-r--r--   0        0        0     2993 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f36d.png
+-rw-r--r--   0        0        0     1876 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f36e.png
+-rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f36f.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f370.png
+-rw-r--r--   0        0        0     4187 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f371.png
+-rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f372.png
+-rw-r--r--   0        0        0     2053 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f373.png
+-rw-r--r--   0        0        0     1571 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f374.png
+-rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f375.png
+-rw-r--r--   0        0        0     1653 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f376.png
+-rw-r--r--   0        0        0     1820 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f377.png
+-rw-r--r--   0        0        0     2130 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f378.png
+-rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f379.png
+-rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f37a.png
+-rw-r--r--   0        0        0     3070 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f37b.png
+-rw-r--r--   0        0        0     1840 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f37c.png
+-rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f37d.png
+-rw-r--r--   0        0        0     2490 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f37e.png
+-rw-r--r--   0        0        0     3063 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f37f.png
+-rw-r--r--   0        0        0     2216 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f380.png
+-rw-r--r--   0        0        0     2290 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f381.png
+-rw-r--r--   0        0        0     2452 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f382.png
+-rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f383.png
+-rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f384.png
+-rw-r--r--   0        0        0     3193 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f385.png
+-rw-r--r--   0        0        0     2478 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f386.png
+-rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f387.png
+-rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f388.png
+-rw-r--r--   0        0        0     3725 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f389.png
+-rw-r--r--   0        0        0     3748 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f38a.png
+-rw-r--r--   0        0        0     2909 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f38b.png
+-rw-r--r--   0        0        0     2120 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f38c.png
+-rw-r--r--   0        0        0     2268 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f38d.png
+-rw-r--r--   0        0        0     3885 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f38e.png
+-rw-r--r--   0        0        0    13409 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f38f.png
+-rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f390.png
+-rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f391.png
+-rw-r--r--   0        0        0     2593 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f392.png
+-rw-r--r--   0        0        0     1595 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f393.png
+-rw-r--r--   0        0        0     1673 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f396.png
+-rw-r--r--   0        0        0     1273 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f397.png
+-rw-r--r--   0        0        0     2738 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f399.png
+-rw-r--r--   0        0        0     1254 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f39a.png
+-rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f39b.png
+-rw-r--r--   0        0        0     2621 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f39e.png
+-rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f39f.png
+-rw-r--r--   0        0        0     3774 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a0.png
+-rw-r--r--   0        0        0     3756 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a1.png
+-rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a2.png
+-rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a3.png
+-rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a4.png
+-rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a5.png
+-rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a6.png
+-rw-r--r--   0        0        0     2400 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a7.png
+-rw-r--r--   0        0        0     3744 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a8.png
+-rw-r--r--   0        0        0     1380 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3a9.png
+-rw-r--r--   0        0        0     3014 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3aa.png
+-rw-r--r--   0        0        0     1519 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ab.png
+-rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ac.png
+-rw-r--r--   0        0        0     3610 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ad.png
+-rw-r--r--   0        0        0     2008 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ae.png
+-rw-r--r--   0        0        0     2799 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3af.png
+-rw-r--r--   0        0        0     2850 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b0.png
+-rw-r--r--   0        0        0     1685 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b1.png
+-rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b2.png
+-rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b3.png
+-rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b4.png
+-rw-r--r--   0        0        0      989 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b5.png
+-rw-r--r--   0        0        0     1731 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b6.png
+-rw-r--r--   0        0        0     2673 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b7.png
+-rw-r--r--   0        0        0     2595 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b8.png
+-rw-r--r--   0        0        0     1147 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3b9.png
+-rw-r--r--   0        0        0     3202 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ba.png
+-rw-r--r--   0        0        0     3440 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3bb.png
+-rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3bc.png
+-rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3bd.png
+-rw-r--r--   0        0        0     2114 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3be.png
+-rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3bf.png
+-rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c0.png
+-rw-r--r--   0        0        0     1384 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c1.png
+-rw-r--r--   0        0        0     3205 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c2.png
+-rw-r--r--   0        0        0     2226 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c3.png
+-rw-r--r--   0        0        0     2518 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c3_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2449 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c3_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3228 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c4.png
+-rw-r--r--   0        0        0     3265 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c4_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c4_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2901 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c5.png
+-rw-r--r--   0        0        0     2765 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c6.png
+-rw-r--r--   0        0        0     2834 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c7.png
+-rw-r--r--   0        0        0     2681 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c8.png
+-rw-r--r--   0        0        0     2430 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3c9.png
+-rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ca.png
+-rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ca_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2879 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ca_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3446 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cb.png
+-rw-r--r--   0        0        0     3400 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3505 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cc.png
+-rw-r--r--   0        0        0     2502 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cd.png
+-rw-r--r--   0        0        0     2826 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ce.png
+-rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3cf.png
+-rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d0.png
+-rw-r--r--   0        0        0     1866 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d1.png
+-rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d2.png
+-rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d3.png
+-rw-r--r--   0        0        0     3018 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d4.png
+-rw-r--r--   0        0        0     2698 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d5.png
+-rw-r--r--   0        0        0     3183 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d6.png
+-rw-r--r--   0        0        0     3121 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d7.png
+-rw-r--r--   0        0        0     3021 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d8.png
+-rw-r--r--   0        0        0     1628 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3d9.png
+-rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3da.png
+-rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3db.png
+-rw-r--r--   0        0        0     3123 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3dc.png
+-rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3dd.png
+-rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3de.png
+-rw-r--r--   0        0        0     4049 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3df.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e0.png
+-rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e1.png
+-rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e2.png
+-rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e3.png
+-rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e4.png
+-rw-r--r--   0        0        0     1880 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e5.png
+-rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e6.png
+-rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e7.png
+-rw-r--r--   0        0        0     2990 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e8.png
+-rw-r--r--   0        0        0     3226 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3e9.png
+-rw-r--r--   0        0        0     2202 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ea.png
+-rw-r--r--   0        0        0     2239 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3eb.png
+-rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ec.png
+-rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ed.png
+-rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ee.png
+-rw-r--r--   0        0        0     2396 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3ef.png
+-rw-r--r--   0        0        0     3103 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f0.png
+-rw-r--r--   0        0        0      848 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f3.png
+-rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_1f308.png
+-rw-r--r--   0        0        0     1389 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_26a7_fe0f.png
+-rw-r--r--   0        0        0      761 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f4.png
+-rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f4_200d_2620_fe0f.png
+-rw-r--r--   0        0        0     1283 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0065_e006e_e0067_e007f.png
+-rw-r--r--   0        0        0     1451 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0073_e0063_e0074_e007f.png
+-rw-r--r--   0        0        0     2115 2022-11-18 15:36:28.448585 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0077_e006c_e0073_e007f.png
+-rw-r--r--   0        0        0     4095 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f5.png
+-rw-r--r--   0        0        0      495 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f7.png
+-rw-r--r--   0        0        0     3310 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f8.png
+-rw-r--r--   0        0        0     2605 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3f9.png
+-rw-r--r--   0        0        0     2936 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f3fa.png
+-rw-r--r--   0        0        0     1698 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f400.png
+-rw-r--r--   0        0        0     2505 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f401.png
+-rw-r--r--   0        0        0     1710 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f402.png
+-rw-r--r--   0        0        0     1549 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f403.png
+-rw-r--r--   0        0        0     2271 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f404.png
+-rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f405.png
+-rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f406.png
+-rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f407.png
+-rw-r--r--   0        0        0     2893 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f408.png
+-rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f408_200d_2b1b.png
+-rw-r--r--   0        0        0     4191 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f409.png
+-rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f40a.png
+-rw-r--r--   0        0        0     2014 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f40b.png
+-rw-r--r--   0        0        0     3036 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f40c.png
+-rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f40d.png
+-rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f40e.png
+-rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f40f.png
+-rw-r--r--   0        0        0     1862 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f410.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f411.png
+-rw-r--r--   0        0        0     2556 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f412.png
+-rw-r--r--   0        0        0     2453 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f413.png
+-rw-r--r--   0        0        0     2304 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f414.png
+-rw-r--r--   0        0        0     2328 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f415.png
+-rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f415_200d_1f9ba.png
+-rw-r--r--   0        0        0     1591 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f416.png
+-rw-r--r--   0        0        0     1773 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f417.png
+-rw-r--r--   0        0        0     1699 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f418.png
+-rw-r--r--   0        0        0     2151 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f419.png
+-rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f41a.png
+-rw-r--r--   0        0        0     3478 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f41b.png
+-rw-r--r--   0        0        0     2245 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f41c.png
+-rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f41d.png
+-rw-r--r--   0        0        0     3427 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f41e.png
+-rw-r--r--   0        0        0     1868 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f41f.png
+-rw-r--r--   0        0        0     3171 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f420.png
+-rw-r--r--   0        0        0     3511 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f421.png
+-rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f422.png
+-rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f423.png
+-rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f424.png
+-rw-r--r--   0        0        0     2506 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f425.png
+-rw-r--r--   0        0        0     1535 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f426.png
+-rw-r--r--   0        0        0     1612 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f427.png
+-rw-r--r--   0        0        0     1805 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f428.png
+-rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f429.png
+-rw-r--r--   0        0        0     1655 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f42a.png
+-rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f42b.png
+-rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f42c.png
+-rw-r--r--   0        0        0     2063 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f42d.png
+-rw-r--r--   0        0        0     2011 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f42e.png
+-rw-r--r--   0        0        0     3152 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f42f.png
+-rw-r--r--   0        0        0     1994 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f430.png
+-rw-r--r--   0        0        0     2193 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f431.png
+-rw-r--r--   0        0        0     4538 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f432.png
+-rw-r--r--   0        0        0     2468 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f433.png
+-rw-r--r--   0        0        0     2249 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f434.png
+-rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f435.png
+-rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f436.png
+-rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f437.png
+-rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f438.png
+-rw-r--r--   0        0        0     2911 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f439.png
+-rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43a.png
+-rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43b.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43b_200d_2744_fe0f.png
+-rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43c.png
+-rw-r--r--   0        0        0     1528 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43d.png
+-rw-r--r--   0        0        0      771 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43e.png
+-rw-r--r--   0        0        0     3248 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f43f.png
+-rw-r--r--   0        0        0     1237 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f440.png
+-rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f441.png
+-rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f441_fe0f_200d_1f5e8_fe0f.png
+-rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f442.png
+-rw-r--r--   0        0        0     1094 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f443.png
+-rw-r--r--   0        0        0     1491 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f444.png
+-rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f445.png
+-rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f446.png
+-rw-r--r--   0        0        0     1039 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f447.png
+-rw-r--r--   0        0        0      972 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f448.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f449.png
+-rw-r--r--   0        0        0     1180 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f44a.png
+-rw-r--r--   0        0        0     1977 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f44b.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f44c.png
+-rw-r--r--   0        0        0     1454 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f44d.png
+-rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f44e.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f44f.png
+-rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f450.png
+-rw-r--r--   0        0        0     3262 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f451.png
+-rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f452.png
+-rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f453.png
+-rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f454.png
+-rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f455.png
+-rw-r--r--   0        0        0     2568 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f456.png
+-rw-r--r--   0        0        0     1811 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f457.png
+-rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f458.png
+-rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f459.png
+-rw-r--r--   0        0        0     1671 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f45a.png
+-rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f45b.png
+-rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f45c.png
+-rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f45d.png
+-rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f45e.png
+-rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f45f.png
+-rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f460.png
+-rw-r--r--   0        0        0     1465 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f461.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f462.png
+-rw-r--r--   0        0        0      806 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f463.png
+-rw-r--r--   0        0        0      905 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f464.png
+-rw-r--r--   0        0        0     1012 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f465.png
+-rw-r--r--   0        0        0     2126 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f466.png
+-rw-r--r--   0        0        0     2215 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f467.png
+-rw-r--r--   0        0        0     2023 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468.png
+-rw-r--r--   0        0        0     4097 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f33e.png
+-rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f373.png
+-rw-r--r--   0        0        0     2948 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f37c.png
+-rw-r--r--   0        0        0     2403 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f393.png
+-rw-r--r--   0        0        0     3325 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f3a4.png
+-rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f3a8.png
+-rw-r--r--   0        0        0     2669 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f3eb.png
+-rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f3ed.png
+-rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f466.png
+-rw-r--r--   0        0        0     2694 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f467.png
+-rw-r--r--   0        0        0     3625 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     3062 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466.png
+-rw-r--r--   0        0        0     4079 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     3727 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467.png
+-rw-r--r--   0        0        0     4567 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     4614 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     3437 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466.png
+-rw-r--r--   0        0        0     4310 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     3696 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467.png
+-rw-r--r--   0        0        0     4734 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     4600 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f4bb.png
+-rw-r--r--   0        0        0     2409 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f4bc.png
+-rw-r--r--   0        0        0     3178 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f527.png
+-rw-r--r--   0        0        0     3350 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f52c.png
+-rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f680.png
+-rw-r--r--   0        0        0     3740 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f692.png
+-rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9af.png
+-rw-r--r--   0        0        0     2081 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9b0.png
+-rw-r--r--   0        0        0     2301 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9b1.png
+-rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9b2.png
+-rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9b3.png
+-rw-r--r--   0        0        0     3029 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9bc.png
+-rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_1f9bd.png
+-rw-r--r--   0        0        0     2561 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_2695_fe0f.png
+-rw-r--r--   0        0        0     2680 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_2696_fe0f.png
+-rw-r--r--   0        0        0     2660 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_2708_fe0f.png
+-rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f468.png
+-rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f48b_200d_1f468.png
+-rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469.png
+-rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f33e.png
+-rw-r--r--   0        0        0     3312 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f373.png
+-rw-r--r--   0        0        0     2951 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f37c.png
+-rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f393.png
+-rw-r--r--   0        0        0     3648 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f3a4.png
+-rw-r--r--   0        0        0     3778 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f3a8.png
+-rw-r--r--   0        0        0     2988 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f3eb.png
+-rw-r--r--   0        0        0     3394 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f3ed.png
+-rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f466.png
+-rw-r--r--   0        0        0     2793 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f467.png
+-rw-r--r--   0        0        0     3700 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     3363 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466.png
+-rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     3860 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467.png
+-rw-r--r--   0        0        0     4626 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     4582 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     2002 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f4bb.png
+-rw-r--r--   0        0        0     2411 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f4bc.png
+-rw-r--r--   0        0        0     3131 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f527.png
+-rw-r--r--   0        0        0     3659 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f52c.png
+-rw-r--r--   0        0        0     3150 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f680.png
+-rw-r--r--   0        0        0     3773 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f692.png
+-rw-r--r--   0        0        0     2532 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9af.png
+-rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9b0.png
+-rw-r--r--   0        0        0     2744 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9b1.png
+-rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9b2.png
+-rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9b3.png
+-rw-r--r--   0        0        0     3044 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9bc.png
+-rw-r--r--   0        0        0     2575 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_1f9bd.png
+-rw-r--r--   0        0        0     2722 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2695_fe0f.png
+-rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2696_fe0f.png
+-rw-r--r--   0        0        0     2931 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2708_fe0f.png
+-rw-r--r--   0        0        0     3634 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f468.png
+-rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f469.png
+-rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f468.png
+-rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f469.png
+-rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46a.png
+-rw-r--r--   0        0        0     3563 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46b.png
+-rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46c.png
+-rw-r--r--   0        0        0     3729 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46d.png
+-rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46e.png
+-rw-r--r--   0        0        0     3026 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46e_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3184 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46e_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46f.png
+-rw-r--r--   0        0        0     3282 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f46f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2859 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f470.png
+-rw-r--r--   0        0        0     2914 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f470_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2994 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f470_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2408 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f471.png
+-rw-r--r--   0        0        0     2558 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f471_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f471_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2225 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f472.png
+-rw-r--r--   0        0        0     2279 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f473.png
+-rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f473_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f473_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f474.png
+-rw-r--r--   0        0        0     2445 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f475.png
+-rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f476.png
+-rw-r--r--   0        0        0     3221 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f477.png
+-rw-r--r--   0        0        0     3455 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f477_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3157 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f477_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2492 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f478.png
+-rw-r--r--   0        0        0     3442 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f479.png
+-rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f47a.png
+-rw-r--r--   0        0        0     2131 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f47b.png
+-rw-r--r--   0        0        0     2657 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f47c.png
+-rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f47d.png
+-rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f47e.png
+-rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f47f.png
+-rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f480.png
+-rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f481.png
+-rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f481_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2232 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f481_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f482.png
+-rw-r--r--   0        0        0     2451 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f482_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f482_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3554 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f483.png
+-rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f484.png
+-rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f485.png
+-rw-r--r--   0        0        0     2577 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f486.png
+-rw-r--r--   0        0        0     2578 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f486_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f486_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2902 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f487.png
+-rw-r--r--   0        0        0     3136 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f487_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2768 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f487_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f488.png
+-rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f489.png
+-rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f48a.png
+-rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f48b.png
+-rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f48c.png
+-rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f48d.png
+-rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f48e.png
+-rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f48f.png
+-rw-r--r--   0        0        0    13813 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f490.png
+-rw-r--r--   0        0        0     3493 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f491.png
+-rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f492.png
+-rw-r--r--   0        0        0     1344 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f493.png
+-rw-r--r--   0        0        0     1561 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f494.png
+-rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f495.png
+-rw-r--r--   0        0        0     2111 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f496.png
+-rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f497.png
+-rw-r--r--   0        0        0     1985 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f498.png
+-rw-r--r--   0        0        0     1130 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f499.png
+-rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f49a.png
+-rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f49b.png
+-rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f49c.png
+-rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f49d.png
+-rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f49e.png
+-rw-r--r--   0        0        0     1082 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f49f.png
+-rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a0.png
+-rw-r--r--   0        0        0     1218 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a1.png
+-rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a2.png
+-rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a3.png
+-rw-r--r--   0        0        0      663 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a4.png
+-rw-r--r--   0        0        0     2101 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a5.png
+-rw-r--r--   0        0        0     1905 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a6.png
+-rw-r--r--   0        0        0     1268 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a7.png
+-rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a8.png
+-rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4a9.png
+-rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4aa.png
+-rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ab.png
+-rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ac.png
+-rw-r--r--   0        0        0     1370 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ad.png
+-rw-r--r--   0        0        0     1790 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ae.png
+-rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4af.png
+-rw-r--r--   0        0        0     2079 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b0.png
+-rw-r--r--   0        0        0      996 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b1.png
+-rw-r--r--   0        0        0      731 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b2.png
+-rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b3.png
+-rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b4.png
+-rw-r--r--   0        0        0     2022 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b5.png
+-rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b6.png
+-rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b7.png
+-rw-r--r--   0        0        0     3067 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b8.png
+-rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4b9.png
+-rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ba.png
+-rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4bb.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4bc.png
+-rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4bd.png
+-rw-r--r--   0        0        0      907 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4be.png
+-rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4bf.png
+-rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c0.png
+-rw-r--r--   0        0        0     1335 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c1.png
+-rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c2.png
+-rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c3.png
+-rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c4.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c5.png
+-rw-r--r--   0        0        0     1568 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c6.png
+-rw-r--r--   0        0        0     2054 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c7.png
+-rw-r--r--   0        0        0     1861 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c8.png
+-rw-r--r--   0        0        0     1762 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4c9.png
+-rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ca.png
+-rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4cb.png
+-rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4cc.png
+-rw-r--r--   0        0        0     1466 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4cd.png
+-rw-r--r--   0        0        0     2382 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ce.png
+-rw-r--r--   0        0        0      803 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4cf.png
+-rw-r--r--   0        0        0      935 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d0.png
+-rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d1.png
+-rw-r--r--   0        0        0     2351 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d2.png
+-rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d3.png
+-rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d4.png
+-rw-r--r--   0        0        0     1593 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d5.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d6.png
+-rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d7.png
+-rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d8.png
+-rw-r--r--   0        0        0     1807 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4d9.png
+-rw-r--r--   0        0        0     2567 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4da.png
+-rw-r--r--   0        0        0     1381 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4db.png
+-rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4dc.png
+-rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4dd.png
+-rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4de.png
+-rw-r--r--   0        0        0     1650 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4df.png
+-rw-r--r--   0        0        0     1045 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e0.png
+-rw-r--r--   0        0        0     2446 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e1.png
+-rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e2.png
+-rw-r--r--   0        0        0     2230 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e3.png
+-rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e4.png
+-rw-r--r--   0        0        0     1396 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e5.png
+-rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e6.png
+-rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e7.png
+-rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e8.png
+-rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4e9.png
+-rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ea.png
+-rw-r--r--   0        0        0     2096 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4eb.png
+-rw-r--r--   0        0        0     2146 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ec.png
+-rw-r--r--   0        0        0     1703 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ed.png
+-rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ee.png
+-rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ef.png
+-rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f0.png
+-rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f1.png
+-rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f2.png
+-rw-r--r--   0        0        0     1436 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f3.png
+-rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f4.png
+-rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f5.png
+-rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f6.png
+-rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f7.png
+-rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f8.png
+-rw-r--r--   0        0        0     1917 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4f9.png
+-rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4fa.png
+-rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4fb.png
+-rw-r--r--   0        0        0     1155 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4fc.png
+-rw-r--r--   0        0        0     2361 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4fd.png
+-rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f4ff.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f500.png
+-rw-r--r--   0        0        0     1196 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f501.png
+-rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f502.png
+-rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f503.png
+-rw-r--r--   0        0        0     1313 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f504.png
+-rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f505.png
+-rw-r--r--   0        0        0     1611 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f506.png
+-rw-r--r--   0        0        0     2099 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f507.png
+-rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f508.png
+-rw-r--r--   0        0        0     2513 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f509.png
+-rw-r--r--   0        0        0     3375 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f50a.png
+-rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f50b.png
+-rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f50c.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f50d.png
+-rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f50e.png
+-rw-r--r--   0        0        0     2493 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f50f.png
+-rw-r--r--   0        0        0     2190 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f510.png
+-rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f511.png
+-rw-r--r--   0        0        0     1356 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f512.png
+-rw-r--r--   0        0        0     1472 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f513.png
+-rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f514.png
+-rw-r--r--   0        0        0     2107 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f515.png
+-rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f516.png
+-rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f517.png
+-rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f518.png
+-rw-r--r--   0        0        0     1003 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f519.png
+-rw-r--r--   0        0        0      723 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f51a.png
+-rw-r--r--   0        0        0      949 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f51b.png
+-rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f51c.png
+-rw-r--r--   0        0        0      731 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f51d.png
+-rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f51e.png
+-rw-r--r--   0        0        0     1156 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f51f.png
+-rw-r--r--   0        0        0     1441 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f520.png
+-rw-r--r--   0        0        0     1340 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f521.png
+-rw-r--r--   0        0        0     1353 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f522.png
+-rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f523.png
+-rw-r--r--   0        0        0     1160 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f524.png
+-rw-r--r--   0        0        0     2128 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f525.png
+-rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f526.png
+-rw-r--r--   0        0        0     1216 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f527.png
+-rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f528.png
+-rw-r--r--   0        0        0     1853 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f529.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f52a.png
+-rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f52b.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f52c.png
+-rw-r--r--   0        0        0     2039 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f52d.png
+-rw-r--r--   0        0        0     3144 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f52e.png
+-rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f52f.png
+-rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f530.png
+-rw-r--r--   0        0        0     2726 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f531.png
+-rw-r--r--   0        0        0      733 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f532.png
+-rw-r--r--   0        0        0      531 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f533.png
+-rw-r--r--   0        0        0      961 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f534.png
+-rw-r--r--   0        0        0      952 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f535.png
+-rw-r--r--   0        0        0      780 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f536.png
+-rw-r--r--   0        0        0      847 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f537.png
+-rw-r--r--   0        0        0      668 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f538.png
+-rw-r--r--   0        0        0      719 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f539.png
+-rw-r--r--   0        0        0      566 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f53a.png
+-rw-r--r--   0        0        0      654 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f53b.png
+-rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f53c.png
+-rw-r--r--   0        0        0      972 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f53d.png
+-rw-r--r--   0        0        0     1553 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f549.png
+-rw-r--r--   0        0        0     1919 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f54a.png
+-rw-r--r--   0        0        0     1294 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f54b.png
+-rw-r--r--   0        0        0     2786 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f54c.png
+-rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f54d.png
+-rw-r--r--   0        0        0     1663 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f54e.png
+-rw-r--r--   0        0        0     1700 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f550.png
+-rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f551.png
+-rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f552.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f553.png
+-rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f554.png
+-rw-r--r--   0        0        0     1687 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f555.png
+-rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f556.png
+-rw-r--r--   0        0        0     1767 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f557.png
+-rw-r--r--   0        0        0     1635 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f558.png
+-rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f559.png
+-rw-r--r--   0        0        0     1720 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f55a.png
+-rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f55b.png
+-rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f55c.png
+-rw-r--r--   0        0        0     1707 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f55d.png
+-rw-r--r--   0        0        0     1648 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f55e.png
+-rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f55f.png
+-rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f560.png
+-rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f561.png
+-rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f562.png
+-rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f563.png
+-rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f564.png
+-rw-r--r--   0        0        0     1619 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f565.png
+-rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f566.png
+-rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f567.png
+-rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f56f.png
+-rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f570.png
+-rw-r--r--   0        0        0      714 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f573.png
+-rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f574.png
+-rw-r--r--   0        0        0     3208 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f575.png
+-rw-r--r--   0        0        0     3188 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0      841 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f576.png
+-rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f577.png
+-rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f578.png
+-rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f579.png
+-rw-r--r--   0        0        0     2299 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f57a.png
+-rw-r--r--   0        0        0     3424 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f587.png
+-rw-r--r--   0        0        0     1232 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f58a.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f58b.png
+-rw-r--r--   0        0        0     1928 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f58c.png
+-rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f58d.png
+-rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f590.png
+-rw-r--r--   0        0        0      871 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f595.png
+-rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f596.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5a4.png
+-rw-r--r--   0        0        0      973 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5a5.png
+-rw-r--r--   0        0        0     1403 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5a8.png
+-rw-r--r--   0        0        0      761 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5b1.png
+-rw-r--r--   0        0        0     1783 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5b2.png
+-rw-r--r--   0        0        0     2515 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5bc.png
+-rw-r--r--   0        0        0      831 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5c2.png
+-rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5c3.png
+-rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5c4.png
+-rw-r--r--   0        0        0     4755 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5d1.png
+-rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5d2.png
+-rw-r--r--   0        0        0     2281 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5d3.png
+-rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5dc.png
+-rw-r--r--   0        0        0     1484 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5dd.png
+-rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5de.png
+-rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5e1.png
+-rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5e3.png
+-rw-r--r--   0        0        0      839 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5e8.png
+-rw-r--r--   0        0        0     1569 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5ef.png
+-rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5f3.png
+-rw-r--r--   0        0        0     4392 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5fa.png
+-rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5fb.png
+-rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5fc.png
+-rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5fd.png
+-rw-r--r--   0        0        0     1010 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5fe.png
+-rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f5ff.png
+-rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f600.png
+-rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f601.png
+-rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f602.png
+-rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f603.png
+-rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f604.png
+-rw-r--r--   0        0        0     2690 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f605.png
+-rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f606.png
+-rw-r--r--   0        0        0     3349 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f607.png
+-rw-r--r--   0        0        0     2347 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f608.png
+-rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f609.png
+-rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f60a.png
+-rw-r--r--   0        0        0     2305 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f60b.png
+-rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f60c.png
+-rw-r--r--   0        0        0     2417 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f60d.png
+-rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f60e.png
+-rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f60f.png
+-rw-r--r--   0        0        0     1777 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f610.png
+-rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f611.png
+-rw-r--r--   0        0        0     1865 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f612.png
+-rw-r--r--   0        0        0     2480 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f613.png
+-rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f614.png
+-rw-r--r--   0        0        0     1847 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f615.png
+-rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f616.png
+-rw-r--r--   0        0        0     1878 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f617.png
+-rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f618.png
+-rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f619.png
+-rw-r--r--   0        0        0     2040 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f61a.png
+-rw-r--r--   0        0        0     2093 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f61b.png
+-rw-r--r--   0        0        0     2563 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f61c.png
+-rw-r--r--   0        0        0     2292 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f61d.png
+-rw-r--r--   0        0        0     1764 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f61e.png
+-rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f61f.png
+-rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f620.png
+-rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f621.png
+-rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f622.png
+-rw-r--r--   0        0        0     1947 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f623.png
+-rw-r--r--   0        0        0     3109 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f624.png
+-rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f625.png
+-rw-r--r--   0        0        0     1691 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f626.png
+-rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f627.png
+-rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f628.png
+-rw-r--r--   0        0        0     2300 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f629.png
+-rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62a.png
+-rw-r--r--   0        0        0     2376 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62b.png
+-rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62c.png
+-rw-r--r--   0        0        0     2464 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62d.png
+-rw-r--r--   0        0        0     1681 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62e.png
+-rw-r--r--   0        0        0     3413 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62e_200d_1f4a8.png
+-rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f62f.png
+-rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f630.png
+-rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f631.png
+-rw-r--r--   0        0        0     2122 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f632.png
+-rw-r--r--   0        0        0     2367 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f633.png
+-rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f634.png
+-rw-r--r--   0        0        0     2059 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f635.png
+-rw-r--r--   0        0        0     3751 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f635_200d_1f4ab.png
+-rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f636.png
+-rw-r--r--   0        0        0     4477 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f636_200d_1f32b_fe0f.png
+-rw-r--r--   0        0        0     2431 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f637.png
+-rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f638.png
+-rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f639.png
+-rw-r--r--   0        0        0     2628 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f63a.png
+-rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f63b.png
+-rw-r--r--   0        0        0     2509 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f63c.png
+-rw-r--r--   0        0        0     2625 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f63d.png
+-rw-r--r--   0        0        0     2423 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f63e.png
+-rw-r--r--   0        0        0     2830 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f63f.png
+-rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f640.png
+-rw-r--r--   0        0        0     1784 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f641.png
+-rw-r--r--   0        0        0     1841 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f642.png
+-rw-r--r--   0        0        0     1804 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f643.png
+-rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f644.png
+-rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f645.png
+-rw-r--r--   0        0        0     2860 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f645_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3058 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f645_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3132 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f646.png
+-rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f646_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3260 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f646_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f647.png
+-rw-r--r--   0        0        0     2862 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f647_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2829 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f647_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f648.png
+-rw-r--r--   0        0        0     2640 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f649.png
+-rw-r--r--   0        0        0     2350 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64a.png
+-rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64b.png
+-rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64b_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2406 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64b_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1918 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64c.png
+-rw-r--r--   0        0        0     2133 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64d.png
+-rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64d_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1984 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64d_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2123 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64e.png
+-rw-r--r--   0        0        0     2383 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64e_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64e_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1910 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f64f.png
+-rw-r--r--   0        0        0     3216 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f680.png
+-rw-r--r--   0        0        0     3045 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f681.png
+-rw-r--r--   0        0        0     3402 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f682.png
+-rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f683.png
+-rw-r--r--   0        0        0     2088 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f684.png
+-rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f685.png
+-rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f686.png
+-rw-r--r--   0        0        0     2168 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f687.png
+-rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f688.png
+-rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f689.png
+-rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f68a.png
+-rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f68b.png
+-rw-r--r--   0        0        0     2469 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f68c.png
+-rw-r--r--   0        0        0     2164 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f68d.png
+-rw-r--r--   0        0        0     3075 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f68e.png
+-rw-r--r--   0        0        0     1852 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f68f.png
+-rw-r--r--   0        0        0     2315 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f690.png
+-rw-r--r--   0        0        0     2769 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f691.png
+-rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f692.png
+-rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f693.png
+-rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f694.png
+-rw-r--r--   0        0        0     3166 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f695.png
+-rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f696.png
+-rw-r--r--   0        0        0     2501 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f697.png
+-rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f698.png
+-rw-r--r--   0        0        0     2429 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f699.png
+-rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f69a.png
+-rw-r--r--   0        0        0     2309 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f69b.png
+-rw-r--r--   0        0        0     2980 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f69c.png
+-rw-r--r--   0        0        0     1988 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f69d.png
+-rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f69e.png
+-rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f69f.png
+-rw-r--r--   0        0        0     2526 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a0.png
+-rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a1.png
+-rw-r--r--   0        0        0     2413 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a2.png
+-rw-r--r--   0        0        0     1966 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a3.png
+-rw-r--r--   0        0        0     2262 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a3_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a3_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2041 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a4.png
+-rw-r--r--   0        0        0     1795 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a5.png
+-rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a6.png
+-rw-r--r--   0        0        0     2554 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a7.png
+-rw-r--r--   0        0        0     2975 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a8.png
+-rw-r--r--   0        0        0      917 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6a9.png
+-rw-r--r--   0        0        0      951 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6aa.png
+-rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ab.png
+-rw-r--r--   0        0        0     1543 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ac.png
+-rw-r--r--   0        0        0     1875 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ad.png
+-rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ae.png
+-rw-r--r--   0        0        0     1929 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6af.png
+-rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b0.png
+-rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b1.png
+-rw-r--r--   0        0        0     2702 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b2.png
+-rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b3.png
+-rw-r--r--   0        0        0     3994 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b4.png
+-rw-r--r--   0        0        0     3960 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b4_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3931 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b4_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b5.png
+-rw-r--r--   0        0        0     4684 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b5_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     4495 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b5_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b6.png
+-rw-r--r--   0        0        0     2212 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b6_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b6_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2018 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b7.png
+-rw-r--r--   0        0        0     1190 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b8.png
+-rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6b9.png
+-rw-r--r--   0        0        0     1170 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ba.png
+-rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6bb.png
+-rw-r--r--   0        0        0     1188 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6bc.png
+-rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6bd.png
+-rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6be.png
+-rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6bf.png
+-rw-r--r--   0        0        0     2399 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6c0.png
+-rw-r--r--   0        0        0     2784 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6c1.png
+-rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6c2.png
+-rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6c3.png
+-rw-r--r--   0        0        0     1089 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6c4.png
+-rw-r--r--   0        0        0     1292 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6c5.png
+-rw-r--r--   0        0        0     1881 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6cb.png
+-rw-r--r--   0        0        0     1564 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6cc.png
+-rw-r--r--   0        0        0     4037 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6cd.png
+-rw-r--r--   0        0        0     2362 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ce.png
+-rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6cf.png
+-rw-r--r--   0        0        0     1220 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6d0.png
+-rw-r--r--   0        0        0      875 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6d1.png
+-rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6d2.png
+-rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6d5.png
+-rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6d6.png
+-rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6d7.png
+-rw-r--r--   0        0        0     8111 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6dd.png
+-rw-r--r--   0        0        0     4305 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6de.png
+-rw-r--r--   0        0        0     3886 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6df.png
+-rw-r--r--   0        0        0     2317 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e0.png
+-rw-r--r--   0        0        0     1601 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e1.png
+-rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e2.png
+-rw-r--r--   0        0        0     2352 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e3.png
+-rw-r--r--   0        0        0     3595 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e4.png
+-rw-r--r--   0        0        0     2267 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e5.png
+-rw-r--r--   0        0        0     2443 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6e9.png
+-rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6eb.png
+-rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6ec.png
+-rw-r--r--   0        0        0     3617 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f0.png
+-rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f3.png
+-rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f4.png
+-rw-r--r--   0        0        0     3308 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f5.png
+-rw-r--r--   0        0        0     1926 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f6.png
+-rw-r--r--   0        0        0     2647 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f7.png
+-rw-r--r--   0        0        0     1416 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f8.png
+-rw-r--r--   0        0        0     1452 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6f9.png
+-rw-r--r--   0        0        0     3549 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6fa.png
+-rw-r--r--   0        0        0     1981 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6fb.png
+-rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f6fc.png
+-rw-r--r--   0        0        0      911 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e0.png
+-rw-r--r--   0        0        0      949 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e1.png
+-rw-r--r--   0        0        0      857 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e2.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e3.png
+-rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e4.png
+-rw-r--r--   0        0        0      630 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e5.png
+-rw-r--r--   0        0        0      544 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e6.png
+-rw-r--r--   0        0        0      486 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e7.png
+-rw-r--r--   0        0        0      695 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e8.png
+-rw-r--r--   0        0        0      568 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7e9.png
+-rw-r--r--   0        0        0      537 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7ea.png
+-rw-r--r--   0        0        0      534 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7eb.png
+-rw-r--r--   0        0        0      335 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f7f0.png
+-rw-r--r--   0        0        0     1468 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f90c.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f90d.png
+-rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f90e.png
+-rw-r--r--   0        0        0     1031 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f90f.png
+-rw-r--r--   0        0        0     2728 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f910.png
+-rw-r--r--   0        0        0     2691 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f911.png
+-rw-r--r--   0        0        0     2684 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f912.png
+-rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f913.png
+-rw-r--r--   0        0        0     2157 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f914.png
+-rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f915.png
+-rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f916.png
+-rw-r--r--   0        0        0     2530 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f917.png
+-rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f918.png
+-rw-r--r--   0        0        0     1397 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f919.png
+-rw-r--r--   0        0        0     1383 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f91a.png
+-rw-r--r--   0        0        0     1239 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f91b.png
+-rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f91c.png
+-rw-r--r--   0        0        0     1399 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f91d.png
+-rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f91e.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f91f.png
+-rw-r--r--   0        0        0     2550 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f920.png
+-rw-r--r--   0        0        0     3526 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f921.png
+-rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f922.png
+-rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.336582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f923.png
+-rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f924.png
+-rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f925.png
+-rw-r--r--   0        0        0     2211 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f926.png
+-rw-r--r--   0        0        0     2487 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f926_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2222 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f926_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2604 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f927.png
+-rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f928.png
+-rw-r--r--   0        0        0     3007 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f929.png
+-rw-r--r--   0        0        0     2941 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f92a.png
+-rw-r--r--   0        0        0     2316 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f92b.png
+-rw-r--r--   0        0        0     2135 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f92c.png
+-rw-r--r--   0        0        0     2253 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f92d.png
+-rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f92e.png
+-rw-r--r--   0        0        0     3562 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f92f.png
+-rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f930.png
+-rw-r--r--   0        0        0     2852 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f931.png
+-rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f932.png
+-rw-r--r--   0        0        0     1585 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f933.png
+-rw-r--r--   0        0        0     3154 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f934.png
+-rw-r--r--   0        0        0     2265 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f935.png
+-rw-r--r--   0        0        0     2536 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f935_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2112 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f935_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2791 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f936.png
+-rw-r--r--   0        0        0     2649 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f937.png
+-rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f937_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2398 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f937_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f938.png
+-rw-r--r--   0        0        0     2235 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f938_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2155 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f938_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3423 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f939.png
+-rw-r--r--   0        0        0     3506 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f939_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3465 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f939_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93a.png
+-rw-r--r--   0        0        0     3981 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93c.png
+-rw-r--r--   0        0        0     3878 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93c_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3927 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93c_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93d.png
+-rw-r--r--   0        0        0     3287 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93d_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2618 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93d_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93e.png
+-rw-r--r--   0        0        0     3042 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93e_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3126 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93e_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f93f.png
+-rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f940.png
+-rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f941.png
+-rw-r--r--   0        0        0     2319 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f942.png
+-rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f943.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f944.png
+-rw-r--r--   0        0        0     2674 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f945.png
+-rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f947.png
+-rw-r--r--   0        0        0     1808 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f948.png
+-rw-r--r--   0        0        0     2087 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f949.png
+-rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f94a.png
+-rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f94b.png
+-rw-r--r--   0        0        0     2270 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f94c.png
+-rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f94d.png
+-rw-r--r--   0        0        0     2622 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f94e.png
+-rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f94f.png
+-rw-r--r--   0        0        0     2311 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f950.png
+-rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f951.png
+-rw-r--r--   0        0        0     2890 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f952.png
+-rw-r--r--   0        0        0     2832 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f953.png
+-rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f954.png
+-rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f955.png
+-rw-r--r--   0        0        0     1414 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f956.png
+-rw-r--r--   0        0        0     4262 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f957.png
+-rw-r--r--   0        0        0     3316 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f958.png
+-rw-r--r--   0        0        0     2853 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f959.png
+-rw-r--r--   0        0        0     1015 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f95a.png
+-rw-r--r--   0        0        0     1727 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f95b.png
+-rw-r--r--   0        0        0     3624 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f95c.png
+-rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f95d.png
+-rw-r--r--   0        0        0     2837 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f95e.png
+-rw-r--r--   0        0        0     2009 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f95f.png
+-rw-r--r--   0        0        0     1509 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f960.png
+-rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f961.png
+-rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f962.png
+-rw-r--r--   0        0        0     1504 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f963.png
+-rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f964.png
+-rw-r--r--   0        0        0     2092 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f965.png
+-rw-r--r--   0        0        0     2813 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f966.png
+-rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f967.png
+-rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f968.png
+-rw-r--r--   0        0        0     2651 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f969.png
+-rw-r--r--   0        0        0     2666 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f96a.png
+-rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f96b.png
+-rw-r--r--   0        0        0     3117 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f96c.png
+-rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f96d.png
+-rw-r--r--   0        0        0     2615 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f96e.png
+-rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f96f.png
+-rw-r--r--   0        0        0     2696 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f970.png
+-rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f971.png
+-rw-r--r--   0        0        0     2349 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f972.png
+-rw-r--r--   0        0        0     3929 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f973.png
+-rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f974.png
+-rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f975.png
+-rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f976.png
+-rw-r--r--   0        0        0     2065 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f977.png
+-rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f978.png
+-rw-r--r--   0        0        0     3326 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f979.png
+-rw-r--r--   0        0        0     2404 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f97a.png
+-rw-r--r--   0        0        0     1975 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f97b.png
+-rw-r--r--   0        0        0     1541 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f97c.png
+-rw-r--r--   0        0        0     2260 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f97d.png
+-rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f97e.png
+-rw-r--r--   0        0        0      996 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f97f.png
+-rw-r--r--   0        0        0     3907 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f980.png
+-rw-r--r--   0        0        0     3404 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f981.png
+-rw-r--r--   0        0        0     2013 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f982.png
+-rw-r--r--   0        0        0     3489 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f983.png
+-rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f984.png
+-rw-r--r--   0        0        0     2600 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f985.png
+-rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f986.png
+-rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f987.png
+-rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f988.png
+-rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f989.png
+-rw-r--r--   0        0        0     2522 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f98a.png
+-rw-r--r--   0        0        0     2937 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f98b.png
+-rw-r--r--   0        0        0     2432 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f98c.png
+-rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f98d.png
+-rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f98e.png
+-rw-r--r--   0        0        0     1713 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f98f.png
+-rw-r--r--   0        0        0     4212 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f990.png
+-rw-r--r--   0        0        0     4058 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f991.png
+-rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f992.png
+-rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f993.png
+-rw-r--r--   0        0        0     2587 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f994.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f995.png
+-rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f996.png
+-rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f997.png
+-rw-r--r--   0        0        0     1932 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f998.png
+-rw-r--r--   0        0        0     1793 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f999.png
+-rw-r--r--   0        0        0     4253 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f99a.png
+-rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f99b.png
+-rw-r--r--   0        0        0     2652 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f99c.png
+-rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f99d.png
+-rw-r--r--   0        0        0     3170 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f99e.png
+-rw-r--r--   0        0        0     3035 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f99f.png
+-rw-r--r--   0        0        0     3160 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a0.png
+-rw-r--r--   0        0        0     1386 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a1.png
+-rw-r--r--   0        0        0     1745 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a2.png
+-rw-r--r--   0        0        0     1946 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a3.png
+-rw-r--r--   0        0        0     2772 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a4.png
+-rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a5.png
+-rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a6.png
+-rw-r--r--   0        0        0     2603 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a7.png
+-rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a8.png
+-rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9a9.png
+-rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9aa.png
+-rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.372583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ab.png
+-rw-r--r--   0        0        0     1659 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ac.png
+-rw-r--r--   0        0        0     1328 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ad.png
+-rw-r--r--   0        0        0     3191 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ae.png
+-rw-r--r--   0        0        0      801 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9af.png
+-rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b0.png
+-rw-r--r--   0        0        0     1559 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b1.png
+-rw-r--r--   0        0        0      833 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b2.png
+-rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b3.png
+-rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b4.png
+-rw-r--r--   0        0        0      921 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b5.png
+-rw-r--r--   0        0        0     1240 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b6.png
+-rw-r--r--   0        0        0     1290 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b7.png
+-rw-r--r--   0        0        0     3429 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b8.png
+-rw-r--r--   0        0        0     3693 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b8_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3512 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b8_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3996 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b9.png
+-rw-r--r--   0        0        0     4529 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b9_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3957 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9b9_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ba.png
+-rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9bb.png
+-rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9bc.png
+-rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9bd.png
+-rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9be.png
+-rw-r--r--   0        0        0     1429 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9bf.png
+-rw-r--r--   0        0        0     1368 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c0.png
+-rw-r--r--   0        0        0     3498 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c1.png
+-rw-r--r--   0        0        0     1692 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c2.png
+-rw-r--r--   0        0        0     1825 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c3.png
+-rw-r--r--   0        0        0     1754 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c4.png
+-rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c5.png
+-rw-r--r--   0        0        0     2313 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c6.png
+-rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c7.png
+-rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c8.png
+-rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9c9.png
+-rw-r--r--   0        0        0     2521 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ca.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cb.png
+-rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cc.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cd.png
+-rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cd_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cd_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ce.png
+-rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ce_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ce_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cf.png
+-rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cf_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9cf_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d0.png
+-rw-r--r--   0        0        0     2148 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1.png
+-rw-r--r--   0        0        0     4085 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f33e.png
+-rw-r--r--   0        0        0     3096 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f373.png
+-rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f37c.png
+-rw-r--r--   0        0        0     3304 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f384.png
+-rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f393.png
+-rw-r--r--   0        0        0     3162 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a4.png
+-rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a8.png
+-rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3eb.png
+-rw-r--r--   0        0        0     3277 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3ed.png
+-rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bb.png
+-rw-r--r--   0        0        0     2284 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bc.png
+-rw-r--r--   0        0        0     3264 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f527.png
+-rw-r--r--   0        0        0     3470 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f52c.png
+-rw-r--r--   0        0        0     3285 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f680.png
+-rw-r--r--   0        0        0     3739 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f692.png
+-rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f91d_200d_1f9d1.png
+-rw-r--r--   0        0        0     2547 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9af.png
+-rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b0.png
+-rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b1.png
+-rw-r--r--   0        0        0     1800 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b2.png
+-rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b3.png
+-rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bc.png
+-rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bd.png
+-rw-r--r--   0        0        0     2529 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_2695_fe0f.png
+-rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_2696_fe0f.png
+-rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d1_200d_2708_fe0f.png
+-rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d2.png
+-rw-r--r--   0        0        0     2801 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d3.png
+-rw-r--r--   0        0        0     2178 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d4.png
+-rw-r--r--   0        0        0     4333 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d4_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3689 2022-11-18 15:36:28.352583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d4_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2258 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d5.png
+-rw-r--r--   0        0        0     3176 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d6.png
+-rw-r--r--   0        0        0     3180 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d6_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d6_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3412 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d7.png
+-rw-r--r--   0        0        0     3963 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d7_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3608 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d7_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d8.png
+-rw-r--r--   0        0        0     2189 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d8_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d8_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3401 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d9.png
+-rw-r--r--   0        0        0     3318 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d9_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3327 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9d9_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2627 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9da.png
+-rw-r--r--   0        0        0     3146 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9da_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2586 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9da_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2949 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9db.png
+-rw-r--r--   0        0        0     3078 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9db_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3077 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9db_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3533 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9dc.png
+-rw-r--r--   0        0        0     3786 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9dc_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3488 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9dc_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3089 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9dd.png
+-rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9dd_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9dd_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9de.png
+-rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9de_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2841 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9de_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2737 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9df.png
+-rw-r--r--   0        0        0     2739 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9df_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2760 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9df_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2467 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e0.png
+-rw-r--r--   0        0        0     1175 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e1.png
+-rw-r--r--   0        0        0     1084 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e2.png
+-rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e3.png
+-rw-r--r--   0        0        0     1581 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e4.png
+-rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e5.png
+-rw-r--r--   0        0        0     1914 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e6.png
+-rw-r--r--   0        0        0     1351 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e7.png
+-rw-r--r--   0        0        0     2523 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e8.png
+-rw-r--r--   0        0        0     1911 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9e9.png
+-rw-r--r--   0        0        0     2524 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ea.png
+-rw-r--r--   0        0        0     1718 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9eb.png
+-rw-r--r--   0        0        0     3148 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ec.png
+-rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ed.png
+-rw-r--r--   0        0        0     3580 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ee.png
+-rw-r--r--   0        0        0     3068 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ef.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f0.png
+-rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f1.png
+-rw-r--r--   0        0        0     1816 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f2.png
+-rw-r--r--   0        0        0     2325 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f3.png
+-rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f4.png
+-rw-r--r--   0        0        0     2571 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f5.png
+-rw-r--r--   0        0        0     2874 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f6.png
+-rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f7.png
+-rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f8.png
+-rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9f9.png
+-rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9fa.png
+-rw-r--r--   0        0        0     1623 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9fb.png
+-rw-r--r--   0        0        0     2401 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9fc.png
+-rw-r--r--   0        0        0     2080 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9fd.png
+-rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9fe.png
+-rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1f9ff.png
+-rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa70.png
+-rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa71.png
+-rw-r--r--   0        0        0     1002 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa72.png
+-rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa73.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa74.png
+-rw-r--r--   0        0        0     1146 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa78.png
+-rw-r--r--   0        0        0     1312 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa79.png
+-rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa7a.png
+-rw-r--r--   0        0        0     4290 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa7b.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa7c.png
+-rw-r--r--   0        0        0     2378 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa80.png
+-rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa81.png
+-rw-r--r--   0        0        0     3182 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa82.png
+-rw-r--r--   0        0        0     1651 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa83.png
+-rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa84.png
+-rw-r--r--   0        0        0     9582 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa85.png
+-rw-r--r--   0        0        0     3331 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa86.png
+-rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa90.png
+-rw-r--r--   0        0        0     1145 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa91.png
+-rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa92.png
+-rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa93.png
+-rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa94.png
+-rw-r--r--   0        0        0     1644 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa95.png
+-rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa96.png
+-rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa97.png
+-rw-r--r--   0        0        0     1906 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa98.png
+-rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa99.png
+-rw-r--r--   0        0        0     1455 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa9a.png
+-rw-r--r--   0        0        0     1387 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa9b.png
+-rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa9c.png
+-rw-r--r--   0        0        0     1534 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa9d.png
+-rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa9e.png
+-rw-r--r--   0        0        0      844 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fa9f.png
+-rw-r--r--   0        0        0     1214 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa0.png
+-rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa1.png
+-rw-r--r--   0        0        0     3421 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa2.png
+-rw-r--r--   0        0        0     2517 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa3.png
+-rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa4.png
+-rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa5.png
+-rw-r--r--   0        0        0     1357 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa6.png
+-rw-r--r--   0        0        0      739 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa7.png
+-rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa8.png
+-rw-r--r--   0        0        0     4069 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faa9.png
+-rw-r--r--   0        0        0     3116 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faaa.png
+-rw-r--r--   0        0        0     2959 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faab.png
+-rw-r--r--   0        0        0     3385 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1faac.png
+-rw-r--r--   0        0        0     3390 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab0.png
+-rw-r--r--   0        0        0     2544 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab1.png
+-rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab2.png
+-rw-r--r--   0        0        0     2220 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab3.png
+-rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab4.png
+-rw-r--r--   0        0        0     1796 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab5.png
+-rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.376583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab6.png
+-rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab7.png
+-rw-r--r--   0        0        0     8701 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab8.png
+-rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fab9.png
+-rw-r--r--   0        0        0     3143 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1faba.png
+-rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fac0.png
+-rw-r--r--   0        0        0     2355 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fac1.png
+-rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.368583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fac2.png
+-rw-r--r--   0        0        0     2880 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fac3.png
+-rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fac4.png
+-rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fac5.png
+-rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad0.png
+-rw-r--r--   0        0        0     2166 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad1.png
+-rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad2.png
+-rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad3.png
+-rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad4.png
+-rw-r--r--   0        0        0     2275 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad5.png
+-rw-r--r--   0        0        0     1506 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad6.png
+-rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad7.png
+-rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.384583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad8.png
+-rw-r--r--   0        0        0     2883 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/1fad9.png
+-rw-r--r--   0        0        0     3754 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae0.png
+-rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae1.png
+-rw-r--r--   0        0        0     3645 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae2.png
+-rw-r--r--   0        0        0     3805 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae3.png
+-rw-r--r--   0        0        0     3362 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae4.png
+-rw-r--r--   0        0        0     2324 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae5.png
+-rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae6.png
+-rw-r--r--   0        0        0     8233 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/1fae7.png
+-rw-r--r--   0        0        0     3094 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf0.png
+-rw-r--r--   0        0        0     3119 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf1.png
+-rw-r--r--   0        0        0     3274 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf2.png
+-rw-r--r--   0        0        0     2474 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf3.png
+-rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf4.png
+-rw-r--r--   0        0        0     4017 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf5.png
+-rw-r--r--   0        0        0     2903 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/1faf6.png
+-rw-r--r--   0        0        0      979 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/203c.png
+-rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2049.png
+-rw-r--r--   0        0        0      574 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/2122.png
+-rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/2139.png
+-rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2194.png
+-rw-r--r--   0        0        0     1027 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2195.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2196.png
+-rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2197.png
+-rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2198.png
+-rw-r--r--   0        0        0     1000 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2199.png
+-rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/21a9.png
+-rw-r--r--   0        0        0     1061 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/21aa.png
+-rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/231a.png
+-rw-r--r--   0        0        0     2614 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/231b.png
+-rw-r--r--   0        0        0      983 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/2328.png
+-rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23cf.png
+-rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23e9.png
+-rw-r--r--   0        0        0     1097 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23ea.png
+-rw-r--r--   0        0        0     1069 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23eb.png
+-rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23ec.png
+-rw-r--r--   0        0        0     1085 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23ed.png
+-rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23ee.png
+-rw-r--r--   0        0        0     1009 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23ef.png
+-rw-r--r--   0        0        0     3657 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/23f0.png
+-rw-r--r--   0        0        0     2800 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/23f1.png
+-rw-r--r--   0        0        0     2100 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/23f2.png
+-rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/23f3.png
+-rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23f8.png
+-rw-r--r--   0        0        0      952 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23f9.png
+-rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/23fa.png
+-rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/24c2.png
+-rw-r--r--   0        0        0      408 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/25aa.png
+-rw-r--r--   0        0        0      194 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/25ab.png
+-rw-r--r--   0        0        0     1011 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/25b6.png
+-rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/25c0.png
+-rw-r--r--   0        0        0      196 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/25fb.png
+-rw-r--r--   0        0        0      291 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/25fc.png
+-rw-r--r--   0        0        0      175 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/25fd.png
+-rw-r--r--   0        0        0      283 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/25fe.png
+-rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2600.png
+-rw-r--r--   0        0        0      934 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2601.png
+-rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2602.png
+-rw-r--r--   0        0        0     3102 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2603.png
+-rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2604.png
+-rw-r--r--   0        0        0     2616 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/260e.png
+-rw-r--r--   0        0        0     1309 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2611.png
+-rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2614.png
+-rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/2615.png
+-rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.380583 a2-0.3.8/src/a2/data/emoji/emoji_images/2618.png
+-rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/261d.png
+-rw-r--r--   0        0        0     1956 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/2620.png
+-rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2622.png
+-rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2623.png
+-rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2626.png
+-rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/262a.png
+-rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/262e.png
+-rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/262f.png
+-rw-r--r--   0        0        0     1621 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2638.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/2639.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.340582 a2-0.3.8/src/a2/data/emoji/emoji_images/263a.png
+-rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2640.png
+-rw-r--r--   0        0        0     1449 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2642.png
+-rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2648.png
+-rw-r--r--   0        0        0     1302 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2649.png
+-rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/264a.png
+-rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/264b.png
+-rw-r--r--   0        0        0     1435 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/264c.png
+-rw-r--r--   0        0        0     1437 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/264d.png
+-rw-r--r--   0        0        0     1217 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/264e.png
+-rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/264f.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2650.png
+-rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2651.png
+-rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2652.png
+-rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2653.png
+-rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/265f.png
+-rw-r--r--   0        0        0      990 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/2660.png
+-rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/2663.png
+-rw-r--r--   0        0        0     1024 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/2665.png
+-rw-r--r--   0        0        0      819 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/2666.png
+-rw-r--r--   0        0        0     1476 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/2668.png
+-rw-r--r--   0        0        0     1547 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/267b.png
+-rw-r--r--   0        0        0      902 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/267e.png
+-rw-r--r--   0        0        0     1487 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/267f.png
+-rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/2692.png
+-rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/2693.png
+-rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/2694.png
+-rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2695.png
+-rw-r--r--   0        0        0     2360 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/2696.png
+-rw-r--r--   0        0        0     2664 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/2697.png
+-rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/2699.png
+-rw-r--r--   0        0        0     1680 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/269b.png
+-rw-r--r--   0        0        0     2332 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/269c.png
+-rw-r--r--   0        0        0      862 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/26a0.png
+-rw-r--r--   0        0        0      822 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/26a1.png
+-rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/26a7.png
+-rw-r--r--   0        0        0      833 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/26aa.png
+-rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/26ab.png
+-rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/26b0.png
+-rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/26b1.png
+-rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/26bd.png
+-rw-r--r--   0        0        0     2594 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/26be.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/26c4.png
+-rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/26c5.png
+-rw-r--r--   0        0        0     2224 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/26c8.png
+-rw-r--r--   0        0        0     1288 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/26ce.png
+-rw-r--r--   0        0        0     1106 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/26cf.png
+-rw-r--r--   0        0        0     2363 2022-11-18 15:36:28.408584 a2-0.3.8/src/a2/data/emoji/emoji_images/26d1.png
+-rw-r--r--   0        0        0     3241 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/26d3.png
+-rw-r--r--   0        0        0     1286 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/26d4.png
+-rw-r--r--   0        0        0     1219 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/26e9.png
+-rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/26ea.png
+-rw-r--r--   0        0        0     2999 2022-11-18 15:36:28.388583 a2-0.3.8/src/a2/data/emoji/emoji_images/26f0.png
+-rw-r--r--   0        0        0     1902 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/26f1.png
+-rw-r--r--   0        0        0     3153 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/26f2.png
+-rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/26f3.png
+-rw-r--r--   0        0        0     2385 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/26f4.png
+-rw-r--r--   0        0        0     2439 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/26f5.png
+-rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.360583 a2-0.3.8/src/a2/data/emoji/emoji_images/26f7.png
+-rw-r--r--   0        0        0     1886 2022-11-18 15:36:28.404584 a2-0.3.8/src/a2/data/emoji/emoji_images/26f8.png
+-rw-r--r--   0        0        0     3213 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/26f9.png
+-rw-r--r--   0        0        0     3294 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3168 2022-11-18 15:36:28.364583 a2-0.3.8/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.392583 a2-0.3.8/src/a2/data/emoji/emoji_images/26fa.png
+-rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/26fd.png
+-rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.416584 a2-0.3.8/src/a2/data/emoji/emoji_images/2702.png
+-rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2705.png
+-rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.396584 a2-0.3.8/src/a2/data/emoji/emoji_images/2708.png
+-rw-r--r--   0        0        0      871 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/2709.png
+-rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/270a.png
+-rw-r--r--   0        0        0     1464 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/270b.png
+-rw-r--r--   0        0        0     1407 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/270c.png
+-rw-r--r--   0        0        0     1751 2022-11-18 15:36:28.348582 a2-0.3.8/src/a2/data/emoji/emoji_images/270d.png
+-rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/270f.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.412584 a2-0.3.8/src/a2/data/emoji/emoji_images/2712.png
+-rw-r--r--   0        0        0      631 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2714.png
+-rw-r--r--   0        0        0      518 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2716.png
+-rw-r--r--   0        0        0      890 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/271d.png
+-rw-r--r--   0        0        0     1315 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2721.png
+-rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2728.png
+-rw-r--r--   0        0        0     1187 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/2733.png
+-rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/2734.png
+-rw-r--r--   0        0        0     3717 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2744.png
+-rw-r--r--   0        0        0     1179 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/2747.png
+-rw-r--r--   0        0        0      782 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/274c.png
+-rw-r--r--   0        0        0     1100 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/274e.png
+-rw-r--r--   0        0        0      685 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2753.png
+-rw-r--r--   0        0        0      624 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2754.png
+-rw-r--r--   0        0        0      690 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2755.png
+-rw-r--r--   0        0        0      568 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2757.png
+-rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/2763.png
+-rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/2764.png
+-rw-r--r--   0        0        0     3565 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1f525.png
+-rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.344582 a2-0.3.8/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1fa79.png
+-rw-r--r--   0        0        0      251 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2795.png
+-rw-r--r--   0        0        0      200 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2796.png
+-rw-r--r--   0        0        0      249 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2797.png
+-rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/27a1.png
+-rw-r--r--   0        0        0      858 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/27b0.png
+-rw-r--r--   0        0        0      686 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/27bf.png
+-rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2934.png
+-rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2935.png
+-rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b05.png
+-rw-r--r--   0        0        0     1034 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b06.png
+-rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.420584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b07.png
+-rw-r--r--   0        0        0      700 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b1b.png
+-rw-r--r--   0        0        0      203 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b1c.png
+-rw-r--r--   0        0        0     1704 2022-11-18 15:36:28.400584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b50.png
+-rw-r--r--   0        0        0     1025 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/2b55.png
+-rw-r--r--   0        0        0      614 2022-11-18 15:36:28.424584 a2-0.3.8/src/a2/data/emoji/emoji_images/3030.png
+-rw-r--r--   0        0        0      791 2022-11-18 15:36:28.428584 a2-0.3.8/src/a2/data/emoji/emoji_images/303d.png
+-rw-r--r--   0        0        0     1614 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/3297.png
+-rw-r--r--   0        0        0     1733 2022-11-18 15:36:28.432584 a2-0.3.8/src/a2/data/emoji/emoji_images/3299.png
+-rw-r--r--   0        0        0  2152796 2022-07-06 14:12:42.663962 a2-0.3.8/src/a2/data/font/Symbola.ttf
+-rw-r--r--   0        0        0  3727644 2022-07-06 14:12:42.683963 a2-0.3.8/src/a2/data/font/Symbola_hint.ttf
+-rw-r--r--   0        0        0       44 2022-07-06 14:12:42.683963 a2-0.3.8/src/a2/data/font/sharefonts.net.txt
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.8/src/a2/data/vocabularies/__init__.py
+-rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.8/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
+-rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.8/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
+-rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.8/src/a2/dataset/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-21 14:04:45.557653 a2-0.3.8/src/a2/dataset/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      645 2023-01-30 15:08:36.152054 a2-0.3.8/src/a2/dataset/__pycache__/emojis.cpython-310.pyc
+-rw-r--r--   0        0        0     8810 2023-06-06 15:04:03.968979 a2-0.3.8/src/a2/dataset/__pycache__/load_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0      434 2022-08-02 15:37:53.112570 a2-0.3.8/src/a2/dataset/__pycache__/manipulate_datasets.cpython-310.pyc
+-rw-r--r--   0        0        0    39422 2023-01-30 15:08:36.940073 a2-0.3.8/src/a2/dataset/__pycache__/radar.cpython-310.pyc
+-rw-r--r--   0        0        0     8738 2023-01-30 15:08:36.944073 a2-0.3.8/src/a2/dataset/__pycache__/stations.cpython-310.pyc
+-rw-r--r--   0        0        0     1040 2023-02-20 13:59:16.193086 a2-0.3.8/src/a2/dataset/__pycache__/tweets.cpython-310.pyc
+-rw-r--r--   0        0        0     2155 2022-12-14 09:39:28.258310 a2-0.3.8/src/a2/dataset/__pycache__/units.cpython-310.pyc
+-rw-r--r--   0        0        0    15533 2023-06-06 13:09:57.413845 a2-0.3.8/src/a2/dataset/__pycache__/utils_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.8/src/a2/dataset/emojis.py
+-rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.3.8/src/a2/dataset/load_dataset.py
+-rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.8/src/a2/dataset/radar.py
+-rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.8/src/a2/dataset/stations.py
+-rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.8/src/a2/dataset/tweets.py
+-rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.8/src/a2/dataset/units.py
+-rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.3.8/src/a2/dataset/utils_dataset.py
+-rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.8/src/a2/plotting/__init__.py
+-rw-r--r--   0        0        0      366 2022-12-14 09:39:30.762420 a2-0.3.8/src/a2/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7136 2023-05-16 09:07:00.708334 a2-0.3.8/src/a2/plotting/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     1901 2023-02-14 15:41:10.653195 a2-0.3.8/src/a2/plotting/__pycache__/axes_utils.cpython-310.pyc
+-rw-r--r--   0        0        0    22974 2023-05-16 11:22:14.741608 a2-0.3.8/src/a2/plotting/__pycache__/histograms.cpython-310.pyc
+-rw-r--r--   0        0        0     3123 2022-12-14 09:39:32.242484 a2-0.3.8/src/a2/plotting/__pycache__/parallel_plotting.cpython-310.pyc
+-rw-r--r--   0        0        0     2721 2022-12-14 09:39:32.242484 a2-0.3.8/src/a2/plotting/__pycache__/timeseries.cpython-310.pyc
+-rw-r--r--   0        0        0    14561 2023-05-16 09:07:00.712334 a2-0.3.8/src/a2/plotting/__pycache__/utils_plotting.cpython-310.pyc
+-rw-r--r--   0        0        0    29227 2023-02-20 13:59:16.709099 a2-0.3.8/src/a2/plotting/__pycache__/weather_maps.cpython-310.pyc
+-rw-r--r--   0        0        0     8164 2023-05-12 12:06:36.401113 a2-0.3.8/src/a2/plotting/analysis.py
+-rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.8/src/a2/plotting/axes_utils.py
+-rw-r--r--   0        0        0    30638 2023-05-16 11:22:03.945363 a2-0.3.8/src/a2/plotting/histograms.py
+-rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.8/src/a2/plotting/parallel_plotting.py
+-rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.8/src/a2/plotting/timeseries.py
+-rw-r--r--   0        0        0    16218 2023-05-12 12:06:36.401113 a2-0.3.8/src/a2/plotting/utils_plotting.py
+-rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.8/src/a2/plotting/weather_maps.py
+-rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.8/src/a2/preprocess/__init__.py
+-rw-r--r--   0        0        0      228 2022-11-10 09:21:06.475180 a2-0.3.8/src/a2/preprocess/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3659 2022-12-06 08:50:28.056225 a2-0.3.8/src/a2/preprocess/__pycache__/embedding.cpython-310.pyc
+-rw-r--r--   0        0        0    26114 2023-05-23 13:01:09.722463 a2-0.3.8/src/a2/preprocess/__pycache__/normalize_text.cpython-310.pyc
+-rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.8/src/a2/preprocess/embedding.py
+-rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.3.8/src/a2/preprocess/normalize_text.py
+-rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.3.8/src/a2/training/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-16 09:06:59.916315 a2-0.3.8/src/a2/training/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4800 2023-05-16 09:07:02.808385 a2-0.3.8/src/a2/training/__pycache__/benchmarks.cpython-310.pyc
+-rw-r--r--   0        0        0     2912 2023-06-06 15:20:27.594394 a2-0.3.8/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     3990 2023-06-06 15:46:01.463325 a2-0.3.8/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     5003 2023-06-06 16:07:08.129768 a2-0.3.8/src/a2/training/__pycache__/tracking.cpython-310.pyc
+-rw-r--r--   0        0        0     2217 2023-05-16 09:07:02.804385 a2-0.3.8/src/a2/training/__pycache__/tracking_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-16 09:07:02.804385 a2-0.3.8/src/a2/training/__pycache__/training_deep500.cpython-310.pyc
+-rw-r--r--   0        0        0     8646 2023-06-06 15:04:05.473018 a2-0.3.8/src/a2/training/__pycache__/training_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     6756 2023-04-18 13:46:32.335340 a2-0.3.8/src/a2/training/__pycache__/training_performance.cpython-310.pyc
+-rw-r--r--   0        0        0      306 2023-01-30 15:08:44.672258 a2-0.3.8/src/a2/training/__pycache__/utils_training.cpython-310.pyc
+-rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.3.8/src/a2/training/benchmarks.py
+-rw-r--r--   0        0        0     2863 2023-06-06 15:14:17.260894 a2-0.3.8/src/a2/training/dataset_hugging.py
+-rw-r--r--   0        0        0     4213 2023-06-06 15:45:58.319253 a2-0.3.8/src/a2/training/evaluate_hugging.py
+-rw-r--r--   0        0        0     4563 2023-06-06 15:48:04.766178 a2-0.3.8/src/a2/training/tracking.py
+-rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.3.8/src/a2/training/tracking_hugging.py
+-rw-r--r--   0        0        0     6390 2023-05-12 12:06:13.512505 a2-0.3.8/src/a2/training/training_deep500.py
+-rw-r--r--   0        0        0    11299 2023-06-06 14:58:39.420340 a2-0.3.8/src/a2/training/training_hugging.py
+-rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.3.8/src/a2/training/training_performance.py
+-rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.8/src/a2/training/utils_training.py
+-rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.8/src/a2/twitter/__init__.py
+-rw-r--r--   0        0        0      249 2022-11-10 09:22:53.001431 a2-0.3.8/src/a2/twitter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4896 2023-02-20 13:59:24.705291 a2-0.3.8/src/a2/twitter/__pycache__/downloader.cpython-310.pyc
+-rw-r--r--   0        0        0     9148 2023-05-23 13:01:12.894332 a2-0.3.8/src/a2/twitter/__pycache__/locations.cpython-310.pyc
+-rw-r--r--   0        0        0     8339 2022-08-01 13:51:16.422462 a2-0.3.8/src/a2/twitter/__pycache__/manipulate_tweets.cpython-310.pyc
+-rw-r--r--   0        0        0     5836 2023-02-20 13:59:24.705291 a2-0.3.8/src/a2/twitter/__pycache__/twitter_api.cpython-310.pyc
+-rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.8/src/a2/twitter/downloader.py
+-rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.3.8/src/a2/twitter/locations.py
+-rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.8/src/a2/twitter/twitter_api.py
+-rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.3.8/src/a2/utils/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-06 12:42:23.443076 a2-0.3.8/src/a2/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7235 2023-06-06 16:07:06.901738 a2-0.3.8/src/a2/utils/__pycache__/argparse.cpython-310.pyc
+-rw-r--r--   0        0        0      787 2023-05-16 09:06:59.920315 a2-0.3.8/src/a2/utils/__pycache__/checks.cpython-310.pyc
+-rw-r--r--   0        0        0      558 2023-02-20 15:49:06.840044 a2-0.3.8/src/a2/utils/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     9546 2023-06-06 15:04:04.548994 a2-0.3.8/src/a2/utils/__pycache__/file_handling.cpython-310.pyc
+-rw-r--r--   0        0        0      445 2023-05-16 09:07:00.248323 a2-0.3.8/src/a2/utils/__pycache__/strings.cpython-310.pyc
+-rw-r--r--   0        0        0     6104 2023-05-16 09:07:00.248323 a2-0.3.8/src/a2/utils/__pycache__/testing.cpython-310.pyc
+-rw-r--r--   0        0        0      545 2022-12-14 09:39:28.222309 a2-0.3.8/src/a2/utils/__pycache__/times.cpython-310.pyc
+-rw-r--r--   0        0        0     6704 2023-05-16 09:07:00.336325 a2-0.3.8/src/a2/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     8692 2023-06-07 07:40:52.055973 a2-0.3.8/src/a2/utils/argparse.py
+-rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.3.8/src/a2/utils/checks.py
+-rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.8/src/a2/utils/constants.py
+-rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.3.8/src/a2/utils/file_handling.py
+-rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.3.8/src/a2/utils/strings.py
+-rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.3.8/src/a2/utils/testing.py
+-rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.8/src/a2/utils/times.py
+-rw-r--r--   0        0        0     6088 2023-05-12 12:06:36.405113 a2-0.3.8/src/a2/utils/utils.py
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 a2-0.3.8/PKG-INFO
```

### Comparing `a2-0.3.7/pyproject.toml` & `a2-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "a2"
-version = "0.3.7"
+version = "0.3.8"
 description = "Package for predicting information about the weather from social media data as application 2 for maelstrom project"
 authors = ["Kristian Ehlert <kristian.ehlert@4-cast.de>"]
 packages = [{ include = "a2", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jupyterlab = "^3.4.3"
```

### Comparing `a2-0.3.7/src/a2/cli/cli_plotting/single_plots.py` & `a2-0.3.8/src/a2/cli/cli_plotting/single_plots.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/data/emoji/emoji_df.csv` & `a2-0.3.8/src/a2/data/emoji/emoji_df.csv`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt` & `a2-0.3.8/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/emojis.py` & `a2-0.3.8/src/a2/dataset/emojis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/load_dataset.py` & `a2-0.3.8/src/a2/dataset/load_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/radar.py` & `a2-0.3.8/src/a2/dataset/radar.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/stations.py` & `a2-0.3.8/src/a2/dataset/stations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/tweets.py` & `a2-0.3.8/src/a2/dataset/tweets.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/units.py` & `a2-0.3.8/src/a2/dataset/units.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/dataset/utils_dataset.py` & `a2-0.3.8/src/a2/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/analysis.py` & `a2-0.3.8/src/a2/plotting/analysis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/axes_utils.py` & `a2-0.3.8/src/a2/plotting/axes_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/histograms.py` & `a2-0.3.8/src/a2/plotting/histograms.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/parallel_plotting.py` & `a2-0.3.8/src/a2/plotting/parallel_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/timeseries.py` & `a2-0.3.8/src/a2/plotting/timeseries.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/utils_plotting.py` & `a2-0.3.8/src/a2/plotting/utils_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/plotting/weather_maps.py` & `a2-0.3.8/src/a2/plotting/weather_maps.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/preprocess/embedding.py` & `a2-0.3.8/src/a2/preprocess/embedding.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/preprocess/normalize_text.py` & `a2-0.3.8/src/a2/preprocess/normalize_text.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/benchmarks.py` & `a2-0.3.8/src/a2/training/benchmarks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/dataset_hugging.py` & `a2-0.3.8/src/a2/training/dataset_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/evaluate_hugging.py` & `a2-0.3.8/src/a2/training/evaluate_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/tracking.py` & `a2-0.3.8/src/a2/training/tracking.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/tracking_hugging.py` & `a2-0.3.8/src/a2/training/tracking_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/training_deep500.py` & `a2-0.3.8/src/a2/training/training_deep500.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/training_hugging.py` & `a2-0.3.8/src/a2/training/training_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/training/training_performance.py` & `a2-0.3.8/src/a2/training/training_performance.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/twitter/downloader.py` & `a2-0.3.8/src/a2/twitter/downloader.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/twitter/locations.py` & `a2-0.3.8/src/a2/twitter/locations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/twitter/twitter_api.py` & `a2-0.3.8/src/a2/twitter/twitter_api.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/utils/argparse.py` & `a2-0.3.8/src/a2/utils/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         default="2017_2020_tweets_rain_sun_vocab_emojis_locations_bba_Tp_era5_no_bots_normalized_filtered.nc",
         help="Filename of training data.",
     )
     parser.add_argument(
         "--n_tweets_irrelevant",
         type=int,
         default=-1,
-        help='Number of irrelevant tweets used to create dataset, use all irrelevant tweets by default (`n_tweets_irrelevant=-1`).',
+        help="Number of irrelevant tweets used to create dataset, "
+        "use all irrelevant tweets by default (`n_tweets_irrelevant=-1`).",
     )
 
     parser.add_argument(
         "--key_relevance",
         type=str,
         default="relevant",
         help="Filename of training data.",
@@ -185,18 +186,21 @@
         "-outdir",
         type=str,
         default=a2.utils.file_handling.get_folder_models(),
         help="Output directory where model is saved.",
     )
 
 
-def mlflow(parser):
+def run(parser):
     parser.add_argument(
         "--run_folder", type=str, required=True, help="Output folder where model is saved in `output_dir`."
     )
+
+
+def mlflow(parser):
     parser.add_argument("--run_name", type=str, default="era5 whole dataset", help="Name of run used for logging only.")
     parser.add_argument(
         "--mlflow_experiment_name",
         type=str,
         default="maelstrom-a2-train",
         help="Name MLflow experiment where results are logged.",
     )
```

### Comparing `a2-0.3.7/src/a2/utils/checks.py` & `a2-0.3.8/src/a2/utils/checks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/utils/file_handling.py` & `a2-0.3.8/src/a2/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/utils/testing.py` & `a2-0.3.8/src/a2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/src/a2/utils/utils.py` & `a2-0.3.8/src/a2/utils/utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.7/PKG-INFO` & `a2-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2
-Version: 0.3.7
+Version: 0.3.8
 Summary: Package for predicting information about the weather from social media data as application 2 for maelstrom project
 Author: Kristian Ehlert
 Author-email: kristian.ehlert@4-cast.de
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

