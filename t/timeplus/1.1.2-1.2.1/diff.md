# Comparing `tmp/timeplus-1.1.2.tar.gz` & `tmp/timeplus-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeplus-1.1.2.tar", last modified: Tue Feb 14 06:04:45 2023, max compression
+gzip compressed data, was "timeplus-1.2.1.tar", last modified: Wed Jun  7 00:11:38 2023, max compression
```

## Comparing `timeplus-1.1.2.tar` & `timeplus-1.2.1.tar`

### file list

```diff
@@ -1,202 +1,174 @@
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:45.000127 timeplus-1.1.2/
--rw-r--r--   0 gangtao    (502) staff       (20)     3921 2023-02-14 06:04:45.000264 timeplus-1.1.2/PKG-INFO
--rw-r--r--   0 gangtao    (502) staff       (20)     3479 2022-12-29 18:08:58.000000 timeplus-1.1.2/README.md
--rw-r--r--   0 gangtao    (502) staff       (20)      633 2023-02-14 06:04:45.000834 timeplus-1.1.2/setup.cfg
--rw-r--r--   0 gangtao    (502) staff       (20)     1247 2022-12-29 18:08:58.000000 timeplus-1.1.2/setup.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.896665 timeplus-1.1.2/swagger_client/
--rw-r--r--   0 gangtao    (502) staff       (20)     5344 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)    25043 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/api_client.py
--rw-r--r--   0 gangtao    (502) staff       (20)     8229 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/configuration.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.939805 timeplus-1.1.2/swagger_client/models/
--rw-r--r--   0 gangtao    (502) staff       (20)     4383 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3010 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/analyze_sql_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6294 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/api_key.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3907 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/batching_policy.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3495 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/column.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6897 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/column_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6070 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/columns_resp.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3738 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/connection.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4036 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/connection_config.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3862 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/connection_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5165 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_api_key_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7665 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_api_key_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5438 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/create_persistent_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5119 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_query_request_v1_beta1.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6083 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/create_query_request_v1_beta2.py
--rw-r--r--   0 gangtao    (502) staff       (20)    16756 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_sink_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6233 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/create_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     8467 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/dashboard_dashboard.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7960 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/dashboard_panel.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3551 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3639 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/error_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2623 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/event.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3056 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/event_infer_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4271 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/event_infer_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5147 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/external_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3038 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/file_upload_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3018 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/format_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3026 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/format_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4282 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/global_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3565 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/graph.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3666 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/ingest_data.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3425 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/internal_http_handler_v1beta2_global_metrics_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5259 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/latency.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5334 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/node.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3443 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/owner.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15636 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/query.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6560 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/query_analysis.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4450 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/query_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3739 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/query_pipeline.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3606 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/query_pipeline_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4921 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/query_pipeline_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4199 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/query_pipeline_node_metric.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3752 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/query_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)    17346 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/query_with_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5611 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/resource_metrics_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6250 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/resource_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)     9946 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/sink.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3988 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/sink_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3879 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/sink_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)    10691 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/sink_with_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)    10291 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/source.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5814 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/source_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4434 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/source_preview_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3189 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/source_upload_body.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11665 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/source_with_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5737 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/sql_analyze_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11019 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/sql_analyze_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)    12462 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)    14411 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3102 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/stream_match_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3579 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/stream_setting.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4888 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/stream_stats.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3786 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/models/throughput.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4794 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/time_columns.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15879 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/models/udf.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3555 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/udf_argument.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3771 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/udf_auth_context.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/update_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5462 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/update_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5941 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/update_stream_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6518 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/update_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11802 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/models/view.py
--rw-r--r--   0 gangtao    (502) staff       (20)    13304 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/rest.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.947224 timeplus-1.1.2/swagger_client/timeplus/
--rw-r--r--   0 gangtao    (502) staff       (20)      896 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11402 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/api_keys_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    19432 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/dashboards_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7912 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/timeplus/metrics_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    19374 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_client/timeplus/persistent_queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    33760 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/queries_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5866 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/timeplus/queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    14675 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/sinks_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    42078 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/sources_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    26190 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/streams_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3866 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/topology_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    18450 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_client/timeplus/udfs_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15666 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_client/timeplus/views_v1beta1_api.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.994545 timeplus-1.1.2/swagger_test/
--rw-r--r--   0 gangtao    (502) staff       (20)        0 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_analyze_sql_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      842 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_api_key.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1215 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_api_keys_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_test/test_batching_policy.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_column_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_columns_resp.py
--rw-r--r--   0 gangtao    (502) staff       (20)      872 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_connection.py
--rw-r--r--   0 gangtao    (502) staff       (20)      922 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_connection_config.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_connection_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)      950 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_api_key_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      958 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_api_key_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1095 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_create_persistent_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_query_request_v1_beta1.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_query_request_v1_beta2.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_sink_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_create_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      938 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_dashboard_dashboard.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_dashboard_panel.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1547 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_dashboards_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_error_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_event.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_event_infer_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_event_infer_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_external_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_file_upload_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_format_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_format_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_global_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_graph.py
--rw-r--r--   0 gangtao    (502) staff       (20)      874 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_ingest_data.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1172 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_internal_http_handler_v1beta2_global_metrics_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      921 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_latency.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1058 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_test/test_metrics_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_owner.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1801 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_persistent_queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2197 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_queries_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      888 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_test/test_queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_query.py
--rw-r--r--   0 gangtao    (502) staff       (20)      971 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_query_analysis.py
--rw-r--r--   0 gangtao    (502) staff       (20)      963 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_query_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_query_pipeline.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_query_pipeline_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_query_pipeline_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)      982 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_query_pipeline_node_metric.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_query_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      997 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_query_with_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_test/test_resource_metrics_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      964 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_resource_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_sink.py
--rw-r--r--   0 gangtao    (502) staff       (20)      955 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_sink_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)      858 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_sink_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)      989 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_sink_with_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1295 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_sinks_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_source.py
--rw-r--r--   0 gangtao    (502) staff       (20)      971 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_source_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)      956 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_source_preview_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_source_upload_body.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1005 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_source_with_metrics.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2519 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_sources_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_sql_analyze_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_sql_analyze_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_stream_match_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_stream_setting.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_stream_stats.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1699 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_streams_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      945 2022-12-29 02:29:17.000000 timeplus-1.1.2/swagger_test/test_throughput.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_time_columns.py
--rw-r--r--   0 gangtao    (502) staff       (20)      873 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_topology_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      816 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_udf.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_udf_argument.py
--rw-r--r--   0 gangtao    (502) staff       (20)      908 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_udf_auth_context.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1438 2023-02-14 06:04:34.000000 timeplus-1.1.2/swagger_test/test_udfs_v1beta1_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_update_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_update_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_update_stream_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_update_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_view.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1311 2023-02-14 03:56:15.000000 timeplus-1.1.2/swagger_test/test_views_v1beta1_api.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.998001 timeplus-1.1.2/test/
--rw-r--r--   0 gangtao    (502) staff       (20)      624 2022-12-29 02:29:17.000000 timeplus-1.1.2/test/test_stream.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.997612 timeplus-1.1.2/timeplus/
--rw-r--r--   0 gangtao    (502) staff       (20)      240 2022-12-29 02:29:17.000000 timeplus-1.1.2/timeplus/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)      965 2022-12-29 18:08:58.000000 timeplus-1.1.2/timeplus/env.py
--rw-r--r--   0 gangtao    (502) staff       (20)      423 2022-12-29 02:29:17.000000 timeplus-1.1.2/timeplus/error.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3096 2023-02-14 06:04:34.000000 timeplus-1.1.2/timeplus/query.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4847 2023-02-14 06:04:34.000000 timeplus-1.1.2/timeplus/stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)      527 2022-12-28 18:52:21.000000 timeplus-1.1.2/timeplus/type.py
--rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-02-14 06:04:39.000000 timeplus-1.1.2/timeplus/version.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-02-14 06:04:44.999849 timeplus-1.1.2/timeplus.egg-info/
--rw-r--r--   0 gangtao    (502) staff       (20)     3921 2023-02-14 06:04:44.000000 timeplus-1.1.2/timeplus.egg-info/PKG-INFO
--rw-r--r--   0 gangtao    (502) staff       (20)     7806 2023-02-14 06:04:44.000000 timeplus-1.1.2/timeplus.egg-info/SOURCES.txt
--rw-r--r--   0 gangtao    (502) staff       (20)        1 2023-02-14 06:04:44.000000 timeplus-1.1.2/timeplus.egg-info/dependency_links.txt
--rw-r--r--   0 gangtao    (502) staff       (20)       82 2023-02-14 06:04:44.000000 timeplus-1.1.2/timeplus.egg-info/requires.txt
--rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-02-14 06:04:44.000000 timeplus-1.1.2/timeplus.egg-info/top_level.txt
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.100458 timeplus-1.2.1/
+-rw-r--r--   0 gangtao    (502) staff       (20)     3921 2023-06-07 00:11:38.100624 timeplus-1.2.1/PKG-INFO
+-rw-r--r--   0 gangtao    (502) staff       (20)     3479 2022-12-29 18:08:58.000000 timeplus-1.2.1/README.md
+-rw-r--r--   0 gangtao    (502) staff       (20)      633 2023-06-07 00:11:38.101254 timeplus-1.2.1/setup.cfg
+-rw-r--r--   0 gangtao    (502) staff       (20)     1247 2022-12-29 18:08:58.000000 timeplus-1.2.1/setup.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:37.970289 timeplus-1.2.1/swagger_client/
+-rw-r--r--   0 gangtao    (502) staff       (20)     5204 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    25043 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/api_client.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     8229 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/configuration.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.009478 timeplus-1.2.1/swagger_client/models/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4099 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3010 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/analyze_sql_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6294 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/api_key.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3907 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/batching_policy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3495 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6897 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/column_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4844 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/columns_resp.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5165 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_api_key_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7665 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_api_key_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6083 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/create_query_request_v1_beta2.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_sink_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6899 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/create_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6447 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/create_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     8467 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/dashboard_dashboard.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7960 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/dashboard_panel.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3551 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3639 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/error_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2623 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/event.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3056 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/event_infer_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4271 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/event_infer_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5147 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/external_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3038 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/file_upload_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3018 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/format_query_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3026 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/format_query_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5084 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/global_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3565 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/graph.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3666 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/ingest_data.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3880 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/metrics_query_throughput.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5334 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3443 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/owner.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15636 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3739 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3606 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4921 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4199 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline_node_metric.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3752 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5782 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/resource_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    10676 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/sink.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3879 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/sink_stat.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    12051 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/source.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5811 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/source_preview_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3189 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/source_upload_body.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5737 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/sql_analyze_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11019 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/sql_analyze_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    13632 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15463 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3102 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/stream_match_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3579 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/stream_setting.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6394 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/stream_stats.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4794 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/time_columns.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15879 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/udf.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3555 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/udf_argument.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3771 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/udf_auth_context.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/update_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5961 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/update_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6279 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/update_stream_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6856 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/update_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11854 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/view.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    12995 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/rest.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.018298 timeplus-1.2.1/swagger_client/timeplus/
+-rw-r--r--   0 gangtao    (502) staff       (20)     1040 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4723 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/alerts_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4385 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/alerts_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11402 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/api_keys_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    19476 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/dashboards_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     9044 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/metrics_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    31463 2023-06-07 00:11:27.000000 timeplus-1.2.1/swagger_client/timeplus/queries_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4703 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/sinks_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    18309 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/sinks_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    42086 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/sources_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    33693 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/streams_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3866 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/timeplus/topology_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    18450 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/udfs_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    22977 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/views_v1beta2_api.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.090202 timeplus-1.2.1/swagger_test/
+-rw-r--r--   0 gangtao    (502) staff       (20)       15 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      920 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_alerts_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      872 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_alerts_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_analyze_sql_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      842 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_api_key.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1215 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_api_keys_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_test/test_batching_policy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_column_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_columns_resp.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      950 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_api_key_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      958 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_api_key_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_query_request_v1_beta2.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_sink_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_create_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      938 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_dashboard_dashboard.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_dashboard_panel.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1547 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_dashboards_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_error_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_event.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_event_infer_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_event_infer_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_external_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_file_upload_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_format_query_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_format_query_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_global_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_graph.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      874 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_ingest_data.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_metrics_query_throughput.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1058 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_test/test_metrics_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_owner.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2014 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_queries_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      982 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline_node_metric.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      964 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_resource_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sink.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      858 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sink_stat.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      911 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_sinks_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1456 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_sinks_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_source.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      956 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_source_preview_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_source_upload_body.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2519 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_sources_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sql_analyze_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sql_analyze_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_match_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_setting.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_stats.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2036 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_streams_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_time_columns.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      873 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_topology_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      816 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_udf.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_udf_argument.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      908 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_udf_auth_context.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1438 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_udfs_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_stream_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_view.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1636 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_views_v1beta2_api.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.097105 timeplus-1.2.1/test/
+-rw-r--r--   0 gangtao    (502) staff       (20)      624 2022-12-29 02:29:17.000000 timeplus-1.2.1/test/test_stream.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.096633 timeplus-1.2.1/timeplus/
+-rw-r--r--   0 gangtao    (502) staff       (20)      240 2022-12-29 02:29:17.000000 timeplus-1.2.1/timeplus/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      931 2023-06-06 23:40:05.000000 timeplus-1.2.1/timeplus/env.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      423 2022-12-29 02:29:17.000000 timeplus-1.2.1/timeplus/error.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2912 2023-06-06 23:40:05.000000 timeplus-1.2.1/timeplus/query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4847 2023-06-06 23:40:05.000000 timeplus-1.2.1/timeplus/stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      527 2022-12-28 18:52:21.000000 timeplus-1.2.1/timeplus/type.py
+-rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-07 00:11:31.000000 timeplus-1.2.1/timeplus/version.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.100043 timeplus-1.2.1/timeplus.egg-info/
+-rw-r--r--   0 gangtao    (502) staff       (20)     3921 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/PKG-INFO
+-rw-r--r--   0 gangtao    (502) staff       (20)     6532 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/SOURCES.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)        1 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/dependency_links.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)       82 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/requires.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/top_level.txt
```

### Comparing `timeplus-1.1.2/PKG-INFO` & `timeplus-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeplus
-Version: 1.1.2
+Version: 1.2.1
 Summary: Timeplus python SDK
 Home-page: https://github.com/timeplus-io/gluon/tree/develop/python
 Author: Gang Tao
 Author-email: gang@timeplus.io
 Project-URL: Bug Tracker, https://github.com/timeplus-io/gluon/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `timeplus-1.1.2/README.md` & `timeplus-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/setup.cfg` & `timeplus-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/setup.py` & `timeplus-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/__init__.py` & `timeplus-1.2.1/swagger_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,69 +11,67 @@
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
-from swagger_client.timeplus.api_keys_v1beta1_api import APIKeysV1beta1Api
+from swagger_client.timeplus.api_keys_v1beta2_api import APIKeysV1beta2Api
+from swagger_client.timeplus.alerts_internal_api import AlertsInternalApi
+from swagger_client.timeplus.alerts_v1beta2_api import AlertsV1beta2Api
 from swagger_client.timeplus.dashboards_v1beta2_api import DashboardsV1beta2Api
 from swagger_client.timeplus.metrics_v1beta2_api import MetricsV1beta2Api
-from swagger_client.timeplus.queries_v1beta1_api import QueriesV1beta1Api
 from swagger_client.timeplus.queries_v1beta2_api import QueriesV1beta2Api
-from swagger_client.timeplus.sinks_v1beta1_api import SinksV1beta1Api
-from swagger_client.timeplus.sources_v1beta1_api import SourcesV1beta1Api
-from swagger_client.timeplus.streams_v1beta1_api import StreamsV1beta1Api
+from swagger_client.timeplus.sinks_internal_api import SinksInternalApi
+from swagger_client.timeplus.sinks_v1beta2_api import SinksV1beta2Api
+from swagger_client.timeplus.sources_v1beta2_api import SourcesV1beta2Api
+from swagger_client.timeplus.streams_v1beta2_api import StreamsV1beta2Api
 from swagger_client.timeplus.topology_v1beta2_api import TopologyV1beta2Api
-from swagger_client.timeplus.udfs_v1beta1_api import UDFsV1beta1Api
-from swagger_client.timeplus.views_v1beta1_api import ViewsV1beta1Api
+from swagger_client.timeplus.udfs_v1beta2_api import UDFsV1beta2Api
+from swagger_client.timeplus.views_v1beta2_api import ViewsV1beta2Api
 # import ApiClient
 from swagger_client.api_client import ApiClient
 from swagger_client.configuration import Configuration
 # import models into sdk package
 from swagger_client.models.api_key import APIKey
 from swagger_client.models.analyze_sql_request import AnalyzeSQLRequest
 from swagger_client.models.batching_policy import BatchingPolicy
 from swagger_client.models.column import Column
 from swagger_client.models.column_def import ColumnDef
 from swagger_client.models.columns_resp import ColumnsResp
-from swagger_client.models.connection import Connection
-from swagger_client.models.connection_config import ConnectionConfig
-from swagger_client.models.connection_stat import ConnectionStat
 from swagger_client.models.create_api_key_request import CreateAPIKeyRequest
 from swagger_client.models.create_api_key_response import CreateAPIKeyResponse
 from swagger_client.models.create_dashboard_request import CreateDashboardRequest
-from swagger_client.models.create_query_request_v1_beta1 import CreateQueryRequestV1Beta1
 from swagger_client.models.create_query_request_v1_beta2 import CreateQueryRequestV1Beta2
-from swagger_client.models.create_query_response import CreateQueryResponse
 from swagger_client.models.create_sink_request import CreateSinkRequest
 from swagger_client.models.create_source_request import CreateSourceRequest
+from swagger_client.models.create_view_request import CreateViewRequest
 from swagger_client.models.dashboard_dashboard import DashboardDashboard
 from swagger_client.models.dashboard_panel import DashboardPanel
 from swagger_client.models.edge import Edge
 from swagger_client.models.error_response import ErrorResponse
 from swagger_client.models.event import Event
 from swagger_client.models.event_infer_request import EventInferRequest
 from swagger_client.models.event_infer_response import EventInferResponse
 from swagger_client.models.external_stream_def import ExternalStreamDef
 from swagger_client.models.file_upload_response import FileUploadResponse
 from swagger_client.models.format_query_request import FormatQueryRequest
 from swagger_client.models.format_query_response import FormatQueryResponse
 from swagger_client.models.global_metrics_result import GlobalMetricsResult
 from swagger_client.models.graph import Graph
 from swagger_client.models.ingest_data import IngestData
+from swagger_client.models.metrics_query_throughput import MetricsQueryThroughput
 from swagger_client.models.node import Node
 from swagger_client.models.owner import Owner
 from swagger_client.models.query import Query
 from swagger_client.models.query_pipeline import QueryPipeline
 from swagger_client.models.query_pipeline_edge import QueryPipelineEdge
 from swagger_client.models.query_pipeline_node import QueryPipelineNode
 from swagger_client.models.query_pipeline_node_metric import QueryPipelineNodeMetric
 from swagger_client.models.query_result import QueryResult
-from swagger_client.models.resource_metrics_request import ResourceMetricsRequest
 from swagger_client.models.resource_metrics_result import ResourceMetricsResult
 from swagger_client.models.sql_analyze_column import SQLAnalyzeColumn
 from swagger_client.models.sql_analyze_result import SQLAnalyzeResult
 from swagger_client.models.sink import Sink
 from swagger_client.models.sink_stat import SinkStat
 from swagger_client.models.source import Source
 from swagger_client.models.source_preview_request import SourcePreviewRequest
```

### Comparing `timeplus-1.1.2/swagger_client/api_client.py` & `timeplus-1.2.1/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/configuration.py` & `timeplus-1.2.1/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/__init__.py` & `timeplus-1.2.1/swagger_client/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,48 +16,44 @@
 # import models into model package
 from swagger_client.models.api_key import APIKey
 from swagger_client.models.analyze_sql_request import AnalyzeSQLRequest
 from swagger_client.models.batching_policy import BatchingPolicy
 from swagger_client.models.column import Column
 from swagger_client.models.column_def import ColumnDef
 from swagger_client.models.columns_resp import ColumnsResp
-from swagger_client.models.connection import Connection
-from swagger_client.models.connection_config import ConnectionConfig
-from swagger_client.models.connection_stat import ConnectionStat
 from swagger_client.models.create_api_key_request import CreateAPIKeyRequest
 from swagger_client.models.create_api_key_response import CreateAPIKeyResponse
 from swagger_client.models.create_dashboard_request import CreateDashboardRequest
-from swagger_client.models.create_query_request_v1_beta1 import CreateQueryRequestV1Beta1
 from swagger_client.models.create_query_request_v1_beta2 import CreateQueryRequestV1Beta2
-from swagger_client.models.create_query_response import CreateQueryResponse
 from swagger_client.models.create_sink_request import CreateSinkRequest
 from swagger_client.models.create_source_request import CreateSourceRequest
+from swagger_client.models.create_view_request import CreateViewRequest
 from swagger_client.models.dashboard_dashboard import DashboardDashboard
 from swagger_client.models.dashboard_panel import DashboardPanel
 from swagger_client.models.edge import Edge
 from swagger_client.models.error_response import ErrorResponse
 from swagger_client.models.event import Event
 from swagger_client.models.event_infer_request import EventInferRequest
 from swagger_client.models.event_infer_response import EventInferResponse
 from swagger_client.models.external_stream_def import ExternalStreamDef
 from swagger_client.models.file_upload_response import FileUploadResponse
 from swagger_client.models.format_query_request import FormatQueryRequest
 from swagger_client.models.format_query_response import FormatQueryResponse
 from swagger_client.models.global_metrics_result import GlobalMetricsResult
 from swagger_client.models.graph import Graph
 from swagger_client.models.ingest_data import IngestData
+from swagger_client.models.metrics_query_throughput import MetricsQueryThroughput
 from swagger_client.models.node import Node
 from swagger_client.models.owner import Owner
 from swagger_client.models.query import Query
 from swagger_client.models.query_pipeline import QueryPipeline
 from swagger_client.models.query_pipeline_edge import QueryPipelineEdge
 from swagger_client.models.query_pipeline_node import QueryPipelineNode
 from swagger_client.models.query_pipeline_node_metric import QueryPipelineNodeMetric
 from swagger_client.models.query_result import QueryResult
-from swagger_client.models.resource_metrics_request import ResourceMetricsRequest
 from swagger_client.models.resource_metrics_result import ResourceMetricsResult
 from swagger_client.models.sql_analyze_column import SQLAnalyzeColumn
 from swagger_client.models.sql_analyze_result import SQLAnalyzeResult
 from swagger_client.models.sink import Sink
 from swagger_client.models.sink_stat import SinkStat
 from swagger_client.models.source import Source
 from swagger_client.models.source_preview_request import SourcePreviewRequest
```

### Comparing `timeplus-1.1.2/swagger_client/models/analyze_sql_request.py` & `timeplus-1.2.1/swagger_client/models/analyze_sql_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/api_key.py` & `timeplus-1.2.1/swagger_client/models/api_key.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/batching_policy.py` & `timeplus-1.2.1/swagger_client/models/batching_policy.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/column.py` & `timeplus-1.2.1/swagger_client/models/column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/column_def.py` & `timeplus-1.2.1/swagger_client/models/column_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/columns_resp.py` & `timeplus-1.2.1/swagger_client/models/columns_resp.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,96 +24,44 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'alias': 'str',
-        'comment': 'str',
         'default': 'str',
         'name': 'str',
         'nullable': 'bool',
         'type': 'str'
     }
 
     attribute_map = {
-        'alias': 'alias',
-        'comment': 'comment',
         'default': 'default',
         'name': 'name',
         'nullable': 'nullable',
         'type': 'type'
     }
 
-    def __init__(self, alias=None, comment=None, default=None, name=None, nullable=None, type=None):  # noqa: E501
+    def __init__(self, default=None, name=None, nullable=None, type=None):  # noqa: E501
         """ColumnsResp - a model defined in Swagger"""  # noqa: E501
-        self._alias = None
-        self._comment = None
         self._default = None
         self._name = None
         self._nullable = None
         self._type = None
         self.discriminator = None
-        if alias is not None:
-            self.alias = alias
-        if comment is not None:
-            self.comment = comment
         if default is not None:
             self.default = default
         if name is not None:
             self.name = name
         if nullable is not None:
             self.nullable = nullable
         if type is not None:
             self.type = type
 
     @property
-    def alias(self):
-        """Gets the alias of this ColumnsResp.  # noqa: E501
-
-
-        :return: The alias of this ColumnsResp.  # noqa: E501
-        :rtype: str
-        """
-        return self._alias
-
-    @alias.setter
-    def alias(self, alias):
-        """Sets the alias of this ColumnsResp.
-
-
-        :param alias: The alias of this ColumnsResp.  # noqa: E501
-        :type: str
-        """
-
-        self._alias = alias
-
-    @property
-    def comment(self):
-        """Gets the comment of this ColumnsResp.  # noqa: E501
-
-
-        :return: The comment of this ColumnsResp.  # noqa: E501
-        :rtype: str
-        """
-        return self._comment
-
-    @comment.setter
-    def comment(self, comment):
-        """Sets the comment of this ColumnsResp.
-
-
-        :param comment: The comment of this ColumnsResp.  # noqa: E501
-        :type: str
-        """
-
-        self._comment = comment
-
-    @property
     def default(self):
         """Gets the default of this ColumnsResp.  # noqa: E501
 
 
         :return: The default of this ColumnsResp.  # noqa: E501
         :rtype: str
         """
```

### Comparing `timeplus-1.1.2/swagger_client/models/connection.py` & `timeplus-1.2.1/swagger_client/models/udf_auth_context.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,88 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Connection(object):
+class UDFAuthContext(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'config': 'ConnectionConfig',
-        'stat': 'ConnectionStat'
+        'key_name': 'str',
+        'key_value': 'str'
     }
 
     attribute_map = {
-        'config': 'config',
-        'stat': 'stat'
+        'key_name': 'key_name',
+        'key_value': 'key_value'
     }
 
-    def __init__(self, config=None, stat=None):  # noqa: E501
-        """Connection - a model defined in Swagger"""  # noqa: E501
-        self._config = None
-        self._stat = None
+    def __init__(self, key_name=None, key_value=None):  # noqa: E501
+        """UDFAuthContext - a model defined in Swagger"""  # noqa: E501
+        self._key_name = None
+        self._key_value = None
         self.discriminator = None
-        if config is not None:
-            self.config = config
-        self.stat = stat
+        if key_name is not None:
+            self.key_name = key_name
+        if key_value is not None:
+            self.key_value = key_value
 
     @property
-    def config(self):
-        """Gets the config of this Connection.  # noqa: E501
+    def key_name(self):
+        """Gets the key_name of this UDFAuthContext.  # noqa: E501
 
 
-        :return: The config of this Connection.  # noqa: E501
-        :rtype: ConnectionConfig
+        :return: The key_name of this UDFAuthContext.  # noqa: E501
+        :rtype: str
         """
-        return self._config
+        return self._key_name
 
-    @config.setter
-    def config(self, config):
-        """Sets the config of this Connection.
+    @key_name.setter
+    def key_name(self, key_name):
+        """Sets the key_name of this UDFAuthContext.
 
 
-        :param config: The config of this Connection.  # noqa: E501
-        :type: ConnectionConfig
+        :param key_name: The key_name of this UDFAuthContext.  # noqa: E501
+        :type: str
         """
 
-        self._config = config
+        self._key_name = key_name
 
     @property
-    def stat(self):
-        """Gets the stat of this Connection.  # noqa: E501
+    def key_value(self):
+        """Gets the key_value of this UDFAuthContext.  # noqa: E501
 
 
-        :return: The stat of this Connection.  # noqa: E501
-        :rtype: ConnectionStat
+        :return: The key_value of this UDFAuthContext.  # noqa: E501
+        :rtype: str
         """
-        return self._stat
+        return self._key_value
 
-    @stat.setter
-    def stat(self, stat):
-        """Sets the stat of this Connection.
+    @key_value.setter
+    def key_value(self, key_value):
+        """Sets the key_value of this UDFAuthContext.
 
 
-        :param stat: The stat of this Connection.  # noqa: E501
-        :type: ConnectionStat
+        :param key_value: The key_value of this UDFAuthContext.  # noqa: E501
+        :type: str
         """
-        if stat is None:
-            raise ValueError("Invalid value for `stat`, must not be `None`")  # noqa: E501
 
-        self._stat = stat
+        self._key_value = key_value
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -107,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Connection, dict):
+        if issubclass(UDFAuthContext, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -123,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Connection):
+        if not isinstance(other, UDFAuthContext):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/connection_stat.py` & `timeplus-1.2.1/swagger_client/models/udf_argument.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,89 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ConnectionStat(object):
+class UDFArgument(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'message': 'str',
-        'status': 'str'
+        'name': 'str',
+        'type': 'str'
     }
 
     attribute_map = {
-        'message': 'message',
-        'status': 'status'
+        'name': 'name',
+        'type': 'type'
     }
 
-    def __init__(self, message=None, status=None):  # noqa: E501
-        """ConnectionStat - a model defined in Swagger"""  # noqa: E501
-        self._message = None
-        self._status = None
+    def __init__(self, name=None, type=None):  # noqa: E501
+        """UDFArgument - a model defined in Swagger"""  # noqa: E501
+        self._name = None
+        self._type = None
         self.discriminator = None
-        self.message = message
-        self.status = status
+        if name is not None:
+            self.name = name
+        if type is not None:
+            self.type = type
 
     @property
-    def message(self):
-        """Gets the message of this ConnectionStat.  # noqa: E501
+    def name(self):
+        """Gets the name of this UDFArgument.  # noqa: E501
 
 
-        :return: The message of this ConnectionStat.  # noqa: E501
+        :return: The name of this UDFArgument.  # noqa: E501
         :rtype: str
         """
-        return self._message
+        return self._name
 
-    @message.setter
-    def message(self, message):
-        """Sets the message of this ConnectionStat.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this UDFArgument.
 
 
-        :param message: The message of this ConnectionStat.  # noqa: E501
+        :param name: The name of this UDFArgument.  # noqa: E501
         :type: str
         """
-        if message is None:
-            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
-        self._message = message
+        self._name = name
 
     @property
-    def status(self):
-        """Gets the status of this ConnectionStat.  # noqa: E501
+    def type(self):
+        """Gets the type of this UDFArgument.  # noqa: E501
 
 
-        :return: The status of this ConnectionStat.  # noqa: E501
+        :return: The type of this UDFArgument.  # noqa: E501
         :rtype: str
         """
-        return self._status
+        return self._type
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this ConnectionStat.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this UDFArgument.
 
 
-        :param status: The status of this ConnectionStat.  # noqa: E501
+        :param type: The type of this UDFArgument.  # noqa: E501
         :type: str
         """
-        if status is None:
-            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
-        self._status = status
+        self._type = type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ConnectionStat, dict):
+        if issubclass(UDFArgument, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ConnectionStat):
+        if not isinstance(other, UDFArgument):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/create_api_key_request.py` & `timeplus-1.2.1/swagger_client/models/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/create_api_key_response.py` & `timeplus-1.2.1/swagger_client/models/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/create_dashboard_request.py` & `timeplus-1.2.1/swagger_client/models/create_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/create_persistent_query_request.py` & `timeplus-1.2.1/swagger_client/models/update_source_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,151 +1,155 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CreatePersistentQueryRequest(object):
+class UpdateSourceRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'description': 'str',
         'name': 'str',
-        'sinks': 'list[str]',
-        'sql': 'str'
+        'properties': 'dict(str, object)',
+        'stream': 'str'
     }
 
     attribute_map = {
         'description': 'description',
         'name': 'name',
-        'sinks': 'sinks',
-        'sql': 'sql'
+        'properties': 'properties',
+        'stream': 'stream'
     }
 
-    def __init__(self, description=None, name=None, sinks=None, sql=None):  # noqa: E501
-        """CreatePersistentQueryRequest - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, description=None, name=None, properties=None, stream=None):  # noqa: E501
+        """UpdateSourceRequest - a model defined in Swagger"""  # noqa: E501
         self._description = None
         self._name = None
-        self._sinks = None
-        self._sql = None
+        self._properties = None
+        self._stream = None
         self.discriminator = None
         if description is not None:
             self.description = description
         if name is not None:
             self.name = name
-        self.sinks = sinks
-        self.sql = sql
+        if properties is not None:
+            self.properties = properties
+        if stream is not None:
+            self.stream = stream
 
     @property
     def description(self):
-        """Gets the description of this CreatePersistentQueryRequest.  # noqa: E501
+        """Gets the description of this UpdateSourceRequest.  # noqa: E501
 
 
-        :return: The description of this CreatePersistentQueryRequest.  # noqa: E501
+        :return: The description of this UpdateSourceRequest.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreatePersistentQueryRequest.
+        """Sets the description of this UpdateSourceRequest.
 
 
-        :param description: The description of this CreatePersistentQueryRequest.  # noqa: E501
+        :param description: The description of this UpdateSourceRequest.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
     def name(self):
-        """Gets the name of this CreatePersistentQueryRequest.  # noqa: E501
+        """Gets the name of this UpdateSourceRequest.  # noqa: E501
 
+        Source name should only contain a maximum of 64 letters, numbers, or _, and start with a letter  # noqa: E501
 
-        :return: The name of this CreatePersistentQueryRequest.  # noqa: E501
+        :return: The name of this UpdateSourceRequest.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreatePersistentQueryRequest.
+        """Sets the name of this UpdateSourceRequest.
 
+        Source name should only contain a maximum of 64 letters, numbers, or _, and start with a letter  # noqa: E501
 
-        :param name: The name of this CreatePersistentQueryRequest.  # noqa: E501
+        :param name: The name of this UpdateSourceRequest.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
-    def sinks(self):
-        """Gets the sinks of this CreatePersistentQueryRequest.  # noqa: E501
+    def properties(self):
+        """Gets the properties of this UpdateSourceRequest.  # noqa: E501
 
+        Additional properties that required to read the data from source. Please refer to the documentation for this source type  # noqa: E501
 
-        :return: The sinks of this CreatePersistentQueryRequest.  # noqa: E501
-        :rtype: list[str]
+        :return: The properties of this UpdateSourceRequest.  # noqa: E501
+        :rtype: dict(str, object)
         """
-        return self._sinks
+        return self._properties
 
-    @sinks.setter
-    def sinks(self, sinks):
-        """Sets the sinks of this CreatePersistentQueryRequest.
+    @properties.setter
+    def properties(self, properties):
+        """Sets the properties of this UpdateSourceRequest.
 
+        Additional properties that required to read the data from source. Please refer to the documentation for this source type  # noqa: E501
 
-        :param sinks: The sinks of this CreatePersistentQueryRequest.  # noqa: E501
-        :type: list[str]
+        :param properties: The properties of this UpdateSourceRequest.  # noqa: E501
+        :type: dict(str, object)
         """
