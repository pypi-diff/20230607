# Comparing `tmp/splink-3.9.0.tar.gz` & `tmp/splink-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.9.0.tar", max compression
+gzip compressed data, was "splink-3.9.1.tar", max compression
```

## Comparing `splink-3.9.0.tar` & `splink-3.9.1.tar`

### file list

```diff
@@ -1,124 +1,140 @@
--rw-r--r--   0        0        0     1076 2023-05-31 15:25:25.311725 splink-3.9.0/LICENSE
--rw-r--r--   0        0        0     8777 2023-05-31 15:25:25.311725 splink-3.9.0/README.md
--rw-r--r--   0        0        0     1799 2023-05-31 15:25:25.343744 splink-3.9.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-31 15:25:25.347747 splink-3.9.0/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-05-31 15:25:25.347747 splink-3.9.0/splink/accuracy.py
--rw-r--r--   0        0        0     4759 2023-05-31 15:25:25.347747 splink-3.9.0/splink/analyse_blocking.py
--rw-r--r--   0        0        0      366 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0      221 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0      252 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_comparison_template_library.py
--rw-r--r--   0        0        0      661 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_base.py
--rw-r--r--   0        0        0     3120 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_comparison_imports.py
--rw-r--r--   0        0        0      350 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2903 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0    20688 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_linker.py
--rw-r--r--   0        0        0     2867 2023-05-31 15:25:25.347747 splink-3.9.0/splink/block_from_labels.py
--rw-r--r--   0        0        0     6239 2023-05-31 15:25:25.347747 splink-3.9.0/splink/blocking.py
--rw-r--r--   0        0        0    11739 2023-05-31 15:25:25.347747 splink-3.9.0/splink/charts.py
--rw-r--r--   0        0        0     9088 2023-05-31 15:25:25.347747 splink-3.9.0/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison.py
--rw-r--r--   0        0        0     8766 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_helpers.py
--rw-r--r--   0        0        0      554 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_helpers_utils.py
--rw-r--r--   0        0        0    25479 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level.py
--rw-r--r--   0        0        0    16492 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    46215 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    54177 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_library.py
--rw-r--r--   0        0        0     4727 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    59497 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16886 2023-05-31 15:25:25.347747 splink-3.9.0/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-05-31 15:25:25.347747 splink-3.9.0/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-05-31 15:25:25.347747 splink-3.9.0/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-05-31 15:25:25.347747 splink-3.9.0/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0      609 2023-05-31 15:25:25.347747 splink-3.9.0/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1608 2023-05-31 15:25:25.347747 splink-3.9.0/splink/dialect_base.py
--rw-r--r--   0        0        0      476 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0      371 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      172 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1532 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_base.py
--rw-r--r--   0        0        0     5597 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
--rw-r--r--   0        0        0     1750 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0    11482 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    17471 2023-05-31 15:25:25.347747 splink-3.9.0/splink/em_training_session.py
--rw-r--r--   0        0        0     5244 2023-05-31 15:25:25.347747 splink-3.9.0/splink/estimate_u.py
--rw-r--r--   0        0        0      144 2023-05-31 15:25:25.347747 splink-3.9.0/splink/exceptions.py
--rw-r--r--   0        0        0     7333 2023-05-31 15:25:25.347747 splink-3.9.0/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1558 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     5212 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     1907 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2779 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     6737 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
--rw-r--r--   0        0        0     7747 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
--rw-r--r--   0        0        0     6298 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/compare_estimates.json
--rw-r--r--   0        0        0     2155 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json
--rw-r--r--   0        0        0      743 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/gamma_histogram.json
--rw-r--r--   0        0        0     1309 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/score_histogram.json
--rw-r--r--   0        0        0     5831 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0      977 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5766 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9159 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1734 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     1730 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1962 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1465 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1123 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1745 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9924 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0     2645 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-05-31 15:25:25.351749 splink-3.9.0/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-05-31 15:25:25.351749 splink-3.9.0/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-05-31 15:25:25.355752 splink-3.9.0/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0    12871 2023-05-31 15:25:25.355752 splink-3.9.0/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-05-31 15:25:25.363757 splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-05-31 15:25:25.367759 splink-3.9.0/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-05-31 15:25:25.367759 splink-3.9.0/splink/input_column.py
--rw-r--r--   0        0        0   124599 2023-05-31 15:25:25.367759 splink-3.9.0/splink/linker.py
--rw-r--r--   0        0        0      300 2023-05-31 15:25:25.367759 splink-3.9.0/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-05-31 15:25:25.367759 splink-3.9.0/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-05-31 15:25:25.367759 splink-3.9.0/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-05-31 15:25:25.367759 splink-3.9.0/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-05-31 15:25:25.367759 splink-3.9.0/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-05-31 15:25:25.367759 splink-3.9.0/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-05-31 15:25:25.367759 splink-3.9.0/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     4548 2023-05-31 15:25:25.367759 splink-3.9.0/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-05-31 15:25:25.367759 splink-3.9.0/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-05-31 15:25:25.367759 splink-3.9.0/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-05-31 15:25:25.367759 splink-3.9.0/splink/pipeline.py
--rw-r--r--   0        0        0     3205 2023-05-31 15:25:25.367759 splink-3.9.0/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-05-31 15:25:25.367759 splink-3.9.0/splink/profile_data.py
--rw-r--r--   0        0        0    18694 2023-05-31 15:25:25.367759 splink-3.9.0/splink/settings.py
--rw-r--r--   0        0        0      473 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/jar_location.py
--rw-r--r--   0        0        0      474 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      170 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0     1083 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     2280 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_helpers/spark_base.py
--rw-r--r--   0        0        0     5565 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_helpers/spark_comparison_imports.py
--rw-r--r--   0        0        0    23101 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-05-31 15:25:25.367759 splink-3.9.0/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     3836 2023-05-31 15:25:25.367759 splink-3.9.0/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1181 2023-05-31 15:25:25.367759 splink-3.9.0/splink/sql_transform.py
--rw-r--r--   0        0        0      313 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      157 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0      390 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_comparison_template_library.py
--rw-r--r--   0        0        0      148 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_helpers/sqlite_base.py
--rw-r--r--   0        0        0     2061 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
--rw-r--r--   0        0        0     6159 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0    10207 2023-05-31 15:25:25.371761 splink-3.9.0/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-05-31 15:25:25.371761 splink-3.9.0/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1424 2023-05-31 15:25:25.371761 splink-3.9.0/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-05-31 15:25:25.371761 splink-3.9.0/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-05-31 15:25:25.371761 splink-3.9.0/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-05-31 15:25:25.371761 splink-3.9.0/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9745 1970-01-01 00:00:00.000000 splink-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-07 15:39:58.384966 splink-3.9.1/LICENSE
+-rw-r--r--   0        0        0     8787 2023-06-07 15:39:58.384966 splink-3.9.1/README.md
+-rw-r--r--   0        0        0     1799 2023-06-07 15:39:58.420966 splink-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-07 15:39:58.420966 splink-3.9.1/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-06-07 15:39:58.420966 splink-3.9.1/splink/accuracy.py
+-rw-r--r--   0        0        0     4759 2023-06-07 15:39:58.420966 splink-3.9.1/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      387 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_comparison_template_library.py
+-rw-r--r--   0        0        0      661 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_base.py
+-rw-r--r--   0        0        0     3120 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_comparison_imports.py
+-rw-r--r--   0        0        0      350 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2903 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0      361 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      366 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/comparison_level_library.py
+-rw-r--r--   0        0        0      221 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/comparison_library.py
+-rw-r--r--   0        0        0      252 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/comparison_template_library.py
+-rw-r--r--   0        0        0    20873 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/linker.py
+-rw-r--r--   0        0        0     2867 2023-06-07 15:39:58.420966 splink-3.9.1/splink/block_from_labels.py
+-rw-r--r--   0        0        0     6239 2023-06-07 15:39:58.420966 splink-3.9.1/splink/blocking.py
+-rw-r--r--   0        0        0    11739 2023-06-07 15:39:58.420966 splink-3.9.1/splink/charts.py
+-rw-r--r--   0        0        0     9088 2023-06-07 15:39:58.420966 splink-3.9.1/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison.py
+-rw-r--r--   0        0        0     8766 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_helpers.py
+-rw-r--r--   0        0        0      554 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_helpers_utils.py
+-rw-r--r--   0        0        0    25479 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level.py
+-rw-r--r--   0        0        0    16492 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    48250 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    56259 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_library.py
+-rw-r--r--   0        0        0     4810 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    62023 2023-06-07 15:39:58.424966 splink-3.9.1/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-06-07 15:39:58.424966 splink-3.9.1/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-06-07 15:39:58.424966 splink-3.9.1/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16886 2023-06-07 15:39:58.424966 splink-3.9.1/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-06-07 15:39:58.424966 splink-3.9.1/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-06-07 15:39:58.424966 splink-3.9.1/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-06-07 15:39:58.424966 splink-3.9.1/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0      609 2023-06-07 15:39:58.424966 splink-3.9.1/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1608 2023-06-07 15:39:58.424966 splink-3.9.1/splink/dialect_base.py
+-rw-r--r--   0        0        0      476 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/comparison_level_library.py
+-rw-r--r--   0        0        0      371 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/comparison_library.py
+-rw-r--r--   0        0        0      172 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/comparison_template_library.py
+-rw-r--r--   0        0        0      387 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1532 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_base.py
+-rw-r--r--   0        0        0     5597 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
+-rw-r--r--   0        0        0     1750 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0      367 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    11612 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/linker.py
+-rw-r--r--   0        0        0    17471 2023-06-07 15:39:58.424966 splink-3.9.1/splink/em_training_session.py
+-rw-r--r--   0        0        0     5244 2023-06-07 15:39:58.424966 splink-3.9.1/splink/estimate_u.py
+-rw-r--r--   0        0        0      268 2023-06-07 15:39:58.424966 splink-3.9.1/splink/exceptions.py
+-rw-r--r--   0        0        0     7333 2023-06-07 15:39:58.424966 splink-3.9.1/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1558 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     5212 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     1907 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2779 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     6737 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
+-rw-r--r--   0        0        0     7747 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
+-rw-r--r--   0        0        0     6298 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/compare_estimates.json
+-rw-r--r--   0        0        0     2155 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json
+-rw-r--r--   0        0        0      743 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/gamma_histogram.json
+-rw-r--r--   0        0        0     1309 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/score_histogram.json
+-rw-r--r--   0        0        0     5831 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0      977 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5766 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9159 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1734 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2708 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1962 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1465 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1123 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1745 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9924 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0     2645 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-06-07 15:39:58.428966 splink-3.9.1/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0    12871 2023-06-07 15:39:58.428966 splink-3.9.1/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-06-07 15:39:58.436967 splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-06-07 15:39:58.444967 splink-3.9.1/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-06-07 15:39:58.444967 splink-3.9.1/splink/files/templates/single_chart_template.txt
+-rw-r--r--   0        0        0      195 2023-06-07 15:39:58.444967 splink-3.9.1/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-06-07 15:39:58.444967 splink-3.9.1/splink/input_column.py
+-rw-r--r--   0        0        0   131359 2023-06-07 15:39:58.444967 splink-3.9.1/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-06-07 15:39:58.444967 splink-3.9.1/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-06-07 15:39:58.444967 splink-3.9.1/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-06-07 15:39:58.444967 splink-3.9.1/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-06-07 15:39:58.444967 splink-3.9.1/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-06-07 15:39:58.444967 splink-3.9.1/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-06-07 15:39:58.444967 splink-3.9.1/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-06-07 15:39:58.444967 splink-3.9.1/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     4548 2023-06-07 15:39:58.444967 splink-3.9.1/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-06-07 15:39:58.444967 splink-3.9.1/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-06-07 15:39:58.444967 splink-3.9.1/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-06-07 15:39:58.444967 splink-3.9.1/splink/pipeline.py
+-rw-r--r--   0        0        0     3205 2023-06-07 15:39:58.444967 splink-3.9.1/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-06-07 15:39:58.444967 splink-3.9.1/splink/profile_data.py
+-rw-r--r--   0        0        0    18694 2023-06-07 15:39:58.444967 splink-3.9.1/splink/settings.py
+-rw-r--r--   0        0        0      474 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/comparison_library.py
+-rw-r--r--   0        0        0      170 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/comparison_template_library.py
+-rw-r--r--   0        0        0      473 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/jar_location.py
+-rw-r--r--   0        0        0    23101 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/linker.py
+-rw-r--r--   0        0        0      384 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0      366 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      393 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0     1083 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     1875 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_helpers/spark_base.py
+-rw-r--r--   0        0        0     5565 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_helpers/spark_comparison_imports.py
+-rw-r--r--   0        0        0      356 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4507 2023-06-07 15:39:58.444967 splink-3.9.1/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     3836 2023-06-07 15:39:58.444967 splink-3.9.1/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1181 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sql_transform.py
+-rw-r--r--   0        0        0      313 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/comparison_level_library.py
+-rw-r--r--   0        0        0      157 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/comparison_library.py
+-rw-r--r--   0        0        0      390 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/comparison_template_library.py
+-rw-r--r--   0        0        0     6173 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/linker.py
+-rw-r--r--   0        0        0      387 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_comparison_template_library.py
+-rw-r--r--   0        0        0      148 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_helpers/sqlite_base.py
+-rw-r--r--   0        0        0     2061 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
+-rw-r--r--   0        0        0      361 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0    10205 2023-06-07 15:39:58.444967 splink-3.9.1/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-06-07 15:39:58.444967 splink-3.9.1/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1424 2023-06-07 15:39:58.444967 splink-3.9.1/splink/unlinkables.py
+-rw-r--r--   0        0        0     2431 2023-06-07 15:39:58.444967 splink-3.9.1/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-06-07 15:39:58.444967 splink-3.9.1/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-06-07 15:39:58.444967 splink-3.9.1/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9755 1970-01-01 00:00:00.000000 splink-3.9.1/PKG-INFO
```

### Comparing `splink-3.9.0/LICENSE` & `splink-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/README.md` & `splink-3.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
 
 ## Key Features
 
-⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.
-🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.
-🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.
-🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.
-📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
+⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
+🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
+🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
+🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
+📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.  
 
 Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
