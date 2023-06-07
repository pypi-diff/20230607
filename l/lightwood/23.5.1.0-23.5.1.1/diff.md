# Comparing `tmp/lightwood-23.5.1.0.tar.gz` & `tmp/lightwood-23.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwood-23.5.1.0.tar", last modified: Sun May  7 10:11:05 2023, max compression
+gzip compressed data, was "lightwood-23.5.1.1.tar", last modified: Wed Jun  7 04:40:16 2023, max compression
```

## Comparing `lightwood-23.5.1.0.tar` & `lightwood-23.5.1.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-05-07 10:10:52.000000 lightwood-23.5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 10:10:52.000000 lightwood-23.5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-05-07 10:10:52.000000 lightwood-23.5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.380733 lightwood-23.5.1.0/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/categorical/onehot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.388733 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.392734 lightwood-23.5.1.0/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.392734 lightwood-23.5.1.0/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:11:05.384734 lightwood-23.5.1.0/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 10:11:05.000000 lightwood-23.5.1.0/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:11:05.396734 lightwood-23.5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-07 10:10:53.000000 lightwood-23.5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/onehot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/setup.py
```

### Comparing `lightwood-23.5.1.0/LICENSE` & `lightwood-23.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/PKG-INFO` & `lightwood-23.5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.5.1.0
+Version: 23.5.1.1
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -216,15 +216,15 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: image
-Provides-Extra: quantum
-Provides-Extra: extra
-Provides-Extra: audio
 Provides-Extra: extra_ts
 Provides-Extra: xai
+Provides-Extra: quantum
+Provides-Extra: image
+Provides-Extra: audio
+Provides-Extra: dev
+Provides-Extra: extra
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.5.1.0/README.md` & `lightwood-23.5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/__init__.py` & `lightwood-23.5.1.1/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/analyze.py` & `lightwood-23.5.1.1/lightwood/analysis/analyze.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/base.py` & `lightwood-23.5.1.1/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/explain.py` & `lightwood-23.5.1.1/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.5.1.1/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.5.1.1/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.5.1.1/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/helpers/pyod.py` & `lightwood-23.5.1.1/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/helpers/shap.py` & `lightwood-23.5.1.1/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/base.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/calibrate.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/icp.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/metrics.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/nc.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/norm.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nc/util.py` & `lightwood-23.5.1.1/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.5.1.1/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/api/__init__.py` & `lightwood-23.5.1.1/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/api/high_level.py` & `lightwood-23.5.1.1/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/api/json_ai.py` & `lightwood-23.5.1.1/lightwood/api/json_ai.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/api/predictor.py` & `lightwood-23.5.1.1/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/api/types.py` & `lightwood-23.5.1.1/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/data/encoded_ds.py` & `lightwood-23.5.1.1/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/data/timeseries_analyzer.py` & `lightwood-23.5.1.1/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/data/timeseries_transform.py` & `lightwood-23.5.1.1/lightwood/data/timeseries_transform.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/__init__.py` & `lightwood-23.5.1.1/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/array/array.py` & `lightwood-23.5.1.1/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.5.1.1/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.5.1.1/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/audio/mfcc.py` & `lightwood-23.5.1.1/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/base.py` & `lightwood-23.5.1.1/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/categorical/autoencoder.py` & `lightwood-23.5.1.1/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/categorical/binary.py` & `lightwood-23.5.1.1/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/categorical/gym.py` & `lightwood-23.5.1.1/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/categorical/multihot.py` & `lightwood-23.5.1.1/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/categorical/onehot.py` & `lightwood-23.5.1.1/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/datetime/datetime.py` & `lightwood-23.5.1.1/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-23.5.1.1/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/helpers.py` & `lightwood-23.5.1.1/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/identity/identity.py` & `lightwood-23.5.1.1/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.5.1.1/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.5.1.1/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/numeric/numeric.py` & `lightwood-23.5.1.1/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-23.5.1.1/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.5.1.1/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.5.1.1/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/pretrained.py` & `lightwood-23.5.1.1/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/rnn.py` & `lightwood-23.5.1.1/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/short.py` & `lightwood-23.5.1.1/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/tfidf.py` & `lightwood-23.5.1.1/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/text/vocab.py` & `lightwood-23.5.1.1/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/time_series/rnn.py` & `lightwood-23.5.1.1/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/encoder/time_series/ts.py` & `lightwood-23.5.1.1/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/__init__.py` & `lightwood-23.5.1.1/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/base.py` & `lightwood-23.5.1.1/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/best_of.py` & `lightwood-23.5.1.1/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.5.1.1/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.5.1.1/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.5.1.1/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.5.1.1/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.5.1.1/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/__init__.py` & `lightwood-23.5.1.1/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/device.py` & `lightwood-23.5.1.1/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/general.py` & `lightwood-23.5.1.1/lightwood/helpers/general.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/io.py` & `lightwood-23.5.1.1/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/log.py` & `lightwood-23.5.1.1/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/parallelism.py` & `lightwood-23.5.1.1/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/templating.py` & `lightwood-23.5.1.1/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/text.py` & `lightwood-23.5.1.1/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/torch.py` & `lightwood-23.5.1.1/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/helpers/ts.py` & `lightwood-23.5.1.1/lightwood/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/__init__.py` & `lightwood-23.5.1.1/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/arima.py` & `lightwood-23.5.1.1/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/base.py` & `lightwood-23.5.1.1/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/ets.py` & `lightwood-23.5.1.1/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/gluonts.py` & `lightwood-23.5.1.1/lightwood/mixer/gluonts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/default_net.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/ranger.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/helpers/ts.py` & `lightwood-23.5.1.1/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/lightgbm.py` & `lightwood-23.5.1.1/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/lightgbm_array.py` & `lightwood-23.5.1.1/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/neural.py` & `lightwood-23.5.1.1/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/neural_ts.py` & `lightwood-23.5.1.1/lightwood/mixer/neural_ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/nhits.py` & `lightwood-23.5.1.1/lightwood/mixer/nhits.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,19 @@
         self.target = target
         self.window = window
         self.horizon = horizon
         self.dtype_dict = dtype_dict
         self.ts_analysis = ts_analysis
         self.grouped_by = ['__default'] if not ts_analysis['tss'].group_by else ts_analysis['tss'].group_by
         self.train_args = train_args.get('trainer_args', {}) if train_args else {}
