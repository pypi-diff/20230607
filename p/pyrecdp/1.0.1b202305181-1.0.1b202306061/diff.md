# Comparing `tmp/pyrecdp-1.0.1b202305181.tar.gz` & `tmp/pyrecdp-1.0.1b202306061.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.0.1b202305181.tar", last modified: Fri May 19 16:51:25 2023, max compression
+gzip compressed data, was "pyrecdp-1.0.1b202306061.tar", last modified: Tue Jun  6 22:28:10 2023, max compression
```

## Comparing `pyrecdp-1.0.1b202305181.tar` & `pyrecdp-1.0.1b202306061.tar`

### file list

```diff
@@ -1,116 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10481 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4010 2023-05-19 16:51:22.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13436 2023-05-18 19:47:36.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 21:49:59.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-08 21:21:08.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-19 16:40:19.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-05-18 19:26:45.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 06:07:04.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-03-01 06:17:33.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/engines/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-13 22:10:56.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 20:38:27.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-05-13 20:11:42.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-12 03:42:22.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     4047 2023-05-12 20:27:56.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-05-12 20:55:11.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 21:52:17.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-05-05 19:42:48.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-08 18:34:18.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-05-19 16:42:22.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4398 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54029 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 22:08:36.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10481 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:42:06.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1486 2023-05-18 19:00:07.000000 pyrecdp-1.0.1b202305181/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.151224 pyrecdp-1.0.1b202306061/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-06-02 20:11:31.000000 pyrecdp-1.0.1b202306061/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-06-06 22:28:10.151224 pyrecdp-1.0.1b202306061/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-02 20:11:31.000000 pyrecdp-1.0.1b202306061/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    13436 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     4047 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-06-06 22:13:53.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54029 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:27:26.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 22:28:10.151224 pyrecdp-1.0.1b202306061/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-06-06 22:27:24.000000 pyrecdp-1.0.1b202306061/setup.py
```

### Comparing `pyrecdp-1.0.1b202305181/LICENSE` & `pyrecdp-1.0.1b202306061/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/PKG-INFO` & `pyrecdp-1.0.1b202306061/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,219 +1,222 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202305181
+Version: 1.0.1b202306061
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Description: # RecDP v2.0
-        
-        # INTRODUCTION
-        
-        ## Problem Statement
-        
-        Data Preparation is an essential step to build AI pipelines 
-        * key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
-        * exploration of optimal Data preparation consumes majority of Data Science time
-        
-        ## Solution with RecDP v2.0
-        
-        * Auto pipeline
-            * only 3 lines of codes required
-        * Pipeline Generator
-            * Data Profiling:
-                * Auto anomalies detection
-                * Auto missing value impute
-                * Profiling Visualizzation        
-            * Feature Wrangling:
-                * feature transformation(datetime, geo_info, text_nlp, url, etc.)
-                * multiple data auto joining
-                * feature cross(aggregation transformation - sum, avg, count, etc.)
-            * export pipeline as JSON file, can be import to other data platform
-        * Pipeline Runner:
-            * spark engine: convert pipeline to spark codes to run
-            * pandas engine: convert pipeline to pandas codes to run
-            * sql engine: convert pipeline to sql
-        * DataLoader:
-            * parquet, csv, json, database
-        * FeatureWriter - ML/DL connector:
-            * Data Lineage
-            * Feature Store
-            * numpy, csv, parquet, dgl / pyG graph
-        ![RecDP v2.0 Overview](resources/recdp_intro.png)
-        
-        ## This solution is intended for
-        citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-        
-        # Getting Start
-        ## setup with pip
-        ```
-        git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
-        cd frameworks.bigdata.AIDK/RecDP
-        # install dependencies
-        apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
-        DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
-        # install recdp
-        python setup.py sdist
-        pip install dist/pyrecdp-1.0.1.tar.gz
-        
-        sh start-jupyter.sh
-        # open browser with http://hostname:8888
-        ```
-        
-        ## run
-        ![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
-        
-        ## modify pipeline (add user defined function or remove operation)
-        ``` python
-        def filter_with_cond(df):
-            df = df[df['Year'] <= 2018]
-            return df
-        operation = {
-            "children": [6], # will to append this new op
-            "next": [7], # who will be connected to this new op
-            "inline_function": filter_with_cond, # function
-        }
-        pipeline.add_operation(operation)
-        ```
-        ``` python
-        operation = {
-            "idx": 6, # OP id to be deleted
-            "next": [10] # who is connected to the to_be_deleted op
-        }
-        pipeline.delete_operation(operation)
-        ```
-        
-        ## export pipeline
-        ``` python
-        pipeline.export(file_path = "exported_pipeline.json")
-        ```
-        ``` json
-        {
-            "0": {
-                "children": null,
-                "op": "DataFrame",
-                "config": "main_table"
-            },
-            "1": {
-                "children": [0],
-                "op": "type_infer",
-                "config": [
-                    ["pickup_datetime",["is_string","is_datetime"]],
-                    ["pickup_longitude",["is_numeric","is_float"]],
-                    ["pickup_latitude",["is_numeric","is_float"]],
-                    ["dropoff_longitude",["is_numeric","is_float"]],
-                    ["dropoff_latitude",["is_numeric","is_float"]],
-                    ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
-                ]
-            },
-            "2": {
-                "children": [1],
-                "op": "tuple",
-                "config": {
-                    "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
-                }
-            },
-            "3": {
-                "children": [2],
-                "op": "tuple",
-                "config": {
-                    "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
-                }
-            },
-            "4": {
-                "children": [3],
-                "op": "fillna",
-                "config": {
-                    "pickup_longitude": -1,
-                    "pickup_latitude": -1,
-                    "dropoff_longitude": -1,
-                    "dropoff_latitude": -1,
-                    "passenger_count": -1
-                }
-            },
-            "5": {
-                "children": [4],
-                "op": "datetime_feature",
-                "config": {
-                    "pickup_datetime": [
-                        ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
-                        ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
-                        ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
-                        ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
-                        ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
-                    ]
-                }
-            },
-            "6": {
-                "children": [5],
-                "op": "haversine",
-                "config": {
-                    "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
-                }
-            },
-            "7": {
-                "children": [6],
-                "op": "drop",
-                "config": [
-                    "pickup_datetime",
-                    "pickup_coordinates",
-                    "dropoff_coordinates"
-                ]
-            },
-            "8": {
-                "children": [7],
-                "op": "lightgbm",
-                "config": {
-                    "label": "fare_amount",
-                    "metrics": "rmse",
-                    "objective": "regression",
-                    "model_file": "lightgbm_regression_label.mdl",
-                    "method": "predict"
-                }
-            }
-        }
-        ```
-        
-        
-        ## Quick Example
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
-        
-        # More Examples - completed example including training
-        
-        ## Auto Feature Engineering vs. featuretools
-        * [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
-        
-        ## load PIPELINE and execute
-        * [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
-        
-        ## Realtime Inference pipeline
-        * [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
-        
-        ## Data Profiler Examples
-        * [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-        
-        * [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-        
-        
-        ## LICENSE
-        * Apache 2.0
-        
-        ## Dependency
-        * Spark 3.x
-        * python 3.*
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# RecDP v2.0
+
+# INTRODUCTION
+
+## Problem Statement
+
+Data Preparation is an essential step to build AI pipelines 
+* key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
+* exploration of optimal Data preparation consumes majority of Data Science time
+
+## Solution with RecDP v2.0
+
+* Auto pipeline
+    * only 3 lines of codes required
+* Pipeline Generator
+    * Data Profiling:
+        * Auto anomalies detection
+        * Auto missing value impute
+        * Profiling Visualizzation        
+    * Feature Wrangling:
+        * feature transformation(datetime, geo_info, text_nlp, url, etc.)
+        * multiple data auto joining
+        * feature cross(aggregation transformation - sum, avg, count, etc.)
+    * export pipeline as JSON file, can be import to other data platform
+* Pipeline Runner:
+    * spark engine: convert pipeline to spark codes to run
+    * pandas engine: convert pipeline to pandas codes to run
+    * sql engine: convert pipeline to sql
+* DataLoader:
+    * parquet, csv, json, database
+* FeatureWriter - ML/DL connector:
+    * Data Lineage
+    * Feature Store
+    * numpy, csv, parquet, dgl / pyG graph
+![RecDP v2.0 Overview](resources/recdp_intro.png)
+
+## This solution is intended for
+citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+
+# Getting Start
+## setup with pip
+```
+git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
+cd frameworks.bigdata.AIDK/RecDP
+# install dependencies
+apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
+DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
+# install recdp
+python setup.py sdist
+pip install dist/pyrecdp-1.0.1.tar.gz
+
+sh start-jupyter.sh
+# open browser with http://hostname:8888
+```
+
+## run
+![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
+
+## modify pipeline (add user defined function or remove operation)
+``` python
+def filter_with_cond(df):
+    df = df[df['Year'] <= 2018]
+    return df
+operation = {
+    "children": [6], # will to append this new op
+    "next": [7], # who will be connected to this new op
+    "inline_function": filter_with_cond, # function
+}
+pipeline.add_operation(operation)
+```
+``` python
+operation = {
+    "idx": 6, # OP id to be deleted
+    "next": [10] # who is connected to the to_be_deleted op
+}
+pipeline.delete_operation(operation)
+```
+
+## export pipeline
+``` python
+pipeline.export(file_path = "exported_pipeline.json")
+```
+``` json
+{
+    "0": {
+        "children": null,
+        "op": "DataFrame",
+        "config": "main_table"
+    },
+    "1": {
+        "children": [0],
+        "op": "type_infer",
+        "config": [
+            ["pickup_datetime",["is_string","is_datetime"]],
+            ["pickup_longitude",["is_numeric","is_float"]],
+            ["pickup_latitude",["is_numeric","is_float"]],
+            ["dropoff_longitude",["is_numeric","is_float"]],
+            ["dropoff_latitude",["is_numeric","is_float"]],
+            ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
+        ]
+    },
+    "2": {
+        "children": [1],
+        "op": "tuple",
+        "config": {
+            "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
+        }
+    },
+    "3": {
+        "children": [2],
+        "op": "tuple",
+        "config": {
+            "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
+        }
+    },
+    "4": {
+        "children": [3],
+        "op": "fillna",
+        "config": {
+            "pickup_longitude": -1,
+            "pickup_latitude": -1,
+            "dropoff_longitude": -1,
+            "dropoff_latitude": -1,
+            "passenger_count": -1
+        }
+    },
+    "5": {
+        "children": [4],
+        "op": "datetime_feature",
+        "config": {
+            "pickup_datetime": [
+                ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
+                ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
+                ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
+                ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
+                ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
+            ]
+        }
+    },
+    "6": {
+        "children": [5],
+        "op": "haversine",
+        "config": {
+            "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
+        }
+    },
+    "7": {
+        "children": [6],
+        "op": "drop",
+        "config": [
+            "pickup_datetime",
+            "pickup_coordinates",
+            "dropoff_coordinates"
+        ]
+    },
+    "8": {
+        "children": [7],
+        "op": "lightgbm",
+        "config": {
+            "label": "fare_amount",
+            "metrics": "rmse",
+            "objective": "regression",
+            "model_file": "lightgbm_regression_label.mdl",
+            "method": "predict"
+        }
+    }
+}
+```
+
+
+## Quick Example
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
+
+# More Examples - completed example including training
+
+## Auto Feature Engineering vs. featuretools
+* [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
+
+## load PIPELINE and execute
+* [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
+
+## Realtime Inference pipeline
+* [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
+
+## Data Profiler Examples
+* [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+
+* [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+
+
+## LICENSE
+* Apache 2.0
+
+## Dependency
+* Spark 3.x
+* python 3.*
+
+
```

### Comparing `pyrecdp-1.0.1b202305181/README.md` & `pyrecdp-1.0.1b202306061/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/__init__.py` & `pyrecdp-1.0.1b202306061/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.0.1b202306061/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.0.1b202306061/pyrecdp/autofe/BasePipeline.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.0.1b202306061/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/core/dataframe.py` & `pyrecdp-1.0.1b202306061/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/core/di_graph.py` & `pyrecdp-1.0.1b202306061/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/core/schema.py` & `pyrecdp-1.0.1b202306061/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/core/utils.py` & `pyrecdp-1.0.1b202306061/pyrecdp/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.0.1b202306061/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.0.1b202306061/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/datasets/base_api.py` & `pyrecdp-1.0.1b202306061/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.0.1b202306061/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.0.1b202306061/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.0.1b202306061/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/statics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 from pyrecdp.core import SeriesSchema
 from pyrecdp.core.utils import is_text_series
 from pyrecdp.core.utils import Timer
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 from pyrecdp.core.dataframe import DataFrameAPI
+import matplotlib.pyplot as plt
 
 def draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row):
-    from plotly.subplots import make_subplots
-    import plotly.graph_objs as go
     import math
     
     n_feat = len(xy_scatter_features)
     n_row = math.ceil(n_feat / n_plot_per_row)
     n_col = n_plot_per_row if n_feat > n_plot_per_row else n_feat
-    subplot_titles = xy_scatter_features
+    label = y.name
 
-    fig_list = make_subplots(rows=n_row, cols=n_col, subplot_titles  = subplot_titles, y_title = y.name)
+    height = int(n_row * 3)
+    fig, axs = plt.subplots(nrows=n_row, ncols=n_col, figsize=(10,height))
 
     X = DataFrameAPI().instiate(feature_data)
     sampled_data = X.may_sample(nrows = 1000)
     y = sampled_data[y.name]
 
     for idx, c_name in tqdm(enumerate(xy_scatter_features), total=len(xy_scatter_features)):
         feature = sampled_data[c_name]
         # if string, wrap when too long
         sch = SeriesSchema(feature)
         is_feature_string = True if (sch.is_string or sch.is_categorical_and_string) else False
         
+        row_id = int(idx / n_plot_per_row)
+        col_id = idx % n_plot_per_row
         if is_feature_string:
             tmp = feature.str.slice(0, 12, 1)
-            fig = go.Scatter(x=tmp, y=y, mode='markers', name=c_name, showlegend=False)
+            axs[row_id, col_id].scatter(x=tmp, y=y, s=5)
         else:
-            fig = go.Scatter(x=feature, y=y, mode='markers', name=c_name, showlegend=False)
-
-        fig_list.add_trace(fig, row = int(idx / n_plot_per_row) + 1, col = ((idx % n_plot_per_row) + 1))
+            axs[row_id, col_id].scatter(x=feature, y=y, s=5)
+         
+        axs[row_id, col_id].set_xlabel(c_name)
+        axs[row_id, col_id].set_ylabel(label)
 
-    print("prepare xy scatter subplot completed, start to add them as one global plot")
-    fig_list.update_layout(height=row_height * n_row, width=400 * n_col)
     print("prepare xy scatter plot completed")
     
-    return fig_list
+    fig.tight_layout()
+    return fig
 
 def draw_mapbox_plot(mapbox_scatter_features, feature_data):
     import plotly.graph_objs as go
 
     from shapely.geometry import MultiPoint
     fig_list = go.Figure()
 
@@ -113,14 +115,16 @@
         interactions_detail = self.get_interactive_plot(X, y)
         data_stats['interactions']=(dict(), interactions_detail)
         
         return data_stats
     
     def get_interactive_plot(self, feature_data, y):
         from plotly.offline import plot
+        import base64
+        from io import BytesIO
         row_height = 300
         n_plot_per_row = 2
         
         # we will create types of plot
         xy_scatter_features = []
         mapbox_scatter_features = []
         word_cloud_features = []
@@ -139,16 +143,20 @@
         
         ret = {}
         ret = {"error": False}
 
         # draw xy scatter
         if len(xy_scatter_features) > 0:
             with Timer("Draw xy scatter plot"):
-                fig_list = draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row)
-            ret['html'] = plot(fig_list, output_type='div')
+                fig = draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row)
+                tmpfile = BytesIO()
+                fig.savefig(tmpfile, format='png')
+                plt.close(fig)
+                encoded = base64.b64encode(tmpfile.getvalue()).decode('utf-8')
+                ret['html'] = '<div><img src=\'data:image/png;base64,{}\'></div>'.format(encoded)
         
         # draw mapbox
         if len(mapbox_scatter_features) > 0:
             with Timer("Draw mapbox plot"):
                 fig_list = draw_mapbox_plot(mapbox_scatter_features, feature_data)
             ret['html'] += plot(fig_list, output_type='div')
```

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/type_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.0.1b202306061/pyrecdp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,219 +1,222 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202305181
+Version: 1.0.1b202306061
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Description: # RecDP v2.0
-        
-        # INTRODUCTION
-        
-        ## Problem Statement
-        
-        Data Preparation is an essential step to build AI pipelines 
-        * key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
-        * exploration of optimal Data preparation consumes majority of Data Science time
-        
-        ## Solution with RecDP v2.0
-        
-        * Auto pipeline
-            * only 3 lines of codes required
-        * Pipeline Generator
-            * Data Profiling:
-                * Auto anomalies detection
-                * Auto missing value impute
-                * Profiling Visualizzation        
-            * Feature Wrangling:
-                * feature transformation(datetime, geo_info, text_nlp, url, etc.)
-                * multiple data auto joining
-                * feature cross(aggregation transformation - sum, avg, count, etc.)
-            * export pipeline as JSON file, can be import to other data platform
-        * Pipeline Runner:
-            * spark engine: convert pipeline to spark codes to run
-            * pandas engine: convert pipeline to pandas codes to run
-            * sql engine: convert pipeline to sql
-        * DataLoader:
-            * parquet, csv, json, database
-        * FeatureWriter - ML/DL connector:
-            * Data Lineage
-            * Feature Store
-            * numpy, csv, parquet, dgl / pyG graph
-        ![RecDP v2.0 Overview](resources/recdp_intro.png)
-        
-        ## This solution is intended for
-        citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-        
-        # Getting Start
-        ## setup with pip
-        ```
-        git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
-        cd frameworks.bigdata.AIDK/RecDP
-        # install dependencies
-        apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
-        DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
-        # install recdp
-        python setup.py sdist
-        pip install dist/pyrecdp-1.0.1.tar.gz
-        
-        sh start-jupyter.sh
-        # open browser with http://hostname:8888
-        ```
-        
-        ## run
-        ![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
-        
-        ## modify pipeline (add user defined function or remove operation)
-        ``` python
-        def filter_with_cond(df):
-            df = df[df['Year'] <= 2018]
-            return df
-        operation = {
-            "children": [6], # will to append this new op
-            "next": [7], # who will be connected to this new op
-            "inline_function": filter_with_cond, # function
-        }
-        pipeline.add_operation(operation)
-        ```
-        ``` python
-        operation = {
-            "idx": 6, # OP id to be deleted
-            "next": [10] # who is connected to the to_be_deleted op
-        }
-        pipeline.delete_operation(operation)
-        ```
-        
-        ## export pipeline
-        ``` python
-        pipeline.export(file_path = "exported_pipeline.json")
-        ```
-        ``` json
-        {
-            "0": {
-                "children": null,
-                "op": "DataFrame",
-                "config": "main_table"
-            },
-            "1": {
-                "children": [0],
-                "op": "type_infer",
-                "config": [
-                    ["pickup_datetime",["is_string","is_datetime"]],
-                    ["pickup_longitude",["is_numeric","is_float"]],
-                    ["pickup_latitude",["is_numeric","is_float"]],
-                    ["dropoff_longitude",["is_numeric","is_float"]],
-                    ["dropoff_latitude",["is_numeric","is_float"]],
-                    ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
-                ]
-            },
-            "2": {
-                "children": [1],
-                "op": "tuple",
-                "config": {
-                    "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
-                }
-            },
-            "3": {
-                "children": [2],
-                "op": "tuple",
-                "config": {
-                    "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
-                }
-            },
-            "4": {
-                "children": [3],
-                "op": "fillna",
-                "config": {
-                    "pickup_longitude": -1,
-                    "pickup_latitude": -1,
-                    "dropoff_longitude": -1,
-                    "dropoff_latitude": -1,
-                    "passenger_count": -1
-                }
-            },
-            "5": {
-                "children": [4],
-                "op": "datetime_feature",
-                "config": {
-                    "pickup_datetime": [
-                        ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
-                        ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
-                        ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
-                        ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
-                        ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
-                    ]
-                }
-            },
-            "6": {
-                "children": [5],
-                "op": "haversine",
-                "config": {
-                    "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
-                }
-            },
-            "7": {
-                "children": [6],
-                "op": "drop",
-                "config": [
-                    "pickup_datetime",
-                    "pickup_coordinates",
-                    "dropoff_coordinates"
-                ]
-            },
-            "8": {
-                "children": [7],
-                "op": "lightgbm",
-                "config": {
-                    "label": "fare_amount",
-                    "metrics": "rmse",
-                    "objective": "regression",
-                    "model_file": "lightgbm_regression_label.mdl",
-                    "method": "predict"
-                }
-            }
-        }
-        ```
-        
-        
-        ## Quick Example
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
-        
-        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
-        
-        # More Examples - completed example including training
-        
-        ## Auto Feature Engineering vs. featuretools
-        * [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
-        
-        ## load PIPELINE and execute
-        * [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
-        
-        ## Realtime Inference pipeline
-        * [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
-        
-        ## Data Profiler Examples
-        * [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-        
-        * [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-        
-        
-        ## LICENSE
-        * Apache 2.0
-        
-        ## Dependency
-        * Spark 3.x
-        * python 3.*
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# RecDP v2.0
+
+# INTRODUCTION
+
+## Problem Statement
+
+Data Preparation is an essential step to build AI pipelines 
+* key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
+* exploration of optimal Data preparation consumes majority of Data Science time
+
+## Solution with RecDP v2.0
+
+* Auto pipeline
+    * only 3 lines of codes required
+* Pipeline Generator
+    * Data Profiling:
+        * Auto anomalies detection
+        * Auto missing value impute
+        * Profiling Visualizzation        
+    * Feature Wrangling:
+        * feature transformation(datetime, geo_info, text_nlp, url, etc.)
+        * multiple data auto joining
+        * feature cross(aggregation transformation - sum, avg, count, etc.)
+    * export pipeline as JSON file, can be import to other data platform
+* Pipeline Runner:
+    * spark engine: convert pipeline to spark codes to run
+    * pandas engine: convert pipeline to pandas codes to run
+    * sql engine: convert pipeline to sql
+* DataLoader:
+    * parquet, csv, json, database
+* FeatureWriter - ML/DL connector:
+    * Data Lineage
+    * Feature Store
+    * numpy, csv, parquet, dgl / pyG graph
+![RecDP v2.0 Overview](resources/recdp_intro.png)
+
+## This solution is intended for
+citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+
+# Getting Start
+## setup with pip
+```
+git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
+cd frameworks.bigdata.AIDK/RecDP
+# install dependencies
+apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
+DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
+# install recdp
+python setup.py sdist
+pip install dist/pyrecdp-1.0.1.tar.gz
+
+sh start-jupyter.sh
+# open browser with http://hostname:8888
+```
+
+## run
+![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
+
+## modify pipeline (add user defined function or remove operation)
+``` python
+def filter_with_cond(df):
+    df = df[df['Year'] <= 2018]
+    return df
+operation = {
+    "children": [6], # will to append this new op
+    "next": [7], # who will be connected to this new op
+    "inline_function": filter_with_cond, # function
+}
+pipeline.add_operation(operation)
+```
+``` python
+operation = {
+    "idx": 6, # OP id to be deleted
+    "next": [10] # who is connected to the to_be_deleted op
+}
+pipeline.delete_operation(operation)
+```
+
+## export pipeline
+``` python
+pipeline.export(file_path = "exported_pipeline.json")
+```
+``` json
+{
+    "0": {
+        "children": null,
+        "op": "DataFrame",
+        "config": "main_table"
+    },
+    "1": {
+        "children": [0],
+        "op": "type_infer",
+        "config": [
+            ["pickup_datetime",["is_string","is_datetime"]],
+            ["pickup_longitude",["is_numeric","is_float"]],
+            ["pickup_latitude",["is_numeric","is_float"]],
+            ["dropoff_longitude",["is_numeric","is_float"]],
+            ["dropoff_latitude",["is_numeric","is_float"]],
+            ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
+        ]
+    },
+    "2": {
+        "children": [1],
+        "op": "tuple",
+        "config": {
+            "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
+        }
+    },
+    "3": {
+        "children": [2],
+        "op": "tuple",
+        "config": {
+            "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
+        }
+    },
+    "4": {
+        "children": [3],
+        "op": "fillna",
+        "config": {
+            "pickup_longitude": -1,
+            "pickup_latitude": -1,
+            "dropoff_longitude": -1,
+            "dropoff_latitude": -1,
+            "passenger_count": -1
+        }
+    },
+    "5": {
+        "children": [4],
+        "op": "datetime_feature",
+        "config": {
+            "pickup_datetime": [
+                ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
+                ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
+                ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
+                ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
+                ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
+            ]
+        }
+    },
+    "6": {
+        "children": [5],
+        "op": "haversine",
+        "config": {
+            "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
+        }
+    },
+    "7": {
+        "children": [6],
+        "op": "drop",
+        "config": [
+            "pickup_datetime",
+            "pickup_coordinates",
+            "dropoff_coordinates"
+        ]
+    },
+    "8": {
+        "children": [7],
+        "op": "lightgbm",
+        "config": {
+            "label": "fare_amount",
+            "metrics": "rmse",
+            "objective": "regression",
+            "model_file": "lightgbm_regression_label.mdl",
+            "method": "predict"
+        }
+    }
+}
+```
+
+
+## Quick Example
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
+
+* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
+
+# More Examples - completed example including training
+
+## Auto Feature Engineering vs. featuretools
+* [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
+
+## load PIPELINE and execute
+* [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
+
+## Realtime Inference pipeline
+* [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
+
+## Data Profiler Examples
+* [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+
+* [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+
+
+## LICENSE
+* Apache 2.0
+
+## Dependency
+* Spark 3.x
+* python 3.*
+
+
```

### Comparing `pyrecdp-1.0.1b202305181/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.0.1b202306061/pyrecdp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,14 @@
 pyrecdp/datasets/download.py
 pyrecdp/datasets/ibm_fraud_detect.py
 pyrecdp/datasets/nyc_taxi.py
 pyrecdp/datasets/outbrain.py
 pyrecdp/datasets/pretrained.py
 pyrecdp/datasets/twitter_recsys.py
 pyrecdp/primitives/__init__.py
-pyrecdp/primitives/engines/__init__.py
-pyrecdp/primitives/engines/runner.py
 pyrecdp/primitives/estimators/__init__.py
 pyrecdp/primitives/estimators/base.py
 pyrecdp/primitives/estimators/lightgbm.py
 pyrecdp/primitives/generators/__init__.py
 pyrecdp/primitives/generators/base.py
 pyrecdp/primitives/generators/binned.py
 pyrecdp/primitives/generators/category.py
```

### Comparing `pyrecdp-1.0.1b202305181/setup.py` & `pyrecdp-1.0.1b202306061/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="pyrecdp",
-    version="1.0.1b202305181",
+    version="1.0.1b202306061",
     author="INTEL AIA",
     description=
     "A data processing bundle for spark based recommender system operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/intel/e2eAIOK/",
     project_urls={
```