-        if sinks is None:
-            raise ValueError("Invalid value for `sinks`, must not be `None`")  # noqa: E501
 
-        self._sinks = sinks
+        self._properties = properties
 
     @property
-    def sql(self):
-        """Gets the sql of this CreatePersistentQueryRequest.  # noqa: E501
+    def stream(self):
+        """Gets the stream of this UpdateSourceRequest.  # noqa: E501
 
+        The name of the target stream that this source writes to. The stream needs to be created first.  # noqa: E501
 
-        :return: The sql of this CreatePersistentQueryRequest.  # noqa: E501
+        :return: The stream of this UpdateSourceRequest.  # noqa: E501
         :rtype: str
         """
-        return self._sql
+        return self._stream
 
-    @sql.setter
-    def sql(self, sql):
-        """Sets the sql of this CreatePersistentQueryRequest.
+    @stream.setter
+    def stream(self, stream):
+        """Sets the stream of this UpdateSourceRequest.
 
+        The name of the target stream that this source writes to. The stream needs to be created first.  # noqa: E501
 
-        :param sql: The sql of this CreatePersistentQueryRequest.  # noqa: E501
+        :param stream: The stream of this UpdateSourceRequest.  # noqa: E501
         :type: str
         """
-        if sql is None:
-            raise ValueError("Invalid value for `sql`, must not be `None`")  # noqa: E501
 
-        self._sql = sql
+        self._stream = stream
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -160,15 +164,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CreatePersistentQueryRequest, dict):
+        if issubclass(UpdateSourceRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -176,15 +180,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreatePersistentQueryRequest):
+        if not isinstance(other, UpdateSourceRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/create_query_request_v1_beta1.py` & `timeplus-1.2.1/swagger_client/models/create_query_request_v1_beta2.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,135 +11,162 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CreateQueryRequestV1Beta1(object):
+class CreateQueryRequestV1Beta2(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'batching_policy': 'BatchingPolicy',
         'description': 'str',
         'name': 'str',
         'sql': 'str',
         'tags': 'list[str]'
     }
 
     attribute_map = {
+        'batching_policy': 'batching_policy',
         'description': 'description',
         'name': 'name',
         'sql': 'sql',
         'tags': 'tags'
     }
 
-    def __init__(self, description=None, name=None, sql=None, tags=None):  # noqa: E501
-        """CreateQueryRequestV1Beta1 - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, batching_policy=None, description=None, name=None, sql=None, tags=None):  # noqa: E501
+        """CreateQueryRequestV1Beta2 - a model defined in Swagger"""  # noqa: E501
+        self._batching_policy = None
         self._description = None
         self._name = None
         self._sql = None
         self._tags = None
         self.discriminator = None
+        if batching_policy is not None:
+            self.batching_policy = batching_policy
         if description is not None:
             self.description = description
         if name is not None:
             self.name = name
-        if sql is not None:
-            self.sql = sql
+        self.sql = sql
         if tags is not None:
             self.tags = tags
 
     @property
+    def batching_policy(self):
+        """Gets the batching_policy of this CreateQueryRequestV1Beta2.  # noqa: E501
+
+
+        :return: The batching_policy of this CreateQueryRequestV1Beta2.  # noqa: E501
+        :rtype: BatchingPolicy
+        """
+        return self._batching_policy
+
+    @batching_policy.setter
+    def batching_policy(self, batching_policy):
+        """Sets the batching_policy of this CreateQueryRequestV1Beta2.
+
+
+        :param batching_policy: The batching_policy of this CreateQueryRequestV1Beta2.  # noqa: E501
+        :type: BatchingPolicy
+        """
+
+        self._batching_policy = batching_policy
+
+    @property
     def description(self):
-        """Gets the description of this CreateQueryRequestV1Beta1.  # noqa: E501
+        """Gets the description of this CreateQueryRequestV1Beta2.  # noqa: E501
 
 
-        :return: The description of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :return: The description of this CreateQueryRequestV1Beta2.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateQueryRequestV1Beta1.
+        """Sets the description of this CreateQueryRequestV1Beta2.
 
 
-        :param description: The description of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :param description: The description of this CreateQueryRequestV1Beta2.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
     def name(self):
-        """Gets the name of this CreateQueryRequestV1Beta1.  # noqa: E501
+        """Gets the name of this CreateQueryRequestV1Beta2.  # noqa: E501
 
 
-        :return: The name of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :return: The name of this CreateQueryRequestV1Beta2.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreateQueryRequestV1Beta1.
+        """Sets the name of this CreateQueryRequestV1Beta2.
 
 
-        :param name: The name of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :param name: The name of this CreateQueryRequestV1Beta2.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def sql(self):
-        """Gets the sql of this CreateQueryRequestV1Beta1.  # noqa: E501
+        """Gets the sql of this CreateQueryRequestV1Beta2.  # noqa: E501
 
 
-        :return: The sql of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :return: The sql of this CreateQueryRequestV1Beta2.  # noqa: E501
         :rtype: str
         """
         return self._sql
 
     @sql.setter
     def sql(self, sql):
-        """Sets the sql of this CreateQueryRequestV1Beta1.
+        """Sets the sql of this CreateQueryRequestV1Beta2.
 
 
-        :param sql: The sql of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :param sql: The sql of this CreateQueryRequestV1Beta2.  # noqa: E501
         :type: str
         """
+        if sql is None:
+            raise ValueError("Invalid value for `sql`, must not be `None`")  # noqa: E501
 
         self._sql = sql
 
     @property
     def tags(self):
-        """Gets the tags of this CreateQueryRequestV1Beta1.  # noqa: E501
+        """Gets the tags of this CreateQueryRequestV1Beta2.  # noqa: E501
 
 
-        :return: The tags of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :return: The tags of this CreateQueryRequestV1Beta2.  # noqa: E501
         :rtype: list[str]
         """
         return self._tags
 
     @tags.setter
     def tags(self, tags):
-        """Sets the tags of this CreateQueryRequestV1Beta1.
+        """Sets the tags of this CreateQueryRequestV1Beta2.
 
 
-        :param tags: The tags of this CreateQueryRequestV1Beta1.  # noqa: E501
+        :param tags: The tags of this CreateQueryRequestV1Beta2.  # noqa: E501
         :type: list[str]
         """
 
         self._tags = tags
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -158,15 +185,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CreateQueryRequestV1Beta1, dict):
+        if issubclass(CreateQueryRequestV1Beta2, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +201,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateQueryRequestV1Beta1):
+        if not isinstance(other, CreateQueryRequestV1Beta2):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/create_query_response.py` & `timeplus-1.2.1/swagger_client/models/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CreateQueryResponse(object):
+class Query(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -68,15 +68,15 @@
         'start_time': 'start_time',
         'status': 'status',
         'tags': 'tags',
         'time_columns': 'timeColumns'
     }
 
     def __init__(self, analysis=None, created_at=None, created_by=None, description=None, duration=None, end_time=None, id=None, last_updated_at=None, last_updated_by=None, message=None, name=None, response_time=None, result=None, sinks=None, sql=None, start_time=None, status=None, tags=None, time_columns=None):  # noqa: E501
-        """CreateQueryResponse - a model defined in Swagger"""  # noqa: E501
+        """Query - a model defined in Swagger"""  # noqa: E501
         self._analysis = None
         self._created_at = None
         self._created_by = None
         self._description = None
         self._duration = None
         self._end_time = None
         self._id = None
@@ -118,428 +118,428 @@
         self.status = status
         if tags is not None:
             self.tags = tags
         self.time_columns = time_columns
 
     @property
     def analysis(self):
-        """Gets the analysis of this CreateQueryResponse.  # noqa: E501
+        """Gets the analysis of this Query.  # noqa: E501
 
 
-        :return: The analysis of this CreateQueryResponse.  # noqa: E501
+        :return: The analysis of this Query.  # noqa: E501
         :rtype: SQLAnalyzeResult
         """
         return self._analysis
 
     @analysis.setter
     def analysis(self, analysis):
-        """Sets the analysis of this CreateQueryResponse.
+        """Sets the analysis of this Query.
 
 
-        :param analysis: The analysis of this CreateQueryResponse.  # noqa: E501
+        :param analysis: The analysis of this Query.  # noqa: E501
         :type: SQLAnalyzeResult
         """
         if analysis is None:
             raise ValueError("Invalid value for `analysis`, must not be `None`")  # noqa: E501
 
         self._analysis = analysis
 
     @property
     def created_at(self):
-        """Gets the created_at of this CreateQueryResponse.  # noqa: E501
+        """Gets the created_at of this Query.  # noqa: E501
 
 
-        :return: The created_at of this CreateQueryResponse.  # noqa: E501
+        :return: The created_at of this Query.  # noqa: E501
         :rtype: str
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
-        """Sets the created_at of this CreateQueryResponse.
+        """Sets the created_at of this Query.
 
 
-        :param created_at: The created_at of this CreateQueryResponse.  # noqa: E501
+        :param created_at: The created_at of this Query.  # noqa: E501
         :type: str
         """
 
         self._created_at = created_at
 
     @property
     def created_by(self):
-        """Gets the created_by of this CreateQueryResponse.  # noqa: E501
+        """Gets the created_by of this Query.  # noqa: E501
 
 
-        :return: The created_by of this CreateQueryResponse.  # noqa: E501
+        :return: The created_by of this Query.  # noqa: E501
         :rtype: Owner
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
-        """Sets the created_by of this CreateQueryResponse.
+        """Sets the created_by of this Query.
 
 
-        :param created_by: The created_by of this CreateQueryResponse.  # noqa: E501
+        :param created_by: The created_by of this Query.  # noqa: E501
         :type: Owner
         """
 
         self._created_by = created_by
 
     @property
     def description(self):
-        """Gets the description of this CreateQueryResponse.  # noqa: E501
+        """Gets the description of this Query.  # noqa: E501
 
 
-        :return: The description of this CreateQueryResponse.  # noqa: E501
+        :return: The description of this Query.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateQueryResponse.
+        """Sets the description of this Query.
 
 
-        :param description: The description of this CreateQueryResponse.  # noqa: E501
+        :param description: The description of this Query.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
     def duration(self):
-        """Gets the duration of this CreateQueryResponse.  # noqa: E501
+        """Gets the duration of this Query.  # noqa: E501
 
 
-        :return: The duration of this CreateQueryResponse.  # noqa: E501
+        :return: The duration of this Query.  # noqa: E501
         :rtype: int
         """
         return self._duration
 
     @duration.setter
     def duration(self, duration):
-        """Sets the duration of this CreateQueryResponse.
+        """Sets the duration of this Query.
 
 
-        :param duration: The duration of this CreateQueryResponse.  # noqa: E501
+        :param duration: The duration of this Query.  # noqa: E501
         :type: int
         """
         if duration is None:
             raise ValueError("Invalid value for `duration`, must not be `None`")  # noqa: E501
 
         self._duration = duration
 
     @property
     def end_time(self):
-        """Gets the end_time of this CreateQueryResponse.  # noqa: E501
+        """Gets the end_time of this Query.  # noqa: E501
 
 
-        :return: The end_time of this CreateQueryResponse.  # noqa: E501
+        :return: The end_time of this Query.  # noqa: E501
         :rtype: int
         """
         return self._end_time
 
     @end_time.setter
     def end_time(self, end_time):
-        """Sets the end_time of this CreateQueryResponse.
+        """Sets the end_time of this Query.
 
 
-        :param end_time: The end_time of this CreateQueryResponse.  # noqa: E501
+        :param end_time: The end_time of this Query.  # noqa: E501
         :type: int
         """
         if end_time is None:
             raise ValueError("Invalid value for `end_time`, must not be `None`")  # noqa: E501
 
         self._end_time = end_time
 
     @property
     def id(self):
-        """Gets the id of this CreateQueryResponse.  # noqa: E501
+        """Gets the id of this Query.  # noqa: E501
 
 
-        :return: The id of this CreateQueryResponse.  # noqa: E501
+        :return: The id of this Query.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this CreateQueryResponse.
+        """Sets the id of this Query.
 
 
-        :param id: The id of this CreateQueryResponse.  # noqa: E501
+        :param id: The id of this Query.  # noqa: E501
         :type: str
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def last_updated_at(self):
-        """Gets the last_updated_at of this CreateQueryResponse.  # noqa: E501
+        """Gets the last_updated_at of this Query.  # noqa: E501
 
 
-        :return: The last_updated_at of this CreateQueryResponse.  # noqa: E501
+        :return: The last_updated_at of this Query.  # noqa: E501
         :rtype: str
         """
         return self._last_updated_at
 
     @last_updated_at.setter
     def last_updated_at(self, last_updated_at):
-        """Sets the last_updated_at of this CreateQueryResponse.
+        """Sets the last_updated_at of this Query.
 
 
-        :param last_updated_at: The last_updated_at of this CreateQueryResponse.  # noqa: E501
+        :param last_updated_at: The last_updated_at of this Query.  # noqa: E501
         :type: str
         """
 
         self._last_updated_at = last_updated_at
 
     @property
     def last_updated_by(self):
-        """Gets the last_updated_by of this CreateQueryResponse.  # noqa: E501
+        """Gets the last_updated_by of this Query.  # noqa: E501
 
 
-        :return: The last_updated_by of this CreateQueryResponse.  # noqa: E501
+        :return: The last_updated_by of this Query.  # noqa: E501
         :rtype: Owner
         """
         return self._last_updated_by
 
     @last_updated_by.setter
     def last_updated_by(self, last_updated_by):
-        """Sets the last_updated_by of this CreateQueryResponse.
+        """Sets the last_updated_by of this Query.
 
 
-        :param last_updated_by: The last_updated_by of this CreateQueryResponse.  # noqa: E501
+        :param last_updated_by: The last_updated_by of this Query.  # noqa: E501
         :type: Owner
         """
 
         self._last_updated_by = last_updated_by
 
     @property
     def message(self):
-        """Gets the message of this CreateQueryResponse.  # noqa: E501
+        """Gets the message of this Query.  # noqa: E501
 
 
-        :return: The message of this CreateQueryResponse.  # noqa: E501
+        :return: The message of this Query.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this CreateQueryResponse.
+        """Sets the message of this Query.
 
 
-        :param message: The message of this CreateQueryResponse.  # noqa: E501
+        :param message: The message of this Query.  # noqa: E501
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
         self._message = message
 
     @property
     def name(self):
-        """Gets the name of this CreateQueryResponse.  # noqa: E501
+        """Gets the name of this Query.  # noqa: E501
 
 
-        :return: The name of this CreateQueryResponse.  # noqa: E501
+        :return: The name of this Query.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreateQueryResponse.
+        """Sets the name of this Query.
 
 
-        :param name: The name of this CreateQueryResponse.  # noqa: E501
+        :param name: The name of this Query.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def response_time(self):
-        """Gets the response_time of this CreateQueryResponse.  # noqa: E501
+        """Gets the response_time of this Query.  # noqa: E501
 
 
-        :return: The response_time of this CreateQueryResponse.  # noqa: E501
+        :return: The response_time of this Query.  # noqa: E501
         :rtype: int
         """
         return self._response_time
 
     @response_time.setter
     def response_time(self, response_time):
-        """Sets the response_time of this CreateQueryResponse.
+        """Sets the response_time of this Query.
 
 
-        :param response_time: The response_time of this CreateQueryResponse.  # noqa: E501
+        :param response_time: The response_time of this Query.  # noqa: E501
         :type: int
         """
         if response_time is None:
             raise ValueError("Invalid value for `response_time`, must not be `None`")  # noqa: E501
 
         self._response_time = response_time
 
     @property
     def result(self):
-        """Gets the result of this CreateQueryResponse.  # noqa: E501
+        """Gets the result of this Query.  # noqa: E501
 
 
-        :return: The result of this CreateQueryResponse.  # noqa: E501
+        :return: The result of this Query.  # noqa: E501
         :rtype: QueryResult
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this CreateQueryResponse.
+        """Sets the result of this Query.
 
 
-        :param result: The result of this CreateQueryResponse.  # noqa: E501
+        :param result: The result of this Query.  # noqa: E501
         :type: QueryResult
         """
         if result is None:
             raise ValueError("Invalid value for `result`, must not be `None`")  # noqa: E501
 
         self._result = result
 
     @property
     def sinks(self):
-        """Gets the sinks of this CreateQueryResponse.  # noqa: E501
+        """Gets the sinks of this Query.  # noqa: E501
 
 
-        :return: The sinks of this CreateQueryResponse.  # noqa: E501
+        :return: The sinks of this Query.  # noqa: E501
         :rtype: dict(str, SinkStat)
         """
         return self._sinks
 
     @sinks.setter
     def sinks(self, sinks):
-        """Sets the sinks of this CreateQueryResponse.
+        """Sets the sinks of this Query.
 
 
-        :param sinks: The sinks of this CreateQueryResponse.  # noqa: E501
+        :param sinks: The sinks of this Query.  # noqa: E501
         :type: dict(str, SinkStat)
         """
         if sinks is None:
             raise ValueError("Invalid value for `sinks`, must not be `None`")  # noqa: E501
 
         self._sinks = sinks
 
     @property
     def sql(self):
-        """Gets the sql of this CreateQueryResponse.  # noqa: E501
+        """Gets the sql of this Query.  # noqa: E501
 
 
-        :return: The sql of this CreateQueryResponse.  # noqa: E501
+        :return: The sql of this Query.  # noqa: E501
         :rtype: str
         """
         return self._sql
 
     @sql.setter
     def sql(self, sql):
-        """Sets the sql of this CreateQueryResponse.
+        """Sets the sql of this Query.
 
 
-        :param sql: The sql of this CreateQueryResponse.  # noqa: E501
+        :param sql: The sql of this Query.  # noqa: E501
         :type: str
         """
         if sql is None:
             raise ValueError("Invalid value for `sql`, must not be `None`")  # noqa: E501
 
         self._sql = sql
 
     @property
     def start_time(self):
-        """Gets the start_time of this CreateQueryResponse.  # noqa: E501
+        """Gets the start_time of this Query.  # noqa: E501
 
 
-        :return: The start_time of this CreateQueryResponse.  # noqa: E501
+        :return: The start_time of this Query.  # noqa: E501
         :rtype: int
         """
         return self._start_time
 
     @start_time.setter
     def start_time(self, start_time):
-        """Sets the start_time of this CreateQueryResponse.
+        """Sets the start_time of this Query.
 
 
-        :param start_time: The start_time of this CreateQueryResponse.  # noqa: E501
+        :param start_time: The start_time of this Query.  # noqa: E501
         :type: int
         """
         if start_time is None:
             raise ValueError("Invalid value for `start_time`, must not be `None`")  # noqa: E501
 
         self._start_time = start_time
 
     @property
     def status(self):
-        """Gets the status of this CreateQueryResponse.  # noqa: E501
+        """Gets the status of this Query.  # noqa: E501
 
 
-        :return: The status of this CreateQueryResponse.  # noqa: E501
+        :return: The status of this Query.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this CreateQueryResponse.
+        """Sets the status of this Query.
 
 
-        :param status: The status of this CreateQueryResponse.  # noqa: E501
+        :param status: The status of this Query.  # noqa: E501
         :type: str
         """
         if status is None:
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
     def tags(self):
-        """Gets the tags of this CreateQueryResponse.  # noqa: E501
+        """Gets the tags of this Query.  # noqa: E501
 
 
-        :return: The tags of this CreateQueryResponse.  # noqa: E501
+        :return: The tags of this Query.  # noqa: E501
         :rtype: list[str]
         """
         return self._tags
 
     @tags.setter
     def tags(self, tags):
-        """Sets the tags of this CreateQueryResponse.
+        """Sets the tags of this Query.
 
 
-        :param tags: The tags of this CreateQueryResponse.  # noqa: E501
+        :param tags: The tags of this Query.  # noqa: E501
         :type: list[str]
         """
 
         self._tags = tags
 
     @property
     def time_columns(self):
-        """Gets the time_columns of this CreateQueryResponse.  # noqa: E501
+        """Gets the time_columns of this Query.  # noqa: E501
 
 
-        :return: The time_columns of this CreateQueryResponse.  # noqa: E501
+        :return: The time_columns of this Query.  # noqa: E501
         :rtype: TimeColumns
         """
         return self._time_columns
 
     @time_columns.setter
     def time_columns(self, time_columns):
-        """Sets the time_columns of this CreateQueryResponse.
+        """Sets the time_columns of this Query.
 
 
-        :param time_columns: The time_columns of this CreateQueryResponse.  # noqa: E501
+        :param time_columns: The time_columns of this Query.  # noqa: E501
         :type: TimeColumns
         """
         if time_columns is None:
             raise ValueError("Invalid value for `time_columns`, must not be `None`")  # noqa: E501
 
         self._time_columns = time_columns
 
@@ -560,15 +560,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CreateQueryResponse, dict):
+        if issubclass(Query, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -576,15 +576,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateQueryResponse):
+        if not isinstance(other, Query):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/create_sink_request.py` & `timeplus-1.2.1/swagger_client/models/create_sink_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/create_source_request.py` & `timeplus-1.2.1/swagger_client/models/create_source_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,68 +24,46 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'connection_config': 'ConnectionConfig',
         'description': 'str',
         'name': 'str',
         'properties': 'dict(str, object)',
+        'stream': 'str',
         'type': 'str'
     }
 
     attribute_map = {
-        'connection_config': 'connection_config',
         'description': 'description',
         'name': 'name',
         'properties': 'properties',
+        'stream': 'stream',
         'type': 'type'
     }
 
-    def __init__(self, connection_config=None, description=None, name=None, properties=None, type=None):  # noqa: E501
+    def __init__(self, description=None, name=None, properties=None, stream=None, type=None):  # noqa: E501
         """CreateSourceRequest - a model defined in Swagger"""  # noqa: E501
-        self._connection_config = None
         self._description = None
         self._name = None
         self._properties = None
+        self._stream = None
         self._type = None
         self.discriminator = None
-        if connection_config is not None:
-            self.connection_config = connection_config
         if description is not None:
             self.description = description
         self.name = name
         if properties is not None:
             self.properties = properties
+        self.stream = stream
         self.type = type
 
     @property
-    def connection_config(self):
-        """Gets the connection_config of this CreateSourceRequest.  # noqa: E501
-
-
-        :return: The connection_config of this CreateSourceRequest.  # noqa: E501
-        :rtype: ConnectionConfig
-        """
-        return self._connection_config
-
-    @connection_config.setter
-    def connection_config(self, connection_config):
-        """Sets the connection_config of this CreateSourceRequest.
-
-
-        :param connection_config: The connection_config of this CreateSourceRequest.  # noqa: E501
-        :type: ConnectionConfig
-        """
-
-        self._connection_config = connection_config
-
-    @property
     def description(self):
         """Gets the description of this CreateSourceRequest.  # noqa: E501
 
 
         :return: The description of this CreateSourceRequest.  # noqa: E501
         :rtype: str
         """
@@ -102,68 +80,99 @@
 
         self._description = description
 
     @property
     def name(self):
         """Gets the name of this CreateSourceRequest.  # noqa: E501
 
+        Source name should only contain a maximum of 64 letters, numbers, or _, and start with a letter  # noqa: E501
 
         :return: The name of this CreateSourceRequest.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this CreateSourceRequest.
 
+        Source name should only contain a maximum of 64 letters, numbers, or _, and start with a letter  # noqa: E501
 
         :param name: The name of this CreateSourceRequest.  # noqa: E501
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def properties(self):
         """Gets the properties of this CreateSourceRequest.  # noqa: E501
 
+        Additional properties that required to read the data from source. Please refer to the documentation for this source type  # noqa: E501
 
         :return: The properties of this CreateSourceRequest.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._properties
 
     @properties.setter
     def properties(self, properties):
         """Sets the properties of this CreateSourceRequest.
 
+        Additional properties that required to read the data from source. Please refer to the documentation for this source type  # noqa: E501
 
         :param properties: The properties of this CreateSourceRequest.  # noqa: E501
         :type: dict(str, object)
         """
 
         self._properties = properties
 
     @property
+    def stream(self):
+        """Gets the stream of this CreateSourceRequest.  # noqa: E501
+
+        The name of the target stream that this source writes to. The stream needs to be created first.  # noqa: E501
+
+        :return: The stream of this CreateSourceRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._stream
+
+    @stream.setter
+    def stream(self, stream):
+        """Sets the stream of this CreateSourceRequest.
+
+        The name of the target stream that this source writes to. The stream needs to be created first.  # noqa: E501
+
+        :param stream: The stream of this CreateSourceRequest.  # noqa: E501
+        :type: str
+        """
+        if stream is None:
+            raise ValueError("Invalid value for `stream`, must not be `None`")  # noqa: E501
+
+        self._stream = stream
+
+    @property
     def type(self):
         """Gets the type of this CreateSourceRequest.  # noqa: E501
 
+        Type of the source  # noqa: E501
 
         :return: The type of this CreateSourceRequest.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this CreateSourceRequest.
 
+        Type of the source  # noqa: E501
 
         :param type: The type of this CreateSourceRequest.  # noqa: E501
         :type: str
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
```

### Comparing `timeplus-1.1.2/swagger_client/models/dashboard_dashboard.py` & `timeplus-1.2.1/swagger_client/models/dashboard_dashboard.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/dashboard_panel.py` & `timeplus-1.2.1/swagger_client/models/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/edge.py` & `timeplus-1.2.1/swagger_client/models/edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/error_response.py` & `timeplus-1.2.1/swagger_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/event.py` & `timeplus-1.2.1/swagger_client/models/event.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/event_infer_request.py` & `timeplus-1.2.1/swagger_client/models/event_infer_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/event_infer_response.py` & `timeplus-1.2.1/swagger_client/models/event_infer_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/external_stream_def.py` & `timeplus-1.2.1/swagger_client/models/external_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/file_upload_response.py` & `timeplus-1.2.1/swagger_client/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/format_query_request.py` & `timeplus-1.2.1/swagger_client/models/format_query_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/format_query_response.py` & `timeplus-1.2.1/swagger_client/models/format_query_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/global_metrics_result.py` & `timeplus-1.2.1/swagger_client/models/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,113 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GlobalMetricsResult(object):
+class Graph(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'name': 'str',
-        'time': 'str',
-        'value': 'float'
+        'edges': 'list[Edge]',
+        'nodes': 'list[Node]'
     }
 
     attribute_map = {
-        'name': 'name',
-        'time': 'time',
-        'value': 'value'
+        'edges': 'edges',
+        'nodes': 'nodes'
     }
 
-    def __init__(self, name=None, time=None, value=None):  # noqa: E501
-        """GlobalMetricsResult - a model defined in Swagger"""  # noqa: E501
-        self._name = None
-        self._time = None
-        self._value = None
+    def __init__(self, edges=None, nodes=None):  # noqa: E501
+        """Graph - a model defined in Swagger"""  # noqa: E501
+        self._edges = None
+        self._nodes = None
         self.discriminator = None
-        if name is not None:
-            self.name = name
-        if time is not None:
-            self.time = time
-        if value is not None:
-            self.value = value
+        if edges is not None:
+            self.edges = edges
+        if nodes is not None:
+            self.nodes = nodes
 
     @property
-    def name(self):
-        """Gets the name of this GlobalMetricsResult.  # noqa: E501
+    def edges(self):
+        """Gets the edges of this Graph.  # noqa: E501
 
 
-        :return: The name of this GlobalMetricsResult.  # noqa: E501
-        :rtype: str
+        :return: The edges of this Graph.  # noqa: E501
+        :rtype: list[Edge]
         """
-        return self._name
+        return self._edges
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this GlobalMetricsResult.
+    @edges.setter
+    def edges(self, edges):
+        """Sets the edges of this Graph.
 
 
-        :param name: The name of this GlobalMetricsResult.  # noqa: E501
-        :type: str
+        :param edges: The edges of this Graph.  # noqa: E501
+        :type: list[Edge]
         """
 
-        self._name = name
+        self._edges = edges
 
     @property
-    def time(self):
-        """Gets the time of this GlobalMetricsResult.  # noqa: E501
+    def nodes(self):
+        """Gets the nodes of this Graph.  # noqa: E501
 
 
-        :return: The time of this GlobalMetricsResult.  # noqa: E501
-        :rtype: str
+        :return: The nodes of this Graph.  # noqa: E501
+        :rtype: list[Node]
         """
-        return self._time
+        return self._nodes
 
-    @time.setter
-    def time(self, time):
-        """Sets the time of this GlobalMetricsResult.
+    @nodes.setter
+    def nodes(self, nodes):
+        """Sets the nodes of this Graph.
 
 
-        :param time: The time of this GlobalMetricsResult.  # noqa: E501
-        :type: str
+        :param nodes: The nodes of this Graph.  # noqa: E501
+        :type: list[Node]
         """
 
-        self._time = time
-
-    @property
-    def value(self):
-        """Gets the value of this GlobalMetricsResult.  # noqa: E501
-
-
-        :return: The value of this GlobalMetricsResult.  # noqa: E501
-        :rtype: float
-        """
-        return self._value
-
-    @value.setter
-    def value(self, value):
-        """Sets the value of this GlobalMetricsResult.
-
-
-        :param value: The value of this GlobalMetricsResult.  # noqa: E501
-        :type: float
-        """
-
-        self._value = value
+        self._nodes = nodes
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GlobalMetricsResult, dict):
+        if issubclass(Graph, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GlobalMetricsResult):
+        if not isinstance(other, Graph):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/graph.py` & `timeplus-1.2.1/swagger_client/models/query_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,87 +11,88 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Graph(object):
+class QueryResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'edges': 'list[Edge]',
-        'nodes': 'list[Node]'
+        'data': 'list[list[object]]',
+        'header': 'list[Column]'
     }
 
     attribute_map = {
-        'edges': 'edges',
-        'nodes': 'nodes'
+        'data': 'data',
+        'header': 'header'
     }
 
-    def __init__(self, edges=None, nodes=None):  # noqa: E501
-        """Graph - a model defined in Swagger"""  # noqa: E501
-        self._edges = None
-        self._nodes = None
+    def __init__(self, data=None, header=None):  # noqa: E501
+        """QueryResult - a model defined in Swagger"""  # noqa: E501
+        self._data = None
+        self._header = None
         self.discriminator = None
-        if edges is not None:
-            self.edges = edges
-        if nodes is not None:
-            self.nodes = nodes
+        if data is not None:
+            self.data = data
+        self.header = header
 
     @property
-    def edges(self):
-        """Gets the edges of this Graph.  # noqa: E501
+    def data(self):
+        """Gets the data of this QueryResult.  # noqa: E501
 
 
-        :return: The edges of this Graph.  # noqa: E501
-        :rtype: list[Edge]
+        :return: The data of this QueryResult.  # noqa: E501
+        :rtype: list[list[object]]
         """
-        return self._edges
+        return self._data
 
-    @edges.setter
-    def edges(self, edges):
-        """Sets the edges of this Graph.
+    @data.setter
+    def data(self, data):
+        """Sets the data of this QueryResult.
 
 
-        :param edges: The edges of this Graph.  # noqa: E501
-        :type: list[Edge]
+        :param data: The data of this QueryResult.  # noqa: E501
+        :type: list[list[object]]
         """
 
-        self._edges = edges
+        self._data = data
 
     @property
-    def nodes(self):
-        """Gets the nodes of this Graph.  # noqa: E501
+    def header(self):
+        """Gets the header of this QueryResult.  # noqa: E501
 
 
-        :return: The nodes of this Graph.  # noqa: E501
-        :rtype: list[Node]
+        :return: The header of this QueryResult.  # noqa: E501
+        :rtype: list[Column]
         """
-        return self._nodes
+        return self._header
 
-    @nodes.setter
-    def nodes(self, nodes):
-        """Sets the nodes of this Graph.
+    @header.setter
+    def header(self, header):
+        """Sets the header of this QueryResult.
 
 
-        :param nodes: The nodes of this Graph.  # noqa: E501
-        :type: list[Node]
+        :param header: The header of this QueryResult.  # noqa: E501
+        :type: list[Column]
         """
+        if header is None:
+            raise ValueError("Invalid value for `header`, must not be `None`")  # noqa: E501
 
-        self._nodes = nodes
+        self._header = header
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +107,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Graph, dict):
+        if issubclass(QueryResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +123,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Graph):
+        if not isinstance(other, QueryResult):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/ingest_data.py` & `timeplus-1.2.1/swagger_client/models/ingest_data.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/latency.py` & `timeplus-1.2.1/swagger_client/models/resource_metrics_result.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,175 +1,153 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Latency(object):
+class ResourceMetricsResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'avg': 'float',
-        'latest': 'list[float]',
-        'max': 'float',
-        'min': 'float',
-        'sum': 'float'
+        'failure_count': 'float',
+        'id': 'str',
+        'success_count': 'float',
+        'throughput': 'list[MetricsQueryThroughput]'
     }
 
     attribute_map = {
-        'avg': 'avg',
-        'latest': 'latest',
-        'max': 'max',
-        'min': 'min',
-        'sum': 'sum'
+        'failure_count': 'failure_count',
+        'id': 'id',
+        'success_count': 'success_count',
+        'throughput': 'throughput'
     }
 
-    def __init__(self, avg=None, latest=None, max=None, min=None, sum=None):  # noqa: E501
-        """Latency - a model defined in Swagger"""  # noqa: E501
-        self._avg = None
-        self._latest = None
-        self._max = None
-        self._min = None
-        self._sum = None
+    def __init__(self, failure_count=None, id=None, success_count=None, throughput=None):  # noqa: E501
+        """ResourceMetricsResult - a model defined in Swagger"""  # noqa: E501
+        self._failure_count = None
+        self._id = None
+        self._success_count = None
+        self._throughput = None
         self.discriminator = None
-        if avg is not None:
-            self.avg = avg
-        if latest is not None:
-            self.latest = latest
-        if max is not None:
-            self.max = max
-        if min is not None:
-            self.min = min
-        if sum is not None:
-            self.sum = sum
+        self.failure_count = failure_count
+        self.id = id
+        self.success_count = success_count
+        self.throughput = throughput
 
     @property
-    def avg(self):
-        """Gets the avg of this Latency.  # noqa: E501
+    def failure_count(self):
+        """Gets the failure_count of this ResourceMetricsResult.  # noqa: E501
 
 
-        :return: The avg of this Latency.  # noqa: E501
+        :return: The failure_count of this ResourceMetricsResult.  # noqa: E501
         :rtype: float
         """
-        return self._avg
+        return self._failure_count
 
-    @avg.setter
-    def avg(self, avg):
-        """Sets the avg of this Latency.
+    @failure_count.setter
+    def failure_count(self, failure_count):
+        """Sets the failure_count of this ResourceMetricsResult.
 
 
-        :param avg: The avg of this Latency.  # noqa: E501
+        :param failure_count: The failure_count of this ResourceMetricsResult.  # noqa: E501
         :type: float
         """