```

### Comparing `splink-3.9.0/pyproject.toml` & `splink-3.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splink"
-version = "3.9.0"
+version = "3.9.1"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
```

### Comparing `splink-3.9.0/splink/accuracy.py` & `splink-3.9.1/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/analyse_blocking.py` & `splink-3.9.1/splink/analyse_blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/athena/athena_helpers/athena_base.py` & `splink-3.9.1/splink/athena/athena_helpers/athena_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/athena/athena_helpers/athena_comparison_imports.py` & `splink-3.9.1/splink/athena/athena_helpers/athena_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/athena/athena_helpers/athena_utils.py` & `splink-3.9.1/splink/athena/athena_helpers/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/athena/athena_linker.py` & `splink-3.9.1/splink/athena/linker.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 class AthenaLinker(Linker):
     def __init__(
         self,
         input_table_or_tables,
         boto3_session: boto3.session.Session,
         output_database: str,
         output_bucket: str,
-        settings_dict: dict = None,
+        settings_dict: dict | str = None,
         input_table_aliases: str | list = None,
         set_up_basic_logging=True,
         output_filepath: str = "",
     ):
         """An athena backend for our main linker class. This funnels our generated SQL
         through athena using awswrangler.
         See linker.py for more information on the main linker class.
@@ -133,62 +133,66 @@
                 should contain user credentials and region information.
             output_database (str): The name of the database you wish to export the
                 results of the link job to. This should be created prior to performing
                 your link.
             output_bucket (str): The name of the bucket and the filepath you wish to
                 store your outputs in on aws. The bucket should be created prior to
                 performing your link.
-            settings_dict (dict): A splink settings dictionary.
+            settings_dict (dict | Path, optional): A Splink settings dictionary, or
+                 a path to a json defining a settingss dictionary or pre-trained model.
+                  If not provided when the object is created, can later be added using
+                `linker.load_settings()` or `linker.load_model()` Defaults to None.
             input_table_aliases: Aliases/custom names for your input tables, if
                 a pandas df or a list of dfs are used as inputs. None by default, which
                 saves your tables under a custom name: '__splink__input_table_{n}';
                 where n is the list index.
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             output_filepath (str, optional): Inside of your selected output bucket,
                 where to write output files to.
                 Defaults to "splink_warehouse/{unique_id}".
         Examples:
-            >>> # Creating a database in athena and writing to it
-            >>> import awswrangler as wr
-            >>> wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
-            >>>
-            >>> from splink.athena.athena_linker import AthenaLinker
-            >>> import boto3
-            >>> # Create a session - please see the boto3 documentation for more info
-            >>> my_session = boto3.Session(region_name="eu-west-1")
-            >>>
-            >>> linker = AthenaLinker(
-            >>>     settings_dict=settings_dict,
-            >>>     input_table_or_tables="synthetic_data_all",
-            >>>     boto3_session=my_session,
-            >>>     output_bucket="alpha-splink-db-testing",
-            >>>     output_database="splink_awswrangler_test",
-            >>> )
-            >>>
-            >>>
-            >>>
-            >>> # Creating a secondary database and use data on and existing db
-            >>> import awswrangler as wr
-            >>> wr.catalog.create_database("splink_awswrangler_test2", exist_ok=True)
-            >>>
-            >>> from splink.athena.athena_linker import AthenaLinker
-            >>> import boto3
-            >>> my_session = boto3.Session(region_name="eu-west-1")
-            >>>
-            >>> # To read and write from separate databases, specify your secondary
-            >>> # database as the output and enter your primary database as a schema
-            >>> # for your input table(s)
-            >>> linker = AthenaLinker(
-            >>>     settings_dict=settings_dict,
-            >>>     input_table_or_tables="splink_awswrangler_test.synthetic_data_all",
-            >>>     boto3_session=my_session,
-            >>>     output_bucket="alpha-splink-db-testing",
-            >>>     output_database="splink_awswrangler_test2",
-            >>> )
+            ```py
+            # Creating a database in athena and writing to it
+            import awswrangler as wr
+            wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
+            >>>
+            from splink.athena.athena_linker import AthenaLinker
+            import boto3
+            # Create a session - please see the boto3 documentation for more info
+            my_session = boto3.Session(region_name="eu-west-1")
+            >>>
+            linker = AthenaLinker(
+                settings_dict=settings_dict,
+                input_table_or_tables="synthetic_data_all",
+                boto3_session=my_session,
+                output_bucket="alpha-splink-db-testing",
+                output_database="splink_awswrangler_test",
+            )
+            ```
+            ```py
+            # Creating a secondary database and use data on and existing db
+            import awswrangler as wr
+            wr.catalog.create_database("splink_awswrangler_test2", exist_ok=True)
+            >>>
+            from splink.athena.athena_linker import AthenaLinker
+            import boto3
+            my_session = boto3.Session(region_name="eu-west-1")
+            >>>
+            # To read and write from separate databases, specify your secondary
+            # database as the output and enter your primary database as a schema
+            # for your input table(s)
+            linker = AthenaLinker(
+                settings_dict=settings_dict,
+                input_table_or_tables="splink_awswrangler_test.synthetic_data_all",
+                boto3_session=my_session,
+                output_bucket="alpha-splink-db-testing",
+                output_database="splink_awswrangler_test2",
+            )
+            ```
         """
 
         if not type(boto3_session) == boto3.session.Session:
             raise ValueError("Please enter a valid boto3 session object.")
 
         self._sql_dialect_ = "presto"