-        self.conf_level = self.train_args.pop('conf_level', 90)
+        self.train_args['early_stop_patience_steps'] = self.train_args.get('early_stop_patience_steps', 10)
+        self.conf_level = self.train_args.pop('conf_level', [90])
+        for level in self.conf_level:
+            assert 0 <= level <= 100, f'A provided level is not in the [0, 100] range (found: {level})'
+            assert isinstance(level, int), f'A provided level is not an integer (found: {level})'
 
         self.pretrained = pretrained
         self.base_url = 'https://nixtla-public.s3.amazonaws.com/transfer/pretrained_models/'
         self.freq_to_model = {
             'Y': 'yearly',
             'Q': 'monthly',
             'M': 'monthly',
@@ -116,23 +120,23 @@
                 log.info(f'Successfully loaded pretrained N-HITS forecasting model ({self.model_name})')
 
         if not self.pretrained:
             if self.window + self.horizon > n_time:
                 new_window = max(1, n_time - self.horizon - 1)
                 self.window = new_window
                 log.info(f'Window {self.window} is too long for data provided (group: {df[gby].value_counts()[::-1].index[0]}), reducing window to {new_window}.')  # noqa
-            model = NHITS(h=n_time_out, input_size=self.window, **self.train_args, loss=MQLoss(level=[self.conf_level]))
+            model = NHITS(h=n_time_out, input_size=self.window, **self.train_args, loss=MQLoss(level=self.conf_level))
             self.model = NeuralForecast(models=[model], freq=self.ts_analysis['sample_freqs']['__default'])
             self.model.fit(df=Y_df, val_size=n_ts_val)
             log.info('Successfully trained N-HITS forecasting model.')
 
     def partial_fit(self, train_data: EncodedDs, dev_data: EncodedDs, args: Optional[dict] = None) -> None:
         # TODO: reimplement this with automatic novel-row differential
         self.hyperparam_search = False
-        self.fit(dev_data, train_data)
+        self.fit(dev_data, train_data)  # TODO: add support for passing args (e.g. n_epochs)
         self.prepared = True
 
     def __call__(self, ds: Union[EncodedDs, ConcatedEncodedDs],
                  args: PredictionArguments = PredictionArguments()) -> pd.DataFrame:
         """
         Calls the mixer to emit forecasts.
         
@@ -148,31 +152,39 @@
                            index=np.arange(length),
                            columns=['prediction', 'lower', 'upper'],
                            dtype=object)
 
         input_df = self._make_initial_df(deepcopy(ds.data_frame))
         ydf['index'] = input_df['index']
 
-        pred_cols = [f'NHITS-lo-{self.conf_level}', 'NHITS-median', f'NHITS-hi-{self.conf_level}']
-        target_cols = ['lower', 'prediction', 'upper']
+        pred_cols = ['NHITS-median']
+
+        # provided quantile must match one of the training levels, else we default to the largest one of these
+        if args.fixed_confidence is not None and int(args.fixed_confidence * 100) in self.conf_level:
+            level = int(args.fixed_confidence * 100)
+        else:
+            level = max(self.conf_level)
+        pred_cols.extend([f'NHITS-lo-{level}', f'NHITS-hi-{level}'])
+
+        target_cols = ['prediction', 'lower', 'upper']
         for target_col in target_cols:
             ydf[target_col] = [[0 for _ in range(self.horizon)] for _ in range(len(ydf))]  # zero-filled arrays
 
         group_ends = []
         for group in input_df['unique_id'].unique():
             group_ends.append(input_df[input_df['unique_id'] == group]['index'].iloc[-1])
-        fcst = self.model.predict(futr_df=input_df).reset_index()
+        fcst = self.model.predict(input_df).reset_index()
 
         for gidx, group in zip(group_ends, input_df['unique_id'].unique()):
             for pred_col, target_col in zip(pred_cols, target_cols):
                 group_preds = fcst[fcst['unique_id'] == group][pred_col].tolist()[:self.horizon]
                 idx = ydf[ydf['index'] == gidx].index[0]
                 ydf.at[idx, target_col] = group_preds
 
-        ydf['confidence'] = 0.9  # TODO: set through `args`
+        ydf['confidence'] = level / 100
         return ydf
 
     def _make_initial_df(self, df):
         oby_col = self.ts_analysis["tss"].order_by
         df = df.sort_values(by=f'__mdb_original_{oby_col}')
         df[f'__mdb_parsed_{oby_col}'] = df.index
         df = df.reset_index(drop=True)
```

### Comparing `lightwood-23.5.1.0/lightwood/mixer/prophet.py` & `lightwood-23.5.1.1/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/qclassic.py` & `lightwood-23.5.1.1/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/random_forest.py` & `lightwood-23.5.1.1/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/regression.py` & `lightwood-23.5.1.1/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/sktime.py` & `lightwood-23.5.1.1/lightwood/mixer/sktime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/tabtransformer.py` & `lightwood-23.5.1.1/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/unit.py` & `lightwood-23.5.1.1/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood/mixer/xgboost.py` & `lightwood-23.5.1.1/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood.egg-info/PKG-INFO` & `lightwood-23.5.1.1/lightwood.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.5.1.0
+Version: 23.5.1.1
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -216,15 +216,15 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: image
-Provides-Extra: quantum
-Provides-Extra: extra
-Provides-Extra: audio
 Provides-Extra: extra_ts
 Provides-Extra: xai
+Provides-Extra: quantum
+Provides-Extra: image
+Provides-Extra: audio
+Provides-Extra: dev
+Provides-Extra: extra
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.5.1.0/lightwood.egg-info/SOURCES.txt` & `lightwood-23.5.1.1/lightwood.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.0/lightwood.egg-info/requires.txt` & `lightwood-23.5.1.1/lightwood.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 optuna<2.10.0,>=2.8.0
 scipy>=1.5.4
 psutil>=5.7.0
 setuptools>=21.2.1
 wheel>=0.32.2
 scikit-learn<=1.0.2,>=1.0.0
 dataclasses_json>=0.5.4
-dill==0.3.4
+dill==0.3.6
 sktime<0.15.0,>=0.14.0
 statsforecast==1.4.0
 torch_optimizer==0.1.0
 black>=21.9b0
 typing_extensions
 colorlog==6.5.0
 statsmodels>=0.12.0
@@ -30,28 +30,28 @@
 xgboost<=1.8.0,>=1.6.0
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
-pystan==2.19.1.1
-neuralforecast==1.5.0
-shap>=0.40.0
-qiskit==0.31.0
-torchvision<0.11.0,>=0.10.0
+autopep8>=1.5.7
+mxnet<2.0.0,>=1.6.0
 pillow>8.3.1
+torchvision<0.11.0,>=0.10.0
 librosa==0.8.1
-suod
-mxnet<2.0.0,>=1.6.0
-lightgbm<=3.3.3,>=3.3.0
-gluonts<0.12.0,>=0.11.0
+qiskit==0.31.0
 prophet==1.1
-autopep8>=1.5.7
+pystan==2.19.1.1
+neuralforecast==1.5.0
 pyod==1.0.4
+lightgbm<=3.3.3,>=3.3.0
+gluonts<0.12.0,>=0.11.0
+shap>=0.40.0
+suod
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
```

### Comparing `lightwood-23.5.1.0/requirements.txt` & `lightwood-23.5.1.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 optuna >=2.8.0,<2.10.0
 scipy >=1.5.4
 psutil >=5.7.0
 setuptools >=21.2.1
 wheel >=0.32.2
 scikit-learn >=1.0.0, <=1.0.2
 dataclasses_json >=0.5.4
-dill ==0.3.4
+dill ==0.3.6
 sktime >=0.14.0,<0.15.0
 statsforecast ==1.4.0
 torch_optimizer ==0.1.0
 black >=21.9b0
 typing_extensions
 colorlog ==6.5.0
 statsmodels >=0.12.0
```

### Comparing `lightwood-23.5.1.0/setup.py` & `lightwood-23.5.1.1/setup.py`

 * *Files identical despite different names*