+        if failure_count is None:
+            raise ValueError("Invalid value for `failure_count`, must not be `None`")  # noqa: E501
 
-        self._avg = avg
+        self._failure_count = failure_count
 
     @property
-    def latest(self):
-        """Gets the latest of this Latency.  # noqa: E501
+    def id(self):
+        """Gets the id of this ResourceMetricsResult.  # noqa: E501
 
 
-        :return: The latest of this Latency.  # noqa: E501
-        :rtype: list[float]
+        :return: The id of this ResourceMetricsResult.  # noqa: E501
+        :rtype: str
         """
-        return self._latest
+        return self._id
 
-    @latest.setter
-    def latest(self, latest):
-        """Sets the latest of this Latency.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this ResourceMetricsResult.
 
 
-        :param latest: The latest of this Latency.  # noqa: E501
-        :type: list[float]
+        :param id: The id of this ResourceMetricsResult.  # noqa: E501
+        :type: str
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._latest = latest
+        self._id = id
 
     @property
-    def max(self):
-        """Gets the max of this Latency.  # noqa: E501
+    def success_count(self):
+        """Gets the success_count of this ResourceMetricsResult.  # noqa: E501
 
 
-        :return: The max of this Latency.  # noqa: E501
+        :return: The success_count of this ResourceMetricsResult.  # noqa: E501
         :rtype: float
         """
-        return self._max
+        return self._success_count
 
-    @max.setter
-    def max(self, max):
-        """Sets the max of this Latency.
+    @success_count.setter
+    def success_count(self, success_count):
+        """Sets the success_count of this ResourceMetricsResult.
 
 
-        :param max: The max of this Latency.  # noqa: E501
+        :param success_count: The success_count of this ResourceMetricsResult.  # noqa: E501
         :type: float
         """
+        if success_count is None:
+            raise ValueError("Invalid value for `success_count`, must not be `None`")  # noqa: E501
 
-        self._max = max
+        self._success_count = success_count
 
     @property
-    def min(self):
-        """Gets the min of this Latency.  # noqa: E501
+    def throughput(self):
+        """Gets the throughput of this ResourceMetricsResult.  # noqa: E501
 
 
-        :return: The min of this Latency.  # noqa: E501
-        :rtype: float
-        """
-        return self._min
-
-    @min.setter
-    def min(self, min):
-        """Sets the min of this Latency.
-
-
-        :param min: The min of this Latency.  # noqa: E501
-        :type: float
-        """
-
-        self._min = min
-
-    @property
-    def sum(self):
-        """Gets the sum of this Latency.  # noqa: E501
-
-
-        :return: The sum of this Latency.  # noqa: E501
-        :rtype: float
+        :return: The throughput of this ResourceMetricsResult.  # noqa: E501
+        :rtype: list[MetricsQueryThroughput]
         """
-        return self._sum
+        return self._throughput
 
-    @sum.setter
-    def sum(self, sum):
-        """Sets the sum of this Latency.
+    @throughput.setter
+    def throughput(self, throughput):
+        """Sets the throughput of this ResourceMetricsResult.
 
 
-        :param sum: The sum of this Latency.  # noqa: E501
-        :type: float
+        :param throughput: The throughput of this ResourceMetricsResult.  # noqa: E501
+        :type: list[MetricsQueryThroughput]
         """
+        if throughput is None:
+            raise ValueError("Invalid value for `throughput`, must not be `None`")  # noqa: E501
 
-        self._sum = sum
+        self._throughput = throughput
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -184,15 +162,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Latency, dict):
+        if issubclass(ResourceMetricsResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -200,15 +178,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Latency):
+        if not isinstance(other, ResourceMetricsResult):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/node.py` & `timeplus-1.2.1/swagger_client/models/node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/owner.py` & `timeplus-1.2.1/swagger_client/models/owner.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/query.py` & `timeplus-1.2.1/swagger_client/models/udf.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,541 +11,409 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Query(object):
+class UDF(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'analysis': 'SQLAnalyzeResult',
+        'arguments': 'list[UDFArgument]',
+        'auth_context': 'UDFAuthContext',
+        'auth_method': 'str',
         'created_at': 'str',
         'created_by': 'Owner',
         'description': 'str',
-        'duration': 'int',
-        'end_time': 'int',
-        'id': 'str',
+        'is_aggregation': 'bool',
         'last_updated_at': 'str',
         'last_updated_by': 'Owner',
-        'message': 'str',
         'name': 'str',
-        'response_time': 'int',
-        'result': 'QueryResult',
-        'sinks': 'dict(str, SinkStat)',
-        'sql': 'str',
-        'start_time': 'int',
-        'status': 'str',
-        'tags': 'list[str]',
-        'time_columns': 'TimeColumns'
+        'return_type': 'str',
+        'source': 'str',
+        'type': 'str',
+        'url': 'str'
     }
 
     attribute_map = {
-        'analysis': 'analysis',
+        'arguments': 'arguments',
+        'auth_context': 'auth_context',
+        'auth_method': 'auth_method',
         'created_at': 'created_at',
         'created_by': 'created_by',
         'description': 'description',
-        'duration': 'duration',
-        'end_time': 'end_time',
-        'id': 'id',
+        'is_aggregation': 'is_aggregation',
         'last_updated_at': 'last_updated_at',
         'last_updated_by': 'last_updated_by',
-        'message': 'message',
         'name': 'name',
-        'response_time': 'response_time',
-        'result': 'result',
-        'sinks': 'sinks',
-        'sql': 'sql',
-        'start_time': 'start_time',
-        'status': 'status',
-        'tags': 'tags',
-        'time_columns': 'timeColumns'
+        'return_type': 'return_type',
+        'source': 'source',
+        'type': 'type',
+        'url': 'url'
     }
 
-    def __init__(self, analysis=None, created_at=None, created_by=None, description=None, duration=None, end_time=None, id=None, last_updated_at=None, last_updated_by=None, message=None, name=None, response_time=None, result=None, sinks=None, sql=None, start_time=None, status=None, tags=None, time_columns=None):  # noqa: E501
-        """Query - a model defined in Swagger"""  # noqa: E501
-        self._analysis = None
+    def __init__(self, arguments=None, auth_context=None, auth_method=None, created_at=None, created_by=None, description=None, is_aggregation=None, last_updated_at=None, last_updated_by=None, name=None, return_type=None, source=None, type=None, url=None):  # noqa: E501
+        """UDF - a model defined in Swagger"""  # noqa: E501
+        self._arguments = None
+        self._auth_context = None
+        self._auth_method = None
         self._created_at = None
         self._created_by = None
         self._description = None
-        self._duration = None
-        self._end_time = None
-        self._id = None
+        self._is_aggregation = None
         self._last_updated_at = None
         self._last_updated_by = None
-        self._message = None
         self._name = None
-        self._response_time = None
-        self._result = None
-        self._sinks = None
-        self._sql = None
-        self._start_time = None
-        self._status = None
-        self._tags = None
-        self._time_columns = None
+        self._return_type = None
+        self._source = None
+        self._type = None
+        self._url = None
         self.discriminator = None
-        self.analysis = analysis
+        if arguments is not None:
+            self.arguments = arguments
+        if auth_context is not None:
+            self.auth_context = auth_context
+        if auth_method is not None:
+            self.auth_method = auth_method
         if created_at is not None:
             self.created_at = created_at
         if created_by is not None:
             self.created_by = created_by
         if description is not None:
             self.description = description
-        self.duration = duration
-        self.end_time = end_time
-        self.id = id
+        if is_aggregation is not None:
+            self.is_aggregation = is_aggregation
         if last_updated_at is not None:
             self.last_updated_at = last_updated_at
         if last_updated_by is not None:
             self.last_updated_by = last_updated_by
-        self.message = message
         if name is not None:
             self.name = name
-        self.response_time = response_time
-        self.result = result
-        self.sinks = sinks
-        self.sql = sql
-        self.start_time = start_time
-        self.status = status
-        if tags is not None:
-            self.tags = tags
-        self.time_columns = time_columns
+        if return_type is not None:
+            self.return_type = return_type
+        if source is not None:
+            self.source = source
+        if type is not None:
+            self.type = type
+        if url is not None:
+            self.url = url
 
     @property
-    def analysis(self):
-        """Gets the analysis of this Query.  # noqa: E501
+    def arguments(self):
+        """Gets the arguments of this UDF.  # noqa: E501
 
+        The input argument of the UDF   * For UDA: the number and type of arguments should be consistent with the main function of UDA.     the type should be the data types of proton not javascript types. It only supports int8/16/32/64, uint8/16/32/64,  # noqa: E501
 
-        :return: The analysis of this Query.  # noqa: E501
-        :rtype: SQLAnalyzeResult
+        :return: The arguments of this UDF.  # noqa: E501
+        :rtype: list[UDFArgument]
         """
-        return self._analysis
+        return self._arguments
 
-    @analysis.setter
-    def analysis(self, analysis):
-        """Sets the analysis of this Query.
+    @arguments.setter
+    def arguments(self, arguments):
+        """Sets the arguments of this UDF.
 
+        The input argument of the UDF   * For UDA: the number and type of arguments should be consistent with the main function of UDA.     the type should be the data types of proton not javascript types. It only supports int8/16/32/64, uint8/16/32/64,  # noqa: E501
 
-        :param analysis: The analysis of this Query.  # noqa: E501
-        :type: SQLAnalyzeResult
+        :param arguments: The arguments of this UDF.  # noqa: E501
+        :type: list[UDFArgument]
         """
-        if analysis is None:
-            raise ValueError("Invalid value for `analysis`, must not be `None`")  # noqa: E501
 
-        self._analysis = analysis
+        self._arguments = arguments
 
     @property
-    def created_at(self):
-        """Gets the created_at of this Query.  # noqa: E501
+    def auth_context(self):
+        """Gets the auth_context of this UDF.  # noqa: E501
 
 
-        :return: The created_at of this Query.  # noqa: E501
-        :rtype: str
+        :return: The auth_context of this UDF.  # noqa: E501
+        :rtype: UDFAuthContext
         """
-        return self._created_at
+        return self._auth_context
 
-    @created_at.setter
-    def created_at(self, created_at):
-        """Sets the created_at of this Query.
+    @auth_context.setter
+    def auth_context(self, auth_context):
+        """Sets the auth_context of this UDF.
 
 
-        :param created_at: The created_at of this Query.  # noqa: E501
-        :type: str
+        :param auth_context: The auth_context of this UDF.  # noqa: E501
+        :type: UDFAuthContext
         """
 
-        self._created_at = created_at
+        self._auth_context = auth_context
 
     @property
-    def created_by(self):
-        """Gets the created_by of this Query.  # noqa: E501
+    def auth_method(self):
+        """Gets the auth_method of this UDF.  # noqa: E501
 
 
-        :return: The created_by of this Query.  # noqa: E501
-        :rtype: Owner
+        :return: The auth_method of this UDF.  # noqa: E501
+        :rtype: str
         """
-        return self._created_by
+        return self._auth_method
 
-    @created_by.setter
-    def created_by(self, created_by):
-        """Sets the created_by of this Query.
+    @auth_method.setter
+    def auth_method(self, auth_method):
+        """Sets the auth_method of this UDF.
 
 
-        :param created_by: The created_by of this Query.  # noqa: E501
-        :type: Owner
+        :param auth_method: The auth_method of this UDF.  # noqa: E501
+        :type: str
         """
 
-        self._created_by = created_by
+        self._auth_method = auth_method
 
     @property
-    def description(self):
-        """Gets the description of this Query.  # noqa: E501
+    def created_at(self):
+        """Gets the created_at of this UDF.  # noqa: E501
 
 
-        :return: The description of this Query.  # noqa: E501
+        :return: The created_at of this UDF.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._created_at
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this Query.
+    @created_at.setter
+    def created_at(self, created_at):
+        """Sets the created_at of this UDF.
 
 
-        :param description: The description of this Query.  # noqa: E501
+        :param created_at: The created_at of this UDF.  # noqa: E501
         :type: str
         """
 
-        self._description = description
+        self._created_at = created_at
 
     @property
-    def duration(self):
-        """Gets the duration of this Query.  # noqa: E501
+    def created_by(self):
+        """Gets the created_by of this UDF.  # noqa: E501
 
 
-        :return: The duration of this Query.  # noqa: E501
-        :rtype: int
+        :return: The created_by of this UDF.  # noqa: E501
+        :rtype: Owner
         """
-        return self._duration
+        return self._created_by
 
-    @duration.setter
-    def duration(self, duration):
-        """Sets the duration of this Query.
+    @created_by.setter
+    def created_by(self, created_by):
+        """Sets the created_by of this UDF.
 
 
-        :param duration: The duration of this Query.  # noqa: E501
-        :type: int
+        :param created_by: The created_by of this UDF.  # noqa: E501
+        :type: Owner
         """
-        if duration is None:
-            raise ValueError("Invalid value for `duration`, must not be `None`")  # noqa: E501
 
-        self._duration = duration
+        self._created_by = created_by
 
     @property
-    def end_time(self):
-        """Gets the end_time of this Query.  # noqa: E501
+    def description(self):
+        """Gets the description of this UDF.  # noqa: E501
 
 
-        :return: The end_time of this Query.  # noqa: E501
-        :rtype: int
+        :return: The description of this UDF.  # noqa: E501
+        :rtype: str
         """
-        return self._end_time
+        return self._description
 
-    @end_time.setter
-    def end_time(self, end_time):
-        """Sets the end_time of this Query.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this UDF.
 
 
-        :param end_time: The end_time of this Query.  # noqa: E501
-        :type: int
+        :param description: The description of this UDF.  # noqa: E501
+        :type: str
         """
-        if end_time is None:
-            raise ValueError("Invalid value for `end_time`, must not be `None`")  # noqa: E501
 
-        self._end_time = end_time
+        self._description = description
 
     @property
-    def id(self):
-        """Gets the id of this Query.  # noqa: E501
+    def is_aggregation(self):
+        """Gets the is_aggregation of this UDF.  # noqa: E501
 
+        Whether it is an aggregation function. Only valid when type is 'javascript'  # noqa: E501
 
-        :return: The id of this Query.  # noqa: E501
-        :rtype: str
+        :return: The is_aggregation of this UDF.  # noqa: E501
+        :rtype: bool
         """
-        return self._id
+        return self._is_aggregation
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this Query.
+    @is_aggregation.setter
+    def is_aggregation(self, is_aggregation):
+        """Sets the is_aggregation of this UDF.
 
+        Whether it is an aggregation function. Only valid when type is 'javascript'  # noqa: E501
 
-        :param id: The id of this Query.  # noqa: E501
-        :type: str
+        :param is_aggregation: The is_aggregation of this UDF.  # noqa: E501
+        :type: bool
         """
-        if id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._id = id
+        self._is_aggregation = is_aggregation
 
     @property
     def last_updated_at(self):
-        """Gets the last_updated_at of this Query.  # noqa: E501
+        """Gets the last_updated_at of this UDF.  # noqa: E501
 
 
-        :return: The last_updated_at of this Query.  # noqa: E501
+        :return: The last_updated_at of this UDF.  # noqa: E501
         :rtype: str
         """
         return self._last_updated_at
 
     @last_updated_at.setter
     def last_updated_at(self, last_updated_at):
-        """Sets the last_updated_at of this Query.
+        """Sets the last_updated_at of this UDF.
 
 
-        :param last_updated_at: The last_updated_at of this Query.  # noqa: E501
+        :param last_updated_at: The last_updated_at of this UDF.  # noqa: E501
         :type: str
         """
 
         self._last_updated_at = last_updated_at
 
     @property
     def last_updated_by(self):
-        """Gets the last_updated_by of this Query.  # noqa: E501
+        """Gets the last_updated_by of this UDF.  # noqa: E501
 
 
-        :return: The last_updated_by of this Query.  # noqa: E501
+        :return: The last_updated_by of this UDF.  # noqa: E501
         :rtype: Owner
         """
         return self._last_updated_by
 
     @last_updated_by.setter
     def last_updated_by(self, last_updated_by):
-        """Sets the last_updated_by of this Query.
+        """Sets the last_updated_by of this UDF.
 
 
-        :param last_updated_by: The last_updated_by of this Query.  # noqa: E501
+        :param last_updated_by: The last_updated_by of this UDF.  # noqa: E501
         :type: Owner
         """
 
         self._last_updated_by = last_updated_by
 
     @property
-    def message(self):
-        """Gets the message of this Query.  # noqa: E501
-
-
-        :return: The message of this Query.  # noqa: E501
-        :rtype: str
-        """
-        return self._message
-
-    @message.setter
-    def message(self, message):
-        """Sets the message of this Query.
-
-
-        :param message: The message of this Query.  # noqa: E501
-        :type: str
-        """
-        if message is None:
-            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
-
-        self._message = message
-
-    @property
     def name(self):
-        """Gets the name of this Query.  # noqa: E501
+        """Gets the name of this UDF.  # noqa: E501
 
 
-        :return: The name of this Query.  # noqa: E501
+        :return: The name of this UDF.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this Query.
+        """Sets the name of this UDF.
 
 
-        :param name: The name of this Query.  # noqa: E501
+        :param name: The name of this UDF.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
-    def response_time(self):
-        """Gets the response_time of this Query.  # noqa: E501
-
-
-        :return: The response_time of this Query.  # noqa: E501
-        :rtype: int
-        """
-        return self._response_time
-
-    @response_time.setter
-    def response_time(self, response_time):
-        """Sets the response_time of this Query.
-
-
-        :param response_time: The response_time of this Query.  # noqa: E501
-        :type: int
-        """
-        if response_time is None:
-            raise ValueError("Invalid value for `response_time`, must not be `None`")  # noqa: E501
-
-        self._response_time = response_time
-
-    @property
-    def result(self):
-        """Gets the result of this Query.  # noqa: E501
-
-
-        :return: The result of this Query.  # noqa: E501
-        :rtype: QueryResult
-        """
-        return self._result
-
-    @result.setter
-    def result(self, result):
-        """Sets the result of this Query.
-
-
-        :param result: The result of this Query.  # noqa: E501
-        :type: QueryResult
-        """
-        if result is None:
-            raise ValueError("Invalid value for `result`, must not be `None`")  # noqa: E501
-
-        self._result = result
-
-    @property
-    def sinks(self):
-        """Gets the sinks of this Query.  # noqa: E501
+    def return_type(self):
+        """Gets the return_type of this UDF.  # noqa: E501
 
+        The erturn type of the UDF   * For UDA: if it returns a single value, the return type is the corresponding data type of Timeplus.     It supports the same types of input arguments, except for datetime, it only supports DateTime64(3).  # noqa: E501
 
-        :return: The sinks of this Query.  # noqa: E501
-        :rtype: dict(str, SinkStat)
-        """
-        return self._sinks
-
-    @sinks.setter
-    def sinks(self, sinks):
-        """Sets the sinks of this Query.
-
-
-        :param sinks: The sinks of this Query.  # noqa: E501
-        :type: dict(str, SinkStat)
-        """
-        if sinks is None:
-            raise ValueError("Invalid value for `sinks`, must not be `None`")  # noqa: E501
-
-        self._sinks = sinks
-
-    @property
-    def sql(self):
-        """Gets the sql of this Query.  # noqa: E501
-
-
-        :return: The sql of this Query.  # noqa: E501
+        :return: The return_type of this UDF.  # noqa: E501
         :rtype: str
         """
-        return self._sql
+        return self._return_type
 
-    @sql.setter
-    def sql(self, sql):
-        """Sets the sql of this Query.
+    @return_type.setter
+    def return_type(self, return_type):
+        """Sets the return_type of this UDF.
 
+        The erturn type of the UDF   * For UDA: if it returns a single value, the return type is the corresponding data type of Timeplus.     It supports the same types of input arguments, except for datetime, it only supports DateTime64(3).  # noqa: E501
 
-        :param sql: The sql of this Query.  # noqa: E501
+        :param return_type: The return_type of this UDF.  # noqa: E501
         :type: str
         """
-        if sql is None:
-            raise ValueError("Invalid value for `sql`, must not be `None`")  # noqa: E501
-
-        self._sql = sql
-
-    @property
-    def start_time(self):
-        """Gets the start_time of this Query.  # noqa: E501
-
-
-        :return: The start_time of this Query.  # noqa: E501
-        :rtype: int
-        """
-        return self._start_time
-
-    @start_time.setter
-    def start_time(self, start_time):
-        """Sets the start_time of this Query.
-
-
-        :param start_time: The start_time of this Query.  # noqa: E501
-        :type: int
-        """
-        if start_time is None:
-            raise ValueError("Invalid value for `start_time`, must not be `None`")  # noqa: E501
 
-        self._start_time = start_time
+        self._return_type = return_type
 
     @property
-    def status(self):
-        """Gets the status of this Query.  # noqa: E501
+    def source(self):
+        """Gets the source of this UDF.  # noqa: E501
 
+        The source code of the UDA. There are functions to be defined:  * main function: with the same name as UDA. Timeplus calls this function for each input row. The main function can return two types of result: object or simple data type    - If it returns an object, the object is like {“emit”: true, “result”: …}. ‘Emit’ (boolean) property tells Timeplus whether or not the result should emit. ‘result’ is the current aggregate result, if ‘emit’ is false, the result will be ignored by Timeplus. Timeplus will convert the ‘result’ property of v8 to the data types defined when creating UDA.    - If it returns a simple data type, Timeplus considers the return data as the result to be emitted immediately. It converts the return data to the corresponding data type and Timeplus emits the aggregating result.    - Once UDA tells Timeplus to emit the data, UDA takes the full responsibility to clear the internal state, prepare and restart a new aggregating window, et al.  * state function: which returns the serialized state of all internal states of UDA in string. The UDA takes the responsibility therefore Timeplus can choose to persist the internal state of UDA for query recovery.  * init function: the input of this function is the string of serialized state of the internal states UDA. Timeplus calls this function when it wants to recover the aggregation function with the persisted internal state.  # noqa: E501
 
-        :return: The status of this Query.  # noqa: E501
+        :return: The source of this UDF.  # noqa: E501
         :rtype: str
         """
-        return self._status
+        return self._source
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this Query.
+    @source.setter
+    def source(self, source):
+        """Sets the source of this UDF.
 
+        The source code of the UDA. There are functions to be defined:  * main function: with the same name as UDA. Timeplus calls this function for each input row. The main function can return two types of result: object or simple data type    - If it returns an object, the object is like {“emit”: true, “result”: …}. ‘Emit’ (boolean) property tells Timeplus whether or not the result should emit. ‘result’ is the current aggregate result, if ‘emit’ is false, the result will be ignored by Timeplus. Timeplus will convert the ‘result’ property of v8 to the data types defined when creating UDA.    - If it returns a simple data type, Timeplus considers the return data as the result to be emitted immediately. It converts the return data to the corresponding data type and Timeplus emits the aggregating result.    - Once UDA tells Timeplus to emit the data, UDA takes the full responsibility to clear the internal state, prepare and restart a new aggregating window, et al.  * state function: which returns the serialized state of all internal states of UDA in string. The UDA takes the responsibility therefore Timeplus can choose to persist the internal state of UDA for query recovery.  * init function: the input of this function is the string of serialized state of the internal states UDA. Timeplus calls this function when it wants to recover the aggregation function with the persisted internal state.  # noqa: E501
 
-        :param status: The status of this Query.  # noqa: E501
+        :param source: The source of this UDF.  # noqa: E501
         :type: str
         """
-        if status is None:
-            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
-        self._status = status
+        self._source = source
 
     @property
-    def tags(self):
-        """Gets the tags of this Query.  # noqa: E501
+    def type(self):
+        """Gets the type of this UDF.  # noqa: E501
 
+        Either `javascript` or `remote`  # noqa: E501
 
-        :return: The tags of this Query.  # noqa: E501
-        :rtype: list[str]
+        :return: The type of this UDF.  # noqa: E501
+        :rtype: str
         """
-        return self._tags
+        return self._type
 
-    @tags.setter
-    def tags(self, tags):
-        """Sets the tags of this Query.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this UDF.
 
+        Either `javascript` or `remote`  # noqa: E501
 
-        :param tags: The tags of this Query.  # noqa: E501
-        :type: list[str]
+        :param type: The type of this UDF.  # noqa: E501
+        :type: str
         """
 
-        self._tags = tags
+        self._type = type
 
     @property
-    def time_columns(self):
-        """Gets the time_columns of this Query.  # noqa: E501
+    def url(self):
+        """Gets the url of this UDF.  # noqa: E501
 
 
-        :return: The time_columns of this Query.  # noqa: E501
-        :rtype: TimeColumns
+        :return: The url of this UDF.  # noqa: E501
+        :rtype: str
         """
-        return self._time_columns
+        return self._url
 
-    @time_columns.setter
-    def time_columns(self, time_columns):
-        """Sets the time_columns of this Query.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this UDF.
 
 
-        :param time_columns: The time_columns of this Query.  # noqa: E501
-        :type: TimeColumns
+        :param url: The url of this UDF.  # noqa: E501
+        :type: str
         """
-        if time_columns is None:
-            raise ValueError("Invalid value for `time_columns`, must not be `None`")  # noqa: E501
 
-        self._time_columns = time_columns
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -560,15 +428,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Query, dict):
+        if issubclass(UDF, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -576,15 +444,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Query):
+        if not isinstance(other, UDF):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timeplus-1.1.2/swagger_client/models/query_analysis.py` & `timeplus-1.2.1/swagger_client/models/source_preview_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,151 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class QueryAnalysis(object):
+class SourcePreviewRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'has_aggr': 'bool',
-        'has_subquery': 'bool',
-        'has_table_join': 'bool',
-        'has_union': 'bool',
-        'is_streaming': 'bool'
+        'properties': 'dict(str, object)',
+        'size': 'int',
+        'timeout': 'str',
+        'type': 'str'
     }
 
     attribute_map = {
-        'has_aggr': 'has_aggr',
-        'has_subquery': 'has_subquery',
-        'has_table_join': 'has_table_join',
-        'has_union': 'has_union',
-        'is_streaming': 'is_streaming'
+        'properties': 'properties',
+        'size': 'size',
+        'timeout': 'timeout',
+        'type': 'type'
     }
 
-    def __init__(self, has_aggr=None, has_subquery=None, has_table_join=None, has_union=None, is_streaming=None):  # noqa: E501
-        """QueryAnalysis - a model defined in Swagger"""  # noqa: E501
-        self._has_aggr = None
-        self._has_subquery = None
-        self._has_table_join = None
-        self._has_union = None
-        self._is_streaming = None
+    def __init__(self, properties=None, size=None, timeout=None, type=None):  # noqa: E501
+        """SourcePreviewRequest - a model defined in Swagger"""  # noqa: E501
+        self._properties = None
+        self._size = None
+        self._timeout = None
+        self._type = None
         self.discriminator = None
-        self.has_aggr = has_aggr
-        self.has_subquery = has_subquery
-        self.has_table_join = has_table_join
-        self.has_union = has_union
-        self.is_streaming = is_streaming
+        if properties is not None:
+            self.properties = properties
+        if size is not None:
+            self.size = size
+        if timeout is not None:
+            self.timeout = timeout
+        if type is not None:
+            self.type = type
 
     @property
-    def has_aggr(self):
-        """Gets the has_aggr of this QueryAnalysis.  # noqa: E501
+    def properties(self):
+        """Gets the properties of this SourcePreviewRequest.  # noqa: E501
 
 
-        :return: The has_aggr of this QueryAnalysis.  # noqa: E501
-        :rtype: bool
+        :return: The properties of this SourcePreviewRequest.  # noqa: E501
+        :rtype: dict(str, object)
         """
-        return self._has_aggr
+        return self._properties
 
-    @has_aggr.setter
-    def has_aggr(self, has_aggr):
-        """Sets the has_aggr of this QueryAnalysis.
+    @properties.setter
+    def properties(self, properties):
+        """Sets the properties of this SourcePreviewRequest.
 
 
-        :param has_aggr: The has_aggr of this QueryAnalysis.  # noqa: E501
-        :type: bool
+        :param properties: The properties of this SourcePreviewRequest.  # noqa: E501
+        :type: dict(str, object)
         """
-        if has_aggr is None:
-            raise ValueError("Invalid value for `has_aggr`, must not be `None`")  # noqa: E501
 
-        self._has_aggr = has_aggr
+        self._properties = properties
 
     @property
-    def has_subquery(self):
-        """Gets the has_subquery of this QueryAnalysis.  # noqa: E501
+    def size(self):
+        """Gets the size of this SourcePreviewRequest.  # noqa: E501
 
 
-        :return: The has_subquery of this QueryAnalysis.  # noqa: E501
-        :rtype: bool
+        :return: The size of this SourcePreviewRequest.  # noqa: E501
+        :rtype: int
         """
-        return self._has_subquery
+        return self._size
 
-    @has_subquery.setter
-    def has_subquery(self, has_subquery):
-        """Sets the has_subquery of this QueryAnalysis.
+    @size.setter
+    def size(self, size):
+        """Sets the size of this SourcePreviewRequest.
 
 
-        :param has_subquery: The has_subquery of this QueryAnalysis.  # noqa: E501
-        :type: bool
+        :param size: The size of this SourcePreviewRequest.  # noqa: E501
+        :type: int
         """
-        if has_subquery is None:
-            raise ValueError("Invalid value for `has_subquery`, must not be `None`")  # noqa: E501
 
-        self._has_subquery = has_subquery
+        self._size = size
 
     @property
-    def has_table_join(self):
-        """Gets the has_table_join of this QueryAnalysis.  # noqa: E501
+    def timeout(self):
+        """Gets the timeout of this SourcePreviewRequest.  # noqa: E501
 
+        Indicates how long should preview last to fetch the desired amount of data indicated by `size` A duration string is a possibly signed sequence of decimal numbers, each with optional fraction and a unit suffix, such as \"300ms\", \"-1.5h\" or \"2h45m\". Valid time units are \"ns\", \"us\" (or \"µs\"), \"ms\", \"s\", \"m\", \"h\".  # noqa: E501
 
-        :return: The has_table_join of this QueryAnalysis.  # noqa: E501
-        :rtype: bool
+        :return: The timeout of this SourcePreviewRequest.  # noqa: E501
+        :rtype: str
         """
-        return self._has_table_join
+        return self._timeout
 
-    @has_table_join.setter
-    def has_table_join(self, has_table_join):
-        """Sets the has_table_join of this QueryAnalysis.
+    @timeout.setter
+    def timeout(self, timeout):
+        """Sets the timeout of this SourcePreviewRequest.
 
+        Indicates how long should preview last to fetch the desired amount of data indicated by `size` A duration string is a possibly signed sequence of decimal numbers, each with optional fraction and a unit suffix, such as \"300ms\", \"-1.5h\" or \"2h45m\". Valid time units are \"ns\", \"us\" (or \"µs\"), \"ms\", \"s\", \"m\", \"h\".  # noqa: E501
 
-        :param has_table_join: The has_table_join of this QueryAnalysis.  # noqa: E501
-        :type: bool
+        :param timeout: The timeout of this SourcePreviewRequest.  # noqa: E501
+        :type: str
         """
-        if has_table_join is None:
-            raise ValueError("Invalid value for `has_table_join`, must not be `None`")  # noqa: E501
 
-        self._has_table_join = has_table_join
+        self._timeout = timeout
 
     @property
-    def has_union(self):
-        """Gets the has_union of this QueryAnalysis.  # noqa: E501
+    def type(self):
+        """Gets the type of this SourcePreviewRequest.  # noqa: E501
 
 
-        :return: The has_union of this QueryAnalysis.  # noqa: E501
-        :rtype: bool
+        :return: The type of this SourcePreviewRequest.  # noqa: E501
+        :rtype: str
         """
-        return self._has_union
+        return self._type
 
-    @has_union.setter
-    def has_union(self, has_union):
-        """Sets the has_union of this QueryAnalysis.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this SourcePreviewRequest.
 
 
-        :param has_union: The has_union of this QueryAnalysis.  # noqa: E501
-        :type: bool
+        :param type: The type of this SourcePreviewRequest.  # noqa: E501
+        :type: str
         """
-        if has_union is None:
-            raise ValueError("Invalid value for `has_union`, must not be `None`")  # noqa: E501
 
-        self._has_union = has_union
-
-    @property
-    def is_streaming(self):
-        """Gets the is_streaming of this QueryAnalysis.  # noqa: E501
-
-
-        :return: The is_streaming of this QueryAnalysis.  # noqa: E501
-        :rtype: bool
-        """
-        return self._is_streaming
-
-    @is_streaming.setter
-    def is_streaming(self, is_streaming):
-        """Sets the is_streaming of this QueryAnalysis.
-
-
-        :param is_streaming: The is_streaming of this QueryAnalysis.  # noqa: E501
-        :type: bool
-        """
-        if is_streaming is None:
-            raise ValueError("Invalid value for `is_streaming`, must not be `None`")  # noqa: E501
-
-        self._is_streaming = is_streaming
+        self._type = type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -189,15 +160,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(QueryAnalysis, dict):
+        if issubclass(SourcePreviewRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -205,15 +176,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QueryAnalysis):
+        if not isinstance(other, SourcePreviewRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timeplus-1.1.2/swagger_client/models/query_metrics.py` & `timeplus-1.2.1/swagger_client/models/query_pipeline_node.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,149 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class QueryMetrics(object):
+class QueryPipelineNode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'count': 'int',
-        'latency': 'Latency',
-        'throughput': 'Throughput'
+        'id': 'int',
+        'metric': 'QueryPipelineNodeMetric',
+        'name': 'str',
+        'status': 'str'
     }
 
     attribute_map = {
-        'count': 'count',
-        'latency': 'latency',
-        'throughput': 'throughput'
+        'id': 'id',
+        'metric': 'metric',
+        'name': 'name',
+        'status': 'status'
     }
 
-    def __init__(self, count=None, latency=None, throughput=None):  # noqa: E501
-        """QueryMetrics - a model defined in Swagger"""  # noqa: E501
-        self._count = None
-        self._latency = None
-        self._throughput = None
+    def __init__(self, id=None, metric=None, name=None, status=None):  # noqa: E501
+        """QueryPipelineNode - a model defined in Swagger"""  # noqa: E501
+        self._id = None
+        self._metric = None
+        self._name = None
+        self._status = None
         self.discriminator = None
-        if count is not None:
-            self.count = count
-        if latency is not None:
-            self.latency = latency
-        if throughput is not None:
-            self.throughput = throughput
+        if id is not None:
+            self.id = id
+        if metric is not None:
+            self.metric = metric
+        if name is not None:
+            self.name = name
+        if status is not None:
+            self.status = status
 
     @property
-    def count(self):
-        """Gets the count of this QueryMetrics.  # noqa: E501
+    def id(self):
+        """Gets the id of this QueryPipelineNode.  # noqa: E501
 
 
-        :return: The count of this QueryMetrics.  # noqa: E501
+        :return: The id of this QueryPipelineNode.  # noqa: E501
         :rtype: int
         """