```

### Comparing `splink-3.9.0/splink/block_from_labels.py` & `splink-3.9.1/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/blocking.py` & `splink-3.9.1/splink/blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/charts.py` & `splink-3.9.1/splink/charts.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/cluster_studio.py` & `splink-3.9.1/splink/cluster_studio.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison.py` & `splink-3.9.1/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_helpers.py` & `splink-3.9.1/splink/comparison_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_helpers_utils.py` & `splink-3.9.1/splink/comparison_helpers_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_level.py` & `splink-3.9.1/splink/comparison_level.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_level_composition.py` & `splink-3.9.1/splink/comparison_level_composition.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_level_library.py` & `splink-3.9.1/splink/comparison_level_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,26 @@
 
 
 class ExactMatchLevelBase(ComparisonLevel):
     def __init__(
         self,
         col_name,
         regex_extract: str = None,
+        set_to_lowercase: bool = False,
         m_probability=None,
         term_frequency_adjustments=False,
         include_colname_in_charts_label=False,
         manual_chart_label=None,
     ) -> ComparisonLevel:
         """Represents a comparison level where there is an exact match,
 
         Args:
             col_name (str): Input column name
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             m_probability (float, optional): Starting value for m probability
                 Defaults to None.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             include_colname_in_charts_label (bool, optional): If True, include col_name
                 in chart labels (e.g. linker.match_weights_chart())
             chart_label (str, optional): string to include in chart label. Setting to
@@ -174,19 +176,23 @@
         if include_colname_in_charts_label:
             label_suffix = f" {col_name}"
         elif manual_chart_label:
             label_suffix = f" {manual_chart_label}"
         else:
             label_suffix = ""
 
+        col_name_l, col_name_r = col.name_l(), col.name_r()
+
+        if set_to_lowercase:
+            col_name_l = f"lower({col_name_l})"
+            col_name_r = f"lower({col_name_r})"
+
         if regex_extract:
-            col_name_l = self._regex_extract_function(col.name_l(), regex_extract)
-            col_name_r = self._regex_extract_function(col.name_r(), regex_extract)
-        else:
-            col_name_l, col_name_r = col.name_l(), col.name_r()
+            col_name_l = self._regex_extract_function(col_name_l, regex_extract)
+            col_name_r = self._regex_extract_function(col_name_r, regex_extract)
 
         sql_cond = f"{col_name_l} = {col_name_r}"
         level_dict = {
             "sql_condition": sql_cond,
             "label_for_charts": f"Exact match{label_suffix}",
         }
         if m_probability:
@@ -245,27 +251,29 @@
 class DistanceFunctionLevelBase(ComparisonLevel):
     def __init__(
         self,
         col_name: str,
         distance_function_name: str,
         distance_threshold: int | float,
         regex_extract: str = None,
+        set_to_lowercase=False,
         higher_is_more_similar: bool = True,
         include_colname_in_charts_label=False,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a user-provided distance function,
         where the similarity
 
         Args:
             col_name (str): Input column name
             distance_function_name (str): The name of the distance function
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             higher_is_more_similar (bool): If True, a higher value of the
                 distance function indicates a higher similarity (e.g. jaro_winkler).
                 If false, a higher value indicates a lower similarity
                 (e.g. levenshtein).
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
             m_probability (float, optional): Starting value for m probability
@@ -307,19 +315,23 @@
         col = InputColumn(col_name, sql_dialect=self._sql_dialect)
 
         if higher_is_more_similar:
             operator = ">="
         else:
             operator = "<="
 
+        col_name_l, col_name_r = col.name_l(), col.name_r()
+
+        if set_to_lowercase:
+            col_name_l = f"lower({col_name_l})"
+            col_name_r = f"lower({col_name_r})"
+
         if regex_extract:
-            col_name_l = self._regex_extract_function(col.name_l(), regex_extract)
-            col_name_r = self._regex_extract_function(col.name_r(), regex_extract)
-        else:
-            col_name_l, col_name_r = col.name_l(), col.name_r()
+            col_name_l = self._regex_extract_function(col_name_l, regex_extract)
+            col_name_r = self._regex_extract_function(col_name_r, regex_extract)
 
         sql_cond = (
             f"{distance_function_name}({col_name_l}, {col_name_r}) "
             f"{operator} {distance_threshold}"
         )
 
         label_suffix = f" {col_name}" if include_colname_in_charts_label else ""
@@ -345,24 +357,26 @@
 
 class LevenshteinLevelBase(DistanceFunctionLevelBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold: int,
         regex_extract: str = None,
+        set_to_lowercase=False,
         include_colname_in_charts_label=False,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a levenshtein distance function,
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
@@ -413,40 +427,43 @@
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 levenshtein similarity
         """
         super().__init__(
             col_name,
-            self._levenshtein_name,
-            distance_threshold,
-            regex_extract,
-            False,
+            distance_function_name=self._levenshtein_name,
+            distance_threshold=distance_threshold,
+            regex_extract=regex_extract,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=False,
             include_colname_in_charts_label=include_colname_in_charts_label,
             m_probability=m_probability,
         )
 
 
 class DamerauLevenshteinLevelBase(DistanceFunctionLevelBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold: int,
         regex_extract: str = None,
+        set_to_lowercase=False,
         include_colname_in_charts_label=False,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a damerau-levenshtein distance
         function,
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
@@ -482,39 +499,42 @@
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 Damerau-Levenshtein similarity
         """
         super().__init__(
             col_name,
-            self._damerau_levenshtein_name,
-            distance_threshold,
-            regex_extract,
-            False,
+            distance_function_name=self._damerau_levenshtein_name,
+            distance_threshold=distance_threshold,
+            regex_extract=regex_extract,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=False,
             include_colname_in_charts_label=include_colname_in_charts_label,
             m_probability=m_probability,
         )
 
 
 class JaroLevelBase(DistanceFunctionLevelBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold: float,
         regex_extract: str = None,
+        set_to_lowercase=False,
         include_colname_in_charts_label=False,
         m_probability=None,
     ):
         """Represents a comparison using the jaro distance function
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
@@ -548,38 +568,41 @@
             ComparisonLevel: A comparison level that evaluates the
                 jaro similarity
         """
 
         super().__init__(
             col_name,
             self._jaro_name,
-            distance_threshold,
-            regex_extract,
-            True,
+            distance_threshold=distance_threshold,
+            regex_extract=regex_extract,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=True,
             include_colname_in_charts_label=include_colname_in_charts_label,
             m_probability=m_probability,
         )
 
 
 class JaroWinklerLevelBase(DistanceFunctionLevelBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold: float,
         regex_extract: str = None,
+        set_to_lowercase=False,
         include_colname_in_charts_label=False,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using the jaro winkler distance function
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
@@ -591,15 +614,15 @@
                 Comparison level with jaro-winkler score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
                 import splink.duckdb.duckdb_comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
-                Comparison level with jaro score greater than 0.9
+                Comparison level with jaro-winkler score greater than 0.9
                 ``` python
                 import splink.spark.spark_comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9)
                 ```
                 Comparison level with jaro-winkler score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
@@ -611,17 +634,18 @@
             ComparisonLevel: A comparison level that evaluates the
                 jaro winkler similarity
         """
 
         super().__init__(
             col_name,
             self._jaro_winkler_name,
-            distance_threshold,
-            regex_extract,
-            True,
+            distance_threshold=distance_threshold,
+            regex_extract=regex_extract,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=True,
             include_colname_in_charts_label=include_colname_in_charts_label,
             m_probability=m_probability,
         )
 
     @property
     def _jaro_winkler_name(self):
         raise NotImplementedError(
@@ -631,24 +655,26 @@
 
 class JaccardLevelBase(DistanceFunctionLevelBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold: int | float,
         regex_extract: str = None,
+        set_to_lowercase=False,
         include_colname_in_charts_label=False,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a jaccard distance function
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
         Examples:
             === "DuckDB"
                 Comparison level with jaccard score greater than 0.9
@@ -677,108 +703,119 @@
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the jaccard similarity
         """
         super().__init__(
             col_name,
             self._jaccard_name,
-            distance_threshold,
-            regex_extract,
-            True,
+            distance_threshold=distance_threshold,
+            regex_extract=regex_extract,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=True,
             include_colname_in_charts_label=include_colname_in_charts_label,
             m_probability=m_probability,
         )
 
 
 class ColumnsReversedLevelBase(ComparisonLevel):
     def __init__(
         self,
         col_name_1: str,
         col_name_2: str,
         regex_extract: str = None,
+        set_to_lowercase=False,
         m_probability=None,
         tf_adjustment_column=None,
     ) -> ComparisonLevel:
         """Represents a comparison level where the columns are reversed.  For example,
         if surname is in the forename field and vice versa
 
         Args:
             col_name_1 (str): First column, e.g. forename
             col_name_2 (str): Second column, e.g. surname
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
             tf_adjustment_column (str, optional): Column to use for term frequency
                 adjustments if an exact match is observed. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Comparison level on first_name and surname columns reversed
-
                 ``` python
                 import splink.duckdb.duckdb_comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
                 import splink.duckdb.duckdb_comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
+                Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.spark.spark_comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
                 import splink.spark.spark_comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
             === "Athena"
+                Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.athena.athena_comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
                 import splink.athena.athena_comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
             === "SQLite"
+                Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.sqlite.sqlite_comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
 
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the exact match of two
                 columns.
         """
 
         col_1 = InputColumn(col_name_1, sql_dialect=self._sql_dialect)
         col_2 = InputColumn(col_name_2, sql_dialect=self._sql_dialect)
 
+        col_1_l, col_1_r = col_1.name_l(), col_1.name_r()
+        col_2_l, col_2_r = col_2.name_l(), col_2.name_r()
+
+        if set_to_lowercase:
+            col_1_l = f"lower({col_1_l})"
+            col_1_r = f"lower({col_1_r})"
+            col_2_l = f"lower({col_2_l})"
+            col_2_r = f"lower({col_2_r})"
+
         if regex_extract:
-            col_1_l = self._regex_extract_function(col_1.name_l(), regex_extract)
-            col_1_r = self._regex_extract_function(col_1.name_r(), regex_extract)
-            col_2_l = self._regex_extract_function(col_2.name_l(), regex_extract)
-            col_2_r = self._regex_extract_function(col_2.name_r(), regex_extract)
-        else:
-            col_1_l, col_1_r = col_1.name_l(), col_1.name_r()
-            col_2_l, col_2_r = col_2.name_l(), col_2.name_r()
+            col_1_l = self._regex_extract_function(col_1_l, regex_extract)
+            col_1_r = self._regex_extract_function(col_1_r, regex_extract)
+            col_2_l = self._regex_extract_function(col_2_l, regex_extract)
+            col_2_r = self._regex_extract_function(col_2_r, regex_extract)
 
         s = f"{col_1_l} = {col_2_r} and " f"{col_1_r} = {col_2_l}"
         level_dict = {
             "sql_condition": s,
             "label_for_charts": "Exact match on reversed cols",
         }
         if m_probability:
```

### Comparing `splink-3.9.0/splink/comparison_level_sql.py` & `splink-3.9.1/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_library.py` & `splink-3.9.1/splink/comparison_library.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 
 class ExactMatchBase(Comparison):
     def __init__(
         self,
         col_name,
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_else=None,
         include_colname_in_charts_label=False,
     ) -> Comparison:
         """A comparison of the data in `col_name` with two levels:
         - Exact match
         - Anything else
 
         Args:
             col_name (str): The name of the column to compare
             regex_extract (str): Regular expression pattern to evaluate a match on.
             valid_string_regex (str): regular expression pattern that if not
                 matched will result in column being treated as a null.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             term_frequency_adjustments (bool, optional): If True, term frequency
                 adjustments will be made on the exact match level. Defaults to False.
             m_probability_exact_match (float, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
             include_colname_in_charts_label: If true, append col name to label for
@@ -59,25 +61,27 @@
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
                 import splink.spark.spark_comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
+                ```
             === "Athena"
                 Create comparison with exact match level
                 ``` python
                 import splink.athena.athena_comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
                 import splink.athena.athena_comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
+                ```
             === "SQLite"
                 Create comparison with exact match level
                 ``` python
                 import splink.sqlite.sqlite_comparison_library as cl
                 cl.exact_match("first_name")
                 ```
 
@@ -89,14 +93,15 @@
         comparison_dict = {
             "comparison_description": "Exact match vs. anything else",
             "comparison_levels": [
                 self._null_level(col_name, valid_string_regex),
                 self._exact_match_level(
                     col_name,
                     regex_extract=regex_extract,
+                    set_to_lowercase=set_to_lowercase,
                     term_frequency_adjustments=term_frequency_adjustments,
                     m_probability=m_probability_exact_match,
                     include_colname_in_charts_label=include_colname_in_charts_label,
                 ),
                 self._else_level(m_probability=m_probability_else),
             ],
         }
@@ -107,14 +112,15 @@
     def __init__(
         self,
         col_name: str,
         distance_function_name: str,
         distance_threshold_or_thresholds: float | list,
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         higher_is_more_similar: bool = True,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_thres: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
@@ -138,16 +144,17 @@
         Args:
             col_name (str): The name of the column to compare
             distance_function_name (str): The name of the distance function.
             distance_threshold_or_thresholds (Union[int, list], optional): The
                 threshold(s) to use for the middle similarity level(s).
                 Defaults to [1, 2].
             regex_extract (str): Regular expression pattern to evaluate a match on.
-             valid_string_regex (str): regular expression pattern that if not
+            valid_string_regex (str): regular expression pattern that if not
                 matched will result in column being treated as a null.
+            set_to_lowercase (bool): If True, sets all entries to lowercase.
             higher_is_more_similar (bool): If True, a higher value of the distance
                 function indicates a higher similarity (e.g. jaro_winkler).
                 If false, a higher value indicates a lower similarity
                 (e.g. levenshtein).
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
@@ -237,24 +244,27 @@
 
         comparison_levels = []
         comparison_levels.append(self._null_level(col_name, valid_string_regex))
         if include_exact_match_level:
             level = self._exact_match_level(
                 col_name,
                 term_frequency_adjustments=term_frequency_adjustments,
+                regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_exact_match,
             )
             comparison_levels.append(level)
 
         threshold_comparison_levels = distance_threshold_comparison_levels(
             self,
             col_name,
             distance_function_name,
             distance_threshold_or_thresholds,
             regex_extract,
+            set_to_lowercase,
             m_probability_or_probabilities_thres,
         )
         comparison_levels = comparison_levels + threshold_comparison_levels
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
         )
@@ -285,14 +295,15 @@
 class LevenshteinAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [1, 2],
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_lev: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
         """A comparison of the data in `col_name` with the levenshtein distance used to
@@ -373,24 +384,25 @@
         Returns:
             Comparison: A comparison for Levenshtein similarity that can be included
                 in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
-            self._levenshtein_name,
-            distance_threshold_or_thresholds,
-            regex_extract,
-            valid_string_regex,
-            False,
-            include_exact_match_level,
-            term_frequency_adjustments,
-            m_probability_exact_match,
-            m_probability_or_probabilities_lev,
-            m_probability_else,
+            distance_function_name=self._levenshtein_name,
+            distance_threshold_or_thresholds=distance_threshold_or_thresholds,
+            regex_extract=regex_extract,
+            valid_string_regex=valid_string_regex,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=False,
+            include_exact_match_level=include_exact_match_level,
+            term_frequency_adjustments=term_frequency_adjustments,
+            m_probability_exact_match=m_probability_exact_match,
+            m_probability_or_probabilities_thres=m_probability_or_probabilities_lev,
+            m_probability_else=m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
@@ -399,14 +411,15 @@
 ):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = 1,
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_dl: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
         """A comparison of the data in `col_name` with the damerau-levenshtein distance
@@ -436,36 +449,37 @@
             m_probability_or_probabilities_dl (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
         Examples:
             === "DuckDB"
-                Create comparison with demerau-levenshtein match levels with
+                Create comparison with damerau-levenshtein match levels with
                 distance <= 1
                 ``` python
                 import splink.duckdb.duckdb_comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
-                Create comparison with demerau-levenshtein match levels with
+                Create comparison with damerau-levenshtein match levels with
                 distance <= 1
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.duckdb.duckdb_comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name",
                                                      [1,2],
                                                      regex_extract="^A|B")
                 ```
             === "Spark"
-                Create comparison with demerau-levenshtein match levels with
-                distance <= 1                ``` python
+                Create comparison with damerau-levenshtein match levels with
+                distance <= 1
+                ``` python
                 import splink.spark.spark_comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
-                Create comparison with demerau-evenshtein match levels with
+                Create comparison with damerau-evenshtein match levels with
                 distance <= 1
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.spark.spark_comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name",
                                                      [1,2],
                                                      regex_extract="^A|B")
@@ -474,38 +488,40 @@
         Returns:
             Comparison: A comparison for Damerau-Levenshtein similarity that can be
             included in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
-            self._levenshtein_name,
-            distance_threshold_or_thresholds,
-            regex_extract,
-            valid_string_regex,
-            False,
-            include_exact_match_level,
-            term_frequency_adjustments,
-            m_probability_exact_match,
-            m_probability_or_probabilities_dl,
-            m_probability_else,
+            distance_function_name=self._levenshtein_name,
+            distance_threshold_or_thresholds=distance_threshold_or_thresholds,
+            regex_extract=regex_extract,
+            valid_string_regex=valid_string_regex,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=False,
+            include_exact_match_level=include_exact_match_level,
+            term_frequency_adjustments=term_frequency_adjustments,
+            m_probability_exact_match=m_probability_exact_match,
+            m_probability_or_probabilities_thres=m_probability_or_probabilities_dl,
+            m_probability_else=m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
 class JaccardAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_jac: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
         """A comparison of the data in `col_name` with the jaccard distance used to
@@ -572,38 +588,40 @@
         Returns:
             Comparison: A comparison for Jaccard similarity that can be included
                 in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
-            self._jaccard_name,
-            distance_threshold_or_thresholds,
-            regex_extract,
-            valid_string_regex,
-            True,
-            include_exact_match_level,
-            term_frequency_adjustments,
-            m_probability_exact_match,
-            m_probability_or_probabilities_jac,
-            m_probability_else,
+            distance_function_name=self._jaccard_name,
+            distance_threshold_or_thresholds=distance_threshold_or_thresholds,
+            regex_extract=regex_extract,
+            valid_string_regex=valid_string_regex,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=True,
+            include_exact_match_level=include_exact_match_level,
+            term_frequency_adjustments=term_frequency_adjustments,
+            m_probability_exact_match=m_probability_exact_match,
+            m_probability_or_probabilities_thres=m_probability_or_probabilities_jac,
+            m_probability_else=m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
 class JaroAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_jar: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
         """A comparison of the data in `col_name` with the jaro distance used to
@@ -661,45 +679,48 @@
                 ```
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
                 import splink.spark.spark_comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7], regex_extract="^[A-Z]")
+                ```
 
         Returns:
             Comparison:
         """
 
         super().__init__(
             col_name,
-            self._jaro_name,
-            distance_threshold_or_thresholds,
-            regex_extract,
-            valid_string_regex,
-            True,
-            include_exact_match_level,
-            term_frequency_adjustments,
-            m_probability_exact_match,
-            m_probability_or_probabilities_jar,
-            m_probability_else,
+            distance_function_name=self._jaro_name,
+            distance_threshold_or_thresholds=distance_threshold_or_thresholds,
+            regex_extract=regex_extract,
+            valid_string_regex=valid_string_regex,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=True,
+            include_exact_match_level=include_exact_match_level,
+            term_frequency_adjustments=term_frequency_adjustments,
+            m_probability_exact_match=m_probability_exact_match,
+            m_probability_or_probabilities_thres=m_probability_or_probabilities_jar,
+            m_probability_else=m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
 class JaroWinklerAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         regex_extract: str = None,
         valid_string_regex: str = None,
+        set_to_lowercase: bool = False,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_jw: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
         """A comparison of the data in `col_name` with the jaro_winkler distance used to
@@ -732,44 +753,40 @@
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
 
         Examples:
             === "DuckDB"
-                Create comparison with jaro_winkler match levels with similarity score
-                >=0.9
-                and >=0.7
+                Create comparison with jaro_winkler match levels with similarity
+                score >= 0.9 and >=0.7
                 ``` python
                 import splink.duckdb.duckdb_comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
-                Create comparison with jaro_winkler match levels with similarity score
-                >=0.9
-                and >=0.7 on a substring of name column as determined by a regular
-                expression
+                Create comparison with jaro_winkler match levels with similarity
+                score =>0.9 and >=0.7 on a substring of name column as determined by
+                a regular expression
                 ``` python
                 import splink.duckdb.duckdb_comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name",
                                               [0.9, 0.7],
                                               regex_extract="^[A-Z]"
                                               )
                 ```
             === "Spark"
-                Create comparison with jaro_winkler match levels with similarity score
-                >=0.9
-                and >=0.7
+                Create comparison with jaro_winkler match levels with similarity
+                score >=0.9 and >=0.7
                 ``` python
                 import splink.spark.spark_comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
-                Create comparison with jaro_winkler match levels with similarity score
-                >=0.9
-                and >=0.7 on a substring of name column as determined by a regular
-                expression
+                Create comparison with jaro_winkler match levels with similarity
+                score >=0.9 and >=0.7 on a substring of name column as determined
+                by a regular expression
                 ``` python
                 import splink.spark.spark_comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name",
                                               [0.9, 0.7],
                                               regex_extract="^[A-Z]"
                                               )
                 ```
@@ -777,24 +794,25 @@
         Returns:
             Comparison: A comparison for Jaro Winkler similarity that can be included
                 in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
-            self._jaro_winkler_name,
-            distance_threshold_or_thresholds,
-            regex_extract,
-            valid_string_regex,
-            True,
-            include_exact_match_level,
-            term_frequency_adjustments,
-            m_probability_exact_match,
-            m_probability_or_probabilities_jw,
-            m_probability_else,
+            distance_function_name=self._jaro_winkler_name,
+            distance_threshold_or_thresholds=distance_threshold_or_thresholds,
+            regex_extract=regex_extract,
+            valid_string_regex=valid_string_regex,
+            set_to_lowercase=set_to_lowercase,
+            higher_is_more_similar=True,
+            include_exact_match_level=include_exact_match_level,
+            term_frequency_adjustments=term_frequency_adjustments,
+            m_probability_exact_match=m_probability_exact_match,
+            m_probability_or_probabilities_thres=m_probability_or_probabilities_jw,
+            m_probability_else=m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
```

### Comparing `splink-3.9.0/splink/comparison_library_utils.py` & `splink-3.9.1/splink/comparison_library_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 def distance_threshold_comparison_levels(
     self,
     col_name: str,
     distance_function_name: str,
     distance_threshold_or_thresholds,
     regex_extract: str = None,
+    set_to_lowercase: bool = False,
     higher_is_more_similar: bool = True,
     include_colname_in_charts_label=False,
     m_probability_or_probabilities_thres: list = None,
 ):
     thresholds = ensure_is_iterable(distance_threshold_or_thresholds)
     threshold_comparison_levels = []
 
@@ -100,14 +101,15 @@
 
         # these function arguments hold for all cases.
         kwargs = dict(
             col_name=col_name,
             distance_threshold=thres,
             include_colname_in_charts_label=include_colname_in_charts_label,
             regex_extract=regex_extract,
+            set_to_lowercase=set_to_lowercase,
             m_probability=m_prob,
         )
         # separate out the two that are only used
         # when we have a user-supplied function, rather than a predefined subclass
         # feels a bit hacky, but will do at least for time being
         if not self._is_distance_subclass:
             kwargs["distance_function_name"] = distance_function_name
```

### Comparing `splink-3.9.0/splink/comparison_template_library.py` & `splink-3.9.1/splink/comparison_template_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -294,14 +294,15 @@
 
 
 class NameComparisonBase(Comparison):
     def __init__(
         self,
         col_name: str,
         regex_extract: str = None,
+        set_to_lowercase: str = False,
         include_exact_match_level: bool = True,
         phonetic_col_name: str = None,
         term_frequency_adjustments: bool = False,
         levenshtein_thresholds: int | list = [],
         damerau_levenshtein_thresholds: int | list = [1],
         jaro_thresholds: float | list = [],
         jaro_winkler_thresholds: float | list = [0.9, 0.8],
@@ -324,14 +325,17 @@
         - Jaro Winkler similarity >= 0.9\n
         - Jaro Winkler similarity >= 0.8\n
         - Anything else
 
         Args:
             col_name (str): The name of the column to compare.
             regex_extract (str): Regular expression pattern to evaluate a match on.
+            set_to_lowercase (bool): If True, all names are set to lowercase
+                during the pairwise comparisons.
+                Defaults to False
             include_exact_match_level (bool, optional): If True, include an exact match
                 level for col_name. Defaults to True.
             phonetic_col_name (str): The name of the column with phonetic reduction
                 (such as dmetaphone) of col_name. Including parameter will create
                 an exact match level for  phonetic_col_name. The phonetic column must
                 be present in the dataset to use this parameter.
                 Defaults to None
@@ -434,35 +438,38 @@
         if include_exact_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
                 term_frequency_adjustments=term_frequency_adjustments,
                 m_probability=m_probability_exact_match_name,
                 include_colname_in_charts_label=True,
                 regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
             )
             comparison_levels.append(comparison_level)
 
             if phonetic_col_name is not None:
                 comparison_level = self._exact_match_level(
                     phonetic_col_name,
                     term_frequency_adjustments=term_frequency_adjustments,
                     m_probability=m_probability_exact_match_phonetic_name,
                     include_colname_in_charts_label=True,
                     regex_extract=regex_extract,
+                    set_to_lowercase=set_to_lowercase,
                 )
                 comparison_levels.append(comparison_level)
 
         levenshtein_thresholds = ensure_is_iterable(levenshtein_thresholds)
         if len(levenshtein_thresholds) > 0:
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 col_name,
                 distance_function_name="levenshtein",
                 distance_threshold_or_thresholds=levenshtein_thresholds,
                 regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_lev,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         damerau_levenshtein_thresholds = ensure_is_iterable(
             damerau_levenshtein_thresholds
         )
@@ -470,50 +477,54 @@
             levenshtein_thresholds = ensure_is_iterable(damerau_levenshtein_thresholds)
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 col_name,
                 distance_function_name="damerau-levenshtein",
                 distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
                 regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_dl,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         jaro_thresholds = ensure_is_iterable(jaro_thresholds)
         if len(jaro_thresholds) > 0:
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 col_name,
                 distance_function_name="jaro",
                 distance_threshold_or_thresholds=jaro_thresholds,
                 regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_jar,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         jaro_winkler_thresholds = ensure_is_iterable(jaro_winkler_thresholds)
         if len(jaro_winkler_thresholds) > 0:
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 col_name,
                 distance_function_name="jaro-winkler",
                 distance_threshold_or_thresholds=jaro_winkler_thresholds,
                 regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_jw,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         jaccard_thresholds = ensure_is_iterable(jaccard_thresholds)
         if len(jaccard_thresholds) > 0:
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 col_name,
                 distance_function_name="jaccard",
                 distance_threshold_or_thresholds=jaccard_thresholds,
                 regex_extract=regex_extract,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_jar,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
         )
@@ -568,14 +579,15 @@
 
 
 class ForenameSurnameComparisonBase(Comparison):
     def __init__(
         self,
         forename_col_name,
         surname_col_name,
+        set_to_lowercase=False,
         include_exact_match_level: bool = True,
         include_columns_reversed: bool = True,
         term_frequency_adjustments: bool = False,
         tf_adjustment_col_forename_and_surname: str = None,
         phonetic_forename_col_name: str = None,
         phonetic_surname_col_name: str = None,
         levenshtein_thresholds: int | list = [],
@@ -611,14 +623,17 @@
         - Fuzzy match surname jaro-winkler >= 0.88\n
         - Fuzzy match forename jaro-winkler>=  0.88\n
         - Anything else
 
         Args:
             forename_col_name (str): The name of the forename column to compare
             surname_col_name (str): The name of the surname column to compare
+            set_to_lowercase (bool): If True, all names are set to lowercase
+                during the pairwise comparisons.
+                Defaults to False
             include_exact_match_level (bool, optional): If True, include an exact match
                 level for col_name. Defaults to True.
             include_columns_reversed (bool, optional): If True, include a comparison
                 level for forename and surname being swapped. Defaults to True
             term_frequency_adjustments (bool, optional): If True, apply term
                 frequency adjustments to the exact match level for forename_col_name
                 and surname_col_name.
@@ -629,14 +644,17 @@
                 and phonetic_surname_col_name exact match levels, if they are provided.
                 Defaults to False.
             tf_adjustment_col_forename_and_surname (str, optional): The name
                 of a combined forename surname column. This column is used to provide
                 term frequency adjustments for forename surname exact match and columns
                 reversed levels.
                 Defaults to None
+            set_to_lowercase (bool): If True, all postcodes are set to lowercase
+                during the pairwise comparisons.
+                Defaults to True
             phonetic_forename_col_name (str, optional): The name of the column with
                 phonetic reduction (such as dmetaphone) of forename_col_name. Including
                 parameter will create an exact match level for
                 phonetic_forename_col_name.
                 The phonetic column must be present in the dataset to use this
                 parameter.
                 Defaults to None
@@ -786,17 +804,28 @@
         )
 
         comparison_levels.append(comparison_level)
 
         ### Forename surname exact match
 
         if include_exact_match_level:
+            if set_to_lowercase:
+                forename_col_name_l = f"lower({forename_col_name}_l)"
+                forename_col_name_r = f"lower({forename_col_name}_r)"
+                surname_col_name_l = f"lower({surname_col_name}_l)"
+                surname_col_name_r = f"lower({surname_col_name}_r)"
+            else:
+                forename_col_name_l = f"{forename_col_name}_l"
+                forename_col_name_r = f"{forename_col_name}_r"
+                surname_col_name_l = f"{surname_col_name}_l"
+                surname_col_name_r = f"{surname_col_name}_r"
+
             comparison_level = {
-                "sql_condition": f"{forename_col_name}_l = {forename_col_name}_r "
-                f"AND {surname_col_name}_l = {surname_col_name}_r",
+                "sql_condition": f"{forename_col_name_l} = {forename_col_name_r} "
+                f"AND {surname_col_name_l} = {surname_col_name_r}",
                 "tf_adjustment_column": tf_adjustment_col_forename_and_surname,
                 "tf_adjustment_weight": 1.0,
                 "m_probability": m_probability_exact_match_forename_surname,
                 "label_for_charts": "Full name exact match",
             }
 
             comparison_levels.append(comparison_level)
@@ -817,33 +846,36 @@
 
         ### Columns reversed match
 
         if include_columns_reversed:
             comparison_level = self._columns_reversed_level(
                 forename_col_name,
                 surname_col_name,
+                set_to_lowercase=set_to_lowercase,
                 tf_adjustment_column=tf_adjustment_col_forename_and_surname,
                 m_probability=m_probability_columns_reversed_forename_surname,
             )
             comparison_levels.append(comparison_level)
 
         ### Surname Exact match
 
         comparison_level = self._exact_match_level(
             surname_col_name,
+            set_to_lowercase=set_to_lowercase,
             term_frequency_adjustments=term_frequency_adjustments,
             m_probability=m_probability_exact_match_forename,
             include_colname_in_charts_label=True,
         )
         comparison_levels.append(comparison_level)
 
         ### Forename Exact match
 
         comparison_level = self._exact_match_level(
             forename_col_name,
+            set_to_lowercase=set_to_lowercase,
             term_frequency_adjustments=term_frequency_adjustments,
             m_probability=m_probability_exact_match_forename,
             include_colname_in_charts_label=True,
         )
         comparison_levels.append(comparison_level)
 
         ### Ensure fuzzy match thresholds are iterable
@@ -858,104 +890,113 @@
         ### Surname Fuzzy match
         if len(levenshtein_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 surname_col_name,
                 distance_function_name="levenshtein",
                 distance_threshold_or_thresholds=levenshtein_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_lev,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(damerau_levenshtein_thresholds) > 0:
             levenshtein_thresholds = ensure_is_iterable(damerau_levenshtein_thresholds)
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 surname_col_name,
                 distance_function_name="damerau-levenshtein",
                 distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_dl,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         if len(jaro_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 surname_col_name,
                 distance_function_name="jaro-winkler",
                 distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_jw,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(jaro_winkler_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 surname_col_name,
                 distance_function_name="jaro-winkler",
                 distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_jw,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(jaccard_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 surname_col_name,
                 distance_function_name="jaccard",
                 distance_threshold_or_thresholds=jaccard_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_jac,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         ### Forename Fuzzy match
 
         if len(levenshtein_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 forename_col_name,
                 distance_function_name="levenshtein",
                 distance_threshold_or_thresholds=levenshtein_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_forename_lev,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(damerau_levenshtein_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 forename_col_name,
                 distance_function_name="damerau-levenshtein",
                 distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_forename_dl,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(jaro_winkler_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 forename_col_name,
                 distance_function_name="jaro-winkler",
                 distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_forename_jw,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(jaccard_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 forename_col_name,
                 distance_function_name="jaccard",
                 distance_threshold_or_thresholds=jaccard_thresholds,
+                set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_forename_jac,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
@@ -1040,15 +1081,16 @@
 
 
 class PostcodeComparisonBase(Comparison):
     def __init__(
         self,
         col_name: str,
         invalid_postcodes_as_null=False,
-        valid_postcode_regex="^[A-Z]{1,2}[0-9][A-Z0-9]? [0-9][A-Z]{2}$",
+        set_to_lowercase=True,
+        valid_postcode_regex="^[A-Za-z]{1,2}[0-9][A-Za-z0-9]? [0-9][A-Za-z]{2}$",
         term_frequency_adjustments_full=False,
         include_full_match_level=True,
         include_sector_match_level=True,
         include_district_match_level=True,
         include_area_match_level=True,
         lat_col: str = None,
         long_col: str = None,
@@ -1071,19 +1113,22 @@
         - All other comparisons
 
         Args:
             col_name (str): The name of the column to compare.
             invalid_postcodes_as_null (bool): If True, postcodes that do not adhere
                 to valid_postcode_regex will be included in the null level.
                 Defaults to False
+            set_to_lowercase (bool): If True, all postcodes are set to lowercase
+                during the pairwise comparisons.
+                Defaults to True
             valid_postcode_regex (str): regular expression pattern that is used
                 to validate postcodes. If invalid_postcodes_as_null is True,
                 postcodes that do not adhere to valid_postcode_regex will be included
                  in the null level.
-                 Defaults to "^[A-Z]{1,2}[0-9][A-Z0-9]? [0-9][A-Z]{2}$"
+                 Defaults to "^[A-Za-z]{1,2}[0-9][A-Za-z0-9]? [0-9][A-Za-z]{2}$"
             term_frequency_adjustments_full (bool, optional): If True, apply
                 term frequency adjustments to the full postcode exact match level.
                 Defaults to False.
             include_full_match_level (bool, optional): If True, include an exact
                 match on full postcode level. Defaults to True.
             include_sector_match_level (bool, optional): If True, include an exact
                 match on sector level. Defaults to True.
@@ -1181,41 +1226,45 @@
             comparison_levels.append(self._null_level(col_name))
 
         if include_full_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
                 regex_extract=None,
                 term_frequency_adjustments=term_frequency_adjustments_full,
+                set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_full_match,
                 include_colname_in_charts_label=True,
             )
             comparison_levels.append(comparison_level)
 
         if include_sector_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
-                regex_extract="^[A-Z]{1,2}[0-9][A-Z0-9]? [0-9]",
+                regex_extract="^[A-Za-z]{1,2}[0-9][A-Za-z0-9]? [0-9]",
+                set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_sector_match,
                 manual_chart_label="Postcode Sector",
             )
             comparison_levels.append(comparison_level)
 
         if include_district_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
-                regex_extract="^[A-Z]{1,2}[0-9][A-Z0-9]?",
+                regex_extract="^[A-Za-z]{1,2}[0-9][A-Za-z0-9]?",
+                set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_district_match,
                 manual_chart_label="Postcode District",
             )
             comparison_levels.append(comparison_level)
 
         if include_area_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
-                regex_extract="^[A-Z]{1,2}",
+                regex_extract="^[A-Za-z]{1,2}",
+                set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_area_match,
                 manual_chart_label="Postcode Area",
             )
             comparison_levels.append(comparison_level)
 
         km_thresholds = ensure_is_iterable(km_thresholds)
         if len(km_thresholds) > 0:
```

### Comparing `splink-3.9.0/splink/comparison_vector_distribution.py` & `splink-3.9.1/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/comparison_vector_values.py` & `splink-3.9.1/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/connected_components.py` & `splink-3.9.1/splink/connected_components.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/convert_v2_to_v3.py` & `splink-3.9.1/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/databricks/enable_splink.py` & `splink-3.9.1/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/default_from_jsonschema.py` & `splink-3.9.1/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/dialect_base.py` & `splink-3.9.1/splink/dialect_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_base.py` & `splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py` & `splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/duckdb/duckdb_linker.py` & `splink-3.9.1/splink/duckdb/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 class DuckDBLinker(Linker):
     """Manages the data linkage process and holds the data linkage model."""
 
     def __init__(
         self,
         input_table_or_tables: str | list,
-        settings_dict: dict = None,
+        settings_dict: dict | str = None,
         connection: str | DuckDBPyConnection = ":memory:",
         set_up_basic_logging: bool = True,
         output_schema: str = None,
         input_table_aliases: str | list = None,
     ):
         """The Linker object manages the data linkage process and holds the data linkage
         model.
@@ -113,17 +113,18 @@
         on the linker, such as `linker.predict()`, `linker.profile_columns()` etc.
 
         Args:
             input_table_or_tables (Union[str, list]): Input data into the linkage model.
                 Either a single string (the name of a table in a database) for
                 deduplication jobs, or a list of strings  (the name of tables in a
                 database) for link_only or link_and_dedupe
-            settings_dict (dict, optional): A Splink settings dictionary. If not
-                provided when the object is created, can later be added using
-                `linker.load_settings()` Defaults to None.
+            settings_dict (dict | Path, optional): A Splink settings dictionary, or a
+                 path toa json defining a settingss dictionary or pre-trained model.
+                  If not provided when the object is created, can later be added using
+                `linker.load_settings()` or `linker.load_model()` Defaults to None.
             connection (DuckDBPyConnection or str, optional):  Connection to duckdb.
                 If a a string, will instantiate a new connection.  Defaults to :memory:.
                 If the special :temporary: string is provided, an on-disk duckdb
                 database will be created in a temporary directory.  This can be used
                 if you are running out of memory using :memory:.
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
```

### Comparing `splink-3.9.0/splink/em_training_session.py` & `splink-3.9.1/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/estimate_u.py` & `splink-3.9.1/splink/estimate_u.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/expectation_maximisation.py` & `splink-3.9.1/splink/expectation_maximisation.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.9.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/comparator_score_chart.json` & `splink-3.9.1/splink/files/chart_defs/comparator_score_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-3.9.1/splink/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/completeness.json` & `splink-3.9.1/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json` & `splink-3.9.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json` & `splink-3.9.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/del/compare_estimates.json` & `splink-3.9.1/splink/files/chart_defs/del/compare_estimates.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json` & `splink-3.9.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/del/gamma_histogram.json` & `splink-3.9.1/splink/files/chart_defs/del/gamma_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/del/score_histogram.json` & `splink-3.9.1/splink/files/chart_defs/del/score_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.9.1/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.9.1/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.9.1/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.9.1/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/missingness.json` & `splink-3.9.1/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.9.1/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8586640211640212%*

 * *Differences: {"'config'": "{'title': {'fontSize': 18, 'subtitleFontSize': 14}}",*

 * * "'encoding'": "{'row': {'header': {'labelFontWeight': 'bold', 'labelFontSize': 12}, 'align': "*

 * *               "'each'}, 'column': {'field': 'col_header', 'align': 'each', 'header': "*

 * *               "OrderedDict([('labelFontSize', 14), ('labelFontWeight', 'bold')])}, 'x': {'title': "*

 * *               "'Estimated probability as log odds', 'axis': OrderedDict([('gridColor', "*

 * *               "OrderedDict([('condition', OrderedDict([('test', 'abs […]*

```diff
@@ -1,12 +1,14 @@
 {
     "$schema": "https://vega.github.io/schema/vega-lite/v5.2.0.json",
     "config": {
         "title": {
-            "anchor": "middle"
+            "anchor": "middle",
+            "fontSize": 18,
+            "subtitleFontSize": 14
         },
         "view": {
             "continuousHeight": 300,
             "continuousWidth": 400
         }
     },
     "data": {
@@ -14,24 +16,32 @@
     },
     "encoding": {
         "color": {
             "field": "estimate_description",
             "type": "nominal"
         },
         "column": {
-            "field": "m_or_u",
+            "align": "each",
+            "field": "col_header",
+            "header": {
+                "labelFontSize": 14,
+                "labelFontWeight": "bold"
+            },
             "title": null,
             "type": "nominal"
         },
         "row": {
+            "align": "each",
             "field": "comparison_name",
             "header": {
                 "labelAlign": "left",
                 "labelAnchor": "middle",
-                "labelAngle": 0
+                "labelAngle": 0,
+                "labelFontSize": 12,
+                "labelFontWeight": "bold"
             },
             "sort": {
                 "field": "comparison_sort_order"
             },
             "title": null,
             "type": "nominal"
         },
@@ -58,15 +68,41 @@
             },
             {
                 "field": "estimated_probability",
                 "type": "quantitative"
             }
         ],
         "x": {
+            "axis": {
+                "gridColor": {
+                    "condition": {
+                        "test": "abs(datum.value / 10)  <= 1 & datum.value % 10 === 0",
+                        "value": "#aaa"
+                    },
+                    "value": "#ddd"
+                },
+                "gridDash": {
+                    "condition": {
+                        "test": "abs(datum.value / 10) == 1",
+                        "value": [
+                            3
+                        ]
+                    },
+                    "value": null
+                },
+                "gridWidth": {
+                    "condition": {
+                        "test": "abs(datum.value / 10)  <= 1 & datum.value % 10 === 0",
+                        "value": 2
+                    },
+                    "value": 1
+                }
+            },
             "field": "estimated_probability_as_log_odds",
+            "title": "Estimated probability as log odds",
             "type": "quantitative"
         },
         "y": {
             "axis": {
                 "grid": true,
                 "title": null
             },
@@ -89,17 +125,24 @@
             "y": "independent"
         }
     },
     "selection": {
         "selection_zoom": {
             "bind": "scales",
             "encodings": [
-                "x"
+                "x",
+                "column"
             ],
             "type": "interval"
         }
     },
     "title": {
-        "subtitle": "Use mousewheeel to zoom",
+        "subtitle": "Use mousewheel to zoom",
         "text": "Comparison of parameter estimates across training sessions"
-    }
+    },
+    "transform": [
+        {
+            "as": "col_header",
+            "calculate": "datum.m_or_u + '-probability (as log odds)'"
+        }
+    ]
 }
```

### Comparing `splink-3.9.0/splink/files/chart_defs/phonetic_match_chart.json` & `splink-3.9.1/splink/files/chart_defs/phonetic_match_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/precision_recall.json` & `splink-3.9.1/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.9.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/profile_data.json` & `splink-3.9.1/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/roc.json` & `splink-3.9.1/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/tf_adjustment_chart.json` & `splink-3.9.1/splink/files/chart_defs/tf_adjustment_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.9.1/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/external_js/vega-embed@6.20.2` & `splink-3.9.1/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/external_js/vega-lite@5.2.0` & `splink-3.9.1/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/external_js/vega@5.21.0` & `splink-3.9.1/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/settings_jsonschema.json` & `splink-3.9.1/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.9.1/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/splink_cluster_studio/custom.css` & `splink-3.9.1/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/splink_comparison_viewer/custom.css` & `splink-3.9.1/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/splink_comparison_viewer/template.j2` & `splink-3.9.1/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.9.1/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/input_column.py` & `splink-3.9.1/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/linker.py` & `splink-3.9.1/splink/linker.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,47 +132,77 @@
     The Linker class is intended for subclassing for specific backends, e.g.
     a `DuckDBLinker`.
     """
 
     def __init__(
         self,
         input_table_or_tables: str | list,
-        settings_dict: dict,
+        settings_dict: dict | Path,
         accepted_df_dtypes,
         set_up_basic_logging: bool = True,
         input_table_aliases: str | list = None,
     ):
         """Initialise the linker object, which manages the data linkage process and
         holds the data linkage model.
 
         Examples:
-            >>> # Example 1: DuckDB
-            >>> df = pd.read_csv("data_to_dedupe.csv")
-            >>> linker = DuckDBLinker(df, settings_dict)
-
-
-            >>> # Example 2: Spark
-            >>> df_1 = spark.read.parquet("table_1/")
-            >>> df_2 = spark.read.parquet("table_2/")
-            >>> linker = SparkLinker(
-            >>>     [df_1, df_2],
-            >>>     settings_dict,
-            >>>     input_table_aliases=["customers", "contact_center_callers"]
-            >>>     )
+            === "DuckDB"
+                Dedupe
+                ```py
+                df = pd.read_csv("data_to_dedupe.csv")
+                linker = DuckDBLinker(df, settings_dict)
+                ```
+                Link
+                ```py
+                df_1 = pd.read_parquet("table_1/")
+                df_2 = pd.read_parquet("table_2/")
+                linker = DuckDBLinker(
+                    [df_1, df_2],
+                    settings_dict,
+                    input_table_aliases=["customers", "contact_center_callers"]
+                    )
+                ```
+                Dedupe with a pre-trained model read from a json file
+                ```py
+                df = pd.read_csv("data_to_dedupe.csv")
+                linker = DuckDBLinker(df, "model.json")
+                ```
+            === "Spark"
+                Dedupe
+                ```py
+                df = spark.read.csv("data_to_dedupe.csv")
+                linker = SparkLinker(df, settings_dict)
+                ```
+                Link
+                ```py
+                df_1 = spark.read.parquet("table_1/")
+                df_2 = spark.read.parquet("table_2/")
+                linker = SparkLinker(
+                    [df_1, df_2],
+                    settings_dict,
+                    input_table_aliases=["customers", "contact_center_callers"]
+                    )
+                ```
+                Dedupe with a pre-trained model read from a json file
+                ```py
+                df = spark.read.csv("data_to_dedupe.csv")
+                linker = SparkLinker(df, "model.json")
+                ```
 
         Args:
             input_table_or_tables (Union[str, list]): Input data into the linkage model.
                 Either a single string (the name of a table in a database) for
                 deduplication jobs, or a list of strings  (the name of tables in a
                 database) for link_only or link_and_dedupe.  For some linkers, such as
                 the DuckDBLinker and the SparkLinker, it's also possible to pass in
                 dataframes (Pandas and Spark respectively) rather than strings.
-            settings_dict (dict, optional): A Splink settings dictionary. If not
-                provided when the object is created, can later be added using
-                `linker.load_settings()` Defaults to None.
+            settings_dict (dict | Path, optional): A Splink settings dictionary, or a
+                path to a json defining a settingss dictionary or pre-trained model.
+                If not provided when the object is created, can later be added using
+                `linker.load_settings()` or `linker.load_model()` Defaults to None.
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             input_table_aliases (Union[str, list], optional): Labels assigned to
                 input tables in Splink outputs.  If the names of the tables in the
                 input database are long or unspecific, this argument can be used
                 to attach more easily readable/interpretable names. Defaults to None.
         """
@@ -621,17 +651,19 @@
         Register a table to your backend database, to be used in one of the
         splink methods, or simply to allow querying.
 
         Tables can be of type: dictionary, record level dictionary,
         pandas dataframe, pyarrow table and in the spark case, a spark df.
 
         Examples:
-            >>> test_dict = {"a": [666,777,888],"b": [4,5,6]}
-            >>> linker.register_table(test_dict, "test_dict")
-            >>> linker.query_sql("select * from test_dict")
+            ```py
+            test_dict = {"a": [666,777,888],"b": [4,5,6]}
+            linker.register_table(test_dict, "test_dict")
+            linker.query_sql("select * from test_dict")
+            ```
 
         Args:
             input: The data you wish to register. This can be either a dictionary,
                 pandas dataframe, pyarrow table or a spark dataframe.
             table_name (str): The name you wish to assign to the table.
             overwrite (bool): Overwrite the table in the underlying database if it
                 exists
@@ -669,17 +701,38 @@
 
     def query_sql(self, sql, output_type="pandas"):
         """
         Run a SQL query against your backend database and return
         the resulting output.
 
         Examples:
-            >>> linker = DuckDBLinker(df, settings)
-            >>> df_predict = linker.predict()
-            >>> linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
+            === "DuckDB"
+                ```py
+                linker = DuckDBLinker(df, settings)
+                df_predict = linker.predict()
+                linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
+                ```
+            === "Spark"
+                ```py
+                linker = SparkLinker(df, settings)
+                df_predict = linker.predict()
+                linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
+                ```
+            === "Athena"
+                ```py
+                linker = AthenaLinker(df, settings)
+                df_predict = linker.predict()
+                linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
+                ```
+            === "SQLite"
+                ```py
+                linker = SQLiteLinker(df, settings)
+                df_predict = linker.predict()
+                linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
+            ```
 
         Args:
             sql (str): The SQL to be queried.
             output_type (str): One of splink_df/splinkdf or pandas.
                 This determines the type of table that your results are output in.
         """
 
@@ -992,19 +1045,19 @@
     def load_settings(self, settings_dict: dict | str | Path):
         """Initialise settings for the linker.  To be used if settings were
         not passed to the linker on creation. This can either be in the form
         of a settings dictionary or a filepath to a json file containing a
         valid settings dictionary.
 
         Examples:
-            >>> linker = DuckDBLinker(df, connection=":memory:")
-            >>> linker.profile_columns(["first_name", "surname"])
-            >>> linker.load_settings(settings_dict)
-
-            >>> linker.load_settings("my_settings.json")
+            ```py
+            linker = DuckDBLinker(df)
+            linker.profile_columns(["first_name", "surname"])
+            linker.load_settings(settings_dict)
+            ```
 
         Args:
             settings_dict (dict | str | Path): A Splink settings dictionary or
                 the path to your settings json file.
         """
 
         if not isinstance(settings_dict, dict):
@@ -1036,24 +1089,63 @@
             "sql_dialect", self._sql_dialect
         )
         self._settings_dict = settings_dict
         self._settings_obj_ = Settings(settings_dict)
         self._validate_input_dfs()
         self._validate_dialect()
 
+    def load_model(self, model_path: Path):
+        """
+        Load a pre-defined model from a json file into the linker.
+        This is intended to be used with the output of
+        `save_model_to_json()`.
+
+        Examples:
+            ```py
+            linker.load_model("my_settings.json")
+            ```
+
+        Args:
+            model_path (Path): A path to your model settings json file.
+        """
+
+        return self.load_settings(model_path)
+
     def initialise_settings(self, settings_dict: dict):
         """*This method is now deprecated. Please use `load_settings`
-        when loading existing settings or a pre-trained model.*
+        when loading existing settings or `load_model` when loading
+         a pre-trained model.*
 
         Initialise settings for the linker.  To be used if settings were
         not passed to the linker on creation.
         Examples:
-            >>> linker = DuckDBLinker(df, connection=":memory:")
-            >>> linker.profile_columns(["first_name", "surname"])
-            >>> linker.initialise_settings(settings_dict)
+            === "DuckDB"
+                ```py
+                linker = DuckDBLinker(df")
+                linker.profile_columns(["first_name", "surname"])
+                linker.initialise_settings(settings_dict)
+                ```
+            === "Spark"
+                ```py
+                linker = SparkLinker(df")
+                linker.profile_columns(["first_name", "surname"])
+                linker.initialise_settings(settings_dict)
+                ```
+            === "Athena"
+                ```py
+                linker = AthenaLinker(df")
+                linker.profile_columns(["first_name", "surname"])
+                linker.initialise_settings(settings_dict)
+                ```
+            === "SQLite"
+                ```py
+                linker = SQLiteLinker(df")
+                linker.profile_columns(["first_name", "surname"])
+                linker.initialise_settings(settings_dict)
+                ```
         Args:
             settings_dict (dict): A Splink settings dictionary
         """
         # If a uid already exists in your settings object, prioritise this
         settings_dict["linker_uid"] = settings_dict.get("linker_uid", self._cache_uid)
         settings_dict["sql_dialect"] = settings_dict.get(
             "sql_dialect", self._sql_dialect
@@ -1069,21 +1161,24 @@
             "trained model.",
             DeprecationWarning,
             stacklevel=2,
         )
 
     def load_settings_from_json(self, in_path: str | Path):
         """*This method is now deprecated. Please use `load_settings`
-        when loading existing settings or a pre-trained model.*
+        when loading existing settings or `load_model` when loading
+         a pre-trained model.*
 
         Load settings from a `.json` file.
         This `.json` file would usually be the output of
-        `linker.save_settings_to_json()`
+        `linker.save_model_to_json()`
         Examples:
-            >>> linker.load_settings_from_json("my_settings.json")
+            ```py
+            linker.load_settings_from_json("my_settings.json")
+            ```
         Args:
             in_path (str): Path to settings json file
         """
         self.load_settings(in_path)
 
         warnings.warn(
             "`load_settings_from_json` is deprecated. We advise you use "
@@ -1097,28 +1192,50 @@
         """Compute a term frequency table for a given column and persist to the database
 
         This method is useful if you want to pre-compute term frequency tables e.g.
         so that real time linkage executes faster, or so that you can estimate
         various models without having to recompute term frequency tables each time
 
         Examples:
-            >>> # Example 1: Real time linkage
-            >>> linker = DuckDBLinker(df, connection=":memory:")
-            >>> linker.load_settings("saved_settings.json")
-            >>> linker.compute_tf_table("surname")
-            >>> linker.compare_two_records(record_left, record_right)
-
-            >>> # Example 2: Pre-computed term frequency tables in Spark
-            >>> linker = SparkLinker(df)
-            >>> df_first_name_tf = linker.compute_tf_table("first_name")
-            >>> df_first_name_tf.write.parquet("folder/first_name_tf")
-            >>>
-            >>> # On subsequent data linking job, read this table rather than recompute
-            >>> df_first_name_tf = spark.read.parquet("folder/first_name_tf")
-            >>> df_first_name_tf.createOrReplaceTempView("__splink__df_tf_first_name")
+            === "DuckDB"
+                Real time linkage
+                ```py
+                linker = DuckDBLinker(df)
+                linker.load_settings("saved_settings.json")
+                linker.compute_tf_table("surname")
+                linker.compare_two_records(record_left, record_right)
+                ```
+                Pre-computed term frequency tables
+                ```py
+                linker = DuckDBLinker(df)
+                df_first_name_tf = linker.compute_tf_table("first_name")
+                df_first_name_tf.write.parquet("folder/first_name_tf")
+                >>>
+                # On subsequent data linking job, read this table rather than recompute
+                df_first_name_tf = pd.read_parquet("folder/first_name_tf")
+                df_first_name_tf.createOrReplaceTempView("__splink__df_tf_first_name")
+                ```
+            === "Spark"
+                Real time linkage
+                ```py
+                linker = SparkLinker(df)
+                linker.load_settings("saved_settings.json")
+                linker.compute_tf_table("surname")
+                linker.compare_two_records(record_left, record_right)
+                ```
+                Pre-computed term frequency tables
+                ```py
+                linker = SparkLinker(df)
+                df_first_name_tf = linker.compute_tf_table("first_name")
+                df_first_name_tf.write.parquet("folder/first_name_tf")
+                >>>
+                # On subsequent data linking job, read this table rather than recompute
+                df_first_name_tf = spark.read.parquet("folder/first_name_tf")
+                df_first_name_tf.createOrReplaceTempView("__splink__df_tf_first_name")
+                ```
 
         Args:
             column_name (str): The column name in the input table
 
         Returns:
             SplinkDataFrame: The resultant table as a splink data frame
         """
@@ -1166,29 +1283,78 @@
         For deterministic linkage, this should be a list of blocking rules which
         are strict enough to generate only true links.
 
         Deterministic linkage, however, is likely to result in missed links
         (false negatives).
 
         Examples:
-            >>> linker = DuckDBLinker(df)
-            >>>
-            >>> settings = {
-            >>>     "link_type": "dedupe_only",
-            >>>     "blocking_rules_to_generate_predictions": [
-            >>>         "l.first_name = r.first_name",
-            >>>         "l.surname = r.surname",
-            >>>     ],
-            >>>     "comparisons": []
-            >>> }
-            >>>
-            >>> from splink.duckdb.duckdb_linker import DuckDBLinker
-            >>>
-            >>> linker = DuckDBLinker(df, settings)
-            >>> df = linker.deterministic_link()
+            === "DuckDB"
+            ```py
+            from splink.duckdb.duckdb_linker import DuckDBLinker
+
+            settings = {
+                "link_type": "dedupe_only",
+                "blocking_rules_to_generate_predictions": [
+                    "l.first_name = r.first_name",
+                    "l.surname = r.surname",
+                ],
+                "comparisons": []
+            }
+            >>>
+            linker = DuckDBLinker(df, settings)
+            df = linker.deterministic_link()
+            ```
+            === "Spark"
+            ```py
+            from splink.spark.spark_linker import SparkLinker
+
+            settings = {
+                "link_type": "dedupe_only",
+                "blocking_rules_to_generate_predictions": [
+                    "l.first_name = r.first_name",
+                    "l.surname = r.surname",
+                ],
+                "comparisons": []
+            }
+            >>>
+            linker = SparkLinker(df, settings)
+            df = linker.deterministic_link()
+            ```
+            === "Athena"
+            ```py
+            from splink.athena.athena_linker import AthenaLinker
+
+            settings = {
+                "link_type": "dedupe_only",
+                "blocking_rules_to_generate_predictions": [
+                    "l.first_name = r.first_name",
+                    "l.surname = r.surname",
+                ],
+                "comparisons": []
+            }
+            >>>
+            linker = AthenaLinker(df, settings)
+            df = linker.deterministic_link()
+            ```
+            === "SQLite"
+            ```py
+            from splink.sqlite.sqlite_linker import SQLiteLinker
+
+            settings = {
+                "link_type": "dedupe_only",
+                "blocking_rules_to_generate_predictions": [
+                    "l.first_name = r.first_name",
+                    "l.surname = r.surname",
+                ],
+                "comparisons": []
+            }
+            >>>
+            linker = SQLiteLinker(df, settings)
+            df = linker.deterministic_link()
+            ```
 
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons.  This
                 represents a table materialised in the database. Methods on the
                 SplinkDataFrame allow you to access the underlying data.
         """
 
@@ -1228,15 +1394,17 @@
             is often adequate whilst testing different model specifications, before
             the final model is estimated.
             seed (int): Seed for random sampling. Assign to get reproducible u
             probabilities. Note, seed for random sampling is only supported for
             DuckDB and Spark, for Athena and SQLite set to None.
 
         Examples:
-            >>> linker.estimate_u_using_random_sampling(1e8)
+            ```py
+            linker.estimate_u_using_random_sampling(1e8)
+            ```
 
         Returns:
             None: Updates the estimated u parameters within the linker object
             and returns nothing.
         """
         # TODO: Remove this compatibility code in a future release once we drop
         # support for "target_rows". Deprecation warning added in 3.7.0
@@ -1281,15 +1449,17 @@
         populated.
 
         Args:
             label_colname (str): The name of the column containing the ground truth
                 label in the input data.
 
         Examples:
-            >>> linker.estimate_m_from_label_column("social_security_number")
+            ```py
+            linker.estimate_m_from_label_column("social_security_number")
+            ```
 
         Returns:
             Updates the estimated m parameters within the linker object
             and returns nothing.
         """
 
         # Ensure this has been run on the main linker so that it can be used by
@@ -1340,28 +1510,31 @@
         To control which comparisons should have their parameter estimated, and the
         process of 'reversing out' the global probability two random records match, the
         user may specify `comparisons_to_deactivate` and
         `comparison_levels_to_reverse_blocking_rule`.   This is useful, for example
         if you block on the dmetaphone of a column but match on the original column.
 
         Examples:
-            >>> # Default behaviour
-            >>> br_training = "l.first_name = r.first_name and l.dob = r.dob"
-            >>> linker.estimate_parameters_using_expectation_maximisation(br_training)
-
-            >>> # Specify which comparisons to deactivate
-            >>> br_training = "l.dmeta_first_name = r.dmeta_first_name"
-            >>> settings_obj = linker._settings_obj
-            >>> comp = settings_obj._get_comparison_by_output_column_name("first_name")
-            >>> dmeta_level = comp._get_comparison_level_by_comparison_vector_value(1)
-            >>> linker.estimate_parameters_using_expectation_maximisation(
-            >>>     br_training,
-            >>>     comparisons_to_deactivate=["first_name"],
-            >>>     comparison_levels_to_reverse_blocking_rule=[dmeta_level],
-            >>> )
+            Default behaviour
+            ```py
+            br_training = "l.first_name = r.first_name and l.dob = r.dob"
+            linker.estimate_parameters_using_expectation_maximisation(br_training)
+            ```
+            Specify which comparisons to deactivate
+            ```py
+            br_training = "l.dmeta_first_name = r.dmeta_first_name"
+            settings_obj = linker._settings_obj
+            comp = settings_obj._get_comparison_by_output_column_name("first_name")
+            dmeta_level = comp._get_comparison_level_by_comparison_vector_value(1)
+            linker.estimate_parameters_using_expectation_maximisation(
+                br_training,
+                comparisons_to_deactivate=["first_name"],
+                comparison_levels_to_reverse_blocking_rule=[dmeta_level],
+            )
+            ```
 
         Args:
             blocking_rule (str): The blocking rule used to generate pairwise record
                 comparisons.
             comparisons_to_deactivate (list, optional): By default, splink will
                 analyse the blocking rule provided and estimate the m parameters for
                 all comaprisons except those included in the blocking rule.  If
@@ -1384,16 +1557,18 @@
             fix_u_probabilities (bool, optional): If True, do not update the u
                 probabilities after each iteration. Defaults to True.
             populate_probability_two_random_records_match_from_trained_values
                 (bool, optional): If True, derive this parameter from
                 the blocked value. Defaults to False.
 
         Examples:
-            >>> blocking_rule = "l.first_name = r.first_name and l.dob = r.dob"
-            >>> linker.estimate_parameters_using_expectation_maximisation(blocking_rule)
+            ```py
+            blocking_rule = "l.first_name = r.first_name and l.dob = r.dob"
+            linker.estimate_parameters_using_expectation_maximisation(blocking_rule)
+            ```
 
         Returns:
             EMTrainingSession:  An object containing information about the training
                 session such as how parameters changed during the iteration history
 
         """
         # Ensure this has been run on the main linker so that it's in the cache
@@ -1465,19 +1640,20 @@
                 will materialise the table containing the input nodes (rows)
                 joined to any term frequencies which have been asked
                 for in the settings object.  If False, this will be
                 computed as part of one possibly gigantic CTE
                 pipeline.   Defaults to True
 
         Examples:
-            >>> linker = DuckDBLinker(df, connection=":memory:")
-            >>> linker.load_settings("saved_settings.json")
-            >>> df = linker.predict(threshold_match_probability=0.95)
-            >>> df.as_pandas_dataframe(limit=5)
-
+            ```py
+            linker = DuckDBLinker(df)
+            linker.load_settings("saved_settings.json")
+            df = linker.predict(threshold_match_probability=0.95)
+            df.as_pandas_dataframe(limit=5)
+            ```
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons.  This
                 represents a table materialised in the database. Methods on the
                 SplinkDataFrame allow you to access the underlying data.
 
         """
 
@@ -1540,28 +1716,29 @@
                 which records to find and score. If [], do not use a blocking
                 rule - meaning the input records will be compared to all records
                 provided to the linker when it was instantiated. Defaults to [].
             match_weight_threshold (int, optional): Return matches with a match weight
                 above this threshold. Defaults to -4.
 
         Examples:
-            >>> linker = DuckDBLinker(df)
-            >>> linker.load_settings("saved_settings.json")
-            >>> # Pre-compute tf tables for any tables with
-            >>> # term frequency adjustments
-            >>> linker.compute_tf_table("first_name")
-            >>> record = {'unique_id': 1,
-            >>>     'first_name': "John",
-            >>>     'surname': "Smith",
-            >>>     'dob': "1971-05-24",
-            >>>     'city': "London",
-            >>>     'email': "john@smith.net"
-            >>>     }
-            >>> df = linker.find_matches_to_new_records([record], blocking_rules=[])
-
+            ```py
+            linker = DuckDBLinker(df)
+            linker.load_settings("saved_settings.json")
+            # Pre-compute tf tables for any tables with
+            # term frequency adjustments
+            linker.compute_tf_table("first_name")
+            record = {'unique_id': 1,
+                'first_name': "John",
+                'surname': "Smith",
+                'dob': "1971-05-24",
+                'city': "London",
+                'email': "john@smith.net"
+                }
+            df = linker.find_matches_to_new_records([record], blocking_rules=[])
+            ```
 
         Returns:
             SplinkDataFrame: The pairwise comparisons.
         """
 
         original_blocking_rules = (
             self._settings_obj._blocking_rules_to_generate_predictions
@@ -1653,17 +1830,19 @@
         Args:
             record_1 (dict): dictionary representing the first record.  Columns names
                 and data types must be the same as the columns in the settings object
             record_2 (dict): dictionary representing the second record.  Columns names
                 and data types must be the same as the columns in the settings object
 
         Examples:
-            >>> linker = DuckDBLinker(df)
-            >>> linker.load_settings("saved_settings.json")
-            >>> linker.compare_two_records(record_left, record_right)
+            ```py
+            linker = DuckDBLinker(df)
+            linker.load_settings("saved_settings.json")
+            linker.compare_two_records(record_left, record_right)
+            ```
 
         Returns:
             SplinkDataFrame: Pairwise comparison with scored prediction
         """
         original_blocking_rules = (
             self._settings_obj._blocking_rules_to_generate_predictions
         )
@@ -1876,17 +2055,19 @@
         of 1, i.e. a perfect match.
 
         Args:
           labels_splinkdataframe_or_table_name (str): Name of table containing labels
             in the database or SplinkDataframe
 
         Examples:
-          >>> pairwise_labels = pd.read_csv("./data/pairwise_labels_to_estimate_m.csv")
-          >>> linker.register_table(pairwise_labels, "labels", overwrite=True)
-          >>> linker.estimate_m_from_pairwise_labels("labels")
+            ```py
+            pairwise_labels = pd.read_csv("./data/pairwise_labels_to_estimate_m.csv")
+            linker.register_table(pairwise_labels, "labels", overwrite=True)
+            linker.estimate_m_from_pairwise_labels("labels")
+            ```
         """
         labels_tablename = self._get_labels_tablename_from_input(
             labels_splinkdataframe_or_table_name
         )
         estimate_m_from_pairwise_labels(self, labels_tablename)
 
     def truth_space_table_from_labels_table(
@@ -1921,24 +2102,26 @@
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
 
         Examples:
-            >>> # DuckDBLinker
-            >>> labels = pd.read_csv("my_labels.csv")
-            >>> linker.register_table(labels, "labels")
-            >>> linker.truth_space_table_from_labels_table("labels")
-            >>>
-            >>> # SparkLinker
-            >>> labels = spark.read.csv("my_labels.csv", header=True)
-            >>> labels.createDataFrame("labels")
-            >>> linker.truth_space_table_from_labels_table("labels")
-
+            === "DuckDB"
+                ```py
+                labels = pd.read_csv("my_labels.csv")
+                linker.register_table(labels, "labels")
+                linker.truth_space_table_from_labels_table("labels")
+                ```
+            === "Spark"
+                ```py
+                labels = spark.read.csv("my_labels.csv", header=True)
+                labels.createDataFrame("labels")
+                linker.truth_space_table_from_labels_table("labels")
+                ```
         Returns:
             SplinkDataFrame:  Table of truth statistics
         """
         labels_tablename = self._get_labels_tablename_from_input(
             labels_splinkdataframe_or_table_name
         )
 
@@ -1981,24 +2164,26 @@
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
 
         Examples:
-            >>> # DuckDBLinker
-            >>> labels = pd.read_csv("my_labels.csv")
-            >>> linker.register_table(labels, "labels")
-            >>> linker.roc_chart_from_labels_table("labels")
-            >>>
-            >>> # SparkLinker
-            >>> labels = spark.read.csv("my_labels.csv", header=True)
-            >>> labels.createDataFrame("labels")
-            >>> linker.roc_chart_from_labels_table("labels")
-
+            === "DuckDB"
+                ```py
+                labels = pd.read_csv("my_labels.csv")
+                linker.register_table(labels, "labels")
+                linker.roc_chart_from_labels_table("labels")
+                ```
+            === "Spark"
+                ```py
+                labels = spark.read.csv("my_labels.csv", header=True)
+                labels.createDataFrame("labels")
+                linker.roc_chart_from_labels_table("labels")
+                ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
         labels_tablename = self._get_labels_tablename_from_input(
@@ -2045,24 +2230,26 @@
                 is used as the threshold to classify `clerical_match_score`s as binary
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
         Examples:
-            >>> # DuckDBLinker
-            >>> labels = pd.read_csv("my_labels.csv")
-            >>> linker.register_table(labels, "labels")
-            >>> linker.precision_recall_chart_from_labels_table("labels")
-            >>>
-            >>> # SparkLinker
-            >>> labels = spark.read.csv("my_labels.csv", header=True)
-            >>> labels.createDataFrame("labels")
-            >>> linker.precision_recall_chart_from_labels_table("labels")
-
+            === "DuckDB"
+                ```py
+                labels = pd.read_csv("my_labels.csv")
+                linker.register_table(labels, "labels")
+                linker.precision_recall_chart_from_labels_table("labels")
+                ```
+            === "Spark"
+                ```py
+                labels = spark.read.csv("my_labels.csv", header=True)
+                labels.createDataFrame("labels")
+                linker.precision_recall_chart_from_labels_table("labels")
+                ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
         labels_tablename = self._get_labels_tablename_from_input(
@@ -2131,15 +2318,17 @@
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
 
         Examples:
-            >>> linker.truth_space_table_from_labels_column("cluster")
+            ```py
+            linker.truth_space_table_from_labels_column("cluster")
+            ```
 
         Returns:
             SplinkDataFrame:  Table of truth statistics
         """
 
         return truth_space_table_from_labels_column(
             self, labels_column_name, threshold_actual, match_weight_round_to_nearest
@@ -2162,16 +2351,17 @@
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
 
         Examples:
-            >>> linker.roc_chart_from_labels_column("labels")
-
+            ```py
+            linker.roc_chart_from_labels_column("labels")
+            ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
 
@@ -2200,16 +2390,17 @@
                 is used as the threshold to classify `clerical_match_score`s as binary
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
         Examples:
-            >>> linker.precision_recall_chart_from_labels_column("ground_truth")
-
+            ```py
+            linker.precision_recall_chart_from_labels_column("ground_truth")
+            ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
 
@@ -2280,17 +2471,19 @@
         """Visualise how the final match weight is computed for the provided pairwise
         record comparisons.
 
         Records must be provided as a list of dictionaries. This would usually be
         obtained from `df.as_record_dict(limit=n)` where `df` is a SplinkDataFrame.
 
         Examples:
-            >>> df = linker.predict(threshold_match_weight=2)
-            >>> records = df.as_record_dict(limit=10)
-            >>> linker.waterfall_chart(records)
+            ```py
+            df = linker.predict(threshold_match_weight=2)
+            records = df.as_record_dict(limit=10)
+            linker.waterfall_chart(records)
+            ```
 
         Args:
             records (List[dict]): Usually be obtained from `df.as_record_dict(limit=n)`
                 where `df` is a SplinkDataFrame.
             filter_nulls (bool, optional): Whether the visualiation shows null
                 comparisons, which have no effect on final match weight. Defaults to
                 True.
@@ -2322,23 +2515,24 @@
             x_col (str, optional): Column to use for the x-axis.
                 Defaults to "match_weight".
             source_dataset (str, optional): Name of the source dataset to use for
                 the title of the output chart.
             as_dict (bool, optional): If True, return a dict version of the chart.
 
         Examples:
-            >>> # For the simplest code pipeline, load a pre-trained model
-            >>> # and run this against the test data.
-            >>> df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
-            >>> linker = DuckDBLinker(df)
-            >>> linker.load_settings("saved_settings.json")
-            >>> linker.unlinkables_chart()
-            >>>
-            >>> # For more complex code pipelines, you can run an entire pipeline
-            >>> # that estimates your m and u values, before `unlinkables_chart().
+            For the simplest code pipeline, load a pre-trained model
+            and run this against the test data.
+            ```py
+            df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
+            linker = DuckDBLinker(df)
+            linker.load_settings("saved_settings.json")
+            linker.unlinkables_chart()
+            ```
+            For more complex code pipelines, you can run an entire pipeline
+            that estimates your m and u values, before `unlinkables_chart().
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
 
@@ -2365,21 +2559,25 @@
             overwrite (bool, optional): Overwrite the html file if it already exists?
                 Defaults to False.
             num_example_rows (int, optional): Number of example rows per comparison
                 vector. Defaults to 2.
             return_html_as_string: If True, return the html as a string
 
         Examples:
-            >>> df_predictions = linker.predict()
-            >>> linker.comparison_viewer_dashboard(df_predictions, "scv.html", True, 2)
-            >>>
-            >>> # Optionally, in Jupyter, you can display the results inline
-            >>> # Otherwise you can just load the html file in your browser
-            >>> from IPython.display import IFrame
-            >>> IFrame(src="./scv.html", width="100%", height=1200)
+            ```py
+            df_predictions = linker.predict()
+            linker.comparison_viewer_dashboard(df_predictions, "scv.html", True, 2)
+            ```
+
+            Optionally, in Jupyter, you can display the results inline
+            Otherwise you can just load the html file in your browser
+            ```py
+            from IPython.display import IFrame
+            IFrame(src="./scv.html", width="100%", height=1200)
+            ```
 
         """
         self._raise_error_if_necessary_waterfall_columns_not_computed()
 
         sql = comparison_vector_distribution_sql(self)
         self._enqueue_sql(sql, "__splink__df_comparison_vector_distribution")
 
@@ -2433,25 +2631,28 @@
 
         Args:
             input_dataset (str, optional): Name of one of the input tables in the
             database.  If provided, missingness will be computed for this table alone.
             Defaults to None.
 
         Examples:
-            >>> linker.missingness_chart()
-            >>> # To view offline (if you don't have an internet connection):
-            >>>
-            >>> from splink.charts import save_offline_chart
-            >>> c = linker.missingness_chart()
-            >>> save_offline_chart(c.spec, "test_chart.html")
-            >>>
-            >>> # View resultant html file in Jupyter (or just load it in your browser)
-            >>> from IPython.display import IFrame
-            >>> IFrame(src="./test_chart.html", width=1000, height=500
-
+            ```py
+            linker.missingness_chart()
+            ```
+            To view offline (if you don't have an internet connection):
+            ```py
+            from splink.charts import save_offline_chart
+            c = linker.missingness_chart()
+            save_offline_chart(c.spec, "test_chart.html")
+            ```
+            View resultant html file in Jupyter (or just load it in your browser)
+            ```py
+            from IPython.display import IFrame
+            IFrame(src="./test_chart.html", width=1000, height=500
+            ```
         """
         records = missingness_data(self, input_dataset)
         return missingness_chart(records)
 
     def completeness_chart(self, input_dataset: str = None, cols: list[str] = None):
         """Generate a summary chart of the completeness (proportion of non-nulls) of
         columns in each of the input datasets. By default, completeness is assessed for
@@ -2461,25 +2662,28 @@
             input_dataset (str, optional): Name of one of the input tables in the
                 database.  If provided, completeness will be computed for this table
                 alone. Defaults to None.
             cols (List[str], optional): List of column names to calculate completeness.
                 Default to None.
 
         Examples:
-            >>> linker.completeness_chart()
-            >>> # To view offline (if you don't have an internet connection):
-            >>>
-            >>> from splink.charts import save_offline_chart
-            >>> c = linker.completeness_chart()
-            >>> save_offline_chart(c.spec, "test_chart.html")
-            >>>
-            >>> # View resultant html file in Jupyter (or just load it in your browser)
-            >>> from IPython.display import IFrame
-            >>> IFrame(src="./test_chart.html", width=1000, height=500
-
+            ```py
+            linker.completeness_chart()
+            ```
+            To view offline (if you don't have an internet connection):
+            ```py
+            from splink.charts import save_offline_chart
+            c = linker.completeness_chart()
+            save_offline_chart(c.spec, "test_chart.html")
+            ```
+            View resultant html file in Jupyter (or just load it in your browser)
+            ```py
+            from IPython.display import IFrame
+            IFrame(src="./test_chart.html", width=1000, height=500
+            ```
         """
         records = completeness_data(self, input_dataset, cols)
         return completeness_chart(records)
 
     def count_num_comparisons_from_blocking_rule(
         self,
         blocking_rule: str,
@@ -2493,20 +2697,24 @@
                 linker has not yet been provided with a settings dictionary.  Defaults
                 to None.
             unique_id_column_name (str, optional):  This is needed only if the
                 linker has not yet been provided with a settings dictionary.  Defaults
                 to None.
 
         Examples:
-            >>> br = "l.first_name = r.first_name"
-            >>> linker.count_num_comparisons_from_blocking_rule(br)
-            19387
-            >>> br = "l.name = r.name and substr(l.dob,1,4) = substr(r.dob,1,4)"
-            >>> linker.count_num_comparisons_from_blocking_rule(br)
-            394
+            ```py
+            br = "l.first_name = r.first_name"
+            linker.count_num_comparisons_from_blocking_rule(br)
+            ```
+            > 19387
+            ```py
+            br = "l.name = r.name and substr(l.dob,1,4) = substr(r.dob,1,4)"
+            linker.count_num_comparisons_from_blocking_rule(br)
+            ```
+            > 394
 
         Returns:
             int: The number of comparisons generated by the blocking rule
         """
 
         sql = vertically_concatenate_sql(self)
         self._enqueue_sql(sql, "__splink__df_concat")
@@ -2527,29 +2735,31 @@
         total.
 
         Args:
             blocking_rules (str or list): The blocking rule(s) to compute comparisons
                 for. If null, the rules set out in your settings object will be used.
 
         Examples:
-            >>> linker_settings = DuckDBLinker(df, settings)
-            >>> # Compute the cumulative number of comparisons generated by the rules
-            >>> # in your settings object.
-            >>> linker_settings.cumulative_comparisons_from_blocking_rules_records()
-            >>>
-            >>> # Generate total comparisons with custom blocking rules.
-            >>> blocking_rules = [
-            >>>    "l.surname = r.surname",
-            >>>    "l.first_name = r.first_name
-            >>>     and substr(l.dob,1,4) = substr(r.dob,1,4)"
-            >>> ]
+            ```py
+            linker_settings = DuckDBLinker(df, settings)
+            # Compute the cumulative number of comparisons generated by the rules
+            # in your settings object.
+            linker_settings.cumulative_comparisons_from_blocking_rules_records()
+            >>>
+            # Generate total comparisons with custom blocking rules.
+            blocking_rules = [
+               "l.surname = r.surname",
+               "l.first_name = r.first_name
+                and substr(l.dob,1,4) = substr(r.dob,1,4)"
+            ]
             >>>
-            >>> linker_settings.cumulative_comparisons_from_blocking_rules_records(
-            >>>     blocking_rules
-            >>>  )
+            linker_settings.cumulative_comparisons_from_blocking_rules_records(
+                blocking_rules
+             )
+            ```
 
         Returns:
             List: A list of blocking rules and the corresponding number of
                 comparisons it is forecast to generate.
         """
         if blocking_rules:
             blocking_rules = ensure_is_list(blocking_rules)
@@ -2572,29 +2782,31 @@
         total.
 
         Args:
             blocking_rules (str or list): The blocking rule(s) to compute comparisons
                 for. If null, the rules set out in your settings object will be used.
 
         Examples:
-            >>> linker_settings = DuckDBLinker(df, settings)
-            >>> # Compute the cumulative number of comparisons generated by the rules
-            >>> # in your settings object.
-            >>> linker_settings.cumulative_num_comparisons_from_blocking_rules_chart()
-            >>>
-            >>> # Generate total comparisons with custom blocking rules.
-            >>> blocking_rules = [
-            >>>    "l.surname = r.surname",
-            >>>    "l.first_name = r.first_name
-            >>>     and substr(l.dob,1,4) = substr(r.dob,1,4)"
-            >>> ]
+            ```py
+            linker_settings = DuckDBLinker(df, settings)
+            # Compute the cumulative number of comparisons generated by the rules
+            # in your settings object.
+            linker_settings.cumulative_num_comparisons_from_blocking_rules_chart()
+            >>>
+            # Generate total comparisons with custom blocking rules.
+            blocking_rules = [
+               "l.surname = r.surname",
+               "l.first_name = r.first_name
+                and substr(l.dob,1,4) = substr(r.dob,1,4)"
+            ]
             >>>
-            >>> linker_settings.cumulative_num_comparisons_from_blocking_rules_chart(
-            >>>     blocking_rules
-            >>>  )
+            linker_settings.cumulative_num_comparisons_from_blocking_rules_chart(
+                blocking_rules
+             )
+            ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
 
@@ -2617,19 +2829,21 @@
         marginal effect of each entry in `blocking_rules_to_generate_predictions`
 
         Args:
             df_predict (SplinkDataFrame): SplinkDataFrame with match weights
             and probabilities of rows matching
 
         Examples:
-            >>> linker = DuckDBLinker(df, connection=":memory:")
-            >>> linker.load_settings("saved_settings.json")
-            >>> df_predict = linker.predict(threshold_match_probability=0.95)
-            >>> count_pairwise = linker.count_num_comparisons_from_blocking_rules_for_prediction(df_predict)
-            >>> count_pairwise.as_pandas_dataframe(limit=5)
+            ```py
+            linker = DuckDBLinker(df, connection=":memory:")
+            linker.load_settings("saved_settings.json")
+            df_predict = linker.predict(threshold_match_probability=0.95)
+            count_pairwise = linker.count_num_comparisons_from_blocking_rules_for_prediction(df_predict)
+            count_pairwise.as_pandas_dataframe(limit=5)
+            ```
 
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons and
                 estimated pairwise comparisons generated by the blocking rules.
         """  # noqa: E501
         sql = count_num_comparisons_from_blocking_rules_for_prediction_sql(
             self, df_predict
@@ -2639,26 +2853,28 @@
         )
         return match_key_analysis
 
     def match_weights_chart(self):
         """Display a chart of the (partial) match weights of the linkage model
 
         Examples:
-            >>> linker.match_weights_chart()
-            >>>
-            >>> # To view offline (if you don't have an internet connection):
-            >>>
-            >>> from splink.charts import save_offline_chart
-            >>> c = linker.match_weights_chart()
-            >>> save_offline_chart(c.spec, "test_chart.html")
-            >>>
-            >>> # View resultant html file in Jupyter (or just load it in your browser)
-            >>> from IPython.display import IFrame
-            >>> IFrame(src="./test_chart.html", width=1000, height=500)
-
+            ```py
+            linker.match_weights_chart()
+            ```
+            To view offline (if you don't have an internet connection):
+            ```py
+            from splink.charts import save_offline_chart
+            c = linker.match_weights_chart()
+            save_offline_chart(c.spec, "test_chart.html")
+            ```
+            View resultant html file in Jupyter (or just load it in your browser)
+            ```py
+            from IPython.display import IFrame
+            IFrame(src="./test_chart.html", width=1000, height=500)
+            ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
         return self._settings_obj.match_weights_chart()
@@ -2717,26 +2933,28 @@
             as_dict,
         )
 
     def m_u_parameters_chart(self):
         """Display a chart of the m and u parameters of the linkage model
 
         Examples:
-            >>> linker.m_u_parameters_chart()
-            >>>
-            >>> # To view offline (if you don't have an internet connection):
-            >>>
-            >>> from splink.charts import save_offline_chart
-            >>> c = linker.match_weights_chart()
-            >>> save_offline_chart(c.spec, "test_chart.html")
-            >>>
-            >>> # View resultant html file in Jupyter (or just load it in your browser)
-            >>> from IPython.display import IFrame
-            >>> IFrame(src="./test_chart.html", width=1000, height=500)
-
+            ```py
+            linker.m_u_parameters_chart()
+            ```
+            To view offline (if you don't have an internet connection):
+            ```py
+            from splink.charts import save_offline_chart
+            c = linker.match_weights_chart()
+            save_offline_chart(c.spec, "test_chart.html")
+            ```
+            View resultant html file in Jupyter (or just load it in your browser)
+            ```py
+            from IPython.display import IFrame
+            IFrame(src="./test_chart.html", width=1000, height=500)
+            ```
 
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
 
@@ -2773,25 +2991,27 @@
                 Defaults to False.
             cluster_names (list, optional): If provided, the dashboard will display
                 these names in the selection box. Ony works in conjunction with
                 `cluster_ids`.  Defaults to None.
             return_html_as_string: If True, return the html as a string
 
         Examples:
-            >>> df_p = linker.predict()
-            >>> df_c = linker.cluster_pairwise_predictions_at_threshold(df_p, 0.5)
-            >>> linker.cluster_studio_dashboard(
-            >>>     df_p, df_c, [0, 4, 7], "cluster_studio.html"
-            >>> )
-            >>>
-            >>> # Optionally, in Jupyter, you can display the results inline
-            >>> # Otherwise you can just load the html file in your browser
-            >>> from IPython.display import IFrame
-            >>> IFrame(src="./cluster_studio.html", width="100%", height=1200)
-
+            ```py
+            df_p = linker.predict()
+            df_c = linker.cluster_pairwise_predictions_at_threshold(df_p, 0.5)
+            linker.cluster_studio_dashboard(
+                df_p, df_c, [0, 4, 7], "cluster_studio.html"
+            )
+            ```
+            Optionally, in Jupyter, you can display the results inline
+            Otherwise you can just load the html file in your browser
+            ```py
+            from IPython.display import IFrame
+            IFrame(src="./cluster_studio.html", width="100%", height=1200)
+            ```
         """
         self._raise_error_if_necessary_waterfall_columns_not_computed()
 
         rendered = render_splink_cluster_studio_html(
             self,
             df_predict,
             df_clustered,
@@ -2802,25 +3022,26 @@
             overwrite=overwrite,
             cluster_names=cluster_names,
         )
 
         if return_html_as_string:
             return rendered
 
-    def save_settings_to_json(
+    def save_model_to_json(
         self, out_path: str | None = None, overwrite: bool = False
     ) -> dict:
         """Save the configuration and parameters of the linkage model to a `.json` file.
 
-        The model can later be loaded back in using `linker.load_settings()`.
+        The model can later be loaded back in using `linker.load_model()`.
         The settings dict is also returned in case you want to save it a different way.
 
         Examples:
-            >>> linker.save_settings_to_json("my_settings.json", overwrite=True)
-
+            ```py
+            linker.save_model_to_json("my_settings.json", overwrite=True)
+            ```
         Args:
             out_path (str, optional): File path for json file. If None, don't save to
                 file. Defaults to None.
             overwrite (bool, optional): Overwrite if already exists? Defaults to False.
 
         Returns:
             dict: The settings as a dictionary.
@@ -2832,14 +3053,27 @@
                     f"The path {out_path} already exists. Please provide a different "
                     "path or set overwrite=True"
                 )
             with open(out_path, "w", encoding="utf-8") as f:
                 json.dump(model_dict, f, indent=4)
         return model_dict
 
+    def save_settings_to_json(
+        self, out_path: str | None = None, overwrite: bool = False
+    ) -> dict:
+        """
+        This function is deprecated. Use save_model_to_json() instead.
+        """
+        warnings.warn(
+            "This function is deprecated. Use save_model_to_json() instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.save_model_to_json(out_path, overwrite)
+
     def estimate_probability_two_random_records_match(
         self, deterministic_matching_rules, recall
     ):
         """Estimate the model parameter `probability_two_random_records_match` using
         a direct estimation approach.
 
         See [here](https://github.com/moj-analytical-services/splink/issues/462)
```

### Comparing `splink-3.9.0/splink/lower_id_on_lhs.py` & `splink-3.9.1/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/m_from_labels.py` & `splink-3.9.1/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/m_training.py` & `splink-3.9.1/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/m_u_records_to_parameters.py` & `splink-3.9.1/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/match_key_analysis.py` & `splink-3.9.1/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/match_weights_histogram.py` & `splink-3.9.1/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/misc.py` & `splink-3.9.1/splink/misc.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/missingness.py` & `splink-3.9.1/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/parse_sql.py` & `splink-3.9.1/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/pipeline.py` & `splink-3.9.1/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/predict.py` & `splink-3.9.1/splink/predict.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/profile_data.py` & `splink-3.9.1/splink/profile_data.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/settings.py` & `splink-3.9.1/splink/settings.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-3.9.1/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/spark/spark_helpers/spark_base.py` & `splink-3.9.1/splink/spark/spark_helpers/spark_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,33 +15,24 @@
     cast_str=False,
     date_format=None,
 ):
     if date_format is None:
         date_format = "yyyy-MM-dd"
 
     if cast_str:
-        if date_metric == "day":
-            date_f = f"""abs(datediff(to_timestamp({col_name_l},
-            '{date_format}'),to_timestamp({col_name_r},'{date_format}')))"""
-        elif date_metric in ["month", "year"]:
-            date_f = f"""floor(abs(months_between(to_timestamp({col_name_l},
-            '{date_format}'),to_timestamp({col_name_r}, '{date_format}'))"""
-            if date_metric == "year":
-                date_f += " / 12))"
-            else:
-                date_f += "))"
-    else:
-        if date_metric == "day":
-            date_f = f"abs(datediff({col_name_l}, {col_name_r}))"
-        elif date_metric in ["month", "year"]:
-            date_f = f"ceil(abs(months_between({col_name_l}, {col_name_r})"
-            if date_metric == "year":
-                date_f += " / 12))"
-            else:
-                date_f += "))"
+        col_name_l = f"to_timestamp({col_name_l}, '{date_format}')"
+        col_name_r = f"to_timestamp({col_name_r}, '{date_format}')"
+    if date_metric == "day":
+        date_f = f"abs(datediff({col_name_l}, {col_name_r}))"
+    elif date_metric in ["month", "year"]:
+        date_f = f"ceil(abs(months_between({col_name_l}, {col_name_r})"
+        if date_metric == "year":
+            date_f += " / 12))"
+        else:
+            date_f += "))"
 
     return f"""
         {date_f} <= {date_threshold}
     """
 
 
 def regex_extract_sql(col_name, regex):
```

### Comparing `splink-3.9.0/splink/spark/spark_helpers/spark_comparison_imports.py` & `splink-3.9.1/splink/spark/spark_helpers/spark_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/spark/spark_linker.py` & `splink-3.9.1/splink/spark/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/splink_comparison_viewer.py` & `splink-3.9.1/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/splink_dataframe.py` & `splink-3.9.1/splink/splink_dataframe.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/sql_transform.py` & `splink-3.9.1/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py` & `splink-3.9.1/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/sqlite/sqlite_linker.py` & `splink-3.9.1/splink/sqlite/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         return cur.execute(sql).fetchall()
 
 
 class SQLiteLinker(Linker):
     def __init__(
         self,
         input_table_or_tables,
-        settings_dict=None,
+        settings_dict: dict | str = None,
         connection=":memory:",
         set_up_basic_logging=True,
         input_table_aliases: str | list = None,
     ):
         self._sql_dialect_ = "sqlite"
 
         self.con = connection
```

### Comparing `splink-3.9.0/splink/term_frequencies.py` & `splink-3.9.1/splink/term_frequencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
         else:
             tf_table.append(cache[tf_table_name])
 
     return tf_table
 
 
 def comparison_level_to_tf_chart_data(cl: dict):
-
     df = cl["df_tf"]
     df.columns = ["value", "tf"]
     df = df[df.value.notnull()]
 
     del cl["df_tf"]
     df = df.assign(**cl)
 
@@ -196,15 +195,14 @@
 
     return cl
 
 
 def tf_adjustment_chart(
     linker: Linker, col, n_most_freq, n_least_freq, vals_to_include, as_dict
 ):
-
     # Data for chart
     c = linker._settings_obj._get_comparison_by_output_column_name(col)
     c = c._as_detailed_records
 
     keys_to_retain = [
         "comparison_vector_value",
         "label_for_charts",
```

### Comparing `splink-3.9.0/splink/unique_id_concat.py` & `splink-3.9.1/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/unlinkables.py` & `splink-3.9.1/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/validate_jsonschema.py` & `splink-3.9.1/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/vertically_concatenate.py` & `splink-3.9.1/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/splink/waterfall_chart.py` & `splink-3.9.1/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.0/PKG-INFO` & `splink-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.9.0
+Version: 3.9.1
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -34,19 +34,19 @@
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
 
 ## Key Features
 
-⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.
-🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.
-🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.
-🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.
-📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
+⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
+🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
+🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
+🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
+📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.  
 
 Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
```