-        return self._count
+        return self._id
 
-    @count.setter
-    def count(self, count):
-        """Sets the count of this QueryMetrics.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this QueryPipelineNode.
 
 
-        :param count: The count of this QueryMetrics.  # noqa: E501
+        :param id: The id of this QueryPipelineNode.  # noqa: E501
         :type: int
         """
 
-        self._count = count
+        self._id = id
 
     @property
-    def latency(self):
-        """Gets the latency of this QueryMetrics.  # noqa: E501
+    def metric(self):
+        """Gets the metric of this QueryPipelineNode.  # noqa: E501
 
 
-        :return: The latency of this QueryMetrics.  # noqa: E501
-        :rtype: Latency
+        :return: The metric of this QueryPipelineNode.  # noqa: E501
+        :rtype: QueryPipelineNodeMetric
         """
-        return self._latency
+        return self._metric
 
-    @latency.setter
-    def latency(self, latency):
-        """Sets the latency of this QueryMetrics.
+    @metric.setter
+    def metric(self, metric):
+        """Sets the metric of this QueryPipelineNode.
 
 
-        :param latency: The latency of this QueryMetrics.  # noqa: E501
-        :type: Latency
+        :param metric: The metric of this QueryPipelineNode.  # noqa: E501
+        :type: QueryPipelineNodeMetric
         """
 
-        self._latency = latency
+        self._metric = metric
 
     @property
-    def throughput(self):
-        """Gets the throughput of this QueryMetrics.  # noqa: E501
+    def name(self):
+        """Gets the name of this QueryPipelineNode.  # noqa: E501
 
 
-        :return: The throughput of this QueryMetrics.  # noqa: E501
-        :rtype: Throughput
+        :return: The name of this QueryPipelineNode.  # noqa: E501
+        :rtype: str
         """
-        return self._throughput
+        return self._name
 
-    @throughput.setter
-    def throughput(self, throughput):
-        """Sets the throughput of this QueryMetrics.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this QueryPipelineNode.
 
 
-        :param throughput: The throughput of this QueryMetrics.  # noqa: E501
-        :type: Throughput
+        :param name: The name of this QueryPipelineNode.  # noqa: E501
+        :type: str
         """
 
-        self._throughput = throughput
+        self._name = name
+
+    @property
+    def status(self):
+        """Gets the status of this QueryPipelineNode.  # noqa: E501
+
+
+        :return: The status of this QueryPipelineNode.  # noqa: E501
+        :rtype: str
+        """
+        return self._status
+
+    @status.setter
+    def status(self, status):
+        """Sets the status of this QueryPipelineNode.
+
+
+        :param status: The status of this QueryPipelineNode.  # noqa: E501
+        :type: str
+        """
+
+        self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(QueryMetrics, dict):
+        if issubclass(QueryPipelineNode, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QueryMetrics):
+        if not isinstance(other, QueryPipelineNode):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/query_pipeline.py` & `timeplus-1.2.1/swagger_client/models/query_pipeline.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/query_pipeline_edge.py` & `timeplus-1.2.1/swagger_client/models/query_pipeline_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/query_pipeline_node_metric.py` & `timeplus-1.2.1/swagger_client/models/query_pipeline_node_metric.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/query_result.py` & `timeplus-1.2.1/swagger_client/models/stream_match_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,88 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class QueryResult(object):
+class StreamMatchRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'list[list[object]]',
-        'header': 'list[Column]'
+        'events': 'list[Event]'
     }
 
     attribute_map = {
-        'data': 'data',
-        'header': 'header'
+        'events': 'events'
     }
 
-    def __init__(self, data=None, header=None):  # noqa: E501
-        """QueryResult - a model defined in Swagger"""  # noqa: E501
-        self._data = None
-        self._header = None
+    def __init__(self, events=None):  # noqa: E501
+        """StreamMatchRequest - a model defined in Swagger"""  # noqa: E501
+        self._events = None
         self.discriminator = None
-        if data is not None:
-            self.data = data
-        self.header = header
+        if events is not None:
+            self.events = events
 
     @property
-    def data(self):
-        """Gets the data of this QueryResult.  # noqa: E501
+    def events(self):
+        """Gets the events of this StreamMatchRequest.  # noqa: E501
 
 
-        :return: The data of this QueryResult.  # noqa: E501
-        :rtype: list[list[object]]
+        :return: The events of this StreamMatchRequest.  # noqa: E501
+        :rtype: list[Event]
         """
-        return self._data
+        return self._events
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this QueryResult.
+    @events.setter
+    def events(self, events):
+        """Sets the events of this StreamMatchRequest.
 
 
-        :param data: The data of this QueryResult.  # noqa: E501
-        :type: list[list[object]]
+        :param events: The events of this StreamMatchRequest.  # noqa: E501
+        :type: list[Event]
         """
 
-        self._data = data
-
-    @property
-    def header(self):
-        """Gets the header of this QueryResult.  # noqa: E501
-
-
-        :return: The header of this QueryResult.  # noqa: E501
-        :rtype: list[Column]
-        """
-        return self._header
-
-    @header.setter
-    def header(self, header):
-        """Sets the header of this QueryResult.
-
-
-        :param header: The header of this QueryResult.  # noqa: E501
-        :type: list[Column]
-        """
-        if header is None:
-            raise ValueError("Invalid value for `header`, must not be `None`")  # noqa: E501
-
-        self._header = header
+        self._events = events
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -107,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(QueryResult, dict):
+        if issubclass(StreamMatchRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -123,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QueryResult):
+        if not isinstance(other, StreamMatchRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/sink.py` & `timeplus-1.2.1/swagger_client/models/sink.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,64 +30,67 @@
     swagger_types = {
         'created_at': 'str',
         'created_by': 'Owner',
         'description': 'str',
         'id': 'str',
         'last_updated_at': 'str',
         'last_updated_by': 'Owner',
+        'message': 'str',
         'name': 'str',
         'properties': 'dict(str, object)',
-        'queries': 'list[str]',
-        'query': 'Query',
+        'query': 'str',
+        'status': 'str',
         'type': 'str'
     }
 
     attribute_map = {
         'created_at': 'created_at',
         'created_by': 'created_by',
         'description': 'description',
         'id': 'id',
         'last_updated_at': 'last_updated_at',
         'last_updated_by': 'last_updated_by',
+        'message': 'message',
         'name': 'name',
         'properties': 'properties',
-        'queries': 'queries',
         'query': 'query',
+        'status': 'status',
         'type': 'type'
     }
 
-    def __init__(self, created_at=None, created_by=None, description=None, id=None, last_updated_at=None, last_updated_by=None, name=None, properties=None, queries=None, query=None, type=None):  # noqa: E501
+    def __init__(self, created_at=None, created_by=None, description=None, id=None, last_updated_at=None, last_updated_by=None, message=None, name=None, properties=None, query=None, status=None, type=None):  # noqa: E501
         """Sink - a model defined in Swagger"""  # noqa: E501
         self._created_at = None
         self._created_by = None
         self._description = None
         self._id = None
         self._last_updated_at = None
         self._last_updated_by = None
+        self._message = None
         self._name = None
         self._properties = None
-        self._queries = None
         self._query = None
+        self._status = None
         self._type = None
         self.discriminator = None
         if created_at is not None:
             self.created_at = created_at
         if created_by is not None:
             self.created_by = created_by
         self.description = description
         self.id = id
         if last_updated_at is not None:
             self.last_updated_at = last_updated_at
         if last_updated_by is not None:
             self.last_updated_by = last_updated_by
+        self.message = message
         self.name = name
         self.properties = properties
-        self.queries = queries
-        if query is not None:
-            self.query = query
+        self.query = query
+        self.status = status
         self.type = type
 
     @property
     def created_at(self):
         """Gets the created_at of this Sink.  # noqa: E501
 
 
@@ -213,14 +216,37 @@
         :param last_updated_by: The last_updated_by of this Sink.  # noqa: E501
         :type: Owner
         """
 
         self._last_updated_by = last_updated_by
 
     @property
+    def message(self):
+        """Gets the message of this Sink.  # noqa: E501
+
+
+        :return: The message of this Sink.  # noqa: E501
+        :rtype: str
+        """
+        return self._message
+
+    @message.setter
+    def message(self, message):
+        """Sets the message of this Sink.
+
+
+        :param message: The message of this Sink.  # noqa: E501
+        :type: str
+        """
+        if message is None:
+            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
+
+        self._message = message
+
+    @property
     def name(self):
         """Gets the name of this Sink.  # noqa: E501
 
 
         :return: The name of this Sink.  # noqa: E501
         :rtype: str
         """
@@ -259,56 +285,58 @@
         """
         if properties is None:
             raise ValueError("Invalid value for `properties`, must not be `None`")  # noqa: E501
 
         self._properties = properties
 
     @property
-    def queries(self):
-        """Gets the queries of this Sink.  # noqa: E501
+    def query(self):
+        """Gets the query of this Sink.  # noqa: E501
 
 
-        :return: The queries of this Sink.  # noqa: E501
-        :rtype: list[str]
+        :return: The query of this Sink.  # noqa: E501
+        :rtype: str
         """
-        return self._queries
+        return self._query
 
-    @queries.setter
-    def queries(self, queries):
-        """Sets the queries of this Sink.
+    @query.setter
+    def query(self, query):
+        """Sets the query of this Sink.
 
 
-        :param queries: The queries of this Sink.  # noqa: E501
-        :type: list[str]
+        :param query: The query of this Sink.  # noqa: E501
+        :type: str
         """
-        if queries is None:
-            raise ValueError("Invalid value for `queries`, must not be `None`")  # noqa: E501
+        if query is None:
+            raise ValueError("Invalid value for `query`, must not be `None`")  # noqa: E501
 
-        self._queries = queries
+        self._query = query
 
     @property
-    def query(self):
-        """Gets the query of this Sink.  # noqa: E501
+    def status(self):
+        """Gets the status of this Sink.  # noqa: E501
 
 
-        :return: The query of this Sink.  # noqa: E501
-        :rtype: Query
+        :return: The status of this Sink.  # noqa: E501
+        :rtype: str
         """
-        return self._query
+        return self._status
 
-    @query.setter
-    def query(self, query):
-        """Sets the query of this Sink.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this Sink.
 
 
-        :param query: The query of this Sink.  # noqa: E501
-        :type: Query
+        :param status: The status of this Sink.  # noqa: E501
+        :type: str
         """
+        if status is None:
+            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
-        self._query = query
+        self._status = status
 
     @property
     def type(self):
         """Gets the type of this Sink.  # noqa: E501
 
 
         :return: The type of this Sink.  # noqa: E501
```

### Comparing `timeplus-1.1.2/swagger_client/models/sink_stat.py` & `timeplus-1.2.1/swagger_client/models/sink_stat.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/sink_with_metrics.py` & `timeplus-1.2.1/swagger_client/models/view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,338 +1,387 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SinkWithMetrics(object):
+class View(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'columns': 'list[ColumnsResp]',
         'created_at': 'str',
         'created_by': 'Owner',
         'description': 'str',
-        'id': 'str',
         'last_updated_at': 'str',
         'last_updated_by': 'Owner',
-        'metrics': 'SinkMetrics',
+        'logstore_retention_bytes': 'int',
+        'logstore_retention_ms': 'int',
+        'materialized': 'bool',
         'name': 'str',
-        'properties': 'dict(str, object)',
-        'queries': 'list[str]',
-        'type': 'str'
+        'query': 'str',
+        'target_stream': 'str',
+        'ttl': 'str'
     }
 
     attribute_map = {
+        'columns': 'columns',
         'created_at': 'created_at',
         'created_by': 'created_by',
         'description': 'description',
-        'id': 'id',
         'last_updated_at': 'last_updated_at',
         'last_updated_by': 'last_updated_by',
-        'metrics': 'metrics',
+        'logstore_retention_bytes': 'logstore_retention_bytes',
+        'logstore_retention_ms': 'logstore_retention_ms',
+        'materialized': 'materialized',
         'name': 'name',
-        'properties': 'properties',
-        'queries': 'queries',
-        'type': 'type'
+        'query': 'query',
+        'target_stream': 'target_stream',
+        'ttl': 'ttl'
     }
 
-    def __init__(self, created_at=None, created_by=None, description=None, id=None, last_updated_at=None, last_updated_by=None, metrics=None, name=None, properties=None, queries=None, type=None):  # noqa: E501
-        """SinkWithMetrics - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, columns=None, created_at=None, created_by=None, description=None, last_updated_at=None, last_updated_by=None, logstore_retention_bytes=None, logstore_retention_ms=None, materialized=None, name=None, query=None, target_stream=None, ttl=None):  # noqa: E501
+        """View - a model defined in Swagger"""  # noqa: E501
+        self._columns = None
         self._created_at = None
         self._created_by = None
         self._description = None
-        self._id = None
         self._last_updated_at = None
         self._last_updated_by = None
-        self._metrics = None
+        self._logstore_retention_bytes = None
+        self._logstore_retention_ms = None
+        self._materialized = None
         self._name = None
-        self._properties = None
-        self._queries = None
-        self._type = None
+        self._query = None
+        self._target_stream = None
+        self._ttl = None
         self.discriminator = None
+        self.columns = columns
         if created_at is not None:
             self.created_at = created_at
         if created_by is not None:
             self.created_by = created_by
-        self.description = description
-        self.id = id
+        if description is not None:
+            self.description = description
         if last_updated_at is not None:
             self.last_updated_at = last_updated_at
         if last_updated_by is not None:
             self.last_updated_by = last_updated_by
-        self.metrics = metrics
-        self.name = name
-        self.properties = properties
-        self.queries = queries
-        self.type = type
+        self.logstore_retention_bytes = logstore_retention_bytes
+        self.logstore_retention_ms = logstore_retention_ms
+        if materialized is not None:
+            self.materialized = materialized
+        if name is not None:
+            self.name = name
+        if query is not None:
+            self.query = query
+        if target_stream is not None:
+            self.target_stream = target_stream
+        self.ttl = ttl
+
+    @property
+    def columns(self):
+        """Gets the columns of this View.  # noqa: E501
+
+
+        :return: The columns of this View.  # noqa: E501
+        :rtype: list[ColumnsResp]
+        """
+        return self._columns
+
+    @columns.setter
+    def columns(self, columns):
+        """Sets the columns of this View.
+
+
+        :param columns: The columns of this View.  # noqa: E501
+        :type: list[ColumnsResp]
+        """
+        if columns is None:
+            raise ValueError("Invalid value for `columns`, must not be `None`")  # noqa: E501
+
+        self._columns = columns
 
     @property
     def created_at(self):
-        """Gets the created_at of this SinkWithMetrics.  # noqa: E501
+        """Gets the created_at of this View.  # noqa: E501
 
 
-        :return: The created_at of this SinkWithMetrics.  # noqa: E501
+        :return: The created_at of this View.  # noqa: E501
         :rtype: str
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
-        """Sets the created_at of this SinkWithMetrics.
+        """Sets the created_at of this View.
 
 
-        :param created_at: The created_at of this SinkWithMetrics.  # noqa: E501
+        :param created_at: The created_at of this View.  # noqa: E501
         :type: str
         """
 
         self._created_at = created_at
 
     @property
     def created_by(self):
-        """Gets the created_by of this SinkWithMetrics.  # noqa: E501
+        """Gets the created_by of this View.  # noqa: E501
 
 
-        :return: The created_by of this SinkWithMetrics.  # noqa: E501
+        :return: The created_by of this View.  # noqa: E501
         :rtype: Owner
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
-        """Sets the created_by of this SinkWithMetrics.
+        """Sets the created_by of this View.
 
 
-        :param created_by: The created_by of this SinkWithMetrics.  # noqa: E501
+        :param created_by: The created_by of this View.  # noqa: E501
         :type: Owner
         """
 
         self._created_by = created_by
 
     @property
     def description(self):
-        """Gets the description of this SinkWithMetrics.  # noqa: E501
+        """Gets the description of this View.  # noqa: E501
 
 
-        :return: The description of this SinkWithMetrics.  # noqa: E501
+        :return: The description of this View.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this SinkWithMetrics.
+        """Sets the description of this View.
 
 
-        :param description: The description of this SinkWithMetrics.  # noqa: E501
+        :param description: The description of this View.  # noqa: E501
         :type: str
         """
-        if description is None:
-            raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
 
         self._description = description
 
     @property
-    def id(self):
-        """Gets the id of this SinkWithMetrics.  # noqa: E501
-
-
-        :return: The id of this SinkWithMetrics.  # noqa: E501
-        :rtype: str
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this SinkWithMetrics.
-
-
-        :param id: The id of this SinkWithMetrics.  # noqa: E501
-        :type: str
-        """
-        if id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-
-        self._id = id
-
-    @property
     def last_updated_at(self):
-        """Gets the last_updated_at of this SinkWithMetrics.  # noqa: E501
+        """Gets the last_updated_at of this View.  # noqa: E501
 
 
-        :return: The last_updated_at of this SinkWithMetrics.  # noqa: E501
+        :return: The last_updated_at of this View.  # noqa: E501
         :rtype: str
         """
         return self._last_updated_at
 
     @last_updated_at.setter
     def last_updated_at(self, last_updated_at):
-        """Sets the last_updated_at of this SinkWithMetrics.
+        """Sets the last_updated_at of this View.
 
 
-        :param last_updated_at: The last_updated_at of this SinkWithMetrics.  # noqa: E501
+        :param last_updated_at: The last_updated_at of this View.  # noqa: E501
         :type: str
         """
 
         self._last_updated_at = last_updated_at
 
     @property
     def last_updated_by(self):
-        """Gets the last_updated_by of this SinkWithMetrics.  # noqa: E501
+        """Gets the last_updated_by of this View.  # noqa: E501
 
 
-        :return: The last_updated_by of this SinkWithMetrics.  # noqa: E501
+        :return: The last_updated_by of this View.  # noqa: E501
         :rtype: Owner
         """
         return self._last_updated_by
 
     @last_updated_by.setter
     def last_updated_by(self, last_updated_by):
-        """Sets the last_updated_by of this SinkWithMetrics.
+        """Sets the last_updated_by of this View.
 
 
-        :param last_updated_by: The last_updated_by of this SinkWithMetrics.  # noqa: E501
+        :param last_updated_by: The last_updated_by of this View.  # noqa: E501
         :type: Owner
         """
 
         self._last_updated_by = last_updated_by
 
     @property
-    def metrics(self):
-        """Gets the metrics of this SinkWithMetrics.  # noqa: E501
+    def logstore_retention_bytes(self):
+        """Gets the logstore_retention_bytes of this View.  # noqa: E501
+
+
+        :return: The logstore_retention_bytes of this View.  # noqa: E501
+        :rtype: int
+        """
+        return self._logstore_retention_bytes
+
+    @logstore_retention_bytes.setter
+    def logstore_retention_bytes(self, logstore_retention_bytes):
+        """Sets the logstore_retention_bytes of this View.
+
+
+        :param logstore_retention_bytes: The logstore_retention_bytes of this View.  # noqa: E501
+        :type: int
+        """
+        if logstore_retention_bytes is None:
+            raise ValueError("Invalid value for `logstore_retention_bytes`, must not be `None`")  # noqa: E501
+
+        self._logstore_retention_bytes = logstore_retention_bytes
+
+    @property
+    def logstore_retention_ms(self):
+        """Gets the logstore_retention_ms of this View.  # noqa: E501
 
 
-        :return: The metrics of this SinkWithMetrics.  # noqa: E501
-        :rtype: SinkMetrics
+        :return: The logstore_retention_ms of this View.  # noqa: E501
+        :rtype: int
         """
-        return self._metrics
+        return self._logstore_retention_ms
 
-    @metrics.setter
-    def metrics(self, metrics):
-        """Sets the metrics of this SinkWithMetrics.
+    @logstore_retention_ms.setter
+    def logstore_retention_ms(self, logstore_retention_ms):
+        """Sets the logstore_retention_ms of this View.
 
 
-        :param metrics: The metrics of this SinkWithMetrics.  # noqa: E501
-        :type: SinkMetrics
+        :param logstore_retention_ms: The logstore_retention_ms of this View.  # noqa: E501
+        :type: int
         """
-        if metrics is None:
-            raise ValueError("Invalid value for `metrics`, must not be `None`")  # noqa: E501
+        if logstore_retention_ms is None:
+            raise ValueError("Invalid value for `logstore_retention_ms`, must not be `None`")  # noqa: E501
 
-        self._metrics = metrics
+        self._logstore_retention_ms = logstore_retention_ms
+
+    @property
+    def materialized(self):
+        """Gets the materialized of this View.  # noqa: E501
+
+
+        :return: The materialized of this View.  # noqa: E501
+        :rtype: bool
+        """
+        return self._materialized
+
+    @materialized.setter
+    def materialized(self, materialized):
+        """Sets the materialized of this View.
+
+
+        :param materialized: The materialized of this View.  # noqa: E501
+        :type: bool
+        """
+
+        self._materialized = materialized
 
     @property
     def name(self):
-        """Gets the name of this SinkWithMetrics.  # noqa: E501
+        """Gets the name of this View.  # noqa: E501
 
 
-        :return: The name of this SinkWithMetrics.  # noqa: E501
+        :return: The name of this View.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this SinkWithMetrics.
+        """Sets the name of this View.
 
 
-        :param name: The name of this SinkWithMetrics.  # noqa: E501
+        :param name: The name of this View.  # noqa: E501
         :type: str
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def properties(self):
-        """Gets the properties of this SinkWithMetrics.  # noqa: E501
+    def query(self):
+        """Gets the query of this View.  # noqa: E501
 
 
-        :return: The properties of this SinkWithMetrics.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The query of this View.  # noqa: E501
+        :rtype: str
         """
-        return self._properties
+        return self._query
 
-    @properties.setter
-    def properties(self, properties):
-        """Sets the properties of this SinkWithMetrics.
+    @query.setter
+    def query(self, query):
+        """Sets the query of this View.
 
 
-        :param properties: The properties of this SinkWithMetrics.  # noqa: E501
-        :type: dict(str, object)
+        :param query: The query of this View.  # noqa: E501
+        :type: str
         """
-        if properties is None:
-            raise ValueError("Invalid value for `properties`, must not be `None`")  # noqa: E501
 
-        self._properties = properties
+        self._query = query
 
     @property
-    def queries(self):
-        """Gets the queries of this SinkWithMetrics.  # noqa: E501
+    def target_stream(self):
+        """Gets the target_stream of this View.  # noqa: E501
 
 
-        :return: The queries of this SinkWithMetrics.  # noqa: E501
-        :rtype: list[str]
+        :return: The target_stream of this View.  # noqa: E501
+        :rtype: str
         """
-        return self._queries
+        return self._target_stream
 
-    @queries.setter
-    def queries(self, queries):
-        """Sets the queries of this SinkWithMetrics.
+    @target_stream.setter
+    def target_stream(self, target_stream):
+        """Sets the target_stream of this View.
 
 
-        :param queries: The queries of this SinkWithMetrics.  # noqa: E501
-        :type: list[str]
+        :param target_stream: The target_stream of this View.  # noqa: E501
+        :type: str
         """
-        if queries is None:
-            raise ValueError("Invalid value for `queries`, must not be `None`")  # noqa: E501
 
-        self._queries = queries
+        self._target_stream = target_stream
 
     @property
-    def type(self):
-        """Gets the type of this SinkWithMetrics.  # noqa: E501
+    def ttl(self):
+        """Gets the ttl of this View.  # noqa: E501
 
 
-        :return: The type of this SinkWithMetrics.  # noqa: E501
+        :return: The ttl of this View.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._ttl
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this SinkWithMetrics.
+    @ttl.setter
+    def ttl(self, ttl):
+        """Sets the ttl of this View.
 
 
-        :param type: The type of this SinkWithMetrics.  # noqa: E501
+        :param ttl: The ttl of this View.  # noqa: E501
         :type: str
         """
-        if type is None:
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if ttl is None:
+            raise ValueError("Invalid value for `ttl`, must not be `None`")  # noqa: E501
 
-        self._type = type
+        self._ttl = ttl
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -347,15 +396,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SinkWithMetrics, dict):
+        if issubclass(View, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -363,15 +412,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SinkWithMetrics):
+        if not isinstance(other, View):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/source.py` & `timeplus-1.2.1/swagger_client/models/source.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,95 +24,80 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'connection': 'Connection',
         'created_at': 'str',
         'created_by': 'Owner',
         'description': 'str',
         'id': 'str',
         'last_updated_at': 'str',
         'last_updated_by': 'Owner',
+        'message': 'str',
         'name': 'str',
         'properties': 'dict(str, object)',
         'start_time': 'int',
+        'status': 'str',
+        'stream': 'str',
         'type': 'str'
     }
 
     attribute_map = {
-        'connection': 'connection',
         'created_at': 'created_at',
         'created_by': 'created_by',
         'description': 'description',
         'id': 'id',
         'last_updated_at': 'last_updated_at',
         'last_updated_by': 'last_updated_by',
+        'message': 'message',
         'name': 'name',
         'properties': 'properties',
         'start_time': 'start_time',
+        'status': 'status',
+        'stream': 'stream',
         'type': 'type'
     }
 
-    def __init__(self, connection=None, created_at=None, created_by=None, description=None, id=None, last_updated_at=None, last_updated_by=None, name=None, properties=None, start_time=None, type=None):  # noqa: E501
+    def __init__(self, created_at=None, created_by=None, description=None, id=None, last_updated_at=None, last_updated_by=None, message=None, name=None, properties=None, start_time=None, status=None, stream=None, type=None):  # noqa: E501
         """Source - a model defined in Swagger"""  # noqa: E501
-        self._connection = None
         self._created_at = None
         self._created_by = None
         self._description = None
         self._id = None
         self._last_updated_at = None
         self._last_updated_by = None
+        self._message = None
         self._name = None
         self._properties = None
         self._start_time = None
+        self._status = None
+        self._stream = None
         self._type = None
         self.discriminator = None
-        self.connection = connection
         if created_at is not None:
             self.created_at = created_at
         if created_by is not None:
             self.created_by = created_by
         self.description = description
         self.id = id
         if last_updated_at is not None:
             self.last_updated_at = last_updated_at
         if last_updated_by is not None:
             self.last_updated_by = last_updated_by
+        self.message = message
         self.name = name
         self.properties = properties
         self.start_time = start_time
+        self.status = status
+        self.stream = stream
         self.type = type
 
     @property
-    def connection(self):
-        """Gets the connection of this Source.  # noqa: E501
-
-
-        :return: The connection of this Source.  # noqa: E501
-        :rtype: Connection
-        """
-        return self._connection
-
-    @connection.setter
-    def connection(self, connection):
-        """Sets the connection of this Source.
-
-
-        :param connection: The connection of this Source.  # noqa: E501
-        :type: Connection
-        """
-        if connection is None:
-            raise ValueError("Invalid value for `connection`, must not be `None`")  # noqa: E501
-
-        self._connection = connection
-
-    @property
     def created_at(self):
         """Gets the created_at of this Source.  # noqa: E501
 
 
         :return: The created_at of this Source.  # noqa: E501
         :rtype: str
         """
@@ -235,14 +220,37 @@
         :param last_updated_by: The last_updated_by of this Source.  # noqa: E501
         :type: Owner
         """
 
         self._last_updated_by = last_updated_by
 
     @property
+    def message(self):
+        """Gets the message of this Source.  # noqa: E501
+
+
+        :return: The message of this Source.  # noqa: E501
+        :rtype: str
+        """
+        return self._message
+
+    @message.setter
+    def message(self, message):
+        """Sets the message of this Source.
+
+
+        :param message: The message of this Source.  # noqa: E501
+        :type: str
+        """
+        if message is None:
+            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
+
+        self._message = message
+
+    @property
     def name(self):
         """Gets the name of this Source.  # noqa: E501
 
 
         :return: The name of this Source.  # noqa: E501
         :rtype: str
         """
@@ -261,70 +269,124 @@
 
         self._name = name
 
     @property
     def properties(self):
         """Gets the properties of this Source.  # noqa: E501
 
+        Additional properties of the source  # noqa: E501
 
         :return: The properties of this Source.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._properties
 
     @properties.setter
     def properties(self, properties):
         """Sets the properties of this Source.
 
+        Additional properties of the source  # noqa: E501
 
         :param properties: The properties of this Source.  # noqa: E501
         :type: dict(str, object)
         """
         if properties is None:
             raise ValueError("Invalid value for `properties`, must not be `None`")  # noqa: E501
 
         self._properties = properties
 
     @property
     def start_time(self):
         """Gets the start_time of this Source.  # noqa: E501
 
+        Unix timestamp when the source get started  # noqa: E501
 
         :return: The start_time of this Source.  # noqa: E501
         :rtype: int
         """
         return self._start_time
 
     @start_time.setter
     def start_time(self, start_time):
         """Sets the start_time of this Source.
 
+        Unix timestamp when the source get started  # noqa: E501
 
         :param start_time: The start_time of this Source.  # noqa: E501
         :type: int
         """
         if start_time is None:
             raise ValueError("Invalid value for `start_time`, must not be `None`")  # noqa: E501
 
         self._start_time = start_time
 
     @property
+    def status(self):
+        """Gets the status of this Source.  # noqa: E501
+
+
+        :return: The status of this Source.  # noqa: E501
+        :rtype: str
+        """
+        return self._status
+
+    @status.setter
+    def status(self, status):
+        """Sets the status of this Source.
+
+
+        :param status: The status of this Source.  # noqa: E501
+        :type: str
+        """
+        if status is None:
+            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
+
+        self._status = status
+
+    @property
+    def stream(self):
+        """Gets the stream of this Source.  # noqa: E501
+
+        The name of the target stream that this source writes to.  # noqa: E501
+
+        :return: The stream of this Source.  # noqa: E501
+        :rtype: str
+        """
+        return self._stream
+
+    @stream.setter
+    def stream(self, stream):
+        """Sets the stream of this Source.
+
+        The name of the target stream that this source writes to.  # noqa: E501
+
+        :param stream: The stream of this Source.  # noqa: E501
+        :type: str
+        """
+        if stream is None:
+            raise ValueError("Invalid value for `stream`, must not be `None`")  # noqa: E501
+
+        self._stream = stream
+
+    @property
     def type(self):
         """Gets the type of this Source.  # noqa: E501
 
+        Type of the source  # noqa: E501
 
         :return: The type of this Source.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this Source.
 
+        Type of the source  # noqa: E501
 
         :param type: The type of this Source.  # noqa: E501
         :type: str
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
```

### Comparing `timeplus-1.1.2/swagger_client/models/source_preview_request.py` & `timeplus-1.2.1/swagger_client/models/metrics_query_throughput.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,113 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SourcePreviewRequest(object):
+class MetricsQueryThroughput(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'properties': 'dict(str, object)',
-        'size': 'int',
-        'type': 'str'
+        'time': 'str',
+        'value': 'float'
     }
 
     attribute_map = {
-        'properties': 'properties',
-        'size': 'size',
-        'type': 'type'
+        'time': 'time',
+        'value': 'value'
     }
 
-    def __init__(self, properties=None, size=None, type=None):  # noqa: E501
-        """SourcePreviewRequest - a model defined in Swagger"""  # noqa: E501
-        self._properties = None
-        self._size = None
-        self._type = None
+    def __init__(self, time=None, value=None):  # noqa: E501
+        """MetricsQueryThroughput - a model defined in Swagger"""  # noqa: E501
+        self._time = None
+        self._value = None
         self.discriminator = None
-        if properties is not None:
-            self.properties = properties
-        if size is not None:
-            self.size = size
-        if type is not None:
-            self.type = type
+        self.time = time
+        self.value = value
 
     @property
-    def properties(self):
-        """Gets the properties of this SourcePreviewRequest.  # noqa: E501
+    def time(self):
+        """Gets the time of this MetricsQueryThroughput.  # noqa: E501
 
 
-        :return: The properties of this SourcePreviewRequest.  # noqa: E501
-        :rtype: dict(str, object)
-        """
-        return self._properties
-
-    @properties.setter
-    def properties(self, properties):
-        """Sets the properties of this SourcePreviewRequest.
-
-
-        :param properties: The properties of this SourcePreviewRequest.  # noqa: E501
-        :type: dict(str, object)
-        """
-
-        self._properties = properties
-
-    @property
-    def size(self):
-        """Gets the size of this SourcePreviewRequest.  # noqa: E501
-
-
-        :return: The size of this SourcePreviewRequest.  # noqa: E501
-        :rtype: int
+        :return: The time of this MetricsQueryThroughput.  # noqa: E501
+        :rtype: str
         """
-        return self._size
+        return self._time
 
-    @size.setter
-    def size(self, size):
-        """Sets the size of this SourcePreviewRequest.
+    @time.setter
+    def time(self, time):
+        """Sets the time of this MetricsQueryThroughput.
 
 
-        :param size: The size of this SourcePreviewRequest.  # noqa: E501
-        :type: int
+        :param time: The time of this MetricsQueryThroughput.  # noqa: E501
+        :type: str
         """
+        if time is None:
+            raise ValueError("Invalid value for `time`, must not be `None`")  # noqa: E501
 
-        self._size = size
+        self._time = time
 
     @property
-    def type(self):
-        """Gets the type of this SourcePreviewRequest.  # noqa: E501
+    def value(self):
+        """Gets the value of this MetricsQueryThroughput.  # noqa: E501
 
 
-        :return: The type of this SourcePreviewRequest.  # noqa: E501
-        :rtype: str
+        :return: The value of this MetricsQueryThroughput.  # noqa: E501
+        :rtype: float
         """
-        return self._type
+        return self._value
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this SourcePreviewRequest.
+    @value.setter
+    def value(self, value):
+        """Sets the value of this MetricsQueryThroughput.
 
 
-        :param type: The type of this SourcePreviewRequest.  # noqa: E501
-        :type: str
+        :param value: The value of this MetricsQueryThroughput.  # noqa: E501
+        :type: float
         """
+        if value is None:
+            raise ValueError("Invalid value for `value`, must not be `None`")  # noqa: E501
 
-        self._type = type
+        self._value = value
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SourcePreviewRequest, dict):
+        if issubclass(MetricsQueryThroughput, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SourcePreviewRequest):
+        if not isinstance(other, MetricsQueryThroughput):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `timeplus-1.1.2/swagger_client/models/source_upload_body.py` & `timeplus-1.2.1/swagger_client/models/source_upload_body.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/sql_analyze_column.py` & `timeplus-1.2.1/swagger_client/models/sql_analyze_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/sql_analyze_result.py` & `timeplus-1.2.1/swagger_client/models/sql_analyze_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/stream.py` & `timeplus-1.2.1/swagger_client/models/stream.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,49 +34,52 @@
         'description': 'str',
         'engine': 'str',
         'is_external': 'bool',
         'last_updated_at': 'str',
         'last_updated_by': 'Owner',
         'logstore_retention_bytes': 'int',
         'logstore_retention_ms': 'int',
+        'mode': 'str',
         'name': 'str',
-        'stats': 'StreamStats',
+        'primary_key': 'str',
         'ttl': 'str'
     }
 
     attribute_map = {
         'columns': 'columns',
         'created_at': 'created_at',
         'created_by': 'created_by',
         'description': 'description',
         'engine': 'engine',
         'is_external': 'is_external',
         'last_updated_at': 'last_updated_at',
         'last_updated_by': 'last_updated_by',
         'logstore_retention_bytes': 'logstore_retention_bytes',
         'logstore_retention_ms': 'logstore_retention_ms',
+        'mode': 'mode',
         'name': 'name',
-        'stats': 'stats',
+        'primary_key': 'primary_key',
         'ttl': 'ttl'
     }
 
-    def __init__(self, columns=None, created_at=None, created_by=None, description=None, engine=None, is_external=None, last_updated_at=None, last_updated_by=None, logstore_retention_bytes=None, logstore_retention_ms=None, name=None, stats=None, ttl=None):  # noqa: E501
+    def __init__(self, columns=None, created_at=None, created_by=None, description=None, engine=None, is_external=None, last_updated_at=None, last_updated_by=None, logstore_retention_bytes=None, logstore_retention_ms=None, mode=None, name=None, primary_key=None, ttl=None):  # noqa: E501
         """Stream - a model defined in Swagger"""  # noqa: E501
         self._columns = None
         self._created_at = None
         self._created_by = None
         self._description = None
         self._engine = None
         self._is_external = None
         self._last_updated_at = None
         self._last_updated_by = None
         self._logstore_retention_bytes = None
         self._logstore_retention_ms = None
+        self._mode = None
         self._name = None
-        self._stats = None
+        self._primary_key = None
         self._ttl = None
         self.discriminator = None
         self.columns = columns
         if created_at is not None:
             self.created_at = created_at
         if created_by is not None:
             self.created_by = created_by
@@ -85,17 +88,18 @@
         self.is_external = is_external
         if last_updated_at is not None:
             self.last_updated_at = last_updated_at
         if last_updated_by is not None:
             self.last_updated_by = last_updated_by
         self.logstore_retention_bytes = logstore_retention_bytes
         self.logstore_retention_ms = logstore_retention_ms
+        self.mode = mode
         self.name = name
-        if stats is not None:
-            self.stats = stats
+        if primary_key is not None:
+            self.primary_key = primary_key
         self.ttl = ttl
 
     @property
     def columns(self):
         """Gets the columns of this Stream.  # noqa: E501
 
 
@@ -313,14 +317,39 @@
         """
         if logstore_retention_ms is None:
             raise ValueError("Invalid value for `logstore_retention_ms`, must not be `None`")  # noqa: E501
 
         self._logstore_retention_ms = logstore_retention_ms
 
     @property
+    def mode(self):
+        """Gets the mode of this Stream.  # noqa: E501
+
+        Storage mode of stream. Possible values: `append`, `changelog`, `changelog_kv`, `versioned_kv`  # noqa: E501
+
+        :return: The mode of this Stream.  # noqa: E501
+        :rtype: str
+        """
+        return self._mode
+
+    @mode.setter
+    def mode(self, mode):
+        """Sets the mode of this Stream.
+
+        Storage mode of stream. Possible values: `append`, `changelog`, `changelog_kv`, `versioned_kv`  # noqa: E501
+
+        :param mode: The mode of this Stream.  # noqa: E501
+        :type: str
+        """
+        if mode is None:
+            raise ValueError("Invalid value for `mode`, must not be `None`")  # noqa: E501
+
+        self._mode = mode
+
+    @property
     def name(self):
         """Gets the name of this Stream.  # noqa: E501
 
 
         :return: The name of this Stream.  # noqa: E501
         :rtype: str
         """
@@ -336,33 +365,35 @@
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def stats(self):
-        """Gets the stats of this Stream.  # noqa: E501
+    def primary_key(self):
+        """Gets the primary_key of this Stream.  # noqa: E501
 
+        Expression of primary key, required in `changelog_kv`` and `versioned_kv`` mode  # noqa: E501
 
-        :return: The stats of this Stream.  # noqa: E501
-        :rtype: StreamStats
+        :return: The primary_key of this Stream.  # noqa: E501
+        :rtype: str
         """
-        return self._stats
+        return self._primary_key
 
-    @stats.setter
-    def stats(self, stats):
-        """Sets the stats of this Stream.
+    @primary_key.setter
+    def primary_key(self, primary_key):
+        """Sets the primary_key of this Stream.
 
+        Expression of primary key, required in `changelog_kv`` and `versioned_kv`` mode  # noqa: E501
 
-        :param stats: The stats of this Stream.  # noqa: E501
-        :type: StreamStats
+        :param primary_key: The primary_key of this Stream.  # noqa: E501
+        :type: str
         """
 
-        self._stats = stats
+        self._primary_key = primary_key
 
     @property
     def ttl(self):
         """Gets the ttl of this Stream.  # noqa: E501
 
         ORDER_BY     string        `json:\"order_by_expression\"` PATTITION_BY string        `json:\"partition_by_expression\"`  # noqa: E501
```

### Comparing `timeplus-1.1.2/swagger_client/models/stream_def.py` & `timeplus-1.2.1/swagger_client/models/stream_def.py`

 * *Files 14% similar despite different names*

```diff
@@ -153,108 +153,118 @@
 
         self._description = description
 
     @property
     def event_time_column(self):
         """Gets the event_time_column of this StreamDef.  # noqa: E501
 
+        This column will be used as the event time if specified  # noqa: E501
 
         :return: The event_time_column of this StreamDef.  # noqa: E501
         :rtype: str
         """
         return self._event_time_column
 
     @event_time_column.setter
     def event_time_column(self, event_time_column):
         """Sets the event_time_column of this StreamDef.
 
+        This column will be used as the event time if specified  # noqa: E501
 
         :param event_time_column: The event_time_column of this StreamDef.  # noqa: E501
         :type: str
         """
 
         self._event_time_column = event_time_column
 
     @property
     def event_time_timezone(self):
         """Gets the event_time_timezone of this StreamDef.  # noqa: E501
 
+        The timezone of the `TimestampColumn`  # noqa: E501
 
         :return: The event_time_timezone of this StreamDef.  # noqa: E501
         :rtype: str
         """
         return self._event_time_timezone
 
     @event_time_timezone.setter
     def event_time_timezone(self, event_time_timezone):
         """Sets the event_time_timezone of this StreamDef.
 
+        The timezone of the `TimestampColumn`  # noqa: E501
 
         :param event_time_timezone: The event_time_timezone of this StreamDef.  # noqa: E501
         :type: str
         """
 
         self._event_time_timezone = event_time_timezone
 
     @property
     def logstore_retention_bytes(self):
         """Gets the logstore_retention_bytes of this StreamDef.  # noqa: E501
 
+        The max size a stream can grow. Defaulted to 10 GiB  # noqa: E501
 
         :return: The logstore_retention_bytes of this StreamDef.  # noqa: E501
         :rtype: int
         """
         return self._logstore_retention_bytes
 
     @logstore_retention_bytes.setter
     def logstore_retention_bytes(self, logstore_retention_bytes):
         """Sets the logstore_retention_bytes of this StreamDef.
 
+        The max size a stream can grow. Defaulted to 10 GiB  # noqa: E501
 
         :param logstore_retention_bytes: The logstore_retention_bytes of this StreamDef.  # noqa: E501
         :type: int
         """
 
         self._logstore_retention_bytes = logstore_retention_bytes
 
     @property
     def logstore_retention_ms(self):
         """Gets the logstore_retention_ms of this StreamDef.  # noqa: E501
 
+        The max time the data can be retained in the stream. Defaulted to 7 days  # noqa: E501
 
         :return: The logstore_retention_ms of this StreamDef.  # noqa: E501
         :rtype: int
         """
         return self._logstore_retention_ms
 
     @logstore_retention_ms.setter
     def logstore_retention_ms(self, logstore_retention_ms):
         """Sets the logstore_retention_ms of this StreamDef.
 
+        The max time the data can be retained in the stream. Defaulted to 7 days  # noqa: E501
 
         :param logstore_retention_ms: The logstore_retention_ms of this StreamDef.  # noqa: E501
         :type: int
         """
 
         self._logstore_retention_ms = logstore_retention_ms
 
     @property
     def mode(self):
         """Gets the mode of this StreamDef.  # noqa: E501
 
+        Storage mode of stream. Possible values: `append`, `changelog`, `changelog_kv`, `versioned_kv`  # noqa: E501
 
         :return: The mode of this StreamDef.  # noqa: E501
         :rtype: str
         """
         return self._mode
 
     @mode.setter
     def mode(self, mode):
         """Sets the mode of this StreamDef.
 
+        Storage mode of stream. Possible values: `append`, `changelog`, `changelog_kv`, `versioned_kv`  # noqa: E501
 
         :param mode: The mode of this StreamDef.  # noqa: E501
         :type: str
         """
 
         self._mode = mode
 
@@ -346,24 +356,26 @@
 
         self._partition_by_granularity = partition_by_granularity
 
     @property
     def primary_key(self):
         """Gets the primary_key of this StreamDef.  # noqa: E501
 
+        Expression of primary key, required in `changelog_kv`` and `versioned_kv`` mode  # noqa: E501
 
         :return: The primary_key of this StreamDef.  # noqa: E501
         :rtype: str
         """
         return self._primary_key
 
     @primary_key.setter
     def primary_key(self, primary_key):
         """Sets the primary_key of this StreamDef.
 
+        Expression of primary key, required in `changelog_kv`` and `versioned_kv`` mode  # noqa: E501
 
         :param primary_key: The primary_key of this StreamDef.  # noqa: E501
         :type: str
         """
 
         self._primary_key = primary_key
```

### Comparing `timeplus-1.1.2/swagger_client/models/stream_setting.py` & `timeplus-1.2.1/swagger_client/models/stream_setting.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/time_columns.py` & `timeplus-1.2.1/swagger_client/models/time_columns.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/update_dashboard_request.py` & `timeplus-1.2.1/swagger_client/models/update_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/models/update_stream_request.py` & `timeplus-1.2.1/swagger_client/models/update_stream_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,45 +78,49 @@
 
         self._description = description
 
     @property
     def logstore_retention_bytes(self):
         """Gets the logstore_retention_bytes of this UpdateStreamRequest.  # noqa: E501
 
+        The max size a stream can grow. Defaulted to 10 GiB  # noqa: E501
 
         :return: The logstore_retention_bytes of this UpdateStreamRequest.  # noqa: E501
         :rtype: int
         """
         return self._logstore_retention_bytes
 
     @logstore_retention_bytes.setter
     def logstore_retention_bytes(self, logstore_retention_bytes):
         """Sets the logstore_retention_bytes of this UpdateStreamRequest.
 
+        The max size a stream can grow. Defaulted to 10 GiB  # noqa: E501
 
         :param logstore_retention_bytes: The logstore_retention_bytes of this UpdateStreamRequest.  # noqa: E501
         :type: int
         """
 
         self._logstore_retention_bytes = logstore_retention_bytes
 
     @property
     def logstore_retention_ms(self):
         """Gets the logstore_retention_ms of this UpdateStreamRequest.  # noqa: E501
 
+        The max time the data can be retained in the stream. Defaulted to 7 days  # noqa: E501
 
         :return: The logstore_retention_ms of this UpdateStreamRequest.  # noqa: E501
         :rtype: int
         """
         return self._logstore_retention_ms
 
     @logstore_retention_ms.setter
     def logstore_retention_ms(self, logstore_retention_ms):
         """Sets the logstore_retention_ms of this UpdateStreamRequest.
 
+        The max time the data can be retained in the stream. Defaulted to 7 days  # noqa: E501
 
         :param logstore_retention_ms: The logstore_retention_ms of this UpdateStreamRequest.  # noqa: E501
         :type: int
         """
 
         self._logstore_retention_ms = logstore_retention_ms
```

### Comparing `timeplus-1.1.2/swagger_client/models/update_view_request.py` & `timeplus-1.2.1/swagger_client/models/update_view_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,45 +83,49 @@
 
         self._description = description
 
     @property
     def logstore_retention_bytes(self):
         """Gets the logstore_retention_bytes of this UpdateViewRequest.  # noqa: E501
 
+        The max size a stream can grow. Defaulted to 10 GiB  # noqa: E501
 
         :return: The logstore_retention_bytes of this UpdateViewRequest.  # noqa: E501
         :rtype: int
         """
         return self._logstore_retention_bytes
 
     @logstore_retention_bytes.setter
     def logstore_retention_bytes(self, logstore_retention_bytes):
         """Sets the logstore_retention_bytes of this UpdateViewRequest.
 
+        The max size a stream can grow. Defaulted to 10 GiB  # noqa: E501
 
         :param logstore_retention_bytes: The logstore_retention_bytes of this UpdateViewRequest.  # noqa: E501
         :type: int
         """
 
         self._logstore_retention_bytes = logstore_retention_bytes
 
     @property
     def logstore_retention_ms(self):
         """Gets the logstore_retention_ms of this UpdateViewRequest.  # noqa: E501
 
+        The max time the data can be retained in the stream. Defaulted to 7 days  # noqa: E501
 
         :return: The logstore_retention_ms of this UpdateViewRequest.  # noqa: E501
         :rtype: int
         """
         return self._logstore_retention_ms
 
     @logstore_retention_ms.setter
     def logstore_retention_ms(self, logstore_retention_ms):
         """Sets the logstore_retention_ms of this UpdateViewRequest.
 
+        The max time the data can be retained in the stream. Defaulted to 7 days  # noqa: E501
 
         :param logstore_retention_ms: The logstore_retention_ms of this UpdateViewRequest.  # noqa: E501
         :type: int
         """
 
         self._logstore_retention_ms = logstore_retention_ms
```

### Comparing `timeplus-1.1.2/swagger_client/rest.py` & `timeplus-1.2.1/swagger_client/rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 import io
 import json
 import logging
 import re
 import ssl
 
 import certifi
-
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import urlencode
 
 try:
     import urllib3
 except ImportError:
-    raise ImportError("Swagger python client requires urllib3.")
+    raise ImportError('Swagger python client requires urllib3.')
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
+
     def __init__(self, resp):
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
@@ -46,14 +46,15 @@
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
         return self.urllib3_response.getheader(name, default)
 
 
 class RESTClientObject(object):
+
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
         # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
 
@@ -68,17 +69,15 @@
             ca_certs = configuration.ssl_ca_cert
         else:
             # if not set certificate file, use Mozilla's root certificates.
             ca_certs = certifi.where()
 
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
-            addition_pool_args[
-                "assert_hostname"
-            ] = configuration.assert_hostname  # noqa: E501
+            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
@@ -88,38 +87,30 @@
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
-                **addition_pool_args,
+                **addition_pool_args
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
-                **addition_pool_args,
+                **addition_pool_args
             )
 
-    def request(
-        self,
-        method,
-        url,
-        query_params=None,
-        headers=None,
-        body=None,
-        post_params=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
+    def request(self, method, url, query_params=None, headers=None,
+                body=None, post_params=None, _preload_content=True,
+                _request_timeout=None):
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param query_params: query parameters in the url
         :param headers: http request headers
         :param body: request json body, for `application/json`
@@ -131,113 +122,96 @@
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         """
         method = method.upper()
-        assert method in ["GET", "HEAD", "DELETE", "POST", "PUT", "PATCH", "OPTIONS"]
+        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
+                          'PATCH', 'OPTIONS']
 
         if post_params and body:
             raise ValueError(
                 "body parameter cannot be used with post_params parameter."
             )
 
         post_params = post_params or {}
         headers = headers or {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(
-                _request_timeout, (int,) if six.PY3 else (int, long)
-            ):  # noqa: E501,F821
+            if isinstance(_request_timeout, (int, ) if six.PY3 else (int, long)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
-            elif isinstance(_request_timeout, tuple) and len(_request_timeout) == 2:
+            elif (isinstance(_request_timeout, tuple) and
+                  len(_request_timeout) == 2):
                 timeout = urllib3.Timeout(
-                    connect=_request_timeout[0], read=_request_timeout[1]
-                )
+                    connect=_request_timeout[0], read=_request_timeout[1])
 
-        if "Content-Type" not in headers:
-            headers["Content-Type"] = "application/json"
+        if 'Content-Type' not in headers:
+            headers['Content-Type'] = 'application/json'
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
-            if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
+            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
                 if query_params:
-                    url += "?" + urlencode(query_params)
-                if re.search("json", headers["Content-Type"], re.IGNORECASE):
-                    request_body = "{}"
-                    if not isinstance(body, str):
+                    url += '?' + urlencode(query_params)
+                if re.search('json', headers['Content-Type'], re.IGNORECASE):
+                    request_body = '{}'
+                    if body is not None:
                         request_body = json.dumps(body)
-                    else:
-                        request_body = body
-
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
-                        headers=headers,
-                    )
-                elif (
-                    headers["Content-Type"] == "application/x-www-form-urlencoded"
-                ):  # noqa: E501
+                        headers=headers)
+                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         fields=post_params,
                         encode_multipart=False,
                         preload_content=_preload_content,
                         timeout=timeout,
-                        headers=headers,
-                    )
-                elif headers["Content-Type"] == "multipart/form-data":
+                        headers=headers)
+                elif headers['Content-Type'] == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
-                    del headers["Content-Type"]
+                    del headers['Content-Type']
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         fields=post_params,
                         encode_multipart=True,
                         preload_content=_preload_content,
                         timeout=timeout,
-                        headers=headers,
-                    )
+                        headers=headers)
                 # Pass a `string` parameter directly in the body to support
                 # other content types than Json when `body` argument is
                 # provided in serialized form
                 elif isinstance(body, str):
                     request_body = body
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
-                        headers=headers,
-                    )
+                        headers=headers)
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
-                r = self.pool_manager.request(
-                    method,
-                    url,
-                    fields=query_params,
-                    preload_content=_preload_content,
-                    timeout=timeout,
-                    headers=headers,
-                )
+                r = self.pool_manager.request(method, url,
+                                              fields=query_params,
+                                              preload_content=_preload_content,
+                                              timeout=timeout,
+                                              headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if _preload_content:
             r = RESTResponse(r)
 
@@ -245,168 +219,99 @@
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
             raise ApiException(http_resp=r)
 
         return r
 
-    def GET(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "GET",
-            url,
-            headers=headers,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            query_params=query_params,
-        )
-
-    def HEAD(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "HEAD",
-            url,
-            headers=headers,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            query_params=query_params,
-        )
-
-    def OPTIONS(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        post_params=None,
-        body=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "OPTIONS",
-            url,
-            headers=headers,
-            query_params=query_params,
-            post_params=post_params,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            body=body,
-        )
-
-    def DELETE(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        body=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "DELETE",
-            url,
-            headers=headers,
-            query_params=query_params,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            body=body,
-        )
-
-    def POST(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        post_params=None,
-        body=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "POST",
-            url,
-            headers=headers,
-            query_params=query_params,
-            post_params=post_params,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            body=body,
-        )
-
-    def PUT(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        post_params=None,
-        body=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "PUT",
-            url,
-            headers=headers,
-            query_params=query_params,
-            post_params=post_params,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            body=body,
-        )
-
-    def PATCH(
-        self,
-        url,
-        headers=None,
-        query_params=None,
-        post_params=None,
-        body=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        return self.request(
-            "PATCH",
-            url,
-            headers=headers,
-            query_params=query_params,
-            post_params=post_params,
-            _preload_content=_preload_content,
-            _request_timeout=_request_timeout,
-            body=body,
-        )
+    def GET(self, url, headers=None, query_params=None, _preload_content=True,
+            _request_timeout=None):
+        return self.request("GET", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
+             _request_timeout=None):
+        return self.request("HEAD", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
+                body=None, _preload_content=True, _request_timeout=None):
+        return self.request("OPTIONS", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def DELETE(self, url, headers=None, query_params=None, body=None,
+               _preload_content=True, _request_timeout=None):
+        return self.request("DELETE", url,
+                            headers=headers,
+                            query_params=query_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def POST(self, url, headers=None, query_params=None, post_params=None,
+             body=None, _preload_content=True, _request_timeout=None):
+        return self.request("POST", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def PUT(self, url, headers=None, query_params=None, post_params=None,
+            body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PUT", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def PATCH(self, url, headers=None, query_params=None, post_params=None,
+              body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PATCH", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
 
 
 class ApiException(Exception):
+
     def __init__(self, status=None, reason=None, http_resp=None):
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
             self.body = http_resp.data
             self.headers = http_resp.getheaders()
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
+        error_message = "({0})\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(self.headers)
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/__init__.py` & `timeplus-1.2.1/swagger_client/timeplus/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
-from swagger_client.timeplus.api_keys_v1beta1_api import APIKeysV1beta1Api
+from swagger_client.timeplus.api_keys_v1beta2_api import APIKeysV1beta2Api
+from swagger_client.timeplus.alerts_internal_api import AlertsInternalApi
+from swagger_client.timeplus.alerts_v1beta2_api import AlertsV1beta2Api
 from swagger_client.timeplus.dashboards_v1beta2_api import DashboardsV1beta2Api
 from swagger_client.timeplus.metrics_v1beta2_api import MetricsV1beta2Api
-from swagger_client.timeplus.queries_v1beta1_api import QueriesV1beta1Api
 from swagger_client.timeplus.queries_v1beta2_api import QueriesV1beta2Api
-from swagger_client.timeplus.sinks_v1beta1_api import SinksV1beta1Api
-from swagger_client.timeplus.sources_v1beta1_api import SourcesV1beta1Api
-from swagger_client.timeplus.streams_v1beta1_api import StreamsV1beta1Api
+from swagger_client.timeplus.sinks_internal_api import SinksInternalApi
+from swagger_client.timeplus.sinks_v1beta2_api import SinksV1beta2Api
+from swagger_client.timeplus.sources_v1beta2_api import SourcesV1beta2Api
+from swagger_client.timeplus.streams_v1beta2_api import StreamsV1beta2Api
 from swagger_client.timeplus.topology_v1beta2_api import TopologyV1beta2Api
-from swagger_client.timeplus.udfs_v1beta1_api import UDFsV1beta1Api
-from swagger_client.timeplus.views_v1beta1_api import ViewsV1beta1Api
+from swagger_client.timeplus.udfs_v1beta2_api import UDFsV1beta2Api
+from swagger_client.timeplus.views_v1beta2_api import ViewsV1beta2Api
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/api_keys_v1beta1_api.py` & `timeplus-1.2.1/swagger_client/timeplus/api_keys_v1beta2_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,54 +16,54 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class APIKeysV1beta1Api(object):
+class APIKeysV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta1_auth_api_keys_get(self, **kwargs):  # noqa: E501
+    def v1beta2_auth_api_keys_get(self, **kwargs):  # noqa: E501
         """List API keys  # noqa: E501
 
         list all API keys created by current user  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_auth_api_keys_get(async_req=True)
+        >>> thread = api.v1beta2_auth_api_keys_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: list[APIKey]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_auth_api_keys_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_auth_api_keys_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_auth_api_keys_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_auth_api_keys_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_auth_api_keys_get_with_http_info(self, **kwargs):  # noqa: E501
+    def v1beta2_auth_api_keys_get_with_http_info(self, **kwargs):  # noqa: E501
         """List API keys  # noqa: E501
 
         list all API keys created by current user  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_auth_api_keys_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_auth_api_keys_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: list[APIKey]
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -75,15 +75,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_auth_api_keys_get" % key
+                    " to method v1beta2_auth_api_keys_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -100,58 +100,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/auth/api_keys', 'GET',
+            '/v1beta2/auth/api_keys', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[APIKey]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_auth_api_keys_id_delete(self, id, **kwargs):  # noqa: E501
+    def v1beta2_auth_api_keys_id_delete(self, id, **kwargs):  # noqa: E501
         """Delete an API key  # noqa: E501
 
         delete the API key with the specified ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_auth_api_keys_id_delete(id, async_req=True)
+        >>> thread = api.v1beta2_auth_api_keys_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: API key ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_auth_api_keys_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_auth_api_keys_id_delete_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_auth_api_keys_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_auth_api_keys_id_delete_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_auth_api_keys_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_auth_api_keys_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
         """Delete an API key  # noqa: E501
 
         delete the API key with the specified ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_auth_api_keys_id_delete_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_auth_api_keys_id_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: API key ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -164,22 +164,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_auth_api_keys_id_delete" % key
+                    " to method v1beta2_auth_api_keys_id_delete" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_auth_api_keys_id_delete`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_auth_api_keys_id_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -195,58 +195,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/auth/api_keys/{id}', 'DELETE',
+            '/v1beta2/auth/api_keys/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_auth_api_keys_post(self, **kwargs):  # noqa: E501
+    def v1beta2_auth_api_keys_post(self, **kwargs):  # noqa: E501
         """Create an API key  # noqa: E501
 
         create a new API key with optional expiration, the created API key represents the owner thus has the same permissions as the owner  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_auth_api_keys_post(async_req=True)
+        >>> thread = api.v1beta2_auth_api_keys_post(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param CreateAPIKeyRequest body: API Key parameters
         :return: CreateAPIKeyResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_auth_api_keys_post_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_auth_api_keys_post_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_auth_api_keys_post_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_auth_api_keys_post_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_auth_api_keys_post_with_http_info(self, **kwargs):  # noqa: E501
+    def v1beta2_auth_api_keys_post_with_http_info(self, **kwargs):  # noqa: E501
         """Create an API key  # noqa: E501
 
         create a new API key with optional expiration, the created API key represents the owner thus has the same permissions as the owner  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_auth_api_keys_post_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_auth_api_keys_post_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param CreateAPIKeyRequest body: API Key parameters
         :return: CreateAPIKeyResponse
                  If the method is called asynchronously,
                  returns the request thread.
@@ -259,15 +259,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_auth_api_keys_post" % key
+                    " to method v1beta2_auth_api_keys_post" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -290,15 +290,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/auth/api_keys', 'POST',
+            '/v1beta2/auth/api_keys', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='CreateAPIKeyResponse',  # noqa: E501
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/dashboards_v1beta2_api.py` & `timeplus-1.2.1/swagger_client/timeplus/dashboards_v1beta2_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.v1beta2_dashboards_id_put(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UpdateDashboardRequest body: update dashboard request parameters (required)
         :param str id: dashboard ID (required)
-        :return: None
+        :return: DashboardDashboard
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.v1beta2_dashboards_id_put_with_http_info(body, id, **kwargs)  # noqa: E501
         else:
@@ -340,15 +340,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.v1beta2_dashboards_id_put_with_http_info(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UpdateDashboardRequest body: update dashboard request parameters (required)
         :param str id: dashboard ID (required)
-        :return: None
+        :return: DashboardDashboard
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body', 'id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -404,15 +404,15 @@
             '/v1beta2/dashboards/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type=None,  # noqa: E501
+            response_type='DashboardDashboard',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/metrics_v1beta2_api.py` & `timeplus-1.2.1/swagger_client/timeplus/metrics_v1beta2_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -115,94 +115,107 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta2_resource_metrics_get(self, body, **kwargs):  # noqa: E501
+    def v1beta2_resource_metrics_get(self, metrics_type, resource_ids, time_range, **kwargs):  # noqa: E501
         """query resource metrics.  # noqa: E501
 
         query resource metrics..  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_resource_metrics_get(body, async_req=True)
+        >>> thread = api.v1beta2_resource_metrics_get(metrics_type, resource_ids, time_range, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param ResourceMetricsRequest body: metrics query request parameters (required)
+        :param str metrics_type: (required)
+        :param list[str] resource_ids: (required)
+        :param int time_range: (required)
         :return: ResourceMetricsResult
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta2_resource_metrics_get_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_resource_metrics_get_with_http_info(metrics_type, resource_ids, time_range, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_resource_metrics_get_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_resource_metrics_get_with_http_info(metrics_type, resource_ids, time_range, **kwargs)  # noqa: E501
             return data
 
-    def v1beta2_resource_metrics_get_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_resource_metrics_get_with_http_info(self, metrics_type, resource_ids, time_range, **kwargs):  # noqa: E501
         """query resource metrics.  # noqa: E501
 
         query resource metrics..  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_resource_metrics_get_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_resource_metrics_get_with_http_info(metrics_type, resource_ids, time_range, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param ResourceMetricsRequest body: metrics query request parameters (required)
+        :param str metrics_type: (required)
+        :param list[str] resource_ids: (required)
+        :param int time_range: (required)
         :return: ResourceMetricsResult
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['metrics_type', 'resource_ids', 'time_range']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method v1beta2_resource_metrics_get" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'body' is set
-        if ('body' not in params or
-                params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta2_resource_metrics_get`")  # noqa: E501
+        # verify the required parameter 'metrics_type' is set
+        if ('metrics_type' not in params or
+                params['metrics_type'] is None):
+            raise ValueError("Missing the required parameter `metrics_type` when calling `v1beta2_resource_metrics_get`")  # noqa: E501
+        # verify the required parameter 'resource_ids' is set
+        if ('resource_ids' not in params or
+                params['resource_ids'] is None):
+            raise ValueError("Missing the required parameter `resource_ids` when calling `v1beta2_resource_metrics_get`")  # noqa: E501
+        # verify the required parameter 'time_range' is set
+        if ('time_range' not in params or
+                params['time_range'] is None):
+            raise ValueError("Missing the required parameter `time_range` when calling `v1beta2_resource_metrics_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'metrics_type' in params:
+            query_params.append(('metrics_type', params['metrics_type']))  # noqa: E501
+        if 'resource_ids' in params:
+            query_params.append(('resource_ids[]', params['resource_ids']))  # noqa: E501
+            collection_formats['resource_ids[]'] = 'csv'  # noqa: E501
+        if 'time_range' in params:
+            query_params.append(('time_range', params['time_range']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1beta2/resource-metrics', 'GET',
             path_params,
             query_params,
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/persistent_queries_v1beta2_api.py` & `timeplus-1.2.1/swagger_client/timeplus/sinks_v1beta2_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class PersistentQueriesV1beta2Api(object):
+class SinksV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta2_persistent_queries_get(self, **kwargs):  # noqa: E501
-        """list persistent-queries.  # noqa: E501
+    def v1beta2_sinks_get(self, **kwargs):  # noqa: E501
+        """list sinks  # noqa: E501
 
-        Get all persistent-queries.  # noqa: E501
+        Get all sinks  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_get(async_req=True)
+        >>> thread = api.v1beta2_sinks_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[QueryWithMetrics]
+        :return: list[Sink]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta2_persistent_queries_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_sinks_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_persistent_queries_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_sinks_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta2_persistent_queries_get_with_http_info(self, **kwargs):  # noqa: E501
-        """list persistent-queries.  # noqa: E501
+    def v1beta2_sinks_get_with_http_info(self, **kwargs):  # noqa: E501
+        """list sinks  # noqa: E501
 
-        Get all persistent-queries.  # noqa: E501
+        Get all sinks  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_sinks_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[QueryWithMetrics]
+        :return: list[Sink]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -75,15 +75,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta2_persistent_queries_get" % key
+                    " to method v1beta2_sinks_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -100,62 +100,62 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta2/persistent-queries', 'GET',
+            '/v1beta2/sinks', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[QueryWithMetrics]',  # noqa: E501
+            response_type='list[Sink]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta2_persistent_queries_id_data_get(self, id, **kwargs):  # noqa: E501
-        """stream persistent query result via websocket  # noqa: E501
+    def v1beta2_sinks_id_delete(self, id, **kwargs):  # noqa: E501
+        """delete a sink.  # noqa: E501
 
-        stream persistent query result via websocket  # noqa: E501
+        Delete a sink with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_id_data_get(id, async_req=True)
+        >>> thread = api.v1beta2_sinks_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: persistent query id (required)
+        :param str id: sink ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta2_persistent_queries_id_data_get_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sinks_id_delete_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_persistent_queries_id_data_get_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sinks_id_delete_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta2_persistent_queries_id_data_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """stream persistent query result via websocket  # noqa: E501
+    def v1beta2_sinks_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
+        """delete a sink.  # noqa: E501
 
-        stream persistent query result via websocket  # noqa: E501
+        Delete a sink with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_id_data_get_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sinks_id_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: persistent query id (required)
+        :param str id: sink ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
@@ -164,22 +164,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta2_persistent_queries_id_data_get" % key
+                    " to method v1beta2_sinks_id_delete" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta2_persistent_queries_id_data_get`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sinks_id_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -189,69 +189,69 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta2/persistent-queries/{id}/data', 'GET',
+            '/v1beta2/sinks/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta2_persistent_queries_id_delete(self, id, **kwargs):  # noqa: E501
-        """delete a persistent query.  # noqa: E501
+    def v1beta2_sinks_id_get(self, id, **kwargs):  # noqa: E501
+        """get a sink.  # noqa: E501
 
-        Delete the persistent query with the given ID.  # noqa: E501
+        Get a sink with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_id_delete(id, async_req=True)
+        >>> thread = api.v1beta2_sinks_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: persistent query ID (required)
-        :return: None
+        :param str id: sink ID (required)
+        :return: Sink
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta2_persistent_queries_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sinks_id_get_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_persistent_queries_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sinks_id_get_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta2_persistent_queries_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
-        """delete a persistent query.  # noqa: E501
+    def v1beta2_sinks_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
+        """get a sink.  # noqa: E501
 
-        Delete the persistent query with the given ID.  # noqa: E501
+        Get a sink with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_id_delete_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sinks_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: persistent query ID (required)
-        :return: None
+        :param str id: sink ID (required)
+        :return: Sink
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -259,22 +259,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta2_persistent_queries_id_delete" % key
+                    " to method v1beta2_sinks_id_get" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta2_persistent_queries_id_delete`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sinks_id_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -290,63 +290,63 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta2/persistent-queries/{id}', 'DELETE',
+            '/v1beta2/sinks/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type=None,  # noqa: E501
+            response_type='Sink',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta2_persistent_queries_id_get(self, id, **kwargs):  # noqa: E501
-        """get a persistent query.  # noqa: E501
+    def v1beta2_sinks_id_stop_post(self, id, **kwargs):  # noqa: E501
+        """stop a sink.  # noqa: E501
 
-        Get the persistent query with the given ID.  # noqa: E501
+        Stop the sink with the given ID from sending out data.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_id_get(id, async_req=True)
+        >>> thread = api.v1beta2_sinks_id_stop_post(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: persistent query ID (required)
-        :return: QueryWithMetrics
+        :param str id: sink ID (required)
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta2_persistent_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sinks_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_persistent_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sinks_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta2_persistent_queries_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """get a persistent query.  # noqa: E501
+    def v1beta2_sinks_id_stop_post_with_http_info(self, id, **kwargs):  # noqa: E501
+        """stop a sink.  # noqa: E501
 
-        Get the persistent query with the given ID.  # noqa: E501
+        Stop the sink with the given ID from sending out data.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sinks_id_stop_post_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: persistent query ID (required)
-        :return: QueryWithMetrics
+        :param str id: sink ID (required)
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -354,22 +354,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta2_persistent_queries_id_get" % key
+                    " to method v1beta2_sinks_id_stop_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta2_persistent_queries_id_get`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sinks_id_stop_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -385,63 +385,63 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta2/persistent-queries/{id}', 'GET',
+            '/v1beta2/sinks/{id}/stop', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='QueryWithMetrics',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta2_persistent_queries_post(self, body, **kwargs):  # noqa: E501
-        """execute a persistent query.  # noqa: E501
+    def v1beta2_sinks_post(self, body, **kwargs):  # noqa: E501
+        """create a sink.  # noqa: E501
 
-        execute a persistent query.  # noqa: E501
+        Create a sink.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_post(body, async_req=True)
+        >>> thread = api.v1beta2_sinks_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreatePersistentQueryRequest body: persistent query request parameters (required)
-        :return: Query
+        :param CreateSinkRequest body: create sink request parameters (required)
+        :return: Sink
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta2_persistent_queries_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_sinks_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_persistent_queries_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sinks_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta2_persistent_queries_post_with_http_info(self, body, **kwargs):  # noqa: E501
-        """execute a persistent query.  # noqa: E501
+    def v1beta2_sinks_post_with_http_info(self, body, **kwargs):  # noqa: E501
+        """create a sink.  # noqa: E501
 
-        execute a persistent query.  # noqa: E501
+        Create a sink.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_persistent_queries_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_sinks_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreatePersistentQueryRequest body: persistent query request parameters (required)
-        :return: Query
+        :param CreateSinkRequest body: create sink request parameters (required)
+        :return: Sink
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -449,22 +449,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta2_persistent_queries_post" % key
+                    " to method v1beta2_sinks_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta2_persistent_queries_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_sinks_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -484,21 +484,21 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta2/persistent-queries', 'POST',
+            '/v1beta2/sinks', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Query',  # noqa: E501
+            response_type='Sink',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/queries_v1beta1_api.py` & `timeplus-1.2.1/swagger_client/timeplus/queries_v1beta2_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,55 +16,55 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class QueriesV1beta1Api(object):
+class QueriesV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta1_format_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_format_post(self, body, **kwargs):  # noqa: E501
         """format a query.  # noqa: E501
 
         Format the given query and make it easy to read.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_format_post(body, async_req=True)
+        >>> thread = api.v1beta2_format_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param FormatQueryRequest body: the query SQL to be formatted (required)
         :return: FormatQueryResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_format_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_format_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_format_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_format_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_format_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_format_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """format a query.  # noqa: E501
 
         Format the given query and make it easy to read.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_format_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_format_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param FormatQueryRequest body: the query SQL to be formatted (required)
         :return: FormatQueryResponse
                  If the method is called asynchronously,
                  returns the request thread.
@@ -77,22 +77,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_format_post" % key
+                    " to method v1beta2_format_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_format_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_format_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -102,96 +102,100 @@
         local_var_files = {}
 
         body_params = None
         if 'body' in params:
             body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['application/json', 'text/event-stream'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/format', 'POST',
+            '/v1beta2/format', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='FormatQueryResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_queries_get(self, **kwargs):  # noqa: E501
+    def v1beta2_queries_get(self, **kwargs):  # noqa: E501
         """list queries.  # noqa: E501
 
         Get all queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_get(async_req=True)
+        >>> thread = api.v1beta2_queries_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
+        :param str tag: filter by tag
         :return: list[Query]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_queries_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_queries_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_queries_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_queries_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_queries_get_with_http_info(self, **kwargs):  # noqa: E501
+    def v1beta2_queries_get_with_http_info(self, **kwargs):  # noqa: E501
         """list queries.  # noqa: E501
 
         Get all queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_queries_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
+        :param str tag: filter by tag
         :return: list[Query]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = []  # noqa: E501
+        all_params = ['tag']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_queries_get" % key
+                    " to method v1beta2_queries_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'tag' in params:
+            query_params.append(('tag', params['tag']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -199,58 +203,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/queries', 'GET',
+            '/v1beta2/queries', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[Query]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_queries_id_cancel_post(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_cancel_post(self, id, **kwargs):  # noqa: E501
         """cancel a query.  # noqa: E501
 
         Cancel the query with the given ID. If given query is not running, the request will do nothing. Otherwise, the query will be canceled and the `status` will be set to `canceled`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_cancel_post(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_cancel_post(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_queries_id_cancel_post_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_queries_id_cancel_post_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_queries_id_cancel_post_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_queries_id_cancel_post_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_queries_id_cancel_post_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_cancel_post_with_http_info(self, id, **kwargs):  # noqa: E501
         """cancel a query.  # noqa: E501
 
         Cancel the query with the given ID. If given query is not running, the request will do nothing. Otherwise, the query will be canceled and the `status` will be set to `canceled`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_cancel_post_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_cancel_post_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -263,22 +267,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_queries_id_cancel_post" % key
+                    " to method v1beta2_queries_id_cancel_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_queries_id_cancel_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_queries_id_cancel_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -294,58 +298,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/queries/{id}/cancel', 'POST',
+            '/v1beta2/queries/{id}/cancel', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_queries_id_delete(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_delete(self, id, **kwargs):  # noqa: E501
         """delete a query.  # noqa: E501
 
         Delete the query with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_delete(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_queries_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_queries_id_delete_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_queries_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_queries_id_delete_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_queries_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
         """delete a query.  # noqa: E501
 
         Delete the query with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_delete_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -358,22 +362,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_queries_id_delete" % key
+                    " to method v1beta2_queries_id_delete" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_queries_id_delete`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_queries_id_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -389,58 +393,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/queries/{id}', 'DELETE',
+            '/v1beta2/queries/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_queries_id_get(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_get(self, id, **kwargs):  # noqa: E501
         """get a query.  # noqa: E501
 
         Get the query with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_get(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: Query
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_queries_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
         """get a query.  # noqa: E501
 
         Get the query with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: Query
                  If the method is called asynchronously,
                  returns the request thread.
@@ -453,22 +457,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_queries_id_get" % key
+                    " to method v1beta2_queries_id_get" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_queries_id_get`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_queries_id_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -484,58 +488,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/queries/{id}', 'GET',
+            '/v1beta2/queries/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Query',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_queries_id_pipeline_get(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_pipeline_get(self, id, **kwargs):  # noqa: E501
         """get the pipeline for a query  # noqa: E501
 
         get the pipeline for a query  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_pipeline_get(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_pipeline_get(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: QueryPipeline
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_queries_id_pipeline_get_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_queries_id_pipeline_get_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_queries_id_pipeline_get_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_queries_id_pipeline_get_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_queries_id_pipeline_get_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_queries_id_pipeline_get_with_http_info(self, id, **kwargs):  # noqa: E501
         """get the pipeline for a query  # noqa: E501
 
         get the pipeline for a query  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_id_pipeline_get_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_queries_id_pipeline_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: query ID (required)
         :return: QueryPipeline
                  If the method is called asynchronously,
                  returns the request thread.
@@ -548,22 +552,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_queries_id_pipeline_get" % key
+                    " to method v1beta2_queries_id_pipeline_get" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_queries_id_pipeline_get`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_queries_id_pipeline_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -579,63 +583,63 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/queries/{id}/pipeline', 'GET',
+            '/v1beta2/queries/{id}/pipeline', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='QueryPipeline',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_queries_post(self, body, **kwargs):  # noqa: E501
-        """execute a query.  # noqa: E501
+    def v1beta2_queries_post(self, body, **kwargs):  # noqa: E501
+        """execute a query and return the results.  # noqa: E501
 
-        execute a query.  # noqa: E501
+        Execute a query and return the results. * If the request fails, the response content type will be `application/json`. Please refer to the failure codes in Responses section below. * If the query is executed successfully, the response content type will be `text/event-stream`. **For SSE** There are 3 types of data that will be sent to SSE channel 1. Query (type `query`): The first event of the result will ALWAYS be this type. 2. Metrics (type `metrics`): The query metrics in JSON. They will be sent every 1 seconds. 3. Data (the type is empty): The query result.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_post(body, async_req=True)
+        >>> thread = api.v1beta2_queries_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateQueryRequestV1Beta1 body: query request parameters (required)
-        :return: CreateQueryResponse
+        :param CreateQueryRequestV1Beta2 body: query request parameters (required)
+        :return: Query
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_queries_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_queries_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_queries_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_queries_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_queries_post_with_http_info(self, body, **kwargs):  # noqa: E501
-        """execute a query.  # noqa: E501
+    def v1beta2_queries_post_with_http_info(self, body, **kwargs):  # noqa: E501
+        """execute a query and return the results.  # noqa: E501
 
-        execute a query.  # noqa: E501
+        Execute a query and return the results. * If the request fails, the response content type will be `application/json`. Please refer to the failure codes in Responses section below. * If the query is executed successfully, the response content type will be `text/event-stream`. **For SSE** There are 3 types of data that will be sent to SSE channel 1. Query (type `query`): The first event of the result will ALWAYS be this type. 2. Metrics (type `metrics`): The query metrics in JSON. They will be sent every 1 seconds. 3. Data (the type is empty): The query result.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_queries_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_queries_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateQueryRequestV1Beta1 body: query request parameters (required)
-        :return: CreateQueryResponse
+        :param CreateQueryRequestV1Beta2 body: query request parameters (required)
+        :return: Query
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -643,22 +647,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_queries_post" % key
+                    " to method v1beta2_queries_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_queries_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_queries_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -668,68 +672,68 @@
         local_var_files = {}
 
         body_params = None
         if 'body' in params:
             body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['application/json', 'text/event-stream'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/queries', 'POST',
+            '/v1beta2/queries', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CreateQueryResponse',  # noqa: E501
+            response_type='Query',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sqlanalyze_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_sqlanalyze_post(self, body, **kwargs):  # noqa: E501
         """analyze sql  # noqa: E501
 
         analyze sql  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sqlanalyze_post(body, async_req=True)
+        >>> thread = api.v1beta2_sqlanalyze_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param AnalyzeSQLRequest body: sql request parameters (required)
         :return: SQLAnalyzeResult
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sqlanalyze_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_sqlanalyze_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sqlanalyze_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sqlanalyze_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sqlanalyze_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_sqlanalyze_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """analyze sql  # noqa: E501
 
         analyze sql  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sqlanalyze_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_sqlanalyze_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param AnalyzeSQLRequest body: sql request parameters (required)
         :return: SQLAnalyzeResult
                  If the method is called asynchronously,
                  returns the request thread.
@@ -742,22 +746,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sqlanalyze_post" % key
+                    " to method v1beta2_sqlanalyze_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_sqlanalyze_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_sqlanalyze_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -777,116 +781,21 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sqlanalyze', 'POST',
+            '/v1beta2/sqlanalyze', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='SQLAnalyzeResult',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
-
-    def ws_queries_id_get(self, id, **kwargs):  # noqa: E501
-        """stream query result via websocket [THIS API DOESN'T HAVE `v1beta1` IN PATH]  # noqa: E501
-
-        stream query result via websocket  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ws_queries_id_get(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str id: query id (required)
-        :return: None
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.ws_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
-        else:
-            (data) = self.ws_queries_id_get_with_http_info(id, **kwargs)  # noqa: E501
-            return data
-
-    def ws_queries_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """stream query result via websocket [THIS API DOESN'T HAVE `v1beta1` IN PATH]  # noqa: E501
-
-        stream query result via websocket  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ws_queries_id_get_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str id: query id (required)
-        :return: None
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['id']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method ws_queries_id_get" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'id' is set
-        if ('id' not in params or
-                params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `ws_queries_id_get`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in params:
-            path_params['id'] = params['id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = []  # noqa: E501
-
-        return self.api_client.call_api(
-            '/ws/queries/{id}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type=None,  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/queries_v1beta2_api.py` & `timeplus-1.2.1/swagger_client/timeplus/alerts_v1beta2_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,128 +16,113 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class QueriesV1beta2Api(object):
+class AlertsV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta2_queries_post(self, body, **kwargs):  # noqa: E501
-        """execute a query and return the results.  # noqa: E501
+    def v1beta2_alerts_id_stop_post(self, id, **kwargs):  # noqa: E501
+        """stop an alert.  # noqa: E501
 
-        Execute a query and return the results. * If the request fails, the response content type will be `application/json`. Please refer to the failure codes in Responses section below. * If the query is executed successfully, the response content type will be `text/event-stream`. **For SSE** There are 3 types of data that will be sent to SSE channel 1. Query (type `query`): The first event of the result will ALWAYS be this type. 2. Metrics (type `metrics`): The query metrics in JSON. They will be sent every 1 seconds. 3. Data (the type is empty): The query result.  # noqa: E501
+        Stop the alert with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_queries_post(body, async_req=True)
+        >>> thread = api.v1beta2_alerts_id_stop_post(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateQueryRequestV1Beta2 body: query request parameters (required)
-        :return: Query
+        :param str id: alert ID (required)
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
-        kwargs["_return_http_data_only"] = True
-        if kwargs.get("async_req"):
-            return self.v1beta2_queries_post_with_http_info(
-                body, **kwargs
-            )  # noqa: E501
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.v1beta2_alerts_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta2_queries_post_with_http_info(
-                body, **kwargs
-            )  # noqa: E501
+            (data) = self.v1beta2_alerts_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta2_queries_post_with_http_info(self, body, **kwargs):  # noqa: E501
-        """execute a query and return the results.  # noqa: E501
+    def v1beta2_alerts_id_stop_post_with_http_info(self, id, **kwargs):  # noqa: E501
+        """stop an alert.  # noqa: E501
 
-        Execute a query and return the results. * If the request fails, the response content type will be `application/json`. Please refer to the failure codes in Responses section below. * If the query is executed successfully, the response content type will be `text/event-stream`. **For SSE** There are 3 types of data that will be sent to SSE channel 1. Query (type `query`): The first event of the result will ALWAYS be this type. 2. Metrics (type `metrics`): The query metrics in JSON. They will be sent every 1 seconds. 3. Data (the type is empty): The query result.  # noqa: E501
+        Stop the alert with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta2_queries_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_alerts_id_stop_post_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateQueryRequestV1Beta2 body: query request parameters (required)
-        :return: Query
+        :param str id: alert ID (required)
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ["body"]  # noqa: E501
-        all_params.append("async_req")
-        all_params.append("_return_http_data_only")
-        all_params.append("_preload_content")
-        all_params.append("_request_timeout")
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         params = locals()
-        for key, val in six.iteritems(params["kwargs"]):
+        for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta2_queries_post" % key
+                    " to method v1beta2_alerts_id_stop_post" % key
                 )
             params[key] = val
-        del params["kwargs"]
-        # verify the required parameter 'body' is set
-        if "body" not in params or params["body"] is None:
-            raise ValueError(
-                "Missing the required parameter `body` when calling `v1beta2_queries_post`"
-            )  # noqa: E501
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_alerts_id_stop_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if "body" in params:
-            body_params = params["body"]
         # HTTP header `Accept`
-        header_params["Accept"] = self.api_client.select_header_accept(
-            ["application/json", "text/event-stream"]
-        )  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params[
-            "Content-Type"
-        ] = self.api_client.select_header_content_type(  # noqa: E501
-            ["application/json"]
-        )  # noqa: E501
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ["ApiKeyAuth"]  # noqa: E501
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            "/v1beta2/queries",
-            "POST",
+            '/v1beta2/alerts/{id}/stop', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type="Query",  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
-            async_req=params.get("async_req"),
-            _return_http_data_only=params.get("_return_http_data_only"),
-            _preload_content=params.get("_preload_content", False),
-            _request_timeout=params.get("_request_timeout"),
-            collection_formats=collection_formats,
-        )
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/sinks_v1beta1_api.py` & `timeplus-1.2.1/swagger_client/timeplus/udfs_v1beta2_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,58 +16,58 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class SinksV1beta1Api(object):
+class UDFsV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta1_sinks_get(self, **kwargs):  # noqa: E501
-        """list sinks  # noqa: E501
+    def v1beta2_udfs_get(self, **kwargs):  # noqa: E501
+        """list udf.  # noqa: E501
 
-        Get all sinks  # noqa: E501
+        Get all udf.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_get(async_req=True)
+        >>> thread = api.v1beta2_udfs_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[Sink]
+        :return: list[UDF]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sinks_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_udfs_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sinks_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_udfs_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sinks_get_with_http_info(self, **kwargs):  # noqa: E501
-        """list sinks  # noqa: E501
+    def v1beta2_udfs_get_with_http_info(self, **kwargs):  # noqa: E501
+        """list udf.  # noqa: E501
 
-        Get all sinks  # noqa: E501
+        Get all udf.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_udfs_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[Sink]
+        :return: list[UDF]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -75,15 +75,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sinks_get" % key
+                    " to method v1beta2_udfs_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -100,92 +100,92 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sinks', 'GET',
+            '/v1beta2/udfs', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[Sink]',  # noqa: E501
+            response_type='list[UDF]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sinks_id_delete(self, id, **kwargs):  # noqa: E501
-        """delete a sink.  # noqa: E501
+    def v1beta2_udfs_name_delete(self, name, **kwargs):  # noqa: E501
+        """delete a udf.  # noqa: E501
 
-        Delete a sink with the given ID.  # noqa: E501
+        Delete the udf with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_id_delete(id, async_req=True)
+        >>> thread = api.v1beta2_udfs_name_delete(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: sink ID (required)
+        :param str name: udf name (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sinks_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_udfs_name_delete_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sinks_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_udfs_name_delete_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sinks_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
-        """delete a sink.  # noqa: E501
+    def v1beta2_udfs_name_delete_with_http_info(self, name, **kwargs):  # noqa: E501
+        """delete a udf.  # noqa: E501
 
-        Delete a sink with the given ID.  # noqa: E501
+        Delete the udf with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_id_delete_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_udfs_name_delete_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: sink ID (required)
+        :param str name: udf name (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['id']  # noqa: E501
+        all_params = ['name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sinks_id_delete" % key
+                    " to method v1beta2_udfs_name_delete" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'id' is set
-        if ('id' not in params or
-                params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sinks_id_delete`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_udfs_name_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in params:
-            path_params['id'] = params['id']  # noqa: E501
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -195,92 +195,92 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sinks/{id}', 'DELETE',
+            '/v1beta2/udfs/{name}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sinks_id_get(self, id, **kwargs):  # noqa: E501
-        """get a sink.  # noqa: E501
+    def v1beta2_udfs_name_get(self, name, **kwargs):  # noqa: E501
+        """get a udf.  # noqa: E501
 
-        Get a sink with the given ID.  # noqa: E501
+        get the udf with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_id_get(id, async_req=True)
+        >>> thread = api.v1beta2_udfs_name_get(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: sink ID (required)
-        :return: Sink
+        :param str name: udf name (required)
+        :return: UDF
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sinks_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_udfs_name_get_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sinks_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_udfs_name_get_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sinks_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """get a sink.  # noqa: E501
+    def v1beta2_udfs_name_get_with_http_info(self, name, **kwargs):  # noqa: E501
+        """get a udf.  # noqa: E501
 
-        Get a sink with the given ID.  # noqa: E501
+        get the udf with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_udfs_name_get_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str id: sink ID (required)
-        :return: Sink
+        :param str name: udf name (required)
+        :return: UDF
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['id']  # noqa: E501
+        all_params = ['name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sinks_id_get" % key
+                    " to method v1beta2_udfs_name_get" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'id' is set
-        if ('id' not in params or
-                params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sinks_id_get`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_udfs_name_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'id' in params:
-            path_params['id'] = params['id']  # noqa: E501
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -290,63 +290,63 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sinks/{id}', 'GET',
+            '/v1beta2/udfs/{name}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Sink',  # noqa: E501
+            response_type='UDF',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sinks_post(self, body, **kwargs):  # noqa: E501
-        """create a sink.  # noqa: E501
+    def v1beta2_udfs_name_put(self, body, **kwargs):  # noqa: E501
+        """update a udf.  # noqa: E501
 
-        Create a sink.  # noqa: E501
+        Update a udf.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_post(body, async_req=True)
+        >>> thread = api.v1beta2_udfs_name_put(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateSinkRequest body: create sink request parameters (required)
-        :return: Sink
+        :param UDF body: update udf request parameters (required)
+        :return: UDF
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sinks_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_udfs_name_put_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sinks_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_udfs_name_put_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sinks_post_with_http_info(self, body, **kwargs):  # noqa: E501
-        """create a sink.  # noqa: E501
+    def v1beta2_udfs_name_put_with_http_info(self, body, **kwargs):  # noqa: E501
+        """update a udf.  # noqa: E501
 
-        Create a sink.  # noqa: E501
+        Update a udf.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sinks_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_udfs_name_put_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param CreateSinkRequest body: create sink request parameters (required)
-        :return: Sink
+        :param UDF body: update udf request parameters (required)
+        :return: UDF
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -354,22 +354,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sinks_post" % key
+                    " to method v1beta2_udfs_name_put" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_sinks_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_udfs_name_put`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -389,21 +389,120 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sinks', 'POST',
+            '/v1beta2/udfs/{name}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Sink',  # noqa: E501
+            response_type='UDF',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def v1beta2_udfs_post(self, body, **kwargs):  # noqa: E501
+        """create a udf.  # noqa: E501
+
+        Create a udf.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_udfs_post(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param UDF body: create udf request parameters (required)
+        :return: UDF
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.v1beta2_udfs_post_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.v1beta2_udfs_post_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def v1beta2_udfs_post_with_http_info(self, body, **kwargs):  # noqa: E501
+        """create a udf.  # noqa: E501
+
+        Create a udf.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_udfs_post_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param UDF body: create udf request parameters (required)
+        :return: UDF
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1beta2_udfs_post" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_udfs_post`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1beta2/udfs', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='UDF',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/sources_v1beta1_api.py` & `timeplus-1.2.1/swagger_client/timeplus/sources_v1beta2_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,55 +16,55 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class SourcesV1beta1Api(object):
+class SourcesV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta1_source_infer_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_infer_post(self, body, **kwargs):  # noqa: E501
         """infer schema from an existing event  # noqa: E501
 
         infer schema from an existing event  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_infer_post(body, async_req=True)
+        >>> thread = api.v1beta2_source_infer_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param EventInferRequest body: events used to infer schema (required)
         :return: list[EventInferResponse]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_source_infer_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_source_infer_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_source_infer_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_source_infer_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_source_infer_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_infer_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """infer schema from an existing event  # noqa: E501
 
         infer schema from an existing event  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_infer_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_source_infer_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param EventInferRequest body: events used to infer schema (required)
         :return: list[EventInferResponse]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -77,22 +77,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_source_infer_post" % key
+                    " to method v1beta2_source_infer_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_source_infer_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_source_infer_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -112,58 +112,58 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/source/infer', 'POST',
+            '/v1beta2/source/infer', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[EventInferResponse]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_source_match_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_match_post(self, body, **kwargs):  # noqa: E501
         """return streams match provided events  # noqa: E501
 
         return streams match provided events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_match_post(body, async_req=True)
+        >>> thread = api.v1beta2_source_match_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param StreamMatchRequest body: events to match (required)
         :return: list[str]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_source_match_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_source_match_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_source_match_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_source_match_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_source_match_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_match_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """return streams match provided events  # noqa: E501
 
         return streams match provided events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_match_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_source_match_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param StreamMatchRequest body: events to match (required)
         :return: list[str]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -176,22 +176,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_source_match_post" % key
+                    " to method v1beta2_source_match_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_source_match_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_source_match_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -211,58 +211,58 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/source/match', 'POST',
+            '/v1beta2/source/match', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[str]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_source_preview_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_preview_post(self, body, **kwargs):  # noqa: E501
         """preview a source.  # noqa: E501
 
         Get sample events from the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_preview_post(body, async_req=True)
+        >>> thread = api.v1beta2_source_preview_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SourcePreviewRequest body: source propeties for preview (required)
         :return: list[Event]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_source_preview_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_source_preview_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_source_preview_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_source_preview_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_source_preview_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_preview_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """preview a source.  # noqa: E501
 
         Get sample events from the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_preview_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_source_preview_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SourcePreviewRequest body: source propeties for preview (required)
         :return: list[Event]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -275,22 +275,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_source_preview_post" % key
+                    " to method v1beta2_source_preview_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_source_preview_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_source_preview_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -310,58 +310,58 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/source/preview', 'POST',
+            '/v1beta2/source/preview', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[Event]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_source_upload_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_upload_post(self, body, **kwargs):  # noqa: E501
         """upload a file  # noqa: E501
 
         Upload a file to the system.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_upload_post(body, async_req=True)
+        >>> thread = api.v1beta2_source_upload_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SourceUploadBody body: (required)
         :return: FileUploadResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_source_upload_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_source_upload_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_source_upload_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_source_upload_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_source_upload_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_source_upload_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """upload a file  # noqa: E501
 
         Upload a file to the system.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_source_upload_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_source_upload_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SourceUploadBody body: (required)
         :return: FileUploadResponse
                  If the method is called asynchronously,
                  returns the request thread.
@@ -374,22 +374,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_source_upload_post" % key
+                    " to method v1beta2_source_upload_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_source_upload_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_source_upload_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -409,57 +409,57 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/source/upload', 'POST',
+            '/v1beta2/source/upload', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='FileUploadResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_get(self, **kwargs):  # noqa: E501
+    def v1beta2_sources_get(self, **kwargs):  # noqa: E501
         """list sources.  # noqa: E501
 
         Get all sources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_get(async_req=True)
+        >>> thread = api.v1beta2_sources_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: list[Source]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_sources_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_get_with_http_info(self, **kwargs):  # noqa: E501
+    def v1beta2_sources_get_with_http_info(self, **kwargs):  # noqa: E501
         """list sources.  # noqa: E501
 
         Get all sources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_sources_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: list[Source]
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -471,15 +471,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_get" % key
+                    " to method v1beta2_sources_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -496,58 +496,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources', 'GET',
+            '/v1beta2/sources', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[Source]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_id_delete(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_delete(self, id, **kwargs):  # noqa: E501
         """delete a source.  # noqa: E501
 
         Delete the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_delete(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sources_id_delete_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_id_delete_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_id_delete_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_delete_with_http_info(self, id, **kwargs):  # noqa: E501
         """delete a source.  # noqa: E501
 
         Delete the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_delete_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -560,22 +560,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_id_delete" % key
+                    " to method v1beta2_sources_id_delete" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sources_id_delete`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sources_id_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -591,58 +591,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources/{id}', 'DELETE',
+            '/v1beta2/sources/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_id_get(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_get(self, id, **kwargs):  # noqa: E501
         """get a source.  # noqa: E501
 
         Get a source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_get(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: Source
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sources_id_get_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_id_get_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_id_get_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
         """get a source.  # noqa: E501
 
         Get a source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: Source
                  If the method is called asynchronously,
                  returns the request thread.
@@ -655,22 +655,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_id_get" % key
+                    " to method v1beta2_sources_id_get" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sources_id_get`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sources_id_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -686,65 +686,65 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources/{id}', 'GET',
+            '/v1beta2/sources/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Source',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_id_put(self, body, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_put(self, body, id, **kwargs):  # noqa: E501
         """Update a source.  # noqa: E501
 
         Update the specific source with the given ID. Only stopped sources can be updated.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_put(body, id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_put(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UpdateSourceRequest body: update source request parameters (required)
         :param str id: source ID (required)
-        :return: None
+        :return: Source
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_id_put_with_http_info(body, id, **kwargs)  # noqa: E501
+            return self.v1beta2_sources_id_put_with_http_info(body, id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_id_put_with_http_info(body, id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_id_put_with_http_info(body, id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_id_put_with_http_info(self, body, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_put_with_http_info(self, body, id, **kwargs):  # noqa: E501
         """Update a source.  # noqa: E501
 
         Update the specific source with the given ID. Only stopped sources can be updated.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_put_with_http_info(body, id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_put_with_http_info(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UpdateSourceRequest body: update source request parameters (required)
         :param str id: source ID (required)
-        :return: None
+        :return: Source
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body', 'id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -752,26 +752,26 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_id_put" % key
+                    " to method v1beta2_sources_id_put" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_sources_id_put`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_sources_id_put`")  # noqa: E501
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sources_id_put`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sources_id_put`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -793,58 +793,58 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources/{id}', 'PUT',
+            '/v1beta2/sources/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type=None,  # noqa: E501
+            response_type='Source',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_id_start_post(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_start_post(self, id, **kwargs):  # noqa: E501
         """start a source.  # noqa: E501
 
         Start the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_start_post(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_start_post(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_id_start_post_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sources_id_start_post_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_id_start_post_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_id_start_post_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_id_start_post_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_start_post_with_http_info(self, id, **kwargs):  # noqa: E501
         """start a source.  # noqa: E501
 
         Start the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_start_post_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_start_post_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -857,22 +857,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_id_start_post" % key
+                    " to method v1beta2_sources_id_start_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sources_id_start_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sources_id_start_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -888,58 +888,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources/{id}/start', 'POST',
+            '/v1beta2/sources/{id}/start', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_id_stop_post(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_stop_post(self, id, **kwargs):  # noqa: E501
         """stop a source.  # noqa: E501
 
         Stop the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_stop_post(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_stop_post(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
+            return self.v1beta2_sources_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_id_stop_post_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_id_stop_post_with_http_info(self, id, **kwargs):  # noqa: E501
+    def v1beta2_sources_id_stop_post_with_http_info(self, id, **kwargs):  # noqa: E501
         """stop a source.  # noqa: E501
 
         Stop the source with the given ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_id_stop_post_with_http_info(id, async_req=True)
+        >>> thread = api.v1beta2_sources_id_stop_post_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: source ID (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -952,22 +952,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_id_stop_post" % key
+                    " to method v1beta2_sources_id_stop_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
-            raise ValueError("Missing the required parameter `id` when calling `v1beta1_sources_id_stop_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `id` when calling `v1beta2_sources_id_stop_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
 
@@ -983,58 +983,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources/{id}/stop', 'POST',
+            '/v1beta2/sources/{id}/stop', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_sources_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_sources_post(self, body, **kwargs):  # noqa: E501
         """create a source.  # noqa: E501
 
         Create a source.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_post(body, async_req=True)
+        >>> thread = api.v1beta2_sources_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param CreateSourceRequest body: create source request parameters (required)
         :return: Source
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_sources_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_sources_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_sources_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_sources_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_sources_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_sources_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """create a source.  # noqa: E501
 
         Create a source.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_sources_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_sources_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param CreateSourceRequest body: create source request parameters (required)
         :return: Source
                  If the method is called asynchronously,
                  returns the request thread.
@@ -1047,22 +1047,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_sources_post" % key
+                    " to method v1beta2_sources_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_sources_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_sources_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -1082,15 +1082,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/sources', 'POST',
+            '/v1beta2/sources', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Source',  # noqa: E501
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/streams_v1beta1_api.py` & `timeplus-1.2.1/swagger_client/timeplus/streams_v1beta2_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,55 +16,55 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class StreamsV1beta1Api(object):
+class StreamsV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta1_streams_external_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_streams_external_post(self, body, **kwargs):  # noqa: E501
         """create an external stream.  # noqa: E501
 
         Create an external stream.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_external_post(body, async_req=True)
+        >>> thread = api.v1beta2_streams_external_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ExternalStreamDef body: create external stream request parameters (required)
         :return: ExternalStreamDef
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_streams_external_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_streams_external_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_streams_external_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_streams_external_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_streams_external_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_streams_external_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """create an external stream.  # noqa: E501
 
         Create an external stream.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_external_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_streams_external_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ExternalStreamDef body: create external stream request parameters (required)
         :return: ExternalStreamDef
                  If the method is called asynchronously,
                  returns the request thread.
@@ -77,22 +77,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_streams_external_post" % key
+                    " to method v1beta2_streams_external_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_streams_external_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_streams_external_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -112,57 +112,57 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/streams/external', 'POST',
+            '/v1beta2/streams/external', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='ExternalStreamDef',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_streams_get(self, **kwargs):  # noqa: E501
+    def v1beta2_streams_get(self, **kwargs):  # noqa: E501
         """list streams.  # noqa: E501
 
         Get all streams.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_get(async_req=True)
+        >>> thread = api.v1beta2_streams_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: list[Stream]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_streams_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_streams_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_streams_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_streams_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_streams_get_with_http_info(self, **kwargs):  # noqa: E501
+    def v1beta2_streams_get_with_http_info(self, **kwargs):  # noqa: E501
         """list streams.  # noqa: E501
 
         Get all streams.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_streams_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: list[Stream]
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -174,15 +174,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_streams_get" % key
+                    " to method v1beta2_streams_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -199,58 +199,58 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/streams', 'GET',
+            '/v1beta2/streams', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='list[Stream]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_streams_name_delete(self, name, **kwargs):  # noqa: E501
+    def v1beta2_streams_name_delete(self, name, **kwargs):  # noqa: E501
         """delete a stream.  # noqa: E501
 
         Delete the stream with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_name_delete(name, async_req=True)
+        >>> thread = api.v1beta2_streams_name_delete(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: stream name (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_streams_name_delete_with_http_info(name, **kwargs)  # noqa: E501
+            return self.v1beta2_streams_name_delete_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_streams_name_delete_with_http_info(name, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_streams_name_delete_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_streams_name_delete_with_http_info(self, name, **kwargs):  # noqa: E501
+    def v1beta2_streams_name_delete_with_http_info(self, name, **kwargs):  # noqa: E501
         """delete a stream.  # noqa: E501
 
         Delete the stream with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_name_delete_with_http_info(name, async_req=True)
+        >>> thread = api.v1beta2_streams_name_delete_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str name: stream name (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
@@ -263,22 +263,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_streams_name_delete" % key
+                    " to method v1beta2_streams_name_delete" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `v1beta1_streams_name_delete`")  # noqa: E501
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_streams_name_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'name' in params:
             path_params['name'] = params['name']  # noqa: E501
 
@@ -294,60 +294,60 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/streams/{name}', 'DELETE',
+            '/v1beta2/streams/{name}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_streams_name_ingest_post(self, body, name, **kwargs):  # noqa: E501
+    def v1beta2_streams_name_ingest_post(self, body, name, **kwargs):  # noqa: E501
         """ingest data.  # noqa: E501
 
-        Ingest data to a stream with the given name. For formats are supported: * compact JSON: when `Content-Type` is set to one of `application/json`, `application/json;format=compact`, `application/vnd.timeplus+json`, `application/vnd.timeplus+json;format=compat`, or set `format` query parameter with value `compact`. And this is the API's default format. * JSON stream: when `Content-Type` is set to one of `application/json;format=streaming`, `application/vnd.timeplus+json;format=streaming`, or set `format` query parameter with value `streaming`. * raw string: when `Content-Type` is set to one of `text/plain`, `text/plain;format=raw`, or set `format` query parameter with value `raw`. * string lines: when `Content-Type` is set to `text/plain;format=lines`, or set `format` query parameter with value `lines`.   # noqa: E501
+        Ingest data to a stream with the given name. For formats are supported: * compact JSON: when `Content-Type` is set to one of `application/json`, `application/json;format=compact`, `application/vnd.timeplus+json`, `application/vnd.timeplus+json;format=compat`, or set `format` query parameter with value `compact`. And this is the API's default format. * JSON stream: when `Content-Type` is set to one of `application/json;format=streaming`, `application/vnd.timeplus+json;format=streaming`, or set `format` query parameter with value `streaming`. * raw string: when `Content-Type` is set to one of `text/plain`, `text/plain;format=raw`, or set `format` query parameter with value `raw`. * string lines: when `Content-Type` is set to `text/plain;format=lines`, or set `format` query parameter with value `lines`. * refer to https://docs.timeplus.com/docs/ingest-api for more information *   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_name_ingest_post(body, name, async_req=True)
+        >>> thread = api.v1beta2_streams_name_ingest_post(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param IngestData body: ingest data (required)
         :param str name: stream name (required)
         :param str format: enfoce payload format, if it is set, it overwrite the Content-Type header
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_streams_name_ingest_post_with_http_info(body, name, **kwargs)  # noqa: E501
+            return self.v1beta2_streams_name_ingest_post_with_http_info(body, name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_streams_name_ingest_post_with_http_info(body, name, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_streams_name_ingest_post_with_http_info(body, name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_streams_name_ingest_post_with_http_info(self, body, name, **kwargs):  # noqa: E501
+    def v1beta2_streams_name_ingest_post_with_http_info(self, body, name, **kwargs):  # noqa: E501
         """ingest data.  # noqa: E501
 
-        Ingest data to a stream with the given name. For formats are supported: * compact JSON: when `Content-Type` is set to one of `application/json`, `application/json;format=compact`, `application/vnd.timeplus+json`, `application/vnd.timeplus+json;format=compat`, or set `format` query parameter with value `compact`. And this is the API's default format. * JSON stream: when `Content-Type` is set to one of `application/json;format=streaming`, `application/vnd.timeplus+json;format=streaming`, or set `format` query parameter with value `streaming`. * raw string: when `Content-Type` is set to one of `text/plain`, `text/plain;format=raw`, or set `format` query parameter with value `raw`. * string lines: when `Content-Type` is set to `text/plain;format=lines`, or set `format` query parameter with value `lines`.   # noqa: E501
+        Ingest data to a stream with the given name. For formats are supported: * compact JSON: when `Content-Type` is set to one of `application/json`, `application/json;format=compact`, `application/vnd.timeplus+json`, `application/vnd.timeplus+json;format=compat`, or set `format` query parameter with value `compact`. And this is the API's default format. * JSON stream: when `Content-Type` is set to one of `application/json;format=streaming`, `application/vnd.timeplus+json;format=streaming`, or set `format` query parameter with value `streaming`. * raw string: when `Content-Type` is set to one of `text/plain`, `text/plain;format=raw`, or set `format` query parameter with value `raw`. * string lines: when `Content-Type` is set to `text/plain;format=lines`, or set `format` query parameter with value `lines`. * refer to https://docs.timeplus.com/docs/ingest-api for more information *   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_name_ingest_post_with_http_info(body, name, async_req=True)
+        >>> thread = api.v1beta2_streams_name_ingest_post_with_http_info(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param IngestData body: ingest data (required)
         :param str name: stream name (required)
         :param str format: enfoce payload format, if it is set, it overwrite the Content-Type header
         :return: None
@@ -362,26 +362,26 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_streams_name_ingest_post" % key
+                    " to method v1beta2_streams_name_ingest_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_streams_name_ingest_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_streams_name_ingest_post`")  # noqa: E501
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `v1beta1_streams_name_ingest_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_streams_name_ingest_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'name' in params:
             path_params['name'] = params['name']  # noqa: E501
 
@@ -405,59 +405,59 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/vnd.timeplus+json', 'application/json;format=compat', 'application/vnd.timeplus+json;format=compat', 'application/json;format=stream', 'application/vnd.timeplus+json;format=stream', 'application/x-ndjson', 'text/plain', 'text/plain;format=raw', 'text/plain;format=lines'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/streams/{name}/ingest', 'POST',
+            '/v1beta2/streams/{name}/ingest', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_streams_name_patch(self, body, name, **kwargs):  # noqa: E501
+    def v1beta2_streams_name_patch(self, body, name, **kwargs):  # noqa: E501
         """Update a stream.  # noqa: E501
 
         Update the specific stream with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_name_patch(body, name, async_req=True)
+        >>> thread = api.v1beta2_streams_name_patch(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UpdateStreamRequest body: update stream request parameters (required)
         :param str name: name of the stream (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_streams_name_patch_with_http_info(body, name, **kwargs)  # noqa: E501
+            return self.v1beta2_streams_name_patch_with_http_info(body, name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_streams_name_patch_with_http_info(body, name, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_streams_name_patch_with_http_info(body, name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_streams_name_patch_with_http_info(self, body, name, **kwargs):  # noqa: E501
+    def v1beta2_streams_name_patch_with_http_info(self, body, name, **kwargs):  # noqa: E501
         """Update a stream.  # noqa: E501
 
         Update the specific stream with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_name_patch_with_http_info(body, name, async_req=True)
+        >>> thread = api.v1beta2_streams_name_patch_with_http_info(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UpdateStreamRequest body: update stream request parameters (required)
         :param str name: name of the stream (required)
         :return: None
                  If the method is called asynchronously,
@@ -471,26 +471,26 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_streams_name_patch" % key
+                    " to method v1beta2_streams_name_patch" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_streams_name_patch`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_streams_name_patch`")  # noqa: E501
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `v1beta1_streams_name_patch`")  # noqa: E501
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_streams_name_patch`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'name' in params:
             path_params['name'] = params['name']  # noqa: E501
 
@@ -512,58 +512,58 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/streams/{name}', 'PATCH',
+            '/v1beta2/streams/{name}', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_streams_post(self, body, **kwargs):  # noqa: E501
+    def v1beta2_streams_post(self, body, **kwargs):  # noqa: E501
         """create a stream.  # noqa: E501
 
         Create a stream.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_post(body, async_req=True)
+        >>> thread = api.v1beta2_streams_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param StreamDef body: create stream request parameters (required)
         :return: StreamDef
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_streams_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_streams_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_streams_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_streams_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_streams_post_with_http_info(self, body, **kwargs):  # noqa: E501
+    def v1beta2_streams_post_with_http_info(self, body, **kwargs):  # noqa: E501
         """create a stream.  # noqa: E501
 
         Create a stream.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_streams_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_streams_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param StreamDef body: create stream request parameters (required)
         :return: StreamDef
                  If the method is called asynchronously,
                  returns the request thread.
@@ -576,22 +576,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_streams_post" % key
+                    " to method v1beta2_streams_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_streams_post`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_streams_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -611,21 +611,211 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/streams', 'POST',
+            '/v1beta2/streams', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='StreamDef',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def v1beta2_streamsname_get(self, name, **kwargs):  # noqa: E501
+        """get a stream.  # noqa: E501
+
+        Get a stream with the given name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_streamsname_get(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: stream name (required)
+        :return: Stream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.v1beta2_streamsname_get_with_http_info(name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.v1beta2_streamsname_get_with_http_info(name, **kwargs)  # noqa: E501
+            return data
+
+    def v1beta2_streamsname_get_with_http_info(self, name, **kwargs):  # noqa: E501
+        """get a stream.  # noqa: E501
+
+        Get a stream with the given name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_streamsname_get_with_http_info(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: stream name (required)
+        :return: Stream
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['name']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1beta2_streamsname_get" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_streamsname_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1beta2/streams/:name', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Stream',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def v1beta2_streamsname_stats_get(self, name, **kwargs):  # noqa: E501
+        """get the stats of a stream.  # noqa: E501
+
+        Get the stats of a stream with the given name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_streamsname_stats_get(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: stream name (required)
+        :return: StreamStats
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.v1beta2_streamsname_stats_get_with_http_info(name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.v1beta2_streamsname_stats_get_with_http_info(name, **kwargs)  # noqa: E501
+            return data
+
+    def v1beta2_streamsname_stats_get_with_http_info(self, name, **kwargs):  # noqa: E501
+        """get the stats of a stream.  # noqa: E501
+
+        Get the stats of a stream with the given name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_streamsname_stats_get_with_http_info(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: stream name (required)
+        :return: StreamStats
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['name']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1beta2_streamsname_stats_get" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_streamsname_stats_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1beta2/streams/:name/stats', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='StreamStats',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_client/timeplus/topology_v1beta2_api.py` & `timeplus-1.2.1/swagger_client/timeplus/topology_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_client/timeplus/udfs_v1beta1_api.py` & `timeplus-1.2.1/swagger_client/timeplus/views_v1beta2_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,58 +16,58 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from swagger_client.api_client import ApiClient
 
 
-class UDFsV1beta1Api(object):
+class ViewsV1beta2Api(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def v1beta1_udfs_get(self, **kwargs):  # noqa: E501
-        """list udf.  # noqa: E501
+    def v1beta2_views_get(self, **kwargs):  # noqa: E501
+        """list views.  # noqa: E501
 
-        Get all udf.  # noqa: E501
+        Get all views.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_get(async_req=True)
+        >>> thread = api.v1beta2_views_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[UDF]
+        :return: list[View]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_udfs_get_with_http_info(**kwargs)  # noqa: E501
+            return self.v1beta2_views_get_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_udfs_get_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.v1beta2_views_get_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def v1beta1_udfs_get_with_http_info(self, **kwargs):  # noqa: E501
-        """list udf.  # noqa: E501
+    def v1beta2_views_get_with_http_info(self, **kwargs):  # noqa: E501
+        """list views.  # noqa: E501
 
-        Get all udf.  # noqa: E501
+        Get all views.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_get_with_http_info(async_req=True)
+        >>> thread = api.v1beta2_views_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[UDF]
+        :return: list[View]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -75,15 +75,15 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_udfs_get" % key
+                    " to method v1beta2_views_get" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -100,62 +100,62 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/udfs', 'GET',
+            '/v1beta2/views', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[UDF]',  # noqa: E501
+            response_type='list[View]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_udfs_name_delete(self, name, **kwargs):  # noqa: E501
-        """delete a udf.  # noqa: E501
+    def v1beta2_views_name_delete(self, name, **kwargs):  # noqa: E501
+        """delete a view.  # noqa: E501
 
-        Delete the udf with the given name.  # noqa: E501
+        Delete the view with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_name_delete(name, async_req=True)
+        >>> thread = api.v1beta2_views_name_delete(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: udf name (required)
+        :param str name: view name (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_udfs_name_delete_with_http_info(name, **kwargs)  # noqa: E501
+            return self.v1beta2_views_name_delete_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_udfs_name_delete_with_http_info(name, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_views_name_delete_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_udfs_name_delete_with_http_info(self, name, **kwargs):  # noqa: E501
-        """delete a udf.  # noqa: E501
+    def v1beta2_views_name_delete_with_http_info(self, name, **kwargs):  # noqa: E501
+        """delete a view.  # noqa: E501
 
-        Delete the udf with the given name.  # noqa: E501
+        Delete the view with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_name_delete_with_http_info(name, async_req=True)
+        >>> thread = api.v1beta2_views_name_delete_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: udf name (required)
+        :param str name: view name (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['name']  # noqa: E501
         all_params.append('async_req')
@@ -164,22 +164,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_udfs_name_delete" % key
+                    " to method v1beta2_views_name_delete" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `v1beta1_udfs_name_delete`")  # noqa: E501
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_views_name_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'name' in params:
             path_params['name'] = params['name']  # noqa: E501
 
@@ -195,86 +195,92 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/udfs/{name}', 'DELETE',
+            '/v1beta2/views/{name}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_udfs_name_get(self, name, **kwargs):  # noqa: E501
-        """get a udf.  # noqa: E501
+    def v1beta2_views_name_patch(self, body, name, **kwargs):  # noqa: E501
+        """Update a view.  # noqa: E501
 
-        get the udf with the given name.  # noqa: E501
+        Update the specific view with the given name. Updating the query of a materialized view is not allowed  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_name_get(name, async_req=True)
+        >>> thread = api.v1beta2_views_name_patch(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: udf name (required)
-        :return: UDF
+        :param UpdateViewRequest body: update view request parameters (required)
+        :param str name: name of the view (required)
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_udfs_name_get_with_http_info(name, **kwargs)  # noqa: E501
+            return self.v1beta2_views_name_patch_with_http_info(body, name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_udfs_name_get_with_http_info(name, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_views_name_patch_with_http_info(body, name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_udfs_name_get_with_http_info(self, name, **kwargs):  # noqa: E501
-        """get a udf.  # noqa: E501
+    def v1beta2_views_name_patch_with_http_info(self, body, name, **kwargs):  # noqa: E501
+        """Update a view.  # noqa: E501
 
-        get the udf with the given name.  # noqa: E501
+        Update the specific view with the given name. Updating the query of a materialized view is not allowed  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_name_get_with_http_info(name, async_req=True)
+        >>> thread = api.v1beta2_views_name_patch_with_http_info(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: udf name (required)
-        :return: UDF
+        :param UpdateViewRequest body: update view request parameters (required)
+        :param str name: name of the view (required)
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name']  # noqa: E501
+        all_params = ['body', 'name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_udfs_name_get" % key
+                    " to method v1beta2_views_name_patch" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_views_name_patch`")  # noqa: E501
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `v1beta1_udfs_name_get`")  # noqa: E501
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_views_name_patch`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'name' in params:
             path_params['name'] = params['name']  # noqa: E501
 
@@ -282,71 +288,77 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'body' in params:
+            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/udfs/{name}', 'GET',
+            '/v1beta2/views/{name}', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UDF',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_udfs_name_put(self, body, **kwargs):  # noqa: E501
-        """update a udf.  # noqa: E501
+    def v1beta2_views_post(self, body, **kwargs):  # noqa: E501
+        """create a view.  # noqa: E501
 
-        Update a udf.  # noqa: E501
+        Create a view.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_name_put(body, async_req=True)
+        >>> thread = api.v1beta2_views_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param UDF body: update udf request parameters (required)
-        :return: UDF
+        :param CreateViewRequest body: create view request parameters (required)
+        :return: View
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_udfs_name_put_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_views_post_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_udfs_name_put_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_views_post_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_udfs_name_put_with_http_info(self, body, **kwargs):  # noqa: E501
-        """update a udf.  # noqa: E501
+    def v1beta2_views_post_with_http_info(self, body, **kwargs):  # noqa: E501
+        """create a view.  # noqa: E501
 
-        Update a udf.  # noqa: E501
+        Create a view.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_name_put_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_views_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param UDF body: update udf request parameters (required)
-        :return: UDF
+        :param CreateViewRequest body: create view request parameters (required)
+        :return: View
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -354,22 +366,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_udfs_name_put" % key
+                    " to method v1beta2_views_post" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_udfs_name_put`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `v1beta2_views_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -389,120 +401,211 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/udfs/{name}', 'PUT',
+            '/v1beta2/views', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UDF',  # noqa: E501
+            response_type='View',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def v1beta1_udfs_post(self, body, **kwargs):  # noqa: E501
-        """create a udf.  # noqa: E501
+    def v1beta2_viewsname_get(self, name, **kwargs):  # noqa: E501
+        """get a view.  # noqa: E501
 
-        Create a udf.  # noqa: E501
+        Get a view with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_post(body, async_req=True)
+        >>> thread = api.v1beta2_viewsname_get(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param UDF body: create udf request parameters (required)
-        :return: UDF
+        :param str name: view name (required)
+        :return: View
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.v1beta1_udfs_post_with_http_info(body, **kwargs)  # noqa: E501
+            return self.v1beta2_viewsname_get_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.v1beta1_udfs_post_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.v1beta2_viewsname_get_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def v1beta1_udfs_post_with_http_info(self, body, **kwargs):  # noqa: E501
-        """create a udf.  # noqa: E501
+    def v1beta2_viewsname_get_with_http_info(self, name, **kwargs):  # noqa: E501
+        """get a view.  # noqa: E501
 
-        Create a udf.  # noqa: E501
+        Get a view with the given name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.v1beta1_udfs_post_with_http_info(body, async_req=True)
+        >>> thread = api.v1beta2_viewsname_get_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param UDF body: create udf request parameters (required)
-        :return: UDF
+        :param str name: view name (required)
+        :return: View
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method v1beta1_udfs_post" % key
+                    " to method v1beta2_viewsname_get" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'body' is set
-        if ('body' not in params or
-                params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `v1beta1_udfs_post`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_viewsname_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+        # Authentication setting
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1beta2/views/:name', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='View',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def v1beta2_viewsname_stats_get(self, name, **kwargs):  # noqa: E501
+        """get the stats of a view.  # noqa: E501
+
+        Get the stats of a view with the given name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_viewsname_stats_get(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: view name (required)
+        :return: StreamStats
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.v1beta2_viewsname_stats_get_with_http_info(name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.v1beta2_viewsname_stats_get_with_http_info(name, **kwargs)  # noqa: E501
+            return data
+
+    def v1beta2_viewsname_stats_get_with_http_info(self, name, **kwargs):  # noqa: E501
+        """get the stats of a view.  # noqa: E501
+
+        Get the stats of a view with the given name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.v1beta2_viewsname_stats_get_with_http_info(name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str name: view name (required)
+        :return: StreamStats
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['name']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1beta2_viewsname_stats_get" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `v1beta2_viewsname_stats_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['ApiKeyAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1beta1/udfs', 'POST',
+            '/v1beta2/views/:name/stats', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='UDF',  # noqa: E501
+            response_type='StreamStats',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `timeplus-1.1.2/swagger_test/test_analyze_sql_request.py` & `timeplus-1.2.1/swagger_test/test_analyze_sql_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_api_key.py` & `timeplus-1.2.1/swagger_test/test_api_key.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_api_keys_v1beta1_api.py` & `timeplus-1.2.1/swagger_test/test_api_keys_v1beta2_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.timeplus.api_keys_v1beta1_api import APIKeysV1beta1Api  # noqa: E501
+from swagger_client.timeplus.api_keys_v1beta2_api import APIKeysV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestAPIKeysV1beta1Api(unittest.TestCase):
-    """APIKeysV1beta1Api unit test stubs"""
+class TestAPIKeysV1beta2Api(unittest.TestCase):
+    """APIKeysV1beta2Api unit test stubs"""
 
     def setUp(self):
-        self.api = APIKeysV1beta1Api()  # noqa: E501
+        self.api = APIKeysV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_v1beta1_auth_api_keys_get(self):
-        """Test case for v1beta1_auth_api_keys_get
+    def test_v1beta2_auth_api_keys_get(self):
+        """Test case for v1beta2_auth_api_keys_get
 
         List API keys  # noqa: E501
         """
         pass
 
-    def test_v1beta1_auth_api_keys_id_delete(self):
-        """Test case for v1beta1_auth_api_keys_id_delete
+    def test_v1beta2_auth_api_keys_id_delete(self):
+        """Test case for v1beta2_auth_api_keys_id_delete
 
         Delete an API key  # noqa: E501
         """
         pass
 
-    def test_v1beta1_auth_api_keys_post(self):
-        """Test case for v1beta1_auth_api_keys_post
+    def test_v1beta2_auth_api_keys_post(self):
+        """Test case for v1beta2_auth_api_keys_post
 
         Create an API key  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `timeplus-1.1.2/swagger_test/test_batching_policy.py` & `timeplus-1.2.1/swagger_test/test_batching_policy.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_column.py` & `timeplus-1.2.1/swagger_test/test_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_column_def.py` & `timeplus-1.2.1/swagger_test/test_column_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_columns_resp.py` & `timeplus-1.2.1/swagger_test/test_columns_resp.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_connection.py` & `timeplus-1.2.1/swagger_test/test_ingest_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.connection import Connection  # noqa: E501
+from swagger_client.models.ingest_data import IngestData  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestConnection(unittest.TestCase):
-    """Connection unit test stubs"""
+class TestIngestData(unittest.TestCase):
+    """IngestData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testConnection(self):
-        """Test Connection"""
+    def testIngestData(self):
+        """Test IngestData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.connection.Connection()  # noqa: E501
+        # model = swagger_client.models.ingest_data.IngestData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_connection_config.py` & `timeplus-1.2.1/swagger_test/test_sql_analyze_column.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.connection_config import ConnectionConfig  # noqa: E501
+from swagger_client.models.sql_analyze_column import SQLAnalyzeColumn  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestConnectionConfig(unittest.TestCase):
-    """ConnectionConfig unit test stubs"""
+class TestSQLAnalyzeColumn(unittest.TestCase):
+    """SQLAnalyzeColumn unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testConnectionConfig(self):
-        """Test ConnectionConfig"""
+    def testSQLAnalyzeColumn(self):
+        """Test SQLAnalyzeColumn"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.connection_config.ConnectionConfig()  # noqa: E501
+        # model = swagger_client.models.sql_analyze_column.SQLAnalyzeColumn()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_connection_stat.py` & `timeplus-1.2.1/swagger_test/test_stream_setting.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.connection_stat import ConnectionStat  # noqa: E501
+from swagger_client.models.stream_setting import StreamSetting  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestConnectionStat(unittest.TestCase):
-    """ConnectionStat unit test stubs"""
+class TestStreamSetting(unittest.TestCase):
+    """StreamSetting unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testConnectionStat(self):
-        """Test ConnectionStat"""
+    def testStreamSetting(self):
+        """Test StreamSetting"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.connection_stat.ConnectionStat()  # noqa: E501
+        # model = swagger_client.models.stream_setting.StreamSetting()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_create_api_key_request.py` & `timeplus-1.2.1/swagger_test/test_create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_create_api_key_response.py` & `timeplus-1.2.1/swagger_test/test_create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_create_dashboard_request.py` & `timeplus-1.2.1/swagger_test/test_create_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_create_persistent_query_request.py` & `timeplus-1.2.1/swagger_test/test_alerts_v1beta2_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.create_persistent_query_request import CreatePersistentQueryRequest  # noqa: E501
+from swagger_client.timeplus.alerts_v1beta2_api import AlertsV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestCreatePersistentQueryRequest(unittest.TestCase):
-    """CreatePersistentQueryRequest unit test stubs"""
+class TestAlertsV1beta2Api(unittest.TestCase):
+    """AlertsV1beta2Api unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = AlertsV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testCreatePersistentQueryRequest(self):
-        """Test CreatePersistentQueryRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.create_persistent_query_request.CreatePersistentQueryRequest()  # noqa: E501
+    def test_v1beta2_alerts_id_stop_post(self):
+        """Test case for v1beta2_alerts_id_stop_post
+
+        stop an alert.  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_create_query_request_v1_beta1.py` & `timeplus-1.2.1/swagger_test/test_create_query_request_v1_beta2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.create_query_request_v1_beta1 import CreateQueryRequestV1Beta1  # noqa: E501
+from swagger_client.models.create_query_request_v1_beta2 import CreateQueryRequestV1Beta2  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestCreateQueryRequestV1Beta1(unittest.TestCase):
-    """CreateQueryRequestV1Beta1 unit test stubs"""
+class TestCreateQueryRequestV1Beta2(unittest.TestCase):
+    """CreateQueryRequestV1Beta2 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateQueryRequestV1Beta1(self):
-        """Test CreateQueryRequestV1Beta1"""
+    def testCreateQueryRequestV1Beta2(self):
+        """Test CreateQueryRequestV1Beta2"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.create_query_request_v1_beta1.CreateQueryRequestV1Beta1()  # noqa: E501
+        # model = swagger_client.models.create_query_request_v1_beta2.CreateQueryRequestV1Beta2()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_create_query_request_v1_beta2.py` & `timeplus-1.2.1/swagger_test/test_sql_analyze_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.create_query_request_v1_beta2 import CreateQueryRequestV1Beta2  # noqa: E501
+from swagger_client.models.sql_analyze_result import SQLAnalyzeResult  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestCreateQueryRequestV1Beta2(unittest.TestCase):
-    """CreateQueryRequestV1Beta2 unit test stubs"""
+class TestSQLAnalyzeResult(unittest.TestCase):
+    """SQLAnalyzeResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateQueryRequestV1Beta2(self):
-        """Test CreateQueryRequestV1Beta2"""
+    def testSQLAnalyzeResult(self):
+        """Test SQLAnalyzeResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.create_query_request_v1_beta2.CreateQueryRequestV1Beta2()  # noqa: E501
+        # model = swagger_client.models.sql_analyze_result.SQLAnalyzeResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_create_query_response.py` & `timeplus-1.2.1/swagger_test/test_format_query_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.create_query_response import CreateQueryResponse  # noqa: E501
+from swagger_client.models.format_query_response import FormatQueryResponse  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestCreateQueryResponse(unittest.TestCase):
-    """CreateQueryResponse unit test stubs"""
+class TestFormatQueryResponse(unittest.TestCase):
+    """FormatQueryResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCreateQueryResponse(self):
-        """Test CreateQueryResponse"""
+    def testFormatQueryResponse(self):
+        """Test FormatQueryResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.create_query_response.CreateQueryResponse()  # noqa: E501
+        # model = swagger_client.models.format_query_response.FormatQueryResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_create_sink_request.py` & `timeplus-1.2.1/swagger_test/test_create_sink_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_create_source_request.py` & `timeplus-1.2.1/swagger_test/test_create_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_dashboard_dashboard.py` & `timeplus-1.2.1/swagger_test/test_dashboard_dashboard.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_dashboard_panel.py` & `timeplus-1.2.1/swagger_test/test_dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_dashboards_v1beta2_api.py` & `timeplus-1.2.1/swagger_test/test_dashboards_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_edge.py` & `timeplus-1.2.1/swagger_test/test_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_error_response.py` & `timeplus-1.2.1/swagger_test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_event.py` & `timeplus-1.2.1/swagger_test/test_event.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_event_infer_request.py` & `timeplus-1.2.1/swagger_test/test_event_infer_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_event_infer_response.py` & `timeplus-1.2.1/swagger_test/test_event_infer_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_external_stream_def.py` & `timeplus-1.2.1/swagger_test/test_external_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_file_upload_response.py` & `timeplus-1.2.1/swagger_test/test_file_upload_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_format_query_request.py` & `timeplus-1.2.1/swagger_test/test_format_query_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_format_query_response.py` & `timeplus-1.2.1/swagger_test/test_create_view_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.format_query_response import FormatQueryResponse  # noqa: E501
+from swagger_client.models.create_view_request import CreateViewRequest  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestFormatQueryResponse(unittest.TestCase):
-    """FormatQueryResponse unit test stubs"""
+class TestCreateViewRequest(unittest.TestCase):
+    """CreateViewRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testFormatQueryResponse(self):
-        """Test FormatQueryResponse"""
+    def testCreateViewRequest(self):
+        """Test CreateViewRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.format_query_response.FormatQueryResponse()  # noqa: E501
+        # model = swagger_client.models.create_view_request.CreateViewRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_global_metrics_result.py` & `timeplus-1.2.1/swagger_test/test_global_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_graph.py` & `timeplus-1.2.1/swagger_test/test_graph.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_ingest_data.py` & `timeplus-1.2.1/swagger_test/test_udf_argument.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.ingest_data import IngestData  # noqa: E501
+from swagger_client.models.udf_argument import UDFArgument  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestIngestData(unittest.TestCase):
-    """IngestData unit test stubs"""
+class TestUDFArgument(unittest.TestCase):
+    """UDFArgument unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIngestData(self):
-        """Test IngestData"""
+    def testUDFArgument(self):
+        """Test UDFArgument"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.ingest_data.IngestData()  # noqa: E501
+        # model = swagger_client.models.udf_argument.UDFArgument()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_internal_http_handler_v1beta2_global_metrics_request.py` & `timeplus-1.2.1/swagger_test/test_update_source_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.internal_http_handler_v1beta2_global_metrics_request import InternalHttpHandlerV1beta2GlobalMetricsRequest  # noqa: E501
+from swagger_client.models.update_source_request import UpdateSourceRequest  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestInternalHttpHandlerV1beta2GlobalMetricsRequest(unittest.TestCase):
-    """InternalHttpHandlerV1beta2GlobalMetricsRequest unit test stubs"""
+class TestUpdateSourceRequest(unittest.TestCase):
+    """UpdateSourceRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInternalHttpHandlerV1beta2GlobalMetricsRequest(self):
-        """Test InternalHttpHandlerV1beta2GlobalMetricsRequest"""
+    def testUpdateSourceRequest(self):
+        """Test UpdateSourceRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.internal_http_handler_v1beta2_global_metrics_request.InternalHttpHandlerV1beta2GlobalMetricsRequest()  # noqa: E501
+        # model = swagger_client.models.update_source_request.UpdateSourceRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_latency.py` & `timeplus-1.2.1/swagger_test/test_owner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.latency import Latency  # noqa: E501
+from swagger_client.models.owner import Owner  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestLatency(unittest.TestCase):
-    """Latency unit test stubs"""
+class TestOwner(unittest.TestCase):
+    """Owner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLatency(self):
-        """Test Latency"""
+    def testOwner(self):
+        """Test Owner"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.latency.Latency()  # noqa: E501
+        # model = swagger_client.models.owner.Owner()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_metrics_v1beta2_api.py` & `timeplus-1.2.1/swagger_test/test_metrics_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_node.py` & `timeplus-1.2.1/swagger_test/test_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_owner.py` & `timeplus-1.2.1/swagger_test/test_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.owner import Owner  # noqa: E501
+from swagger_client.models.view import View  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestOwner(unittest.TestCase):
-    """Owner unit test stubs"""
+class TestView(unittest.TestCase):
+    """View unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOwner(self):
-        """Test Owner"""
+    def testView(self):
+        """Test View"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.owner.Owner()  # noqa: E501
+        # model = swagger_client.models.view.View()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_persistent_queries_v1beta2_api.py` & `timeplus-1.2.1/swagger_test/test_queries_v1beta2_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,89 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.timeplus.persistent_queries_v1beta2_api import PersistentQueriesV1beta2Api  # noqa: E501
+from swagger_client.timeplus.queries_v1beta2_api import QueriesV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestPersistentQueriesV1beta2Api(unittest.TestCase):
-    """PersistentQueriesV1beta2Api unit test stubs"""
+class TestQueriesV1beta2Api(unittest.TestCase):
+    """QueriesV1beta2Api unit test stubs"""
 
     def setUp(self):
-        self.api = PersistentQueriesV1beta2Api()  # noqa: E501
+        self.api = QueriesV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_v1beta2_persistent_queries_get(self):
-        """Test case for v1beta2_persistent_queries_get
+    def test_v1beta2_format_post(self):
+        """Test case for v1beta2_format_post
 
-        list persistent-queries.  # noqa: E501
+        format a query.  # noqa: E501
         """
         pass
 
-    def test_v1beta2_persistent_queries_id_data_get(self):
-        """Test case for v1beta2_persistent_queries_id_data_get
+    def test_v1beta2_queries_get(self):
+        """Test case for v1beta2_queries_get
 
-        stream persistent query result via websocket  # noqa: E501
+        list queries.  # noqa: E501
         """
         pass
 
-    def test_v1beta2_persistent_queries_id_delete(self):
-        """Test case for v1beta2_persistent_queries_id_delete
+    def test_v1beta2_queries_id_cancel_post(self):
+        """Test case for v1beta2_queries_id_cancel_post
 
-        delete a persistent query.  # noqa: E501
+        cancel a query.  # noqa: E501
         """
         pass
 
-    def test_v1beta2_persistent_queries_id_get(self):
-        """Test case for v1beta2_persistent_queries_id_get
+    def test_v1beta2_queries_id_delete(self):
+        """Test case for v1beta2_queries_id_delete
 
-        get a persistent query.  # noqa: E501
+        delete a query.  # noqa: E501
         """
         pass
 
-    def test_v1beta2_persistent_queries_post(self):
-        """Test case for v1beta2_persistent_queries_post
+    def test_v1beta2_queries_id_get(self):
+        """Test case for v1beta2_queries_id_get
 
-        execute a persistent query.  # noqa: E501
+        get a query.  # noqa: E501
+        """
+        pass
+
+    def test_v1beta2_queries_id_pipeline_get(self):
+        """Test case for v1beta2_queries_id_pipeline_get
+
+        get the pipeline for a query  # noqa: E501
+        """
+        pass
+
+    def test_v1beta2_queries_post(self):
+        """Test case for v1beta2_queries_post
+
+        execute a query and return the results.  # noqa: E501
+        """
+        pass
+
+    def test_v1beta2_sqlanalyze_post(self):
+        """Test case for v1beta2_sqlanalyze_post
+
+        analyze sql  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_queries_v1beta1_api.py` & `timeplus-1.2.1/swagger_test/test_sinks_v1beta2_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,86 +11,58 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.timeplus.queries_v1beta1_api import QueriesV1beta1Api  # noqa: E501
+from swagger_client.timeplus.sinks_v1beta2_api import SinksV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestQueriesV1beta1Api(unittest.TestCase):
-    """QueriesV1beta1Api unit test stubs"""
+class TestSinksV1beta2Api(unittest.TestCase):
+    """SinksV1beta2Api unit test stubs"""
 
     def setUp(self):
-        self.api = QueriesV1beta1Api()  # noqa: E501
+        self.api = SinksV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_v1beta1_format_post(self):
-        """Test case for v1beta1_format_post
+    def test_v1beta2_sinks_get(self):
+        """Test case for v1beta2_sinks_get
 
-        format a query.  # noqa: E501
+        list sinks  # noqa: E501
         """
         pass
 
-    def test_v1beta1_queries_get(self):
-        """Test case for v1beta1_queries_get
+    def test_v1beta2_sinks_id_delete(self):
+        """Test case for v1beta2_sinks_id_delete
 
-        list queries.  # noqa: E501
+        delete a sink.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_queries_id_cancel_post(self):
-        """Test case for v1beta1_queries_id_cancel_post
+    def test_v1beta2_sinks_id_get(self):
+        """Test case for v1beta2_sinks_id_get
 
-        cancel a query.  # noqa: E501
+        get a sink.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_queries_id_delete(self):
-        """Test case for v1beta1_queries_id_delete
+    def test_v1beta2_sinks_id_stop_post(self):
+        """Test case for v1beta2_sinks_id_stop_post
 
-        delete a query.  # noqa: E501
+        stop a sink.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_queries_id_get(self):
-        """Test case for v1beta1_queries_id_get
+    def test_v1beta2_sinks_post(self):
+        """Test case for v1beta2_sinks_post
 
-        get a query.  # noqa: E501
-        """
-        pass
-
-    def test_v1beta1_queries_id_pipeline_get(self):
-        """Test case for v1beta1_queries_id_pipeline_get
-
-        get the pipeline for a query  # noqa: E501
-        """
-        pass
-
-    def test_v1beta1_queries_post(self):
-        """Test case for v1beta1_queries_post
-
-        execute a query.  # noqa: E501
-        """
-        pass
-
-    def test_v1beta1_sqlanalyze_post(self):
-        """Test case for v1beta1_sqlanalyze_post
-
-        analyze sql  # noqa: E501
-        """
-        pass
-
-    def test_ws_queries_id_get(self):
-        """Test case for ws_queries_id_get
-
-        stream query result via websocket [THIS API DOESN'T HAVE `v1beta1` IN PATH]  # noqa: E501
+        create a sink.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_queries_v1beta2_api.py` & `timeplus-1.2.1/swagger_test/test_sinks_internal_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.timeplus.queries_v1beta2_api import QueriesV1beta2Api  # noqa: E501
+from swagger_client.timeplus.sinks_internal_api import SinksInternalApi  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestQueriesV1beta2Api(unittest.TestCase):
-    """QueriesV1beta2Api unit test stubs"""
+class TestSinksInternalApi(unittest.TestCase):
+    """SinksInternalApi unit test stubs"""
 
     def setUp(self):
-        self.api = QueriesV1beta2Api()  # noqa: E501
+        self.api = SinksInternalApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_v1beta2_queries_post(self):
-        """Test case for v1beta2_queries_post
+    def test_api_internal_tenants_tenant_sinks_id_start_post(self):
+        """Test case for api_internal_tenants_tenant_sinks_id_start_post
 
-        execute a query and return the results.  # noqa: E501
+        start a sink.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_query.py` & `timeplus-1.2.1/swagger_test/test_query.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_query_analysis.py` & `timeplus-1.2.1/swagger_test/test_metrics_query_throughput.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.query_analysis import QueryAnalysis  # noqa: E501
+from swagger_client.models.metrics_query_throughput import MetricsQueryThroughput  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestQueryAnalysis(unittest.TestCase):
-    """QueryAnalysis unit test stubs"""
+class TestMetricsQueryThroughput(unittest.TestCase):
+    """MetricsQueryThroughput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testQueryAnalysis(self):
-        """Test QueryAnalysis"""
+    def testMetricsQueryThroughput(self):
+        """Test MetricsQueryThroughput"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.query_analysis.QueryAnalysis()  # noqa: E501
+        # model = swagger_client.models.metrics_query_throughput.MetricsQueryThroughput()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_query_metrics.py` & `timeplus-1.2.1/swagger_test/test_query_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.query_metrics import QueryMetrics  # noqa: E501
+from swagger_client.models.query_result import QueryResult  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestQueryMetrics(unittest.TestCase):
-    """QueryMetrics unit test stubs"""
+class TestQueryResult(unittest.TestCase):
+    """QueryResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testQueryMetrics(self):
-        """Test QueryMetrics"""
+    def testQueryResult(self):
+        """Test QueryResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.query_metrics.QueryMetrics()  # noqa: E501
+        # model = swagger_client.models.query_result.QueryResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_query_pipeline.py` & `timeplus-1.2.1/swagger_test/test_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_query_pipeline_edge.py` & `timeplus-1.2.1/swagger_test/test_query_pipeline_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_query_pipeline_node.py` & `timeplus-1.2.1/swagger_test/test_query_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_query_pipeline_node_metric.py` & `timeplus-1.2.1/swagger_test/test_query_pipeline_node_metric.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_query_result.py` & `timeplus-1.2.1/swagger_test/test_udf.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.query_result import QueryResult  # noqa: E501
+from swagger_client.models.udf import UDF  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestQueryResult(unittest.TestCase):
-    """QueryResult unit test stubs"""
+class TestUDF(unittest.TestCase):
+    """UDF unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testQueryResult(self):
-        """Test QueryResult"""
+    def testUDF(self):
+        """Test UDF"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.query_result.QueryResult()  # noqa: E501
+        # model = swagger_client.models.udf.UDF()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_query_with_metrics.py` & `timeplus-1.2.1/swagger_test/test_stream_def.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.query_with_metrics import QueryWithMetrics  # noqa: E501
+from swagger_client.models.stream_def import StreamDef  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestQueryWithMetrics(unittest.TestCase):
-    """QueryWithMetrics unit test stubs"""
+class TestStreamDef(unittest.TestCase):
+    """StreamDef unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testQueryWithMetrics(self):
-        """Test QueryWithMetrics"""
+    def testStreamDef(self):
+        """Test StreamDef"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.query_with_metrics.QueryWithMetrics()  # noqa: E501
+        # model = swagger_client.models.stream_def.StreamDef()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_resource_metrics_request.py` & `timeplus-1.2.1/swagger_test/test_source_preview_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.resource_metrics_request import ResourceMetricsRequest  # noqa: E501
+from swagger_client.models.source_preview_request import SourcePreviewRequest  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestResourceMetricsRequest(unittest.TestCase):
-    """ResourceMetricsRequest unit test stubs"""
+class TestSourcePreviewRequest(unittest.TestCase):
+    """SourcePreviewRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testResourceMetricsRequest(self):
-        """Test ResourceMetricsRequest"""
+    def testSourcePreviewRequest(self):
+        """Test SourcePreviewRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.resource_metrics_request.ResourceMetricsRequest()  # noqa: E501
+        # model = swagger_client.models.source_preview_request.SourcePreviewRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_resource_metrics_result.py` & `timeplus-1.2.1/swagger_test/test_resource_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_sink.py` & `timeplus-1.2.1/swagger_test/test_sink.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_sink_metrics.py` & `timeplus-1.2.1/swagger_test/test_stream_stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.sink_metrics import SinkMetrics  # noqa: E501
+from swagger_client.models.stream_stats import StreamStats  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSinkMetrics(unittest.TestCase):
-    """SinkMetrics unit test stubs"""
+class TestStreamStats(unittest.TestCase):
+    """StreamStats unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSinkMetrics(self):
-        """Test SinkMetrics"""
+    def testStreamStats(self):
+        """Test StreamStats"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.sink_metrics.SinkMetrics()  # noqa: E501
+        # model = swagger_client.models.stream_stats.StreamStats()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_sink_stat.py` & `timeplus-1.2.1/swagger_test/test_sink_stat.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_sinks_v1beta1_api.py` & `timeplus-1.2.1/swagger_test/test_udfs_v1beta2_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,51 +11,58 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.timeplus.sinks_v1beta1_api import SinksV1beta1Api  # noqa: E501
+from swagger_client.timeplus.udfs_v1beta2_api import UDFsV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSinksV1beta1Api(unittest.TestCase):
-    """SinksV1beta1Api unit test stubs"""
+class TestUDFsV1beta2Api(unittest.TestCase):
+    """UDFsV1beta2Api unit test stubs"""
 
     def setUp(self):
-        self.api = SinksV1beta1Api()  # noqa: E501
+        self.api = UDFsV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_v1beta1_sinks_get(self):
-        """Test case for v1beta1_sinks_get
+    def test_v1beta2_udfs_get(self):
+        """Test case for v1beta2_udfs_get
 
-        list sinks  # noqa: E501
+        list udf.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sinks_id_delete(self):
-        """Test case for v1beta1_sinks_id_delete
+    def test_v1beta2_udfs_name_delete(self):
+        """Test case for v1beta2_udfs_name_delete
 
-        delete a sink.  # noqa: E501
+        delete a udf.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sinks_id_get(self):
-        """Test case for v1beta1_sinks_id_get
+    def test_v1beta2_udfs_name_get(self):
+        """Test case for v1beta2_udfs_name_get
 
-        get a sink.  # noqa: E501
+        get a udf.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sinks_post(self):
-        """Test case for v1beta1_sinks_post
+    def test_v1beta2_udfs_name_put(self):
+        """Test case for v1beta2_udfs_name_put
 
-        create a sink.  # noqa: E501
+        update a udf.  # noqa: E501
+        """
+        pass
+
+    def test_v1beta2_udfs_post(self):
+        """Test case for v1beta2_udfs_post
+
+        create a udf.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_source.py` & `timeplus-1.2.1/swagger_test/test_source.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_source_metrics.py` & `timeplus-1.2.1/swagger_test/test_topology_v1beta2_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.source_metrics import SourceMetrics  # noqa: E501
+from swagger_client.timeplus.topology_v1beta2_api import TopologyV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSourceMetrics(unittest.TestCase):
-    """SourceMetrics unit test stubs"""
+class TestTopologyV1beta2Api(unittest.TestCase):
+    """TopologyV1beta2Api unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = TopologyV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testSourceMetrics(self):
-        """Test SourceMetrics"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.source_metrics.SourceMetrics()  # noqa: E501
+    def test_v1beta2_topology_get(self):
+        """Test case for v1beta2_topology_get
+
+        get topology graph.  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_source_preview_request.py` & `timeplus-1.2.1/swagger_test/test_stream.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.source_preview_request import SourcePreviewRequest  # noqa: E501
+from swagger_client.models.stream import Stream  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSourcePreviewRequest(unittest.TestCase):
-    """SourcePreviewRequest unit test stubs"""
+class TestStream(unittest.TestCase):
+    """Stream unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSourcePreviewRequest(self):
-        """Test SourcePreviewRequest"""
+    def testStream(self):
+        """Test Stream"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.source_preview_request.SourcePreviewRequest()  # noqa: E501
+        # model = swagger_client.models.stream.Stream()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_source_upload_body.py` & `timeplus-1.2.1/swagger_test/test_source_upload_body.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_source_with_metrics.py` & `timeplus-1.2.1/swagger_test/test_update_stream_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Timeplus
 
-    Welcome to the Timeplus HTTP REST API specification.  # Authentication  <!-- ReDoc-Inject: <security-definitions> -->  # noqa: E501
+    Welcome to the Timeplus HTTP REST API specification.  # noqa: E501
 
-    OpenAPI spec version: 1.0.0-oas3
+    OpenAPI spec version: v1
     Contact: support@timeplus.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.source_with_metrics import SourceWithMetrics  # noqa: E501
+from swagger_client.models.update_stream_request import UpdateStreamRequest  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSourceWithMetrics(unittest.TestCase):
-    """SourceWithMetrics unit test stubs"""
+class TestUpdateStreamRequest(unittest.TestCase):
+    """UpdateStreamRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSourceWithMetrics(self):
-        """Test SourceWithMetrics"""
+    def testUpdateStreamRequest(self):
+        """Test UpdateStreamRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.source_with_metrics.SourceWithMetrics()  # noqa: E501
+        # model = swagger_client.models.update_stream_request.UpdateStreamRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_sources_v1beta1_api.py` & `timeplus-1.2.1/swagger_test/test_sources_v1beta2_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,99 +11,99 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.timeplus.sources_v1beta1_api import SourcesV1beta1Api  # noqa: E501
+from swagger_client.timeplus.sources_v1beta2_api import SourcesV1beta2Api  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSourcesV1beta1Api(unittest.TestCase):
-    """SourcesV1beta1Api unit test stubs"""
+class TestSourcesV1beta2Api(unittest.TestCase):
+    """SourcesV1beta2Api unit test stubs"""
 
     def setUp(self):
-        self.api = SourcesV1beta1Api()  # noqa: E501
+        self.api = SourcesV1beta2Api()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_v1beta1_source_infer_post(self):
-        """Test case for v1beta1_source_infer_post
+    def test_v1beta2_source_infer_post(self):
+        """Test case for v1beta2_source_infer_post
 
         infer schema from an existing event  # noqa: E501
         """
         pass
 
-    def test_v1beta1_source_match_post(self):
-        """Test case for v1beta1_source_match_post
+    def test_v1beta2_source_match_post(self):
+        """Test case for v1beta2_source_match_post
 
         return streams match provided events  # noqa: E501
         """
         pass
 
-    def test_v1beta1_source_preview_post(self):
-        """Test case for v1beta1_source_preview_post
+    def test_v1beta2_source_preview_post(self):
+        """Test case for v1beta2_source_preview_post
 
         preview a source.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_source_upload_post(self):
-        """Test case for v1beta1_source_upload_post
+    def test_v1beta2_source_upload_post(self):
+        """Test case for v1beta2_source_upload_post
 
         upload a file  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_get(self):
-        """Test case for v1beta1_sources_get
+    def test_v1beta2_sources_get(self):
+        """Test case for v1beta2_sources_get
 
         list sources.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_id_delete(self):
-        """Test case for v1beta1_sources_id_delete
+    def test_v1beta2_sources_id_delete(self):
+        """Test case for v1beta2_sources_id_delete
 
         delete a source.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_id_get(self):
-        """Test case for v1beta1_sources_id_get
+    def test_v1beta2_sources_id_get(self):
+        """Test case for v1beta2_sources_id_get
 
         get a source.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_id_put(self):
-        """Test case for v1beta1_sources_id_put
+    def test_v1beta2_sources_id_put(self):
+        """Test case for v1beta2_sources_id_put
 
         Update a source.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_id_start_post(self):
-        """Test case for v1beta1_sources_id_start_post
+    def test_v1beta2_sources_id_start_post(self):
+        """Test case for v1beta2_sources_id_start_post
 
         start a source.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_id_stop_post(self):
-        """Test case for v1beta1_sources_id_stop_post
+    def test_v1beta2_sources_id_stop_post(self):
+        """Test case for v1beta2_sources_id_stop_post
 
         stop a source.  # noqa: E501
         """
         pass
 
-    def test_v1beta1_sources_post(self):
-        """Test case for v1beta1_sources_post
+    def test_v1beta2_sources_post(self):
+        """Test case for v1beta2_sources_post
 
         create a source.  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `timeplus-1.1.2/swagger_test/test_sql_analyze_column.py` & `timeplus-1.2.1/swagger_test/test_update_view_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.sql_analyze_column import SQLAnalyzeColumn  # noqa: E501
+from swagger_client.models.update_view_request import UpdateViewRequest  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSQLAnalyzeColumn(unittest.TestCase):
-    """SQLAnalyzeColumn unit test stubs"""
+class TestUpdateViewRequest(unittest.TestCase):
+    """UpdateViewRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSQLAnalyzeColumn(self):
-        """Test SQLAnalyzeColumn"""
+    def testUpdateViewRequest(self):
+        """Test UpdateViewRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.sql_analyze_column.SQLAnalyzeColumn()  # noqa: E501
+        # model = swagger_client.models.update_view_request.UpdateViewRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_sql_analyze_result.py` & `timeplus-1.2.1/swagger_test/test_udf_auth_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.sql_analyze_result import SQLAnalyzeResult  # noqa: E501
+from swagger_client.models.udf_auth_context import UDFAuthContext  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestSQLAnalyzeResult(unittest.TestCase):
-    """SQLAnalyzeResult unit test stubs"""
+class TestUDFAuthContext(unittest.TestCase):
+    """UDFAuthContext unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSQLAnalyzeResult(self):
-        """Test SQLAnalyzeResult"""
+    def testUDFAuthContext(self):
+        """Test UDFAuthContext"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.sql_analyze_result.SQLAnalyzeResult()  # noqa: E501
+        # model = swagger_client.models.udf_auth_context.UDFAuthContext()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_stream.py` & `timeplus-1.2.1/swagger_test/test_update_dashboard_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.stream import Stream  # noqa: E501
+from swagger_client.models.update_dashboard_request import UpdateDashboardRequest  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestStream(unittest.TestCase):
-    """Stream unit test stubs"""
+class TestUpdateDashboardRequest(unittest.TestCase):
+    """UpdateDashboardRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStream(self):
-        """Test Stream"""
+    def testUpdateDashboardRequest(self):
+        """Test UpdateDashboardRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.stream.Stream()  # noqa: E501
+        # model = swagger_client.models.update_dashboard_request.UpdateDashboardRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/swagger_test/test_stream_match_request.py` & `timeplus-1.2.1/swagger_test/test_stream_match_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/swagger_test/test_stream_stats.py` & `timeplus-1.2.1/swagger_test/test_time_columns.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import swagger_client
-from swagger_client.models.stream_stats import StreamStats  # noqa: E501
+from swagger_client.models.time_columns import TimeColumns  # noqa: E501
 from swagger_client.rest import ApiException
 
 
-class TestStreamStats(unittest.TestCase):
-    """StreamStats unit test stubs"""
+class TestTimeColumns(unittest.TestCase):
+    """TimeColumns unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStreamStats(self):
-        """Test StreamStats"""
+    def testTimeColumns(self):
+        """Test TimeColumns"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = swagger_client.models.stream_stats.StreamStats()  # noqa: E501
+        # model = swagger_client.models.time_columns.TimeColumns()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timeplus-1.1.2/test/test_stream.py` & `timeplus-1.2.1/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/timeplus/env.py` & `timeplus-1.2.1/timeplus/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     def apikey(self, key):
         self._configuration.api_key["X-Api-Key"] = key
         return self
 
     def workspace(self, name):
         self._workspace = name
         if not self._address:
-            self._configuration.host = (
-                f"https//beta.timeplus.cloud/{self._workspace}/api"
-            )
+            self._configuration.host = f"https//us.timeplus.cloud/{self._workspace}/api"
         else:
             self._configuration.host = f"{self._address}/{self._workspace}/api"
         return self
 
     def address(self, url):
         self._address = url
         if self._workspace:
```

### Comparing `timeplus-1.1.2/timeplus/query.py` & `timeplus-1.2.1/timeplus/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 from swagger_client.rest import ApiException
 
 
 class Query:
     def __init__(self, env):
         self._env = env
         self._configuration = self._env._conf()
-        self._api_instance_v1 = swagger_client.QueriesV1beta1Api(
-            swagger_client.ApiClient(self._configuration)
-        )
-        self._api_instance_v2 = swagger_client.QueriesV1beta2Api(
+        self._api_instance = swagger_client.QueriesV1beta2Api(
             swagger_client.ApiClient(self._configuration)
         )
         self._create_response = None
         self._id = None
         self._batching_pilicy = None
 
     def sql(self, query):
@@ -34,15 +31,15 @@
     def create(self):
         body = swagger_client.CreateQueryRequestV1Beta2(
             sql=self._sql, batching_policy=self._batching_pilicy
         )
         try:
             # as to support sse, the reponse is urllib3.response.HTTPResponse
             # instead of swagger_client.models.query.Query
-            self._create_response = self._api_instance_v2.v1beta2_queries_post(body)
+            self._create_response = self._api_instance.v1beta2_queries_post(body)
             _sse_client = sseclient.SSEClient(self._create_response)
             self._events = _sse_client.events()
             self._query = next(self._events)
             self._metadata = json.loads(self._query.data)
             self._id = self._metadata["id"]
             return self
         except ApiException as e:
@@ -55,46 +52,44 @@
     def metadata(self):
         return self._metadata
 
     def result(self):
         return self._events
 
     def delete(self):
-        self._api_instance_v1.v1beta1_queries_id_delete(self._id)
+        self._api_instance.v1beta2_queries_id_delete(self._id)
 
     def cancel(self):
         try:
-            self._cancel_response = (
-                self._api_instance_v1.v1beta1_queries_id_cancel_post(id=self._id)
+            self._cancel_response = self._api_instance.v1beta2_queries_id_cancel_post(
+                id=self._id
             )
         except ApiException as e:
             pprint(
-                "Exception when calling QueriesV1beta1Api->v1beta1_queries_id_cancel_post: %s\n"
+                "Exception when calling QueriesV1beta2Api->v1beta2_queries_id_cancel_post: %s\n"
                 % e
             )
             raise e
 
     def get(self, id):
         self._id = id
         try:
-            self._get_response = self._api_instance_v1.v1beta1_queries_id_get(
-                id=self._id
-            )
+            self._get_response = self._api_instance.v1beta2_queries_id_get(id=self._id)
             self._metadata = self._get_response
             return self
         except ApiException as e:
             pprint(
-                "Exception when calling QueriesV1beta1Api->v1beta1_queries_id_get: %s\n"
+                "Exception when calling QueriesV1beta2Api->v1beta2_queries_id_get: %s\n"
                 % e
             )
             raise e
 
     def list(self):
         try:
-            list_response = self._api_instance_v1.v1beta1_queries_get()
+            list_response = self._api_instance.v1beta2_queries_get()
             return list_response
         except ApiException as e:
             pprint(
-                "Exception when calling QueriesV1beta1Api->v1beta1_queries_id_get: %s\n"
+                "Exception when calling QueriesV1beta2Api->v1beta2_queries_id_get: %s\n"
                 % e
             )
             raise e
```

### Comparing `timeplus-1.1.2/timeplus/stream.py` & `timeplus-1.2.1/timeplus/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .error import TimeplusAPIError
 
 
 class Stream:
     def __init__(self, env):
         self._env = env
         self._configuration = self._env._conf()
-        self._api_instance = swagger_client.StreamsV1beta1Api(
+        self._api_instance = swagger_client.StreamsV1beta2Api(
             swagger_client.ApiClient(self._configuration)
         )
         self._id = None
         self._body = None
         self._columns = None
 
         self._event_time_timezone = None
@@ -93,36 +93,36 @@
         if self._mode:
             body["mode"] = self._mode
 
         if self._primary_key:
             body["primary_key"] = self._primary_key
 
         try:
-            self._metadata = self._api_instance.v1beta1_streams_post(body)
+            self._metadata = self._api_instance.v1beta2_streams_post(body)
             return self
         except ApiException as e:
             pprint(
-                "Exception when calling StreamsV1beta1Api->v1beta1_streams_post: %s\n"
+                "Exception when calling StreamsV1beta2Api->v1beta2_streams_post: %s\n"
                 % e
             )
             raise e
 
     def list(self):
         try:
-            list_response = self._api_instance.v1beta1_streams_get()
+            list_response = self._api_instance.v1beta2_streams_get()
             return list_response
         except ApiException as e:
             pprint(
-                "Exception when calling StreamsV1beta1Api->v1beta1_streams_get: %s\n"
+                "Exception when calling StreamsV1beta2Api->v1beta2_streams_get: %s\n"
                 % e
             )
             raise e
 
     def delete(self):
-        self._api_instance.v1beta1_streams_name_delete(self._name)
+        self._api_instance.v1beta2_streams_name_delete(self._name)
 
     def get(self):
         streams = self.list()
         for s in streams:
             if s.name == self._name:
                 self._metadata = s
                 return self
@@ -131,29 +131,29 @@
     def metadata(self):
         return self._metadata
 
     def ingest(self, colums=None, rows=None, payload=None, format="compact"):
         if format == "compact":
             body = swagger_client.IngestData(colums, rows)
             try:
-                self._api_instance.v1beta1_streams_name_ingest_post(body, self._name)
+                self._api_instance.v1beta2_streams_name_ingest_post(body, self._name)
             except ApiException as e:
                 pprint(
-                    "Exception when calling StreamsV1beta1Api->v1beta1_streams_name_ingest_post: %s\n"
+                    "Exception when calling StreamsV1beta2Api->v1beta2_streams_name_ingest_post: %s\n"
                     % e
                 )
                 raise e
         else:
             try:
-                self._api_instance.v1beta1_streams_name_ingest_post(
+                self._api_instance.v1beta2_streams_name_ingest_post(
                     body=payload, name=self._name, format=format
                 )
             except ApiException as e:
                 pprint(
-                    "Exception when calling StreamsV1beta1Api->v1beta1_streams_name_ingest_post: %s\n"
+                    "Exception when calling StreamsV1beta2Api->v1beta2_streams_name_ingest_post: %s\n"
                     % e
                 )
                 raise e
 
     def exist(self):
         streams = self.list()
         for s in streams:
```

### Comparing `timeplus-1.1.2/timeplus/type.py` & `timeplus-1.2.1/timeplus/type.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.1.2/timeplus.egg-info/PKG-INFO` & `timeplus-1.2.1/timeplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeplus
-Version: 1.1.2
+Version: 1.2.1
 Summary: Timeplus python SDK
 Home-page: https://github.com/timeplus-io/gluon/tree/develop/python
 Author: Gang Tao
 Author-email: gang@timeplus.io
 Project-URL: Bug Tracker, https://github.com/timeplus-io/gluon/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `timeplus-1.1.2/timeplus.egg-info/SOURCES.txt` & `timeplus-1.2.1/timeplus.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,114 +8,97 @@
 ./swagger_client/models/__init__.py
 ./swagger_client/models/analyze_sql_request.py
 ./swagger_client/models/api_key.py
 ./swagger_client/models/batching_policy.py
 ./swagger_client/models/column.py
 ./swagger_client/models/column_def.py
 ./swagger_client/models/columns_resp.py
-./swagger_client/models/connection.py
-./swagger_client/models/connection_config.py
-./swagger_client/models/connection_stat.py
 ./swagger_client/models/create_api_key_request.py
 ./swagger_client/models/create_api_key_response.py
 ./swagger_client/models/create_dashboard_request.py
-./swagger_client/models/create_persistent_query_request.py
-./swagger_client/models/create_query_request_v1_beta1.py
 ./swagger_client/models/create_query_request_v1_beta2.py
-./swagger_client/models/create_query_response.py
 ./swagger_client/models/create_sink_request.py
 ./swagger_client/models/create_source_request.py
+./swagger_client/models/create_view_request.py
 ./swagger_client/models/dashboard_dashboard.py
 ./swagger_client/models/dashboard_panel.py
 ./swagger_client/models/edge.py
 ./swagger_client/models/error_response.py
 ./swagger_client/models/event.py
 ./swagger_client/models/event_infer_request.py
 ./swagger_client/models/event_infer_response.py
 ./swagger_client/models/external_stream_def.py
 ./swagger_client/models/file_upload_response.py
 ./swagger_client/models/format_query_request.py
 ./swagger_client/models/format_query_response.py
 ./swagger_client/models/global_metrics_result.py
 ./swagger_client/models/graph.py
 ./swagger_client/models/ingest_data.py
-./swagger_client/models/internal_http_handler_v1beta2_global_metrics_request.py
-./swagger_client/models/latency.py
+./swagger_client/models/metrics_query_throughput.py
 ./swagger_client/models/node.py
 ./swagger_client/models/owner.py
 ./swagger_client/models/query.py
-./swagger_client/models/query_analysis.py
-./swagger_client/models/query_metrics.py
 ./swagger_client/models/query_pipeline.py
 ./swagger_client/models/query_pipeline_edge.py
 ./swagger_client/models/query_pipeline_node.py
 ./swagger_client/models/query_pipeline_node_metric.py
 ./swagger_client/models/query_result.py
-./swagger_client/models/query_with_metrics.py
-./swagger_client/models/resource_metrics_request.py
 ./swagger_client/models/resource_metrics_result.py
 ./swagger_client/models/sink.py
-./swagger_client/models/sink_metrics.py
 ./swagger_client/models/sink_stat.py
-./swagger_client/models/sink_with_metrics.py
 ./swagger_client/models/source.py
-./swagger_client/models/source_metrics.py
 ./swagger_client/models/source_preview_request.py
 ./swagger_client/models/source_upload_body.py
-./swagger_client/models/source_with_metrics.py
 ./swagger_client/models/sql_analyze_column.py
 ./swagger_client/models/sql_analyze_result.py
 ./swagger_client/models/stream.py
 ./swagger_client/models/stream_def.py
 ./swagger_client/models/stream_match_request.py
 ./swagger_client/models/stream_setting.py
 ./swagger_client/models/stream_stats.py
-./swagger_client/models/throughput.py
 ./swagger_client/models/time_columns.py
 ./swagger_client/models/udf.py
 ./swagger_client/models/udf_argument.py
 ./swagger_client/models/udf_auth_context.py
 ./swagger_client/models/update_dashboard_request.py
 ./swagger_client/models/update_source_request.py
 ./swagger_client/models/update_stream_request.py
 ./swagger_client/models/update_view_request.py
 ./swagger_client/models/view.py
 ./swagger_client/timeplus/__init__.py
-./swagger_client/timeplus/api_keys_v1beta1_api.py
+./swagger_client/timeplus/alerts_internal_api.py
+./swagger_client/timeplus/alerts_v1beta2_api.py
+./swagger_client/timeplus/api_keys_v1beta2_api.py
 ./swagger_client/timeplus/dashboards_v1beta2_api.py
 ./swagger_client/timeplus/metrics_v1beta2_api.py
-./swagger_client/timeplus/persistent_queries_v1beta2_api.py
-./swagger_client/timeplus/queries_v1beta1_api.py
 ./swagger_client/timeplus/queries_v1beta2_api.py
-./swagger_client/timeplus/sinks_v1beta1_api.py
-./swagger_client/timeplus/sources_v1beta1_api.py
-./swagger_client/timeplus/streams_v1beta1_api.py
+./swagger_client/timeplus/sinks_internal_api.py
+./swagger_client/timeplus/sinks_v1beta2_api.py
+./swagger_client/timeplus/sources_v1beta2_api.py
+./swagger_client/timeplus/streams_v1beta2_api.py
 ./swagger_client/timeplus/topology_v1beta2_api.py
-./swagger_client/timeplus/udfs_v1beta1_api.py
-./swagger_client/timeplus/views_v1beta1_api.py
+./swagger_client/timeplus/udfs_v1beta2_api.py
+./swagger_client/timeplus/views_v1beta2_api.py
 ./swagger_test/__init__.py
+./swagger_test/test_alerts_internal_api.py
+./swagger_test/test_alerts_v1beta2_api.py
 ./swagger_test/test_analyze_sql_request.py
 ./swagger_test/test_api_key.py
-./swagger_test/test_api_keys_v1beta1_api.py
+./swagger_test/test_api_keys_v1beta2_api.py
 ./swagger_test/test_batching_policy.py
 ./swagger_test/test_column.py
 ./swagger_test/test_column_def.py
 ./swagger_test/test_columns_resp.py
-./swagger_test/test_connection.py
-./swagger_test/test_connection_config.py
-./swagger_test/test_connection_stat.py
 ./swagger_test/test_create_api_key_request.py
 ./swagger_test/test_create_api_key_response.py
 ./swagger_test/test_create_dashboard_request.py
-./swagger_test/test_create_persistent_query_request.py
-./swagger_test/test_create_query_request_v1_beta1.py
 ./swagger_test/test_create_query_request_v1_beta2.py
-./swagger_test/test_create_query_response.py
 ./swagger_test/test_create_sink_request.py
 ./swagger_test/test_create_source_request.py
+./swagger_test/test_create_view_request.py
 ./swagger_test/test_dashboard_dashboard.py
 ./swagger_test/test_dashboard_panel.py
 ./swagger_test/test_dashboards_v1beta2_api.py
 ./swagger_test/test_edge.py
 ./swagger_test/test_error_response.py
 ./swagger_test/test_event.py
 ./swagger_test/test_event_infer_request.py
@@ -123,65 +106,54 @@
 ./swagger_test/test_external_stream_def.py
 ./swagger_test/test_file_upload_response.py
 ./swagger_test/test_format_query_request.py
 ./swagger_test/test_format_query_response.py
 ./swagger_test/test_global_metrics_result.py
 ./swagger_test/test_graph.py
 ./swagger_test/test_ingest_data.py
-./swagger_test/test_internal_http_handler_v1beta2_global_metrics_request.py
-./swagger_test/test_latency.py
+./swagger_test/test_metrics_query_throughput.py
 ./swagger_test/test_metrics_v1beta2_api.py
 ./swagger_test/test_node.py
 ./swagger_test/test_owner.py
-./swagger_test/test_persistent_queries_v1beta2_api.py
-./swagger_test/test_queries_v1beta1_api.py
 ./swagger_test/test_queries_v1beta2_api.py
 ./swagger_test/test_query.py
-./swagger_test/test_query_analysis.py
-./swagger_test/test_query_metrics.py
 ./swagger_test/test_query_pipeline.py
 ./swagger_test/test_query_pipeline_edge.py
 ./swagger_test/test_query_pipeline_node.py
 ./swagger_test/test_query_pipeline_node_metric.py
 ./swagger_test/test_query_result.py
-./swagger_test/test_query_with_metrics.py
-./swagger_test/test_resource_metrics_request.py
 ./swagger_test/test_resource_metrics_result.py
 ./swagger_test/test_sink.py
-./swagger_test/test_sink_metrics.py
 ./swagger_test/test_sink_stat.py
-./swagger_test/test_sink_with_metrics.py
-./swagger_test/test_sinks_v1beta1_api.py
+./swagger_test/test_sinks_internal_api.py
+./swagger_test/test_sinks_v1beta2_api.py
 ./swagger_test/test_source.py
-./swagger_test/test_source_metrics.py
 ./swagger_test/test_source_preview_request.py
 ./swagger_test/test_source_upload_body.py
-./swagger_test/test_source_with_metrics.py
-./swagger_test/test_sources_v1beta1_api.py
+./swagger_test/test_sources_v1beta2_api.py
 ./swagger_test/test_sql_analyze_column.py
 ./swagger_test/test_sql_analyze_result.py
 ./swagger_test/test_stream.py
 ./swagger_test/test_stream_def.py
 ./swagger_test/test_stream_match_request.py
 ./swagger_test/test_stream_setting.py
 ./swagger_test/test_stream_stats.py
-./swagger_test/test_streams_v1beta1_api.py
-./swagger_test/test_throughput.py
+./swagger_test/test_streams_v1beta2_api.py
 ./swagger_test/test_time_columns.py
 ./swagger_test/test_topology_v1beta2_api.py
 ./swagger_test/test_udf.py
 ./swagger_test/test_udf_argument.py
 ./swagger_test/test_udf_auth_context.py
-./swagger_test/test_udfs_v1beta1_api.py
+./swagger_test/test_udfs_v1beta2_api.py
 ./swagger_test/test_update_dashboard_request.py
 ./swagger_test/test_update_source_request.py
 ./swagger_test/test_update_stream_request.py
 ./swagger_test/test_update_view_request.py
 ./swagger_test/test_view.py
-./swagger_test/test_views_v1beta1_api.py
+./swagger_test/test_views_v1beta2_api.py
 ./timeplus/__init__.py
 ./timeplus/env.py
 ./timeplus/error.py
 ./timeplus/query.py
 ./timeplus/stream.py
 ./timeplus/type.py
 ./timeplus/version.py
```

