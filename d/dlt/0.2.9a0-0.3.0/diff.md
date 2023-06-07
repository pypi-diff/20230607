# Comparing `tmp/dlt-0.2.9a0.tar.gz` & `tmp/dlt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.9a0.tar", max compression
+gzip compressed data, was "dlt-0.3.0.tar", max compression
```

## Comparing `dlt-0.2.9a0.tar` & `dlt-0.3.0.tar`

### file list

```diff
@@ -1,208 +1,213 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.9a0/LICENSE.txt
--rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.9a0/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    15909 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3858 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16665 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18827 2023-05-22 18:37:04.876212 dlt-0.2.9a0/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10489 2023-05-22 18:37:04.876212 dlt-0.2.9a0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9422 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-22 18:37:04.876212 dlt-0.2.9a0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.9a0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1108 2023-05-19 14:44:37.212613 dlt-0.2.9a0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     8349 2023-05-22 21:42:58.160654 dlt-0.2.9a0/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     6560 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    17262 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      912 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0    13108 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5521 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6026 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.9a0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6451 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.9a0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.9a0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.9a0/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.9a0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19121 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.9a0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.9a0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.9a0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8434 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/typing.py
--rw-r--r--   0        0        0    14239 2023-05-22 20:03:28.546212 dlt-0.2.9a0/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12347 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7008 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.9a0/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15625 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1232 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.9a0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.9a0/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.9a0/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26199 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8451 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31737 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-05-22 18:37:10.826212 dlt-0.2.9a0/dlt/extract/schema.py
--rw-r--r--   0        0        0    36384 2023-05-22 21:03:03.346212 dlt-0.2.9a0/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-05-22 18:37:10.826212 dlt-0.2.9a0/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.9a0/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.9a0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0      267 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/helpers/airflow.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19928 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.9a0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16538 2023-05-22 18:37:04.916212 dlt-0.2.9a0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/pipeline/README.md
--rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-22 18:37:04.916212 dlt-0.2.9a0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8764 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    56453 2023-05-22 18:37:10.826212 dlt-0.2.9a0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.9a0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.9a0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.9a0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.9a0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.9a0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9106 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/version.py
--rw-r--r--   0        0        0     4056 2023-05-22 21:06:28.566212 dlt-0.2.9a0/pyproject.toml
--rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 dlt-0.2.9a0/setup.py
--rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.9a0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4131 2023-06-07 09:55:25.911010 dlt-0.3.0/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    16723 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    14636 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14722 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10503 2023-05-28 13:56:42.331452 dlt-0.3.0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-06-07 09:55:25.911010 dlt-0.3.0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.3.0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12390 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2400 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6461 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    18949 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.3.0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14239 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12370 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.3.0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5005 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15639 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.3.0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7117 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8481 2023-06-07 08:32:53.261010 dlt-0.3.0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31816 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38287 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.3.0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.0/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.0/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19925 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16538 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13081 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    59020 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.3.0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.0/dlt/version.py
+-rw-r--r--   0        0        0     4276 2023-06-07 09:58:58.281010 dlt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 dlt-0.3.0/setup.py
+-rw-r--r--   0        0        0     7544 1970-01-01 00:00:00.000000 dlt-0.3.0/PKG-INFO
```

### Comparing `dlt-0.2.9a0/LICENSE.txt` & `dlt-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/README.md` & `dlt-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 - **Easy Maintenance:** Clear data pipeline structure for updates.
 - **Rapid Exploration:** Quickly explore and gain insights from new data sources.
 - **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
 - **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
 - **Incremental Loading:** Load only new or changed data and avoid loading old records again.
 - **Open Source:** Free and Apache 2.0 Licensed.
 
-## Ready to use Pipelines and Destinations
+## Ready to use Sources and Destinations
 
-Explore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
+Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
 
 ## Documentation
 
 For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
 ## Examples
 
@@ -76,14 +76,14 @@
 
 ## Get Involved
 
 The dlt project is quickly growing, and we're excited to have you join our community! Here's how you can get involved:
 
 - **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)
 - **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.
-- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.
+- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.
 - **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.
 - **Improve documentation**: Help us enhance the dlt documentation.
 
 ## License
 
 DLT is released under the [Apache 2.0 License](LICENSE.txt).
```

### Comparing `dlt-0.2.9a0/dlt/__init__.py` & `dlt-0.3.0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/cli/_dlt.py` & `dlt-0.3.0/dlt/cli/_dlt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,95 @@
-from typing import Any, Sequence
+from typing import Any, Sequence, Optional
 import yaml
 import os
 import argparse
 import click
 
 from dlt.version import __version__
 from dlt.common import json
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
 from dlt.common.runners import Venv
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
-from dlt.cli.init_command import init_command, list_pipelines_command, DLT_INIT_DOCS_URL, DEFAULT_PIPELINES_REPO
-from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL
+from dlt.cli.init_command import init_command, list_verified_sources_command, DLT_INIT_DOCS_URL, DEFAULT_VERIFIED_SOURCES_REPO
+from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL, DeploymentMethods, COMMAND_DEPLOY_REPO_LOCATION
 from dlt.cli.pipeline_command import pipeline_command, DLT_PIPELINE_COMMAND_DOCS_URL
 from dlt.cli.telemetry_command import DLT_TELEMETRY_DOCS_URL, change_telemetry_status_command, telemetry_status_command
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 
 
-@utils.track_command("init", False, "pipeline_name", "destination_name")
-def init_command_wrapper(pipeline_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
+@utils.track_command("init", False, "source_name", "destination_name")
+def init_command_wrapper(source_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
     try:
-        init_command(pipeline_name, destination_name, use_generic_template, repo_location, branch)
+        init_command(source_name, destination_name, use_generic_template, repo_location, branch)
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_INIT_DOCS_URL))
         raise
     return 0
 
 
-@utils.track_command("list_pipelines", False)
-def list_pipelines_command_wrapper(repo_location: str, branch: str) -> int:
+@utils.track_command("list_sources", False)
+def list_verified_sources_command_wrapper(repo_location: str, branch: str) -> int:
     try:
-        list_pipelines_command(repo_location, branch)
+        list_verified_sources_command(repo_location, branch)
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_INIT_DOCS_URL))
         return -1
     return 0
 
 
 @utils.track_command("deploy", False, "deployment_method")
-def deploy_command_wrapper(pipeline_script_path: str, deployment_method: str, schedule: str, run_on_push: bool, run_on_dispatch: bool, branch: str) -> int:
+def deploy_command_wrapper(
+    pipeline_script_path: str,
+    deployment_method: str,
+    schedule: Optional[str],
+    run_on_push: bool,
+    run_on_dispatch: bool,
+    repo_location: str,
+    branch: Optional[str]) -> int:
     try:
         utils.ensure_git_command("deploy")
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return -1
 
     from git import InvalidGitRepositoryError, NoSuchPathError
     try:
-        deploy_command(pipeline_script_path, deployment_method, schedule, run_on_push, run_on_dispatch, branch)
+        deploy_command(pipeline_script_path, deployment_method, schedule, run_on_push, run_on_dispatch, repo_location, branch)
     except (CannotRestorePipelineException, PipelineWasNotRun) as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("You must run the pipeline locally successfully at least once in order to deploy it.")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
         return -1
     except InvalidGitRepositoryError:
         click.secho(
-            "No git repository found for pipeline script %s.\nAdd your local code to Github as described here: %s" % (fmt.bold(pipeline_script_path), fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github")),
+            "No git repository found for pipeline script %s." % fmt.bold(pipeline_script_path),
             err=True,
             fg="red"
         )
-        fmt.note("If you do not have a repository yet, the easiest way to proceed is to create one on Github and then clone it here.")
+        fmt.note("If you do not have a repository yet, you can do either of:")
+        fmt.note("- Run the following command to initialize new repository: %s" % fmt.bold("git init"))
+        fmt.note("- Add your local code to Github as described here: %s" % fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github"))
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
         return -1
     except NoSuchPathError as path_ex:
         click.secho(
             "The pipeline script does not exist\n%s" % str(path_ex),
             err=True,
             fg="red"
         )
         return -1
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
+        return -1
         # TODO: display stack trace if with debug flag
     return 0
 
 
 @utils.track_command("pipeline", True, "operation")
 def pipeline_command_wrapper(
         operation: str, pipeline_name: str, pipelines_dir: str, verbosity: int, **command_kwargs: Any
@@ -167,49 +177,55 @@
             help=help
         )
     def __call__(self, parser: argparse.ArgumentParser, namespace: argparse.Namespace, values: Any, option_string: str = None) -> None:
         fmt.ALWAYS_CHOOSE_DEFAULT = True
 
 
 def main() -> int:
-    parser = argparse.ArgumentParser(description="Runs various DLT modules", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser = argparse.ArgumentParser(description="Creates, adds, inspects and deploys dlt pipelines.", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('--version', action="version", version='%(prog)s {version}'.format(version=__version__))
     parser.add_argument('--disable-telemetry', action=TelemetryAction, help="Disables telemetry before command is executed")
     parser.add_argument('--enable-telemetry', action=TelemetryAction, help="Enables telemetry before command is executed")
     parser.add_argument('--non-interactive', action=NonInteractiveAction, help="Non interactive mode. Default choices are automatically made for confirmations and prompts.")
     subparsers = parser.add_subparsers(dest="command")
 
-    init_cmd = subparsers.add_parser("init", help="Adds or creates a pipeline in the current folder.")
-    init_cmd.add_argument("--list-pipelines", "-l",  default=False, action="store_true", help="List available pipelines")
-    init_cmd.add_argument("pipeline", nargs='?', help="Pipeline name. Adds existing pipeline or creates a new pipeline template if pipeline for your data source is not yet implemented.")
+    init_cmd = subparsers.add_parser("init", help="Creates a pipeline project in the current folder by adding existing verified source or creating a new one from template.")
+    init_cmd.add_argument("--list-verified-sources", "-l",  default=False, action="store_true", help="List available verified sources")
+    init_cmd.add_argument("source", nargs='?', help="Name of data source for which to create a pipeline. Adds existing verified source or creates a new pipeline template if verified source for your data source is not yet implemented.")
     init_cmd.add_argument("destination", nargs='?', help="Name of a destination ie. bigquery or redshift")
-    init_cmd.add_argument("--location", default=DEFAULT_PIPELINES_REPO, help="Advanced. Uses a specific url or local path to pipelines repository.")
+    init_cmd.add_argument("--location", default=DEFAULT_VERIFIED_SOURCES_REPO, help="Advanced. Uses a specific url or local path to verified sources repository.")
     init_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the init repository to fetch the template.")
     init_cmd.add_argument("--generic", default=False, action="store_true", help="When present uses a generic template with all the dlt loading code present will be used. Otherwise a debug template is used that can be immediately run to get familiar with the dlt sources.")
 
     deploy_cmd = subparsers.add_parser("deploy", help="Creates a deployment package for a selected pipeline script")
     deploy_cmd.add_argument("pipeline_script_path", metavar="pipeline-script-path", help="Path to a pipeline script")
-    deploy_cmd.add_argument("deployment_method", metavar="deployment-method", choices=["github-action"], default="github-action", help="Deployment method")
-    deploy_cmd.add_argument("--schedule", required=True, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
+    deploy_cmd.add_argument(
+        "deployment_method",
+        metavar="deployment-method",
+        choices=list(map(lambda value: value.value, DeploymentMethods.__members__.values())),
+        default=DeploymentMethods.github_actions.value,
+        help="Deployment method: %s" % ", ".join(map(lambda value: value.value, DeploymentMethods.__members__.values())))
+    deploy_cmd.add_argument("--schedule", required=False, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
     deploy_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
     deploy_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
+    deploy_cmd.add_argument("--location", default=COMMAND_DEPLOY_REPO_LOCATION, help="Advanced. Uses a specific url or local path to pipelines repository.")
     deploy_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the deploy repository to fetch the template.")
 
     schema = subparsers.add_parser("schema", help="Shows, converts and upgrades schemas")
     schema.add_argument("file", help="Schema file name, in yaml or json format, will autodetect based on extension")
     schema.add_argument("--format", choices=["json", "yaml"], default="yaml", help="Display schema in this format")
     schema.add_argument("--remove-defaults", action="store_true", help="Does not show default hint values")
 
     pipe_cmd = subparsers.add_parser("pipeline", help="Operations on pipelines that were ran locally")
     pipe_cmd.add_argument("--list-pipelines", "-l",  default=False, action="store_true", help="List local pipelines")
     pipe_cmd.add_argument("pipeline_name", nargs='?', help="Pipeline name")
     pipe_cmd.add_argument("--pipelines-dir", help="Pipelines working directory", default=None)
     pipe_cmd.add_argument("--verbose", "-v", action='count', default=0, help="Provides more information for certain commands.", dest="verbosity")
     # pipe_cmd.add_argument("--dataset-name", help="Dataset name used to sync destination when local pipeline state is missing.")
-    # pipe_cmd.add_argument("--destination", help="Destination name used to to sync when local pipeline state is missing.")
+    # pipe_cmd.add_argument("--destination", help="Destination name used to sync when local pipeline state is missing.")
 
     pipeline_subparsers = pipe_cmd.add_subparsers(dest="operation", required=False)
 
     pipe_cmd_sync_parent = argparse.ArgumentParser(add_help=False)
     pipe_cmd_sync_parent.add_argument("--destination", help="Sync from this destination when local pipeline state is missing.")
     pipe_cmd_sync_parent.add_argument("--dataset-name", help="Dataset name to sync from when local pipeline state is missing.")
 
@@ -256,24 +272,24 @@
         else:
             command_kwargs = dict(args._get_kwargs())
             command_kwargs['operation'] = args.operation or "info"
             del command_kwargs["command"]
             del command_kwargs["list_pipelines"]
             return pipeline_command_wrapper(**command_kwargs)
     elif args.command == "init":
-        if args.list_pipelines:
-            return list_pipelines_command_wrapper(args.location, args.branch)
+        if args.list_verified_sources:
+            return list_verified_sources_command_wrapper(args.location, args.branch)
         else:
-            if not args.pipeline or not args.destination:
+            if not args.source or not args.destination:
                 init_cmd.print_usage()
                 return -1
             else:
-                return init_command_wrapper(args.pipeline, args.destination, args.generic, args.location, args.branch)
+                return init_command_wrapper(args.source, args.destination, args.generic, args.location, args.branch)
     elif args.command == "deploy":
-        return deploy_command_wrapper(args.pipeline_script_path, args.deployment_method, args.schedule, args.run_on_push, args.run_manually, args.branch)
+        return deploy_command_wrapper(args.pipeline_script_path, args.deployment_method, args.schedule, args.run_on_push, args.run_manually, args.location, args.branch)
     elif args.command == "telemetry":
         return telemetry_status_command_wrapper()
     else:
         print_help(parser)
         return -1
```

### Comparing `dlt-0.2.9a0/dlt/cli/config_toml_writer.py` & `dlt-0.3.0/dlt/cli/config_toml_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,17 +59,16 @@
     if name in toml_table and not overwrite_existing:
         return
     # do not dump final fields
     if is_final_type(hint) or is_optional_type(hint):
         return
     # get the inner hint to generate cool examples
     hint = extract_inner_hint(hint)
-
     if is_base_configuration_inner_hint(hint):
-        inner_table = tomlkit.table(False)
+        inner_table = tomlkit.table(is_super_table=True)
         write_spec(inner_table, hint(), overwrite_existing)
         if len(inner_table) > 0:
             toml_table[name] = inner_table
     else:
         if default_value is None:
             example_value = generate_typed_example(name, hint)
             toml_table[name] = example_value
@@ -89,14 +88,14 @@
 
 
 def write_values(toml: TOMLContainer, values: Iterable[WritableConfigValue], overwrite_existing: bool) -> None:
     for value in values:
         toml_table: TOMLTable = toml  # type: ignore
         for section in value.sections:
             if section not in toml_table:
-                inner_table = tomlkit.table(True)
+                inner_table = tomlkit.table(is_super_table=True)
                 toml_table[section] = inner_table
                 toml_table = inner_table
             else:
                 toml_table = toml_table[section]  # type: ignore
 
         write_value(toml_table, value.name, value.hint, overwrite_existing, default_value=value.default_value, is_default_of_interest=True)
```

### Comparing `dlt-0.2.9a0/dlt/cli/deploy_command.py` & `dlt-0.3.0/dlt/cli/deploy_command_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,229 +1,231 @@
-from itertools import chain
-import os
 import re
-from typing import List
-from astunparse import unparse
+import abc
+import os
 import yaml
 from yaml import Dumper
-import cron_descriptor
-# import pkg_resources
 import pipdeptree
+from itertools import chain
+from typing import List, Optional, Sequence, Tuple, Any, Dict
+from astunparse import unparse
+import cron_descriptor
 
 import dlt
 
 from dlt.common.configuration.exceptions import LookupTrace
-from dlt.common.configuration.providers import ConfigTomlProvider, EnvironProvider, SECRETS_TOML
-from dlt.common.configuration.paths import make_dlt_settings_path
-from dlt.common.configuration.utils import serialize_value
-from dlt.common.git import get_origin, get_repo, is_dirty
+from dlt.common.configuration.providers import ConfigTomlProvider, EnvironProvider
+from dlt.common.git import get_origin, get_repo, Repo
 from dlt.common.configuration.specs.run_configuration import get_default_pipeline_name
+from dlt.common.typing import StrAny
 from dlt.common.reflection.utils import evaluate_node_literal
-from dlt.common.pipeline import LoadInfo
+from dlt.common.pipeline import LoadInfo, TPipelineState
 from dlt.common.storages import FileStorage
-from dlt.common.typing import StrAny
 from dlt.common.utils import set_working_dir
 
+from dlt.pipeline.pipeline import Pipeline
+from dlt.pipeline.trace import PipelineTrace
 from dlt.reflection import names as n
+from dlt.reflection.script_visitor import PipelineScriptVisitor
 
 from dlt.cli import utils
 from dlt.cli import echo as fmt
 from dlt.cli.exceptions import CliCommandException
 
-
-REQUIREMENTS_GITHUB_ACTION = "requirements_github_action.txt"
 GITHUB_URL = "https://github.com/"
-DLT_DEPLOY_DOCS_URL = "https://dlthub.com/docs/walkthroughs/deploy-a-pipeline"
 
 
-def deploy_command(pipeline_script_path: str, deployment_method: str, schedule: str, run_on_push: bool, run_on_dispatch: bool, branch: str = None) -> None:
-    # get current repo local folder
-    with get_repo(pipeline_script_path) as repo:
-        repo_storage = FileStorage(str(repo.working_dir))
+class BaseDeployment(abc.ABC):
+    def __init__(
+        self,
+        pipeline_script_path: str,
+        schedule: Optional[str],
+        run_on_push: bool,
+        run_on_dispatch: bool,
+        repo_location: str,
+        branch: Optional[str] = None
+    ):
+        self.pipeline_script_path = pipeline_script_path
+        self.schedule = schedule
+        self.run_on_push = run_on_push
+        self.run_on_dispatch = run_on_dispatch
+        self.repo_location = repo_location
+        self.branch = branch
+
+        self.pipelines_dir: Optional[str] = None
+        self.pipeline_name: Optional[str] = None
+
+        self.deployment_method: str
+        self.repo: Repo
+        self.repo_storage: FileStorage
+        self.origin: str
+        self.repo_pipeline_script_path: str
+        self.pipeline_script: Any
+        self.schedule_description: Optional[str]
+        self.template_storage: FileStorage
+        self.working_directory: str
+        self.state: TPipelineState
+
+        self.config_prov = ConfigTomlProvider()
+        self.env_prov = EnvironProvider()
+        self.envs: List[LookupTrace] = []
+        self.secret_envs: List[LookupTrace] = []
+        self.artifacts: Dict[str, Any] = {}
+
+    def _prepare_deployment(self) -> None:
+        self.repo_storage = FileStorage(str(self.repo.working_dir))
+        # make sure the repo has origin
+        self.origin = self._get_origin()
+        # convert to path relative to repo
+        self.repo_pipeline_script_path = self.repo_storage.from_wd_to_relative_path(self.pipeline_script_path)
+        # load a pipeline script and extract full_refresh and pipelines_dir args
+        self.pipeline_script = self.repo_storage.load(self.repo_pipeline_script_path)
+        # validate schedule
+        self.schedule_description = self._get_schedule_description()
+        fmt.echo("Looking up the deployment template scripts in %s...\n" % fmt.bold(self.repo_location))
+        self.template_storage = utils.clone_command_repo(self.repo_location, self.branch)
+        self.working_directory = os.path.split(self.pipeline_script_path)[0]
 
-        # check origin
+    def _get_schedule_description(self) -> Optional[Any]:
+        return None if self.schedule is None else cron_descriptor.get_description(self.schedule)
+
+    def _get_origin(self) -> str:
         try:
-            origin = get_origin(repo)
+            origin = get_origin(self.repo)
             if "github.com" not in origin:
                 raise CliCommandException("deploy", f"Your current repository origin is not set to github but to {origin}.\nYou must change it to be able to run the pipelines with github actions: https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories")
         except ValueError:
             raise CliCommandException("deploy", "Your current repository has no origin set. Please set it up to be able to run the pipelines with github actions: https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github")
 
-        # convert to path relative to repo
-        repo_pipeline_script_path = repo_storage.from_wd_to_relative_path(pipeline_script_path)
-        # load pipeline script and extract full_refresh and pipelines_dir args
-        pipeline_script = repo_storage.load(repo_pipeline_script_path)
-        visitor = utils.parse_init_script("deploy", pipeline_script, pipeline_script_path)
-        if n.RUN not in visitor.known_calls:
-            raise CliCommandException("deploy", f"The pipeline script {pipeline_script_path} does not seem to run the pipeline.")
-        # full_refresh = False
-        pipelines_dir: str = None
-        pipeline_name: str = None
-
-        if n.PIPELINE in visitor.known_calls:
-            for call_args in visitor.known_calls[n.PIPELINE]:
-                f_r_node = call_args.arguments.get("full_refresh")
-                if f_r_node:
-                    f_r_value = evaluate_node_literal(f_r_node)
-                    if f_r_value is None:
-                        fmt.warning(f"The value of `full_refresh` in call to `dlt.pipeline` cannot be determined from {unparse(f_r_node).strip()}. We assume that you know what you are doing :)")
-                    if f_r_value is True:
-                        if fmt.confirm("The value of 'full_refresh' is set to True. Do you want to abort to set it to False?", default=True):
-                            return
-                p_d_node = call_args.arguments.get("pipelines_dir")
-                if p_d_node:
-                    pipelines_dir = evaluate_node_literal(p_d_node)
-                    if pipelines_dir is None:
-                        raise CliCommandException("deploy", f"The value of 'pipelines_dir' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipelines-dir option.")
-                p_n_node = call_args.arguments.get("pipeline_name")
-                if p_n_node:
-                    pipeline_name = evaluate_node_literal(p_n_node)
-                    if pipeline_name is None:
-                        raise CliCommandException("deploy", f"The value of 'pipeline_name' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipeline-name option.")
-
-        if pipelines_dir:
-            pipelines_dir = os.path.abspath(pipelines_dir)
-
-        # change the working dir to the script working dir
-        with set_working_dir(os.path.split(pipeline_script_path)[0]):
-            # use script name to derive pipeline name
-            if not pipeline_name:
-                pipeline_name = dlt.config.get("pipeline_name")
-                if not pipeline_name:
-                    pipeline_name = get_default_pipeline_name(pipeline_script_path)
-                    fmt.warning(f"Using default pipeline name {pipeline_name}. The pipeline name is not passed as argument to dlt.pipeline nor configured via config provides ie. config.toml")
-            # attach to pipeline name, get state and trace
-            pipeline = dlt.attach(pipeline_name=pipeline_name, pipelines_dir=pipelines_dir)
-            # trace must exist and end with successful loading step
-            trace = pipeline.last_trace
-            if trace is None or len(trace.steps) == 0:
-                raise PipelineWasNotRun("Pipeline run trace could not be found. Please run the pipeline at least once locally.")
-            last_step = trace.steps[-1]
-            if last_step.step_exception is not None:
-                raise PipelineWasNotRun(f"The last pipeline run ended with error. Please make sure that pipeline runs correctly before deployment.\n{last_step.step_exception}")
-            if not isinstance(last_step.step_info, LoadInfo):
-                raise PipelineWasNotRun("The last pipeline run did not reach the load step. Please run the pipeline locally until it loads data into destination.")
-            # add destination name and dataset name to env
-            state = pipeline.state
-            config_prov = ConfigTomlProvider()
-            env_prov= EnvironProvider()
-            envs: List[LookupTrace] = [
-                # LookupTrace(env_prov.name, (), "destination_name", state["destination"]),
-                LookupTrace(env_prov.name, (), "dataset_name", state["dataset_name"])
-            ]
-            secret_envs: List[LookupTrace] = []
-            for resolved_value in trace.resolved_config_values:
-                if resolved_value.is_secret_hint:
-                    # generate special forms for all secrets
-                    secret_envs.append(LookupTrace(env_prov.name, tuple(resolved_value.sections), resolved_value.key, resolved_value.value))
-                    # fmt.echo(f"{resolved_value.key}:{resolved_value.value}{type(resolved_value.value)} in {resolved_value.sections} is SECRET")
-                else:
-                    # move all config values that are not in config.toml into env
-                    if resolved_value.provider_name != config_prov.name:
-                        envs.append(LookupTrace(env_prov.name, tuple(resolved_value.sections), resolved_value.key, resolved_value.value))
-                        # fmt.echo(f"{resolved_value.key} in {resolved_value.sections} moved to CONFIG")
+        return origin
 
-        # validate schedule
-        schedule_description = cron_descriptor.get_description(schedule)
-
-        template_storage = utils.clone_command_repo("deploy", branch)
-        # template_storage = FileStorage("/home/rudolfix/src/python-dlt-deploy-template")
+    def run_deployment(self) -> None:
+        with get_repo(self.pipeline_script_path) as repo:
+            self.repo = repo
+            self._prepare_deployment()
+            # go through all once launched pipelines
+            visitors = get_visitors(self.pipeline_script, self.pipeline_script_path)
+            pipeline_name, pipelines_dir = parse_pipeline_info(visitors)
+
+            if pipelines_dir:
+                self.pipelines_dir = os.path.abspath(pipelines_dir)
+            if pipeline_name:
+                self.pipeline_name = pipeline_name
+
+            # change the working dir to the script working dir
+            with set_working_dir(self.working_directory):
+                # use script name to derive pipeline name
+                if not self.pipeline_name:
+                    self.pipeline_name = dlt.config.get("pipeline_name")
+                    if not self.pipeline_name:
+                        self.pipeline_name = get_default_pipeline_name(self.pipeline_script_path)
+                        fmt.warning(f"Using default pipeline name {self.pipeline_name}. The pipeline name is not passed as argument to dlt.pipeline nor configured via config provides ie. config.toml")
+
+                # attach to pipeline name, get state and trace
+                pipeline = dlt.attach(pipeline_name=self.pipeline_name, pipelines_dir=self.pipelines_dir)
+                self.state, trace = get_state_and_trace(pipeline)
+                self._update_envs(trace)
+
+            self._generate_workflow()
+            self._echo_instructions()
+            self._make_modification()
+
+    def _update_envs(self, trace: PipelineTrace) -> None:
+        # add destination name and dataset name to env
+        self.envs = [
+            # LookupTrace(self.env_prov.name, (), "destination_name", self.state["destination"]),
+            # LookupTrace(self.env_prov.name, (), "dataset_name", self.state["dataset_name"])
+        ]
+
+        for resolved_value in trace.resolved_config_values:
+            if resolved_value.is_secret_hint:
+                # generate special forms for all secrets
+                self.secret_envs.append(LookupTrace(self.env_prov.name, tuple(resolved_value.sections), resolved_value.key, resolved_value.value))
+                # fmt.echo(f"{resolved_value.key}:{resolved_value.value}{type(resolved_value.value)} in {resolved_value.sections} is SECRET")
+            else:
+                # move all config values that are not in config.toml into env
+                if resolved_value.provider_name != self.config_prov.name:
+                    self.envs.append(LookupTrace(self.env_prov.name, tuple(resolved_value.sections), resolved_value.key, resolved_value.value))
+                    # fmt.echo(f"{resolved_value.key} in {resolved_value.sections} moved to CONFIG")
 
-        # load workload yaml
-        with template_storage.open_file(os.path.join(deployment_method, "run_pipeline_workflow.yml")) as f:
-            workflow = yaml.safe_load(f)
-        # customize the workflow
-        workflow["name"] = f"Run {state['pipeline_name']} pipeline from {pipeline_script_path}"
-        if run_on_push is False:
-            del workflow["on"]["push"]
-        if run_on_dispatch is False:
-            del workflow["on"]["workflow_dispatch"]
-        workflow["on"]["schedule"] = [{"cron": schedule}]
-        workflow["env"] = {}
-        for env_var in envs:
-            env_key = env_prov.get_key_name(env_var.key, *env_var.sections)
-            # print(serialize_value(env_var.value))
-            workflow["env"][env_key] = str(serialize_value(env_var.value))
-        for secret_var in secret_envs:
-            env_key = env_prov.get_key_name(secret_var.key, *secret_var.sections)
-            workflow["env"][env_key] = wrap_template_str("secrets.%s") % env_key
-
-        # run the correct script at the end
-        last_workflow_step = workflow["jobs"]["run_pipeline"]["steps"][-1]
-        assert last_workflow_step["run"] == "python pipeline.py"
-        # must run in the directory of the script
-        wf_run_path, wf_run_name = os.path.split(repo_pipeline_script_path)
-        if wf_run_path:
-            run_cd_cmd = f"cd '{wf_run_path}' && "
-        else:
-            run_cd_cmd = ""
-        last_workflow_step["run"] = f"{run_cd_cmd}python '{wf_run_name}'"
-        serialized_workflow = serialize_templated_yaml(workflow)
-        serialized_workflow_name = f"run_{state['pipeline_name']}_workflow.yml"
-
-        # pip freeze special requirements file
-        with template_storage.open_file(os.path.join(deployment_method, "requirements_blacklist.txt")) as f:
-            requirements_blacklist = f.readlines()
-        requirements_txt = generate_pip_freeze(requirements_blacklist)
-        requirements_txt_name = REQUIREMENTS_GITHUB_ACTION
-
-        # if repo_storage.has_file(utils.REQUIREMENTS_TXT):
-        fmt.echo("Your %s deployment for pipeline %s in script %s is ready!" % (
-            fmt.bold(deployment_method), fmt.bold(state["pipeline_name"]), fmt.bold(pipeline_script_path)
-        ))
-        #  It contains all relevant configurations and references to credentials that are needed to run the pipeline
-        fmt.echo("* A github workflow file %s was created in %s." % (
-            fmt.bold(serialized_workflow_name), fmt.bold(utils.GITHUB_WORKFLOWS_DIR)
-        ))
-        fmt.echo("* The schedule with which the pipeline is run is: %s.%s%s" % (
-            fmt.bold(schedule_description),
-            " You can also run the pipeline manually." if run_on_dispatch else "",
-            " Pipeline will also run on each push to the repository." if run_on_push else "",
-        ))
-        fmt.echo("* The dependencies that will be used to run the pipeline are stored in %s. If you change add more dependencies, remember to refresh your deployment by running the same 'deploy' command again." % fmt.bold(requirements_txt_name))
-        fmt.echo()
-        fmt.echo("You should now add the secrets to github repository secrets, commit and push the pipeline files to github.")
-        fmt.echo("1. Add the following secret values (typically stored in %s): \n%s\nin %s" % (
-            fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
-            fmt.bold("\n".join(env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in secret_envs)),
-            fmt.bold(github_origin_to_url(origin, "/settings/secrets/actions"))
-        ))
-        fmt.echo()
-        # if fmt.confirm("Do you want to list the values of the secrets in the format suitable for github?", default=True):
-        for s_v in secret_envs:
+    def _echo_secrets(self) -> None:
+        for s_v in self.secret_envs:
             fmt.secho("Name:", fg="green")
-            fmt.echo(fmt.bold(env_prov.get_key_name(s_v.key, *s_v.sections)))
+            fmt.echo(fmt.bold(self.env_prov.get_key_name(s_v.key, *s_v.sections)))
             fmt.secho("Secret:", fg="green")
             fmt.echo(s_v.value)
             fmt.echo()
 
-        fmt.echo("2. Add stage deployment files to commit. Use your Git UI or the following command")
-        fmt.echo(fmt.bold(f"git add {repo_storage.from_relative_path_to_wd(requirements_txt_name)} {repo_storage.from_relative_path_to_wd(os.path.join(utils.GITHUB_WORKFLOWS_DIR, serialized_workflow_name))}"))
-        fmt.echo()
-        fmt.echo("3. Commit the files above. Use your Git UI or the following command")
-        fmt.echo(fmt.bold(f"git commit -m 'run {state['pipeline_name']} pipeline with github action'"))
-        if is_dirty(repo):
-            fmt.warning("You have modified files in your repository. Do not forget to push changes to your pipeline script as well!")
-        fmt.echo()
-        fmt.echo("4. Push changes to github. Use your Git UI or the following command")
-        fmt.echo(fmt.bold("git push origin"))
-        fmt.echo()
-        fmt.echo("5. Your pipeline should be running! You can monitor it here:")
-        fmt.echo(fmt.bold(github_origin_to_url(origin, f"/actions/workflows/{serialized_workflow_name}")))
-
-        if not repo_storage.has_folder(utils.GITHUB_WORKFLOWS_DIR):
-            repo_storage.create_folder(utils.GITHUB_WORKFLOWS_DIR)
-
-        repo_storage.save(os.path.join(utils.GITHUB_WORKFLOWS_DIR, serialized_workflow_name), serialized_workflow)
-        repo_storage.save(requirements_txt_name, requirements_txt)
+    def _echo_envs(self) -> None:
+        for v in self.envs:
+            fmt.secho("Name:", fg="green")
+            fmt.echo(fmt.bold(self.env_prov.get_key_name(v.key, *v.sections)))
+            fmt.secho("Value:", fg="green")
+            fmt.echo(v.value)
+            fmt.echo()
 
+    @abc.abstractmethod
+    def _echo_instructions(self, *args: Optional[Any]) -> Optional[Any]:
+        pass
+
+    @abc.abstractmethod
+    def _generate_workflow(self, *args: Optional[Any]) -> Optional[Any]:
+        pass
+
+    @abc.abstractmethod
+    def _make_modification(self) -> None:
+        pass
+
+
+def get_state_and_trace(pipeline: Pipeline) -> Tuple[TPipelineState, PipelineTrace]:
+    # trace must exist and end with a successful loading step
+    trace = pipeline.last_trace
+    if trace is None or len(trace.steps) == 0:
+        raise PipelineWasNotRun("Pipeline run trace could not be found. Please run the pipeline at least once locally.")
+    last_step = trace.steps[-1]
+    if last_step.step_exception is not None:
+        raise PipelineWasNotRun(f"The last pipeline run ended with error. Please make sure that pipeline runs correctly before deployment.\n{last_step.step_exception}")
+    if not isinstance(last_step.step_info, LoadInfo):
+        raise PipelineWasNotRun("The last pipeline run did not reach the load step. Please run the pipeline locally until it loads data into destination.")
+
+    return pipeline.state, trace
+
+
+def get_visitors(pipeline_script: str, pipeline_script_path: str) -> PipelineScriptVisitor:
+    visitor = utils.parse_init_script("deploy", pipeline_script, pipeline_script_path)
+    if n.RUN not in visitor.known_calls:
+        raise CliCommandException("deploy", f"The pipeline script {pipeline_script_path} does not seem to run the pipeline.")
+    return visitor
+
+
+def parse_pipeline_info(visitor: PipelineScriptVisitor) -> Tuple[Optional[str], Optional[str]]:
+    pipeline_name, pipelines_dir = None, None
+    if n.PIPELINE in visitor.known_calls:
+        for call_args in visitor.known_calls[n.PIPELINE]:
+            f_r_node = call_args.arguments.get("full_refresh")
+            if f_r_node:
+                f_r_value = evaluate_node_literal(f_r_node)
+                if f_r_value is None:
+                    fmt.warning(f"The value of `full_refresh` in call to `dlt.pipeline` cannot be determined from {unparse(f_r_node).strip()}. We assume that you know what you are doing :)")
+                if f_r_value is True:
+                    if fmt.confirm("The value of 'full_refresh' is set to True. Do you want to abort to set it to False?", default=True):
+                        return None, None
+
+            p_d_node = call_args.arguments.get("pipelines_dir")
+            if p_d_node:
+                pipelines_dir = evaluate_node_literal(p_d_node)
+                if pipelines_dir is None:
+                    raise CliCommandException("deploy", f"The value of 'pipelines_dir' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipelines-dir option.")
+
+            p_n_node = call_args.arguments.get("pipeline_name")
+            if p_n_node:
+                pipeline_name = evaluate_node_literal(p_n_node)
+                if pipeline_name is None:
+                    raise CliCommandException("deploy", f"The value of 'pipeline_name' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipeline-name option.")
 
-class PipelineWasNotRun(CliCommandException):
-    def __init__(self, msg: str) -> None:
-        super().__init__("deploy", msg, None)
+    return pipeline_name, pipelines_dir
 
 
 def str_representer(dumper: yaml.Dumper, data: str) -> yaml.ScalarNode:
     # format multiline strings as blocks with the exception of placeholders
     # that will be expanded as yaml
     if len(data.splitlines()) > 1 and "{{ toYaml" not in data:  # check for multiline string
         return dumper.represent_scalar('tag:yaml.org,2002:str', data, style='|')
@@ -251,16 +253,15 @@
                             r"\1 \2",
                             serialized)
         return serialized
     finally:
         yaml.add_representer(str, old_representer)
 
 
-def generate_pip_freeze(requirements_blacklist: List[str]) -> str:
-
+def generate_pip_freeze(requirements_blacklist: List[str], requirements_file_name: str) -> str:
     pkgs = pipdeptree.get_installed_distributions(local_only=True, user_only=False)
 
     # construct graph with all packages
     tree = pipdeptree.PackageDAG.from_pkgs(pkgs)
     nodes = tree.keys()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
     # all the top level packages
@@ -277,15 +278,15 @@
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
     nodes = [p for p in nodes if p.key not in branch_keys]
 
     # detect and warn on conflict
     conflicts = pipdeptree.conflicting_deps(tree)
     cycles = pipdeptree.cyclic_deps(tree)
     if conflicts:
-        fmt.warning(f"Unable to create dependencies for the github action. Please edit {REQUIREMENTS_GITHUB_ACTION} yourself")
+        fmt.warning(f"Unable to create dependencies for the github action. Please edit {requirements_file_name} yourself")
         pipdeptree.render_conflicts_text(conflicts)
         pipdeptree.render_cycles_text(cycles)
         fmt.echo()
         # do not create package because it will most probably fail
         return "# please provide valid dependencies including dlt package"
 
     lines = [node.render(None, False) for node in nodes]
@@ -297,12 +298,25 @@
     if origin.endswith(".git"):
         origin = origin[:-4]
     if origin.startswith("git@github.com:"):
         origin = origin[15:]
 
     if not origin.startswith(GITHUB_URL):
         origin = GITHUB_URL + origin
-    #https://github.com/dlt-hub/data-loading-zoomcamp.git
-    #git@github.com:dlt-hub/data-loading-zoomcamp.git
+    # https://github.com/dlt-hub/data-loading-zoomcamp.git
+    # git@github.com:dlt-hub/data-loading-zoomcamp.git
 
     # https://github.com/dlt-hub/data-loading-zoomcamp/settings/secrets/actions
-    return origin + path
+    return origin + path
+
+
+def ask_files_overwrite(files: Sequence[str]) -> None:
+    existing = [file for file in files if os.path.exists(file)]
+    if existing:
+        fmt.echo("Following files will be overwritten: %s" % fmt.bold(str(existing)))
+        if not fmt.confirm("Do you want to continue?", default=False):
+            raise CliCommandException("init", "Aborted")
+
+
+class PipelineWasNotRun(CliCommandException):
+    def __init__(self, msg: str) -> None:
+        super().__init__("deploy", msg, None)
```

### Comparing `dlt-0.2.9a0/dlt/cli/echo.py` & `dlt-0.3.0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/cli/init_command.py` & `dlt-0.3.0/dlt/cli/init_command.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,52 +9,52 @@
 from dlt.common.configuration.paths import get_dlt_settings_dir, make_dlt_settings_path
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.providers import CONFIG_TOML, SECRETS_TOML, ConfigTomlProvider, SecretsTomlProvider
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.pipeline import get_dlt_repos_dir
 from dlt.common.source import _SOURCES
 from dlt.version import DLT_PKG_NAME, __version__
-from dlt.common.destination.reference import DestinationReference
+from dlt.common.destination import DestinationReference
 from dlt.common.reflection.utils import rewrite_python_script
 from dlt.common.schema.exceptions import InvalidSchemaName
 from dlt.common.storages.file_storage import FileStorage
 
 import dlt.reflection.names as n
 from dlt.reflection.script_inspector import inspect_pipeline_script, load_script_module
 
 from dlt.cli import echo as fmt, pipeline_files as files_ops, source_detection
 from dlt.cli import utils
 from dlt.cli.config_toml_writer import WritableConfigValue, write_values
-from dlt.cli.pipeline_files import PipelineFiles, TPipelineFileEntry, TPipelineFileIndex
+from dlt.cli.pipeline_files import VerifiedSourceFiles, TVerifiedSourceFileEntry, TVerifiedSourceFileIndex
 from dlt.cli.exceptions import CliCommandException
 
 DLT_INIT_DOCS_URL = "https://dlthub.com/docs/reference/command-line-interface#dlt-init"
-DEFAULT_PIPELINES_REPO = "https://github.com/dlt-hub/pipelines.git"
+DEFAULT_VERIFIED_SOURCES_REPO = "https://github.com/dlt-hub/verified-sources.git"
 INIT_MODULE_NAME = "init"
-PIPELINES_MODULE_NAME = "pipelines"
+SOURCES_MODULE_NAME = "sources"
 
 
 def _get_template_files(command_module: ModuleType, use_generic_template: bool) -> Tuple[str, List[str]]:
     template_files: List[str] = command_module.TEMPLATE_FILES
     pipeline_script: str = command_module.PIPELINE_SCRIPT
     if use_generic_template:
         pipeline_script, py = os.path.splitext(pipeline_script)
         pipeline_script = f"{pipeline_script}_generic{py}"
     return pipeline_script, template_files
 
 
-def _select_pipeline_files(
-    pipeline_name: str,
-    remote_modified: Dict[str, TPipelineFileEntry],
-    remote_deleted: Dict[str, TPipelineFileEntry],
+def _select_source_files(
+    source_name: str,
+    remote_modified: Dict[str, TVerifiedSourceFileEntry],
+    remote_deleted: Dict[str, TVerifiedSourceFileEntry],
     conflict_modified: Sequence[str],
     conflict_deleted: Sequence[str]
-) -> Tuple[str, Dict[str, TPipelineFileEntry], Dict[str, TPipelineFileEntry]]:
+) -> Tuple[str, Dict[str, TVerifiedSourceFileEntry], Dict[str, TVerifiedSourceFileEntry]]:
     # some files were changed and cannot be updated (or are created without index)
-    fmt.echo("Existing files for %s pipeline were changed and cannot be automatically updated" % fmt.bold(pipeline_name))
+    fmt.echo("Existing files for %s source were changed and cannot be automatically updated" % fmt.bold(source_name))
     if conflict_modified:
         fmt.echo("Following files are MODIFIED locally and CONFLICT with incoming changes: %s" % fmt.bold(", ".join(conflict_modified)))
     if conflict_deleted:
         fmt.echo("Following files are DELETED locally and CONFLICT with incoming changes: %s" % fmt.bold(", ".join(conflict_deleted)))
     can_update_files = set(remote_modified.keys()) - set(conflict_modified)
     can_delete_files = set(remote_deleted.keys()) - set(conflict_deleted)
     if len(can_update_files) > 0 or len(can_delete_files) > 0:
@@ -91,249 +91,248 @@
         return utils.PYPROJECT_TOML
     elif dest_storage.has_file(utils.REQUIREMENTS_TXT):
         return utils.REQUIREMENTS_TXT
     else:
         return None
 
 
-def _list_pipelines(repo_location: str, branch: str = None) -> Dict[str, PipelineFiles]:
+def _list_verified_sources(repo_location: str, branch: str = None) -> Dict[str, VerifiedSourceFiles]:
     clone_storage = git.get_fresh_repo_files(repo_location, get_dlt_repos_dir(), branch=branch)
-    pipelines_storage = FileStorage(clone_storage.make_full_path(PIPELINES_MODULE_NAME))
+    sources_storage = FileStorage(clone_storage.make_full_path(SOURCES_MODULE_NAME))
 
-    pipelines: Dict[str, PipelineFiles] = {}
-    for pipeline_name in files_ops.get_pipeline_names(pipelines_storage):
+    sources: Dict[str, VerifiedSourceFiles] = {}
+    for source_name in files_ops.get_verified_source_names(sources_storage):
         try:
-            pipelines[pipeline_name] = files_ops.get_pipeline_files(pipelines_storage, pipeline_name)
+            sources[source_name] = files_ops.get_verified_source_files(sources_storage, source_name)
         except Exception as ex:
-            fmt.warning(f"Pipeline {pipeline_name} not available: {ex}")
+            fmt.warning(f"Verified source {source_name} not available: {ex}")
 
-    return pipelines
+    return sources
 
 
-def _welcome_message(pipeline_name: str, destination_name: str, pipeline_files: PipelineFiles, dependency_system: str, is_new_pipeline: bool) -> None:
+def _welcome_message(source_name: str, destination_name: str, source_files: VerifiedSourceFiles, dependency_system: str, is_new_source: bool) -> None:
     fmt.echo()
-    if pipeline_files.is_template:
-        fmt.echo("Your new pipeline %s is ready to be customized!" % fmt.bold(pipeline_name))
-        fmt.echo("* Review and change how dlt loads your data in %s" % fmt.bold(pipeline_files.dest_pipeline_script))
+    if source_files.is_template:
+        fmt.echo("Your new pipeline %s is ready to be customized!" % fmt.bold(source_name))
+        fmt.echo("* Review and change how dlt loads your data in %s" % fmt.bold(source_files.dest_pipeline_script))
     else:
-        if is_new_pipeline:
-            fmt.echo("Pipeline %s was added to your project!" % fmt.bold(pipeline_name))
-            fmt.echo("* See the usage examples and code snippets to copy from %s" % fmt.bold(pipeline_files.dest_pipeline_script))
+        if is_new_source:
+            fmt.echo("Verified source %s was added to your project!" % fmt.bold(source_name))
+            fmt.echo("* See the usage examples and code snippets to copy from %s" % fmt.bold(source_files.dest_pipeline_script))
         else:
-            fmt.echo("Pipeline %s was updated to the newest version!" % fmt.bold(pipeline_name))
+            fmt.echo("Verified source %s was updated to the newest version!" % fmt.bold(source_name))
 
-    if is_new_pipeline:
+    if is_new_source:
         fmt.echo("* Add credentials for %s and other secrets in %s" % (fmt.bold(destination_name), fmt.bold(make_dlt_settings_path(SECRETS_TOML))))
 
     if dependency_system:
         fmt.echo("* Add the required dependencies to %s:" % fmt.bold(dependency_system))
-        for dep in pipeline_files.requirements:
+        for dep in source_files.requirements:
             fmt.echo("  " + fmt.bold(dep))
         fmt.echo("  If the dlt dependency is already added, make sure you install the extra for %s to it" % fmt.bold(destination_name))
         if dependency_system == utils.REQUIREMENTS_TXT:
             qs = "' '"
-            fmt.echo("  To install with pip: %s" % fmt.bold(f"pip3 install '{qs.join(pipeline_files.requirements)}'"))
+            fmt.echo("  To install with pip: %s" % fmt.bold(f"pip3 install '{qs.join(source_files.requirements)}'"))
         elif dependency_system == utils.PYPROJECT_TOML:
             fmt.echo("  If you are using poetry you may issue the following command:")
             fmt.echo(fmt.bold("  poetry add %s -E %s" % (DLT_PKG_NAME, destination_name)))
         fmt.echo()
     else:
         fmt.echo("* %s was created. Install it with:\npip3 install -r %s" % (fmt.bold(utils.REQUIREMENTS_TXT), utils.REQUIREMENTS_TXT))
 
-    if is_new_pipeline:
+    if is_new_source:
         fmt.echo("* Read %s for more information" % fmt.bold("https://dlthub.com/docs/walkthroughs/create-a-pipeline"))
     else:
-        fmt.echo("* Read %s for more information" % fmt.bold("https://dlthub.com/docs/walkthroughs/add-a-pipeline"))
+        fmt.echo("* Read %s for more information" % fmt.bold("https://dlthub.com/docs/walkthroughs/add-a-verified-source"))
 
 
-def list_pipelines_command(repo_location: str, branch: str = None) -> None:
-    fmt.echo("Looking up the init scripts in %s..." % fmt.bold(repo_location))
-    for pipeline_name, pipeline_files in _list_pipelines(repo_location, branch).items():
-        fmt.echo("%s: %s" % (fmt.bold(pipeline_name), pipeline_files.doc))
+def list_verified_sources_command(repo_location: str, branch: str = None) -> None:
+    fmt.echo("Looking up for verified sources in %s..." % fmt.bold(repo_location))
+    for source_name, source_files in _list_verified_sources(repo_location, branch).items():
+        fmt.echo("%s: %s" % (fmt.bold(source_name), source_files.doc))
 
 
-def init_command(pipeline_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str = None) -> None:
+def init_command(source_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str = None) -> None:
     # try to import the destination and get config spec
     destination_reference = DestinationReference.from_name(destination_name)
     destination_spec = destination_reference.spec()
 
     fmt.echo("Looking up the init scripts in %s..." % fmt.bold(repo_location))
     clone_storage = git.get_fresh_repo_files(repo_location, get_dlt_repos_dir(), branch=branch)
     # copy init files from here
     init_storage = FileStorage(clone_storage.make_full_path(INIT_MODULE_NAME))
-    # copy pipeline files from here
-    pipelines_storage = FileStorage(clone_storage.make_full_path(PIPELINES_MODULE_NAME))
+    # copy dlt source files from here
+    sources_storage = FileStorage(clone_storage.make_full_path(SOURCES_MODULE_NAME))
     # load init module and get init files and script
     init_module = load_script_module(clone_storage.storage_path, INIT_MODULE_NAME)
     pipeline_script, template_files = _get_template_files(init_module, use_generic_template)
     # prepare destination storage
     dest_storage = FileStorage(os.path.abspath("."))
     if not dest_storage.has_folder(get_dlt_settings_dir()):
         dest_storage.create_folder(get_dlt_settings_dir())
-    # get local index of pipeline files
-    local_index = files_ops.load_pipeline_local_index(pipeline_name)
+    # get local index of verified source files
+    local_index = files_ops.load_verified_sources_local_index(source_name)
     # folder deleted at dest - full refresh
-    if not dest_storage.has_folder(pipeline_name):
+    if not dest_storage.has_folder(source_name):
         local_index["files"] = {}
-    # is update or new pipeline
-    is_new_pipeline = len(local_index["files"]) == 0
+    # is update or new source
+    is_new_source = len(local_index["files"]) == 0
 
-    # look for existing pipeline
-    pipeline_files: PipelineFiles = None
-    remote_index: TPipelineFileIndex = None
-    if pipelines_storage.has_folder(pipeline_name):
+    # look for existing source
+    source_files: VerifiedSourceFiles = None
+    remote_index: TVerifiedSourceFileIndex = None
+    if sources_storage.has_folder(source_name):
         # get pipeline files
-        pipeline_files = files_ops.get_pipeline_files(pipelines_storage, pipeline_name)
-        # get file index from remote pipeline files being copied
-        remote_index = files_ops.get_remote_pipeline_index(pipeline_files.storage.storage_path, pipeline_files.files)
+        source_files = files_ops.get_verified_source_files(sources_storage, source_name)
+        # get file index from remote verified source files being copied
+        remote_index = files_ops.get_remote_source_index(source_files.storage.storage_path, source_files.files)
         # diff local and remote index to get modified and deleted files
         remote_new, remote_modified, remote_deleted = files_ops.gen_index_diff(local_index, remote_index)
         # find files that are modified locally
         conflict_modified, conflict_deleted = files_ops.find_conflict_files(local_index, remote_new, remote_modified, remote_deleted, dest_storage)
         # add new to modified
         remote_modified.update(remote_new)
         if conflict_modified or conflict_deleted:
-            # select pipeline files that can be copied/updated
-            _, remote_modified, remote_deleted = _select_pipeline_files(
-                pipeline_name,
+            # select source files that can be copied/updated
+            _, remote_modified, remote_deleted = _select_source_files(
+                source_name,
                 remote_modified,
                 remote_deleted,
                 conflict_modified,
                 conflict_deleted
             )
         if not remote_deleted and not remote_modified:
             fmt.echo("No files to update, exiting")
             return
 
         if remote_index["is_dirty"]:
-            fmt.warning(f"The pipelines repository is dirty. {pipeline_name} pipeline files may not update correctly in the future.")
+            fmt.warning(f"The verified sources repository is dirty. {source_name} source files may not update correctly in the future.")
         # add template files
-        pipeline_files.files.extend(template_files)
+        source_files.files.extend(template_files)
 
     else:
         # normalize source name
         naming, _ = import_normalizers(default_normalizers())
-        norm_source_name = naming.normalize_identifier(pipeline_name)
-        if norm_source_name != pipeline_name:
-            raise InvalidSchemaName(pipeline_name, norm_source_name)
+        norm_source_name = naming.normalize_identifier(source_name)
+        if norm_source_name != source_name:
+            raise InvalidSchemaName(source_name, norm_source_name)
         dest_pipeline_script = norm_source_name + ".py"
-        pipeline_files = PipelineFiles(True, init_storage, pipeline_script, dest_pipeline_script, template_files, [], "")
+        source_files = VerifiedSourceFiles(True, init_storage, pipeline_script, dest_pipeline_script, template_files, [], "")
         if dest_storage.has_file(dest_pipeline_script):
             fmt.warning("Pipeline script %s already exist, exiting" % dest_pipeline_script)
             return
 
     # add .dlt/*.toml files to be copied
-    pipeline_files.files.extend([make_dlt_settings_path(CONFIG_TOML), make_dlt_settings_path(SECRETS_TOML)])
+    source_files.files.extend([make_dlt_settings_path(CONFIG_TOML), make_dlt_settings_path(SECRETS_TOML)])
 
     # add dlt extras line to requirements
     req_dep = f"{DLT_PKG_NAME}[{destination_name}]"
     req_dep_line = f"{req_dep}>={pkg_version(DLT_PKG_NAME)}"
-    pipeline_files.requirements.insert(0, req_dep_line)
+    source_files.requirements.insert(0, req_dep_line)
 
     # read module source and parse it
-    visitor = utils.parse_init_script("init", pipeline_files.storage.load(pipeline_files.pipeline_script), pipeline_files.pipeline_script)
+    visitor = utils.parse_init_script("init", source_files.storage.load(source_files.pipeline_script), source_files.pipeline_script)
     if visitor.is_destination_imported:
-        raise CliCommandException("init", f"The pipeline script {pipeline_files.pipeline_script} import a destination from dlt.destinations. You should specify destinations by name when calling dlt.pipeline or dlt.run in init scripts.")
+        raise CliCommandException("init", f"The pipeline script {source_files.pipeline_script} import a destination from dlt.destinations. You should specify destinations by name when calling dlt.pipeline or dlt.run in init scripts.")
     if n.PIPELINE not in visitor.known_calls:
-        raise CliCommandException("init", f"The pipeline script {pipeline_files.pipeline_script} does not seem to initialize pipeline with dlt.pipeline. Please initialize pipeline explicitly in init scripts.")
+        raise CliCommandException("init", f"The pipeline script {source_files.pipeline_script} does not seem to initialize pipeline with dlt.pipeline. Please initialize pipeline explicitly in init scripts.")
 
     # find all arguments in all calls to replace
     transformed_nodes = source_detection.find_call_arguments_to_replace(
         visitor,
-        [("destination", destination_name), ("pipeline_name", pipeline_name), ("dataset_name", pipeline_name + "_data")],
-        pipeline_files.pipeline_script
+        [("destination", destination_name), ("pipeline_name", source_name), ("dataset_name", source_name + "_data")],
+        source_files.pipeline_script
     )
 
     # inspect the script
     inspect_pipeline_script(
-        pipeline_files.storage.storage_path,
-        pipeline_files.storage.to_relative_path(pipeline_files.pipeline_script),
+        source_files.storage.storage_path,
+        source_files.storage.to_relative_path(source_files.pipeline_script),
         ignore_missing_imports=True
     )
 
     # detect all the required secrets and configs that should go into tomls files
-    if pipeline_files.is_template:
+    if source_files.is_template:
         # replace destination, pipeline_name and dataset_name in templates
         transformed_nodes = source_detection.find_call_arguments_to_replace(
             visitor,
-            [("destination", destination_name), ("pipeline_name", pipeline_name), ("dataset_name", pipeline_name + "_data")],
-            pipeline_files.pipeline_script
+            [("destination", destination_name), ("pipeline_name", source_name), ("dataset_name", source_name + "_data")],
+            source_files.pipeline_script
         )
         # template sources are always in module starting with "pipeline"
         # for templates, place config and secrets into top level section
         required_secrets, required_config, checked_sources = source_detection.detect_source_configs(_SOURCES, "pipeline", ())
         # template has a strict rules where sources are placed
         for source_q_name, source_config in checked_sources.items():
             if source_q_name not in visitor.known_sources_resources:
-                raise CliCommandException("init", f"The pipeline script {pipeline_files.pipeline_script} imports a source/resource {source_config.f.__name__} from module {source_config.module.__name__}. In init scripts you must declare all sources and resources in single file.")
+                raise CliCommandException("init", f"The pipeline script {source_files.pipeline_script} imports a source/resource {source_config.f.__name__} from module {source_config.module.__name__}. In init scripts you must declare all sources and resources in single file.")
         # rename sources and resources
-        transformed_nodes.extend(source_detection.find_source_calls_to_replace(visitor, pipeline_name))
+        transformed_nodes.extend(source_detection.find_source_calls_to_replace(visitor, source_name))
     else:
         # replace only destination for existing pipelines
-        transformed_nodes = source_detection.find_call_arguments_to_replace(visitor, [("destination", destination_name)], pipeline_files.pipeline_script)
+        transformed_nodes = source_detection.find_call_arguments_to_replace(visitor, [("destination", destination_name)], source_files.pipeline_script)
         # pipeline sources are in module with name starting from {pipeline_name}
         # for verified pipelines place in the specific source section
-        required_secrets, required_config, checked_sources = source_detection.detect_source_configs(_SOURCES, pipeline_name, (known_sections.SOURCES, pipeline_name))
+        required_secrets, required_config, checked_sources = source_detection.detect_source_configs(_SOURCES, source_name, (known_sections.SOURCES, source_name))
 
     if len(checked_sources) == 0:
-        raise CliCommandException("init", f"The pipeline script {pipeline_files.pipeline_script} is not creating or importing any sources or resources")
+        raise CliCommandException("init", f"The pipeline script {source_files.pipeline_script} is not creating or importing any sources or resources")
 
     # add destination spec to required secrets
-    credentials_type = destination_spec().get_resolvable_fields()["credentials"]
-    required_secrets["destinations:" + destination_name] = WritableConfigValue("credentials", credentials_type, None, ("destination", destination_name))
+    required_secrets["destinations:" + destination_name] = WritableConfigValue(destination_name, destination_spec, None, ("destination",))
     # add the global telemetry to required config
     required_config["runtime.dlthub_telemetry"] = WritableConfigValue("dlthub_telemetry", bool, utils.get_telemetry_status(), ("runtime", ))
 
     # modify the script
     script_lines = rewrite_python_script(visitor.source_lines, transformed_nodes)
     dest_script_source = "".join(script_lines)
     # validate by parsing
     ast.parse(source=dest_script_source)
 
     # ask for confirmation
-    if is_new_pipeline:
-        if pipeline_files.is_template:
-            fmt.echo("An existing pipeline %s was not found. Creating a new pipeline with name %s." % (fmt.bold(pipeline_name), fmt.bold(pipeline_name)))
+    if is_new_source:
+        if source_files.is_template:
+            fmt.echo("A verified source %s was not found. Using a template to create a new source and pipeline with name %s." % (fmt.bold(source_name), fmt.bold(source_name)))
         else:
-            fmt.echo("Cloning and configuring an existing pipeline %s (%s)" % (fmt.bold(pipeline_name), pipeline_files.doc))
+            fmt.echo("Cloning and configuring a verified source %s (%s)" % (fmt.bold(source_name), source_files.doc))
             if use_generic_template:
-                fmt.warning("--generic parameter is meaningless if verified pipeline is used")
+                fmt.warning("--generic parameter is meaningless if verified source is found")
         if not fmt.confirm("Do you want to proceed?", default=True):
             raise CliCommandException("init", "Aborted")
 
     dependency_system = _get_dependency_system(dest_storage)
-    _welcome_message(pipeline_name, destination_name, pipeline_files, dependency_system, is_new_pipeline)
+    _welcome_message(source_name, destination_name, source_files, dependency_system, is_new_source)
 
     # copy files at the very end
-    for file_name in pipeline_files.files:
+    for file_name in source_files.files:
         dest_path = dest_storage.make_full_path(file_name)
         # get files from init section first
         if init_storage.has_file(file_name):
             if dest_storage.has_file(dest_path):
                 # do not overwrite any init files
                 continue
             src_path = init_storage.make_full_path(file_name)
         else:
-            # only those that were modified should be copied from pipeline
+            # only those that were modified should be copied from verified sources
             if file_name in remote_modified:
-                src_path = pipeline_files.storage.make_full_path(file_name)
+                src_path = source_files.storage.make_full_path(file_name)
             else:
                 continue
         os.makedirs(os.path.dirname(dest_path), exist_ok=True)
         shutil.copy2(src_path, dest_path)
 
     if remote_index:
         # delete files
         for file_name in remote_deleted:
             if dest_storage.has_file(file_name):
                 dest_storage.delete(file_name)
-        files_ops.save_pipeline_local_index(pipeline_name, remote_index, remote_modified, remote_deleted)
+        files_ops.save_verified_source_local_index(source_name, remote_index, remote_modified, remote_deleted)
     # create script
-    if not dest_storage.has_file(pipeline_files.dest_pipeline_script):
-        dest_storage.save(pipeline_files.dest_pipeline_script, dest_script_source)
+    if not dest_storage.has_file(source_files.dest_pipeline_script):
+        dest_storage.save(source_files.dest_pipeline_script, dest_script_source)
 
     # generate tomls with comments
     secrets_prov = SecretsTomlProvider()
     # print(secrets_prov._toml)
     write_values(secrets_prov._toml, required_secrets.values(), overwrite_existing=False)
     config_prov = ConfigTomlProvider()
     write_values(config_prov._toml, required_config.values(), overwrite_existing=False)
@@ -341,9 +340,9 @@
     secrets_prov.write_toml()
     config_prov.write_toml()
 
     # telemetry_status_command()
 
     # if there's no dependency system write the requirements file
     if dependency_system is None:
-        requirements_txt = "\n".join(pipeline_files.requirements)
+        requirements_txt = "\n".join(source_files.requirements)
         dest_storage.save(utils.REQUIREMENTS_TXT, requirements_txt)
```

### Comparing `dlt-0.2.9a0/dlt/cli/pipeline_command.py` & `dlt-0.3.0/dlt/cli/pipeline_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,19 @@
         if operation == "sync":
             return  # No need to sync again
 
     fmt.echo("Found pipeline %s in %s" % (fmt.bold(p.pipeline_name), fmt.bold(p.pipelines_dir)))
 
     if operation == "show":
         from dlt.common.runtime import signals
-        from dlt.helpers import streamlit
+        from dlt.helpers import streamlit_helper
 
         with signals.delayed_signals():
             venv = Venv.restore_current()
-            for line in iter_stdout(venv, "streamlit", "run", streamlit.__file__, pipeline_name):
+            for line in iter_stdout(venv, "streamlit", "run", streamlit_helper.__file__, pipeline_name):
                 fmt.echo(line)
 
     if operation == "info":
         state: TSourceState = p.state  # type: ignore
         fmt.echo("Synchronized state:")
         for k, v in state.items():
             if not isinstance(v, dict):
```

### Comparing `dlt-0.2.9a0/dlt/cli/pipeline_files.py` & `dlt-0.3.0/dlt/cli/pipeline_files.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 import fnmatch
 import hashlib
 import os
 import yaml
 import posixpath
 from pathlib import Path
 from typing import Dict, NamedTuple, Sequence, Tuple, TypedDict, List
-from dlt.cli.exceptions import PipelineRepoError
+from dlt.cli.exceptions import VerifiedSourceRepoError
 
 from dlt.common import git
 from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.storages import FileStorage
 
 from dlt.common.reflection.utils import get_module_docstring
 
 from dlt.cli import utils
 
 
-PIPELINES_INIT_INFO_ENGINE_VERSION = 1
-PIPELINES_INIT_INFO_FILE = ".pipelines"
+SOURCES_INIT_INFO_ENGINE_VERSION = 1
+SOURCES_INIT_INFO_FILE = ".sources"
 IGNORE_FILES = ["*.py[cod]", "*$py.class", "__pycache__", "py.typed", "requirements.txt"]
-IGNORE_PIPELINES = [".*", "_*"]
+IGNORE_SOURCES = [".*", "_*"]
 
 
-class PipelineFiles(NamedTuple):
+class VerifiedSourceFiles(NamedTuple):
     is_template: bool
     storage: FileStorage
     pipeline_script: str
     dest_pipeline_script: str
     files: List[str]
     requirements: List[str]
     doc: str
 
 
-class TPipelineFileEntry(TypedDict):
+class TVerifiedSourceFileEntry(TypedDict):
     commit_sha: str
     git_sha: str
     sha3_256: str
 
 
-class TPipelineFileIndex(TypedDict):
+class TVerifiedSourceFileIndex(TypedDict):
     is_dirty: bool
     last_commit_sha: str
     last_commit_timestamp: str
-    files: Dict[str, TPipelineFileEntry]
+    files: Dict[str, TVerifiedSourceFileEntry]
 
 
-class TPipelinesFileIndex(TypedDict):
+class TVerifiedSourcesFileIndex(TypedDict):
     engine_version: int
-    pipelines: Dict[str, TPipelineFileIndex]
+    sources: Dict[str, TVerifiedSourceFileIndex]
 
 
-def _save_dot_pipelines(index: TPipelinesFileIndex) -> None:
-    with open(make_dlt_settings_path(PIPELINES_INIT_INFO_FILE), "w", encoding="utf-8") as f:
+def _save_dot_sources(index: TVerifiedSourcesFileIndex) -> None:
+    with open(make_dlt_settings_path(SOURCES_INIT_INFO_FILE), "w", encoding="utf-8") as f:
         yaml.dump(index, f, allow_unicode=True, default_flow_style=False, sort_keys=False)
 
 
-def _load_dot_pipelines() -> TPipelinesFileIndex:
+def _load_dot_sources() -> TVerifiedSourcesFileIndex:
     try:
-        with open(make_dlt_settings_path(PIPELINES_INIT_INFO_FILE), "r", encoding="utf-8") as f:
-            index: TPipelinesFileIndex = yaml.safe_load(f)
+        with open(make_dlt_settings_path(SOURCES_INIT_INFO_FILE), "r", encoding="utf-8") as f:
+            index: TVerifiedSourcesFileIndex = yaml.safe_load(f)
             if not index:
-                raise FileNotFoundError(PIPELINES_INIT_INFO_FILE)
+                raise FileNotFoundError(SOURCES_INIT_INFO_FILE)
             return index
     except FileNotFoundError:
         return {
-            "engine_version": PIPELINES_INIT_INFO_ENGINE_VERSION,
-            "pipelines": {}
+            "engine_version": SOURCES_INIT_INFO_ENGINE_VERSION,
+            "sources": {}
         }
 
 
 def _merge_remote_index(
-    local_index: TPipelineFileIndex,
-    remote_index: TPipelineFileIndex,
-    remote_modified: Dict[str, TPipelineFileEntry],
-    remote_deleted: Dict[str, TPipelineFileEntry]
-) -> TPipelineFileIndex:
+    local_index: TVerifiedSourceFileIndex,
+    remote_index: TVerifiedSourceFileIndex,
+    remote_modified: Dict[str, TVerifiedSourceFileEntry],
+    remote_deleted: Dict[str, TVerifiedSourceFileEntry]
+) -> TVerifiedSourceFileIndex:
     # update all modified files
     local_index["files"].update(remote_modified)
     # delete all deleted
     for deleted in remote_deleted:
         del local_index["files"][deleted]
     # update global info
     local_index["is_dirty"] = remote_index["is_dirty"]
     local_index["last_commit_sha"] = remote_index["last_commit_sha"]
     local_index["last_commit_timestamp"] = remote_index["last_commit_timestamp"]
 
     return local_index
 
 
-def load_pipeline_local_index(pipeline_name: str) -> TPipelineFileIndex:
-    return _load_dot_pipelines()["pipelines"].get(pipeline_name, {
+def load_verified_sources_local_index(source_name: str) -> TVerifiedSourceFileIndex:
+    return _load_dot_sources()["sources"].get(source_name, {
         "is_dirty": False,
         "last_commit_sha": None,
         "last_commit_timestamp": None,
         "files": {}
         }
     )
 
 
-def save_pipeline_local_index(
-    pipeline_name: str,
-    remote_index: TPipelineFileIndex,
-    remote_modified: Dict[str, TPipelineFileEntry],
-    remote_deleted: Dict[str, TPipelineFileEntry]
+def save_verified_source_local_index(
+    source_name: str,
+    remote_index: TVerifiedSourceFileIndex,
+    remote_modified: Dict[str, TVerifiedSourceFileEntry],
+    remote_deleted: Dict[str, TVerifiedSourceFileEntry]
 ) -> None:
 
-    all_pipelines = _load_dot_pipelines()
-    local_index = all_pipelines["pipelines"].setdefault(pipeline_name, remote_index)
+    all_sources = _load_dot_sources()
+    local_index = all_sources["sources"].setdefault(source_name, remote_index)
     _merge_remote_index(local_index, remote_index, remote_modified, remote_deleted)
-    _save_dot_pipelines(all_pipelines)
+    _save_dot_sources(all_sources)
 
 
-def get_remote_pipeline_index(repo_path: str, files: Sequence[str]) -> TPipelineFileIndex:
+def get_remote_source_index(repo_path: str, files: Sequence[str]) -> TVerifiedSourceFileIndex:
 
     with git.get_repo(repo_path) as repo:
         tree = repo.tree()
         commit_sha = repo.head.commit.hexsha
-        files_sha: Dict[str, TPipelineFileEntry] = {}
+        files_sha: Dict[str, TVerifiedSourceFileEntry] = {}
         for file in files:
             posix_file = os.path.join(repo_path, file)
             posix_file = os.path.relpath(posix_file, repo.working_dir)
             posix_file = posixpath.join(*Path(posix_file).parts)
             try:
                 blob_sha3 = tree.join(posix_file).hexsha
             except KeyError:
@@ -139,64 +139,64 @@
             "is_dirty": git.is_dirty(repo),
             "last_commit_sha": commit_sha,
             "last_commit_timestamp": repo.head.commit.committed_datetime.isoformat(),
             "files": files_sha
         }
 
 
-def get_pipeline_names(pipelines_storage: FileStorage) -> List[str]:
+def get_verified_source_names(sources_storage: FileStorage) -> List[str]:
     candidates: List[str] = []
-    for name in [n for n in pipelines_storage.list_folder_dirs(".", to_root=False) if not any(fnmatch.fnmatch(n, ignore) for ignore in IGNORE_PIPELINES)]:
+    for name in [n for n in sources_storage.list_folder_dirs(".", to_root=False) if not any(fnmatch.fnmatch(n, ignore) for ignore in IGNORE_SOURCES)]:
         # must contain at least one valid python script
-        if any(f.endswith(".py") for f in pipelines_storage.list_folder_files(name, to_root=False)):
+        if any(f.endswith(".py") for f in sources_storage.list_folder_files(name, to_root=False)):
             candidates.append(name)
     return candidates
 
 
-def get_pipeline_files(pipelines_storage: FileStorage, pipeline_name: str) -> PipelineFiles:
-    if not pipelines_storage.has_folder(pipeline_name):
-        raise PipelineRepoError(f"Pipeline {pipeline_name} could not be found in the repository", pipeline_name)
+def get_verified_source_files(sources_storage: FileStorage, source_name: str) -> VerifiedSourceFiles:
+    if not sources_storage.has_folder(source_name):
+        raise VerifiedSourceRepoError(f"Verified source {source_name} could not be found in the repository", source_name)
     # find example script
-    example_script = f"{pipeline_name}_pipeline.py"
-    if not pipelines_storage.has_file(example_script):
-        raise PipelineRepoError(f"Pipeline example script {example_script} could not be found in the repository", pipeline_name)
+    example_script = f"{source_name}_pipeline.py"
+    if not sources_storage.has_file(example_script):
+        raise VerifiedSourceRepoError(f"Pipeline example script {example_script} could not be found in the repository", source_name)
     # get all files recursively
     files: List[str] = []
-    for root, subdirs, _files in os.walk(pipelines_storage.make_full_path(pipeline_name)):
+    for root, subdirs, _files in os.walk(sources_storage.make_full_path(source_name)):
         # filter unwanted files
         for subdir in list(subdirs):
             if any(fnmatch.fnmatch(subdir, ignore) for ignore in IGNORE_FILES):
                 subdirs.remove(subdir)
-        rel_root = pipelines_storage.to_relative_path(root)
+        rel_root = sources_storage.to_relative_path(root)
         files.extend([os.path.join(rel_root, file) for file in _files if all(not fnmatch.fnmatch(file, ignore) for ignore in IGNORE_FILES)])
     # read the docs
-    init_py =  os.path.join(pipeline_name, utils.MODULE_INIT)
+    init_py =  os.path.join(source_name, utils.MODULE_INIT)
     docstring: str = ""
-    if pipelines_storage.has_file(init_py):
-        docstring = get_module_docstring(pipelines_storage.load(init_py))
+    if sources_storage.has_file(init_py):
+        docstring = get_module_docstring(sources_storage.load(init_py))
         if docstring:
             docstring = docstring.splitlines()[0]
     # read requirements
-    requirements_path = os.path.join(pipeline_name, utils.REQUIREMENTS_TXT)
-    if pipelines_storage.has_file(requirements_path):
-        requirements = pipelines_storage.load(requirements_path).splitlines()
+    requirements_path = os.path.join(source_name, utils.REQUIREMENTS_TXT)
+    if sources_storage.has_file(requirements_path):
+        requirements = sources_storage.load(requirements_path).splitlines()
     else:
         requirements = []
     # find requirements
-    return PipelineFiles(False, pipelines_storage, example_script, example_script, files, requirements, docstring)
+    return VerifiedSourceFiles(False, sources_storage, example_script, example_script, files, requirements, docstring)
 
 
 def gen_index_diff(
-    local_index: TPipelineFileIndex,
-    remote_index: TPipelineFileIndex
-) -> Tuple[Dict[str, TPipelineFileEntry], Dict[str, TPipelineFileEntry], Dict[str, TPipelineFileEntry]]:
-
-    deleted: Dict[str, TPipelineFileEntry] = {}
-    modified: Dict[str, TPipelineFileEntry] = {}
-    new: Dict[str, TPipelineFileEntry] = {}
+    local_index: TVerifiedSourceFileIndex,
+    remote_index: TVerifiedSourceFileIndex
+) -> Tuple[Dict[str, TVerifiedSourceFileEntry], Dict[str, TVerifiedSourceFileEntry], Dict[str, TVerifiedSourceFileEntry]]:
+
+    deleted: Dict[str, TVerifiedSourceFileEntry] = {}
+    modified: Dict[str, TVerifiedSourceFileEntry] = {}
+    new: Dict[str, TVerifiedSourceFileEntry] = {}
 
     for name, entry in remote_index["files"].items():
         if name not in local_index["files"]:
             new[name] = entry
         elif entry["sha3_256"] != local_index["files"][name]["sha3_256"]:
             modified[name] = entry
 
@@ -210,25 +210,25 @@
     # print(modified)
     # print("DEL")
     # print(deleted)
     return new, modified, deleted
 
 
 def find_conflict_files(
-    local_index: TPipelineFileIndex,
-    remote_new: Dict[str, TPipelineFileEntry],
-    remote_modified: Dict[str, TPipelineFileEntry],
-    remote_deleted: Dict[str, TPipelineFileEntry],
+    local_index: TVerifiedSourceFileIndex,
+    remote_new: Dict[str, TVerifiedSourceFileEntry],
+    remote_modified: Dict[str, TVerifiedSourceFileEntry],
+    remote_deleted: Dict[str, TVerifiedSourceFileEntry],
     dest_storage: FileStorage
 ) -> Tuple[List[str], List[str]]:
-    """Use files index from .pipelines to identify modified files via sha3 content hash"""
+    """Use files index from .sources to identify modified files via sha3 content hash"""
 
     conflict_modified: List[str] = []
 
-    def is_file_modified(file: str, entry: TPipelineFileEntry) -> bool:
+    def is_file_modified(file: str, entry: TVerifiedSourceFileEntry) -> bool:
         with dest_storage.open_file(file, "br") as f:
             file_blob = f.read()
         # file exists but was not changed
         return hashlib.sha3_256(file_blob).hexdigest() != entry["sha3_256"]
 
     for file, entry in remote_new.items():
         if dest_storage.has_file(file):
```

### Comparing `dlt-0.2.9a0/dlt/cli/source_detection.py` & `dlt-0.3.0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/cli/telemetry_command.py` & `dlt-0.3.0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/cli/utils.py` & `dlt-0.3.0/dlt/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 from dlt.common.configuration.specs import RunConfiguration
 
 from dlt.reflection.script_visitor import PipelineScriptVisitor
 
 from dlt.cli.exceptions import CliCommandException
 
 
-COMMAND_REPO_LOCATION = "https://github.com/dlt-hub/python-dlt-%s-template.git"
 REQUIREMENTS_TXT = "requirements.txt"
 PYPROJECT_TOML = "pyproject.toml"
 GITHUB_WORKFLOWS_DIR = os.path.join(".github", "workflows")
+AIRFLOW_DAGS_FOLDER = os.path.join("dags")
+AIRFLOW_BUILD_FOLDER = os.path.join("build")
 LOCAL_COMMAND_REPO_FOLDER = "repos"
 MODULE_INIT = "__init__.py"
 
 
-def clone_command_repo(command: str, branch: str) -> FileStorage:
+def clone_command_repo(repo_location: str, branch: str) -> FileStorage:
     template_dir = tempfile.mkdtemp()
     # TODO: handle ImportError (no git command available) gracefully
-    with git.clone_repo(COMMAND_REPO_LOCATION % command, template_dir, branch=branch):
+    with git.clone_repo(repo_location, template_dir, branch=branch):
         return FileStorage(template_dir)
 
 
 def parse_init_script(command: str, script_source: str, init_script_name: str) -> PipelineScriptVisitor:
     # parse the script first
     tree = ast.parse(source=script_source)
     set_ast_parents(tree)
```

### Comparing `dlt-0.2.9a0/dlt/common/arithmetics.py` & `dlt-0.3.0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/accessors.py` & `dlt-0.3.0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/container.py` & `dlt-0.3.0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/exceptions.py` & `dlt-0.3.0/dlt/common/configuration/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     value: Any
 
 
 class ConfigurationException(DltException, TerminalException):
     pass
 
 
+class ConfigurationValueError(ConfigurationException, ValueError):
+    pass
+
+
 class ContainerException(DltException):
     """base exception for all exceptions related to injectable container"""
     pass
 
 
 class ConfigProviderException(ConfigurationException):
     """base exceptions for all exceptions raised by config providers"""
@@ -44,21 +48,36 @@
             msg += f'\tfor field "{f}" config providers and keys were tried in following order:\n'
             for tr in field_traces:
                 msg += f'\t\tIn {tr.provider} key {tr.key} was not found.\n'
         msg += "Please refer to https://dlthub.com/docs/general-usage/credentials for more information\n"
         return msg
 
 
+class UnmatchedConfigHintResolversException(ConfigurationException):
+    """Raised when using `@resolve_type` on a field that doesn't exist in the spec"""
+    def __init__(self, spec_name: str, field_names: Sequence[str]) -> None:
+        self.field_names = field_names
+        self.spec_name = spec_name
+        example = f">>> class {spec_name}(BaseConfiguration)\n" + "\n".join(f">>>    {name}: Any" for name in field_names)
+        msg = (
+            f"The config spec {spec_name} has dynamic type resolvers for fields: {field_names} "
+            "but these fields are not defined in the spec.\n"
+            "When using @resolve_type() decorator, Add the fields with 'Any' or another common type hint, example:\n"
+            f"\n{example}"
+        )
+        super().__init__(msg)
+
+
 class FinalConfigFieldException(ConfigurationException):
     """rises when field was annotated as final ie Final[str] and the value is modified by config provider"""
     def __init__(self, spec_name: str, field: str) -> None:
         super().__init__(f"Field {field} in spec {spec_name} is final but is being changed by a config provider")
 
 
-class ConfigValueCannotBeCoercedException(ConfigurationException, ValueError):
+class ConfigValueCannotBeCoercedException(ConfigurationValueError):
     """raises when value returned by config provider cannot be coerced to hinted type"""
 
     def __init__(self, field_name: str, field_value: Any, hint: type) -> None:
         self.field_name = field_name
         self.field_value = field_value
         self.hint = hint
         super().__init__('Configured value for field %s cannot be coerced into type %s' % (field_name, str(hint)))
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/inject.py` & `dlt-0.3.0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/paths.py` & `dlt-0.3.0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.0/dlt/common/configuration/providers/airflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-import tomlkit
 from airflow.models import Variable
 
-from .toml import BaseTomlProvider
+from .toml import VaultTomlProvider
 
-AIRFLOW_SECRETS_TOML_VARIABLE_KEY = 'dlt_secrets_toml'
 
-
-class AirflowSecretsTomlProvider(BaseTomlProvider):
-    def __init__(
-        self, variable_key: str = AIRFLOW_SECRETS_TOML_VARIABLE_KEY
-    ) -> None:
-        """Reads TOML configuration data from an Airflow variable specified
-        by the `variable_key` and initializes a BaseTomlProvider with the
-        parsed content.
-
-        Args:
-            variable_key (str, optional): The Airflow variable key to read secrets from.
-                Defaults to AIRFLOW_SECRETS_TOML_VARIABLE_KEY.
-        """
-        toml_content = self._read_toml_from_airflow(variable_key)
-        super().__init__(toml_content)
-
-    def _read_toml_from_airflow(
-        self, variable_key: str
-    ) -> tomlkit.TOMLDocument:
-        toml_string = Variable.get(variable_key)
-        return tomlkit.parse(toml_string)
+class AirflowSecretsTomlProvider(VaultTomlProvider):
+    def __init__(self, only_secrets: bool = False, only_toml_fragments: bool = False) -> None:
+        super().__init__(only_secrets, only_toml_fragments)
 
     @property
     def name(self) -> str:
         return 'Airflow Secrets TOML Provider'
 
+    def _look_vault(self, full_key: str, hint: type) -> str:
+        """Get Airflow Variable with given `full_key`, return None if not found"""
+        return Variable.get(full_key, default_var=None)  # type: ignore
+
     @property
     def supports_secrets(self) -> bool:
         return True
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/providers/context.py` & `dlt-0.3.0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/providers/environ.py` & `dlt-0.3.0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/providers/provider.py` & `dlt-0.3.0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/resolve.py` & `dlt-0.3.0/dlt/common/configuration/resolve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import itertools
 from collections.abc import Mapping as C_Mapping
 from typing import Any, Dict, ContextManager, List, Optional, Sequence, Tuple, Type, TypeVar
 
 from dlt.common.configuration.providers.provider import ConfigProvider
 from dlt.common.typing import AnyType, StrAny, TSecretValue, get_all_types_of_class_in_union, is_final_type, is_optional_type, is_union
 
-from dlt.common.configuration.specs.base_configuration import BaseConfiguration, CredentialsConfiguration, is_secret_hint, extract_inner_hint, is_context_inner_hint, is_base_configuration_inner_hint
+from dlt.common.configuration.specs.base_configuration import BaseConfiguration, CredentialsConfiguration, is_secret_hint, extract_inner_hint, is_context_inner_hint, is_base_configuration_inner_hint, is_valid_hint
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
 from dlt.common.configuration.utils import log_traces, deserialize_value
-from dlt.common.configuration.exceptions import (FinalConfigFieldException, LookupTrace, ConfigFieldMissingException, ConfigurationWrongTypeException, ValueNotSecretException, InvalidNativeValue)
+from dlt.common.configuration.exceptions import (
+    FinalConfigFieldException, LookupTrace, ConfigFieldMissingException, ConfigurationWrongTypeException,
+    ValueNotSecretException, InvalidNativeValue, UnmatchedConfigHintResolversException)
 
 TConfiguration = TypeVar("TConfiguration", bound=BaseConfiguration)
 
 
 def resolve_configuration(config: TConfiguration, *, sections: Tuple[str, ...] = (), explicit_value: Any = None, accept_partial: bool = False) -> TConfiguration:
     if not isinstance(config, BaseConfiguration):
         raise ConfigurationWrongTypeException(type(config))
@@ -113,14 +115,17 @@
         accept_partial: bool
     ) -> None:
 
     fields = config.get_resolvable_fields()
     unresolved_fields: Dict[str, Sequence[LookupTrace]] = {}
 
     for key, hint in fields.items():
+        if key in config.__hint_resolvers__:
+            # Type hint for this field is created dynamically
+            hint = config.__hint_resolvers__[key](config)
         # get default and explicit values
         default_value = getattr(config, key, None)
         traces: List[LookupTrace] = []
 
         if explicit_values:
             explicit_value = explicit_values.get(key)
         else:
@@ -131,43 +136,77 @@
                 explicit_value = None
 
         # if hint is union of configurations, any of them must be resolved
         specs_in_union: List[Type[BaseConfiguration]] = []
         current_value = None
         if is_union(hint):
             # print(f"HINT UNION?: {key}:{hint}")
-            specs_in_union = get_all_types_of_class_in_union(hint, BaseConfiguration)
-        if len(specs_in_union) > 1:
-            for idx, alt_spec in enumerate(specs_in_union):
-                # return first resolved config from an union
-                try:
-                    current_value, traces = _resolve_config_field(key, alt_spec, default_value, explicit_value, config, config.__section__, explicit_sections, embedded_sections, accept_partial)
-                    break
-                except ConfigFieldMissingException as cfm_ex:
-                    # add traces from unresolved union spec
-                    # TODO: we should group traces per hint - currently user will see all options tried without the key info
-                    traces.extend(list(itertools.chain(*cfm_ex.traces.values())))
-                except InvalidNativeValue:
-                    # if none of specs in union parsed
-                    if idx == len(specs_in_union) - 1:
-                        raise
-        else:
-            current_value, traces = _resolve_config_field(key, hint, default_value, explicit_value, config, config.__section__, explicit_sections, embedded_sections, accept_partial)
+            # if union contains a type of explicit value which is not a valid hint, return it as current value
+            if explicit_value and not is_valid_hint(type(explicit_value)) and get_all_types_of_class_in_union(hint, type(explicit_value)):
+                current_value, traces = explicit_value, []
+            else:
+                specs_in_union = get_all_types_of_class_in_union(hint, BaseConfiguration)
+        if not current_value:
+            if len(specs_in_union) > 1:
+                for idx, alt_spec in enumerate(specs_in_union):
+                    # return first resolved config from an union
+                    try:
+                        current_value, traces = _resolve_config_field(
+                            key,
+                            alt_spec,
+                            default_value,
+                            explicit_value,
+                            config,
+                            config.__section__,
+                            explicit_sections,
+                            embedded_sections,
+                            accept_partial
+                        )
+                        break
+                    except ConfigFieldMissingException as cfm_ex:
+                        # add traces from unresolved union spec
+                        # TODO: we should group traces per hint - currently user will see all options tried without the key info
+                        traces.extend(list(itertools.chain(*cfm_ex.traces.values())))
+                    except InvalidNativeValue:
+                        # if none of specs in union parsed
+                        if idx == len(specs_in_union) - 1:
+                            raise
+            else:
+                current_value, traces = _resolve_config_field(
+                    key,
+                    hint,
+                    default_value,
+                    explicit_value,
+                    config,
+                    config.__section__,
+                    explicit_sections,
+                    embedded_sections,
+                    accept_partial
+                )
 
         # check if hint optional
         is_optional = is_optional_type(hint)
         # collect unresolved fields
         if not is_optional and current_value is None:
             unresolved_fields[key] = traces
         # set resolved value in config
         if default_value != current_value:
             if is_final_type(hint):
                 raise FinalConfigFieldException(type(config).__name__, key)
             setattr(config, key, current_value)
 
+    # Check for dynamic hint resolvers which have no corresponding fields
+    unmatched_hint_resolvers: List[str] = []
+    for field_name in config.__hint_resolvers__:
+        if field_name not in fields:
+            unmatched_hint_resolvers.append(field_name)
+
+    if unmatched_hint_resolvers:
+        raise UnmatchedConfigHintResolversException(type(config).__name__, unmatched_hint_resolvers)
+
     if unresolved_fields:
         raise ConfigFieldMissingException(type(config).__name__, unresolved_fields)
 
 
 def _resolve_config_field(
         key: str,
         hint: Type[Any],
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.0/dlt/common/configuration/specs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .run_configuration import RunConfiguration  # noqa: F401
 from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint, configspec  # noqa: F401
 from .config_section_context import ConfigSectionContext  # noqa: F401
 
 from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults, GcpServiceAccountCredentials, GcpOAuthCredentialsWithoutDefaults, GcpOAuthCredentials, GcpCredentials  # noqa: F401
 from .connection_string_credentials import ConnectionStringCredentials  # noqa: F401
 from .api_credentials import OAuth2Credentials  # noqa: F401
+from .aws_credentials import AwsCredentials  # noqa: F401
 
 
 # backward compatibility for service account credentials
-from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults as GcpClientCredentials, GcpServiceAccountCredentials as GcpClientCredentialsWithDefault  # noqa: F401
+from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults as GcpClientCredentials, GcpServiceAccountCredentials as GcpClientCredentialsWithDefault  # noqa: F401
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.0/dlt/common/configuration/specs/base_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import contextlib
 import dataclasses
 from collections.abc import Mapping as C_Mapping
-from typing import Callable, List, Optional, Union, Any, Dict, Iterator, MutableMapping, Type, TYPE_CHECKING, get_args, get_origin, overload, ClassVar
+from typing import Callable, List, Optional, Union, Any, Dict, Iterator, MutableMapping, Type, TYPE_CHECKING, get_args, get_origin, overload, ClassVar, TypeVar
+from functools import wraps
 
 if TYPE_CHECKING:
     TDtcField = dataclasses.Field[Any]
 else:
     TDtcField = dataclasses.Field
 
 from dlt.common.typing import TAnyClass, TSecretValue, extract_inner_type, is_optional_type, is_union
@@ -93,29 +94,34 @@
 
     In comparison the Python dataclass, a spec implements full dictionary interface for its attributes, allows instance creation from ie. strings
     or other types (parsing, deserialization) and control over configuration resolution process. See `BaseConfiguration` and CredentialsConfiguration` for
     more information.
 
     """
     def wrap(cls: Type[TAnyClass]) -> Type[TAnyClass]:
+        cls.__hint_resolvers__ = {}  # type: ignore[attr-defined]
         is_context = issubclass(cls, _F_ContainerInjectableContext)
         # if type does not derive from BaseConfiguration then derive it
         with contextlib.suppress(NameError):
             if not issubclass(cls, BaseConfiguration):
                 # keep the original module
                 fields = {"__module__": cls.__module__, "__annotations__": getattr(cls, "__annotations__", {})}
                 cls = type(cls.__name__, (cls, _F_BaseConfiguration), fields)
         # get all annotations without corresponding attributes and set them to None
         for ann in cls.__annotations__:
             if not hasattr(cls, ann) and not ann.startswith(("__", "_abc_impl")):
                 setattr(cls, ann, None)
         # get all attributes without corresponding annotations
         for att_name, att_value in cls.__dict__.items():
             # skip callables, dunder names, class variables and some special names
-            if not callable(att_value) and not att_name.startswith(("__", "_abc_impl")) and not isinstance(att_value, (staticmethod, classmethod, property)):
+            if callable(att_value):
+                if hint_field_name := getattr(att_value, "__hint_for_field__", None):
+                    cls.__hint_resolvers__[hint_field_name] = att_value  # type: ignore[attr-defined]
+                continue
+            if not att_name.startswith(("__", "_abc_impl")) and not isinstance(att_value, (staticmethod, classmethod, property)):
                 if att_name not in cls.__annotations__:
                     raise ConfigFieldMissingTypeHintException(att_name, cls)
                 hint = cls.__annotations__[att_name]
                 # context can have any type
                 if not is_valid_hint(hint) and not is_context:
                     raise ConfigFieldTypeHintNotSupported(att_name, cls, hint)
         # do not generate repr as it may contain secret values
@@ -124,27 +130,29 @@
     # called with parenthesis
     if cls is None:
         return wrap
 
     return wrap(cls)
 
 
+
 @configspec
 class BaseConfiguration(MutableMapping[str, Any]):
 
     __is_resolved__: bool = dataclasses.field(default = False, init=False, repr=False)
     """True when all config fields were resolved and have a specified value type"""
     __section__: str = dataclasses.field(default = None, init=False, repr=False)
     """Obligatory section used by config providers when searching for keys, always present in the search path"""
     __exception__: Exception = dataclasses.field(default = None, init=False, repr=False)
     """Holds the exception that prevented the full resolution"""
     __config_gen_annotations__: ClassVar[List[str]] = []
     """Additional annotations for config generator, currently holds a list of fields of interest that have defaults"""
     __dataclass_fields__: ClassVar[Dict[str, TDtcField]]
     """Typing for dataclass fields"""
+    __hint_resolvers__: ClassVar[Dict[str, Callable[["BaseConfiguration"], Type[Any]]]] = {}
 
     def parse_native_representation(self, native_value: Any) -> None:
         """Initialize the configuration fields by parsing the `native_value` which should be a native representation of the configuration
         or credentials, for example database connection string or JSON serialized GCP service credentials file.
 
         ### Args:
             native_value (Any): A native representation of the configuration
@@ -165,15 +173,20 @@
             Any: A native representation of the configuration
         """
         raise NotImplementedError()
 
     @classmethod
     def get_resolvable_fields(cls) -> Dict[str, type]:
         """Returns a mapping of fields to their type hints. Dunders should not be resolved and are not returned"""
-        return {f.name:f.type for f in cls.__dataclass_fields__.values() if not f.name.startswith("__")}
+        # Sort dynamic type hint fields last because they depend on other values
+        fields = sorted(
+            (f for f in cls.__dataclass_fields__.values() if not f.name.startswith("__")),
+            key=lambda f: f.name in cls.__hint_resolvers__
+        )
+        return {f.name: f.type for f in fields}
 
     def is_resolved(self) -> bool:
         return self.__is_resolved__
 
     def is_partial(self) -> bool:
         """Returns True when any required resolvable field has its value missing."""
         if self.__is_resolved__:
@@ -305,7 +318,20 @@
 
     def add_extras(self) -> None:
         """Called right after context was added to the container. Benefits mostly the config provider injection context which adds extra providers using the initial ones."""
         pass
 
 
 _F_ContainerInjectableContext = ContainerInjectableContext
+
+
+TSpec = TypeVar("TSpec", bound=BaseConfiguration)
+THintResolver = Callable[[TSpec], Type[Any]]
+
+def resolve_type(field_name: str) -> Callable[[THintResolver[TSpec]], THintResolver[TSpec]]:
+    def decorator(func: THintResolver[TSpec]) -> THintResolver[TSpec]:
+        func.__hint_for_field__ = field_name  # type: ignore[attr-defined]
+        @wraps(func)
+        def wrapper(self: TSpec) -> Type[Any]:
+            return func(self)
+        return wrapper
+    return decorator
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,20 +61,24 @@
     def add_provider(self, provider: ConfigProvider) -> None:
         if provider.name in self:
             raise DuplicateConfigProviderException(provider.name)
         self.providers.append(provider)
 
     @staticmethod
     def initial_providers() -> List[ConfigProvider]:
-        providers = [
-            EnvironProvider(),
-            SecretsTomlProvider(add_global_config=True),
-            ConfigTomlProvider(add_global_config=True)
-        ]
-        return providers
+        return _initial_providers()
+
+
+def _initial_providers() -> List[ConfigProvider]:
+    providers = [
+        EnvironProvider(),
+        SecretsTomlProvider(add_global_config=True),
+        ConfigTomlProvider(add_global_config=True)
+    ]
+    return providers
 
 
 def _extra_providers() -> List[ConfigProvider]:
     from dlt.common.configuration.resolve import resolve_configuration
     providers_config = resolve_configuration(ConfigProvidersConfiguration())
     extra_providers = []
     if providers_config.enable_airflow_secrets:
@@ -101,40 +105,33 @@
 
     Depending on how DAG is defined this function may be called outside of task and
     task context will be not available. Still we want the provider to function so
     we just test if Airflow can be imported.
     """
     if not is_airflow_installed():
         return []
+    from dlt.common.configuration.providers.toml import SECRETS_TOML_KEY
 
     # hide stdio. airflow typically dumps tons of warnings and deprecations to stdout and stderr
     with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
         from airflow.models import Variable # noqa
+        from dlt.common.configuration.providers.airflow import AirflowSecretsTomlProvider
+
+        secrets_toml_var = Variable.get(SECRETS_TOML_KEY, default_var=None)
 
-        from dlt.common.configuration.providers.airflow import (
-            AirflowSecretsTomlProvider,
-            AIRFLOW_SECRETS_TOML_VARIABLE_KEY
-        )
-
-        secrets_toml_var = Variable.get(
-            AIRFLOW_SECRETS_TOML_VARIABLE_KEY,
-            default_var=None
-        )
-
-    if secrets_toml_var is not None:
-        return [AirflowSecretsTomlProvider()]
-    else:
-        message = f"Airflow variable '{AIRFLOW_SECRETS_TOML_VARIABLE_KEY}' not found. AirflowSecretsTomlProvider will not be used."
+    if secrets_toml_var is None:
+        message = f"Airflow variable '{SECRETS_TOML_KEY}' not found. AirflowSecretsTomlProvider will not be used."
         try:
             # prefer logging to task logger
             from airflow.operators.python import get_current_context  # noqa
 
             ti = get_current_context()["ti"]
             ti.log.warning(message)
         except Exception:
             # otherwise log to dlt logger
             from dlt.common import logger
             if logger.is_logging():
                 logger.warning(message)
             else:
                 print(message)
-        return []
+
+    return [AirflowSecretsTomlProvider()]
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.0/dlt/common/configuration/specs/config_section_context.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class ConfigSectionContext(ContainerInjectableContext):
 
     TMergeFunc = Callable[["ConfigSectionContext", "ConfigSectionContext"], None]
 
     pipeline_name: Optional[str]
     sections: Tuple[str, ...] = ()
     merge_style: TMergeFunc = None
+    source_state_key: str = None
 
 
     def merge(self, existing: "ConfigSectionContext") -> None:
         """Merges existing context into incoming using a merge style function"""
         merge_style_f = self.merge_style or self.prefer_incoming
         merge_style_f(self, existing)
 
@@ -30,28 +31,34 @@
             return self.sections[1]
         raise ValueError(self.sections)
 
     @staticmethod
     def prefer_incoming(incoming: "ConfigSectionContext", existing: "ConfigSectionContext") -> None:
         incoming.pipeline_name = incoming.pipeline_name or existing.pipeline_name
         incoming.sections = incoming.sections or existing.sections
+        incoming.source_state_key = incoming.source_state_key or existing.source_state_key
 
     @staticmethod
     def prefer_existing(incoming: "ConfigSectionContext", existing: "ConfigSectionContext") -> None:
         """Prefer existing section context when merging this context before injecting"""
         incoming.pipeline_name =  existing.pipeline_name or incoming.pipeline_name
         incoming.sections =  existing.sections or incoming.sections
+        incoming.source_state_key =  existing.source_state_key or incoming.source_state_key
 
     @staticmethod
     def resource_merge_style(incoming: "ConfigSectionContext", existing: "ConfigSectionContext") -> None:
         """If top level section is same and there are 3 sections it replaces second element (source module) from existing and keeps the 3rd element (name)"""
         incoming.pipeline_name = incoming.pipeline_name or existing.pipeline_name
         if len(incoming.sections) == 3 == len(existing.sections) and incoming.sections[0] == existing.sections[0]:
             incoming.sections = (incoming.sections[0], existing.sections[1], incoming.sections[2])
+            incoming.source_state_key = existing.source_state_key or incoming.source_state_key
         else:
             incoming.sections = incoming.sections or existing.sections
+            incoming.source_state_key = incoming.source_state_key or existing.source_state_key
 
+    def __str__(self) -> str:
+        return super().__str__() + f": {self.pipeline_name} {self.sections}@{self.merge_style} state['{self.source_state_key}']"
 
     if TYPE_CHECKING:
         # provide __init__ signature when type checking
-        def __init__(self, pipeline_name:str = None, sections: Tuple[str, ...] = (), merge_style: TMergeFunc = None) -> None:
+        def __init__(self, pipeline_name:str = None, sections: Tuple[str, ...] = (), merge_style: TMergeFunc = None, source_state_key: str = None) -> None:
             ...
```

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/configuration/utils.py` & `dlt-0.3.0/dlt/common/configuration/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,20 @@
     return value
 
 
 
 def log_traces(config: Optional[BaseConfiguration], key: str, hint: Type[Any], value: Any, default_value: Any, traces: Sequence[LookupTrace]) -> None:
     from dlt.common import logger
 
-    if logger.is_logging() and logger.log_level() == "DEBUG" and config:
-        logger.debug(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
+    # if logger.is_logging() and logger.log_level() == "DEBUG" and config:
+    #     logger.debug(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
         # print(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
-        for tr in traces:
-            # print(str(tr))
-            logger.debug(str(tr))
+        # for tr in traces:
+        #     # print(str(tr))
+        #     logger.debug(str(tr))
     # store all traces with resolved values
     resolved_trace = next((trace for trace in traces if trace.value is not None), None)
     if resolved_trace is not None:
         path = f'{".".join(resolved_trace.sections)}.{key}'
         _RESOLVED_TRACES[path] = ResolvedValueTrace(key, resolved_trace.value, default_value, hint, resolved_trace.sections, resolved_trace.provider, config)
```

### Comparing `dlt-0.2.9a0/dlt/common/data_types/type_helpers.py` & `dlt-0.3.0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/data_writers/buffered.py` & `dlt-0.3.0/dlt/common/data_writers/buffered.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     def _rotate_file(self) -> None:
         self._flush_and_close_file()
         self._file_name = self.file_name_template % uniq_id(5) + "." + self._file_format_spec.file_extension
 
     def _flush_items(self) -> None:
         if len(self._buffered_items) > 0:
-            # we only open a writer when there are any files in the buffer and first flush is requested
+            # we only open a writer when there are any items in the buffer and first flush is requested
             if not self._writer:
                 # create new writer and write header
                 if self._file_format_spec.is_binary_format:
                     self._file = open(self._file_name, "wb")
                 else:
                     self._file = open(self._file_name, "wt", encoding="utf-8")
                 self._writer = DataWriter.from_file_format(self.file_format, self._file, caps=self._caps)
```

### Comparing `dlt-0.2.9a0/dlt/common/data_writers/escape.py` & `dlt-0.3.0/dlt/common/data_writers/escape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import base64
 from typing import Any
 from datetime import date, datetime  # noqa: I251
 
-from dlt.common import json
+from dlt.common.json import json
 
 # use regex to escape characters in single pass
 SQL_ESCAPE_DICT = {"'": "''", "\\": "\\\\", "\n": "\\n", "\r": "\\r"}
 SQL_ESCAPE_RE = re.compile("|".join([re.escape(k) for k in sorted(SQL_ESCAPE_DICT, key=len, reverse=True)]), flags=re.DOTALL)
 
 
 def _escape_extended(v: str, prefix:str = "E'") -> str:
```

### Comparing `dlt-0.2.9a0/dlt/common/data_writers/exceptions.py` & `dlt-0.3.0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/data_writers/writers.py` & `dlt-0.3.0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/destination/capabilities.py` & `dlt-0.3.0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/destination/reference.py` & `dlt-0.3.0/dlt/common/destination/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration, CredentialsConfiguration
 from dlt.common.configuration.accessors import config
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
 from dlt.common.schema.utils import is_complete_column
 from dlt.common.storages import FileStorage
 from dlt.common.storages.load_storage import ParsedLoadJobFileName
+from dlt.common.utils import get_module_name
 
 
 @configspec(init=True)
 class DestinationClientConfiguration(BaseConfiguration):
     destination_name: str = None  # which destination to load data to
     credentials: Optional[CredentialsConfiguration]
 
+    def __str__(self) -> str:
+        """Return displayable destination location"""
+        return str(self.credentials)
+
     if TYPE_CHECKING:
         def __init__(self, destination_name: str = None, credentials: Optional[CredentialsConfiguration] = None) -> None:
             ...
 
 
 @configspec(init=True)
 class DestinationClientDwhConfiguration(DestinationClientConfiguration):
@@ -136,15 +141,15 @@
         Returns:
             Optional[TSchemaTables]: Returns an update that was applied at the destination.
         """
         self._verify_schema()
         return expected_update
 
     @abstractmethod
-    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
+    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         """Creates a job for a particular `table` with content in `file_path`"""
         pass
 
     @abstractmethod
     def restore_file_load(self, file_path: str) -> LoadJob:
         pass
 
@@ -245,7 +250,13 @@
         try:
             c = destination_ref.spec()
             c.credentials
         except Exception:
             raise InvalidDestinationReference(destination)
 
         return destination_ref
+
+    @staticmethod
+    def to_name(destination: TDestinationReferenceArg) -> str:
+        if isinstance(destination, ModuleType):
+            return get_module_name(destination)
+        return destination.split(".")[-1]  # type: ignore
```

### Comparing `dlt-0.2.9a0/dlt/common/exceptions.py` & `dlt-0.3.0/dlt/common/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,27 +140,27 @@
     def __init__(self, pipeline_name: str, msg: str) -> None:
         """Base class for all pipeline exceptions. Should not be raised."""
         self.pipeline_name = pipeline_name
         super().__init__(msg)
 
 
 class PipelineStateNotAvailable(PipelineException):
-    def __init__(self, source_name: Optional[str] = None) -> None:
-        if source_name:
-            msg = f"The source {source_name} requested the access to pipeline state but no pipeline is active right now."
+    def __init__(self, source_state_key: Optional[str] = None) -> None:
+        if source_state_key:
+            msg = f"The source {source_state_key} requested the access to pipeline state but no pipeline is active right now."
         else:
             msg = "The resource you called requested the access to pipeline state but no pipeline is active right now."
         msg += " Call dlt.pipeline(...) before you call the @dlt.source or  @dlt.resource decorated function."
-        self.source_name = source_name
+        self.source_state_key = source_state_key
         super().__init__(None, msg)
 
 
 class ResourceNameNotAvailable(PipelineException):
     def __init__(self) -> None:
         super().__init__(None,
-            "A resource state was requested but no resource marked callable was found in the call stack. Resource state may be only requested from @dlt.resource decorated function or with explicit resource name.")
+            "A resource state was requested but no active extract pipe context was found. Resource state may be only requested from @dlt.resource decorated function or with explicit resource name.")
 
 
 class SourceSectionNotAvailable(PipelineException):
     def __init__(self) -> None:
         msg = "Access to state was requested without source section active. State should be requested from within the @dlt.source and @dlt.resource decorated function."
         super().__init__(None, msg)
```

### Comparing `dlt-0.2.9a0/dlt/common/git.py` & `dlt-0.3.0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/json/__init__.py` & `dlt-0.3.0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/json/_orjson.py` & `dlt-0.3.0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/json/_simplejson.py` & `dlt-0.3.0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/jsonpath.py` & `dlt-0.3.0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/configuration.py` & `dlt-0.3.0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/json/relational.py` & `dlt-0.3.0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/normalizers/utils.py` & `dlt-0.3.0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/pipeline.py` & `dlt-0.3.0/dlt/common/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs import ContainerInjectableContext
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.paths import get_dlt_data_dir
 from dlt.common.configuration.specs import RunConfiguration
-from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
+from dlt.common.destination import DestinationReference, TDestinationReferenceArg
 from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, ResourceNameNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TWriteDisposition
 from dlt.common.source import get_current_pipe_name
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.typing import DictStrAny, REPattern
 from dlt.common.jsonpath import delete_matches, TAnyJsonPath
@@ -139,14 +139,16 @@
     sources: Dict[str, Dict[str, Any]]
 
 
 class SupportsPipeline(Protocol):
     """A protocol with core pipeline operations that lets high level abstractions ie. sources to access pipeline methods and properties"""
     pipeline_name: str
     """Name of the pipeline"""
+    default_schema_name: str
+    """Name of the default schema"""
     destination: DestinationReference
     """The destination reference which is ModuleType. `destination.__name__` returns the name string"""
     dataset_name: str
     """Name of the dataset to which pipeline will be loaded to"""
     runtime_config: RunConfiguration
     """A configuration of runtime options like logging level and format and various tracing options"""
     working_dir: str
@@ -179,15 +181,17 @@
         primary_key: TColumnKey = None,
         schema: Schema = None
     ) -> LoadInfo:
         ...
 
     def _set_context(self, is_active: bool) -> None:
         """Called when pipeline context activated or deactivate"""
-        ...
+
+    def _make_schema_with_default_name(self) -> Schema:
+        """Make a schema from the pipeline name using the name normalizer. "_pipeline" suffix is removed if present"""
 
 
 class SupportsPipelineRun(Protocol):
     def __call__(
         self,
         *,
         destination: TDestinationReferenceArg = None,
@@ -212,14 +216,17 @@
         """Creates or returns exiting pipeline"""
         if not self._pipeline:
             # delayed pipeline creation
             self.activate(self._deferred_pipeline())
         return self._pipeline
 
     def activate(self, pipeline: SupportsPipeline) -> None:
+        # do not activate currently active pipeline
+        if pipeline == self._pipeline:
+            return
         self.deactivate()
         pipeline._set_context(True)
         self._pipeline = pipeline
 
     def is_active(self) -> bool:
         return self._pipeline is not None
 
@@ -262,27 +269,17 @@
             return initial_default, False
         else:
             # get unmanaged state that is read only
             # TODO: make sure that state if up to date by syncing the pipeline earlier
             return proxy.pipeline().state, False
 
 
-def sources_state(pipeline_state_: Optional[TPipelineState] = None, /) -> DictStrAny:
+def _sources_state(pipeline_state_: Optional[TPipelineState] = None, /) -> DictStrAny:
     global _last_full_state
 
-    # # get the source name from the section context
-    # source_section: str = None
-    # with contextlib.suppress(ContextDefaultCannotBeCreated):
-    #     sections_context = container[ConfigSectionContext]
-    #     with contextlib.suppress(ValueError):
-    #         source_section = sections_context.source_section()
-
-    # if not source_section:
-    #     raise SourceSectionNotAvailable()
-
     if pipeline_state_ is None:
         state, _ = pipeline_state(Container())
     else:
         state = pipeline_state_
     if state is None:
         raise PipelineStateNotAvailable()
 
@@ -297,41 +294,40 @@
     """Returns a dictionary with the source-scoped state. Source-scoped state may be shared across the resources of a particular source. Please avoid using source scoped state. Check
     the `resource_state` function for resource-scoped state that is visible within particular resource. Dlt state is preserved across pipeline runs and may be used to implement incremental loads.
 
     ### Summary
     The source state is a python dictionary-like object that is available within the `@dlt.source` and `@dlt.resource` decorated functions and may be read and written to.
     The data within the state is loaded into destination together with any other extracted data and made automatically available to the source/resource extractor functions when they are run next time.
     When using the state:
-    * The source state is scoped to a section of the source. The source section is set by default to the module name in which source function is defined.
-    * If the `section` argument when decorating source function is not specified, all sources in the module will share the state
+    * The source state is scoped to a particular source and will be stored under the source name in the pipeline state
+    * It is possible to share state across many sources if they share a schema with the same name
     * Any JSON-serializable values can be written and the read from the state. `dlt` dumps and restores instances of Python bytes, DateTime, Date and Decimal types.
     * The state available in the source decorated function is read only and any changes will be discarded.
     * The state available in the resource decorated function is writable and written values will be available on the next pipeline run
     """
     global _last_full_state
 
     container = Container()
 
     # get the source name from the section context
-    source_section: str = None
+    source_state_key: str = None
     with contextlib.suppress(ContextDefaultCannotBeCreated):
         sections_context = container[ConfigSectionContext]
-        with contextlib.suppress(ValueError):
-            source_section = sections_context.source_section()
+        source_state_key = sections_context.source_state_key
 
-    if not source_section:
+    if not source_state_key:
         raise SourceSectionNotAvailable()
 
     try:
-        state = sources_state()
+        state = _sources_state()
     except PipelineStateNotAvailable as e:
         # Reraise with source section
-        raise PipelineStateNotAvailable(source_section) from e
+        raise PipelineStateNotAvailable(source_state_key) from e
 
-    return state.setdefault(source_section, {})  # type: ignore[no-any-return]
+    return state.setdefault(source_state_key, {})  # type: ignore[no-any-return]
 
 
 _last_full_state: TPipelineState = None
 
 
 def _delete_source_state_keys(key: TAnyJsonPath, source_state_: Optional[DictStrAny] = None, /) -> None:
     """Remove one or more key from the source state.
```

### Comparing `dlt-0.2.9a0/dlt/common/reflection/spec.py` & `dlt-0.3.0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/reflection/utils.py` & `dlt-0.3.0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runners/configuration.py` & `dlt-0.3.0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runners/pool_runner.py` & `dlt-0.3.0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runners/runnable.py` & `dlt-0.3.0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runners/stdout.py` & `dlt-0.3.0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runners/synth_pickle.py` & `dlt-0.3.0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runners/venv.py` & `dlt-0.3.0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/collector.py` & `dlt-0.3.0/dlt/common/runtime/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import sys
 import logging
 import time
-import psutil
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Any, ContextManager, Dict, Type, TYPE_CHECKING, DefaultDict, NamedTuple, Optional, Union, TextIO, TypeVar
 if TYPE_CHECKING:
     from tqdm import tqdm
     import enlighten
     from enlighten import Counter as EnlCounter, StatusBar as EnlStatusBar, Manager as EnlManager
@@ -116,14 +115,20 @@
         """
         self.log_period = log_period
         self.logger = logger
         self.log_level = log_level
         self.counters: DefaultDict[str, int] = None
         self.counter_info: Dict[str, LogCollector.CounterInfo] = None
         self.messages: Dict[str, Optional[str]] = None
+        if dump_system_stats:
+            try:
+                import psutil
+            except ImportError:
+                self._log(logging.WARNING, "psutil dependency is not installed and mem stats will not be available. add psutil to your environment or pass dump_system_stats argument as False to disable warning.")
+                dump_system_stats = False
         self.dump_system_stats = dump_system_stats
         self.last_log_time: float = None
 
     def update(self, name: str, inc: int = 1, total: int = None, message: str = None, label: str = None) -> None:
         counter_key = f"{name}_{label}" if label else name
 
         if counter_key not in self.counters:
@@ -164,28 +169,33 @@
             items_per_second_str = f"{items_per_second:.2f}/s"
             message = f"[{self.messages[name]}]" if self.messages[name] is not None else ""
 
             counter_line = f"{info.description}: {progress} {percentage} | Time: {elapsed_time_str} | Rate: {items_per_second_str} {message}"
             log_lines.append(counter_line.strip())
 
         if self.dump_system_stats:
+            import psutil
+
             process = psutil.Process(os.getpid())
             mem_info = process.memory_info()
             current_mem = mem_info.rss / (1024 ** 2)  # Convert to MB
             mem_percent = psutil.virtual_memory().percent
             cpu_percent = process.cpu_percent()
-
             log_lines.append(f"Memory usage: {current_mem:.2f} MB ({mem_percent:.2f}%) | CPU usage: {cpu_percent:.2f}%")
+
         log_lines.append("")
         log_message = "\n".join(log_lines)
         if not self.logger:
             # try to attach dlt logger
             self.logger = dlt_logger.LOGGER
+        self._log(self.log_level, log_message)
+
+    def _log(self, log_level: int, log_message: str) -> None:
         if isinstance(self.logger, logging.Logger):
-            self.logger.log(self.log_level, log_message)
+            self.logger.log(log_level, log_message)
         else:
             print(log_message, file=self.logger or sys.stdout)
 
     def _start(self, step: str) -> None:
         self.counters = defaultdict(int)
         self.counter_info = {}
         self.messages = {}
```

### Comparing `dlt-0.2.9a0/dlt/common/runtime/exec_info.py` & `dlt-0.3.0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/init.py` & `dlt-0.3.0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/logger.py` & `dlt-0.3.0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/prometheus.py` & `dlt-0.3.0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/segment.py` & `dlt-0.3.0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/sentry.py` & `dlt-0.3.0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/signals.py` & `dlt-0.3.0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/slack.py` & `dlt-0.3.0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/runtime/telemetry.py` & `dlt-0.3.0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/schema/detections.py` & `dlt-0.3.0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/schema/exceptions.py` & `dlt-0.3.0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/schema/schema.py` & `dlt-0.3.0/dlt/common/schema/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
     def to_pretty_json(self, remove_defaults: bool = True) -> str:
         d = self.to_dict(remove_defaults=remove_defaults)
         return json.dumps(d, pretty=True)
 
     def to_pretty_yaml(self, remove_defaults: bool = True) -> str:
         d = self.to_dict(remove_defaults=remove_defaults)
-        return cast(str, yaml.dump(d, allow_unicode=True, default_flow_style=False, sort_keys=False))
+        return yaml.dump(d, allow_unicode=True, default_flow_style=False, sort_keys=False)
 
     def clone(self) -> "Schema":
         d = deepcopy(self.to_dict())
         return Schema.from_dict(d)  # type: ignore
 
     def _infer_column(self, k: str, v: Any, data_type: TDataType = None, is_variant: bool = False) -> TColumnSchema:
         column_schema =  TColumnSchema(
```

### Comparing `dlt-0.2.9a0/dlt/common/schema/typing.py` & `dlt-0.3.0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/schema/utils.py` & `dlt-0.3.0/dlt/common/schema/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import base64
 import hashlib
 
 from copy import deepcopy
-from typing import Dict, List, Sequence, Tuple, Type, Any, cast, Union, Iterable, Optional
+from typing import Dict, List, Sequence, Tuple, Type, Any, cast, Iterable, Optional
 
 from dlt.common import json
 from dlt.common.data_types import TDataType
 from dlt.common.exceptions import DictValidationException
 from dlt.common.normalizers import default_normalizers
 from dlt.common.normalizers.naming import NamingConvention
 from dlt.common.typing import DictStrAny, REPattern
```

### Comparing `dlt-0.2.9a0/dlt/common/source.py` & `dlt-0.3.0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/__init__.py` & `dlt-0.3.0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/configuration.py` & `dlt-0.3.0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/data_item_storage.py` & `dlt-0.3.0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/exceptions.py` & `dlt-0.3.0/dlt/common/storages/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,7 +57,12 @@
 
 class SchemaNotFoundError(SchemaStorageException, FileNotFoundError, KeyError):
     def __init__(self, schema_name: str, storage_path: str, import_path: str = None, import_format: str = None) -> None:
         msg = f"Schema {schema_name} in {storage_path} could not be found."
         if import_path:
             msg += f"Import from {import_path} and format {import_format} failed."
         super().__init__(msg)
+
+
+class UnexpectedSchemaName(SchemaStorageException, ValueError):
+    def __init__(self, schema_name: str, storage_path: str, stored_name: str) -> None:
+        super().__init__(f"A schema file name '{schema_name}' in {storage_path} does not correspond to the name of schema in the file {stored_name}")
```

### Comparing `dlt-0.2.9a0/dlt/common/storages/file_storage.py` & `dlt-0.3.0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/load_storage.py` & `dlt-0.3.0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/normalize_storage.py` & `dlt-0.3.0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/storages/schema_storage.py` & `dlt-0.3.0/dlt/common/storages/schema_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dlt.common.configuration import with_config
 from dlt.common.configuration.accessors import config
 from dlt.common.storages.configuration import SchemaStorageConfiguration, TSchemaFileFormat, SchemaFileExtensions
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.schema import Schema, verify_schema_hash
 from dlt.common.typing import DictStrAny
 
-from dlt.common.storages.exceptions import InStorageSchemaModified, SchemaNotFoundError
+from dlt.common.storages.exceptions import InStorageSchemaModified, SchemaNotFoundError, UnexpectedSchemaName
 
 
 class SchemaStorage(Mapping[str, Schema]):
 
     SCHEMA_FILE_NAME = "schema.%s"
     NAMED_SCHEMA_FILE_PATTERN = f"%s.{SCHEMA_FILE_NAME}"
 
@@ -147,15 +147,18 @@
     @staticmethod
     def load_schema_file(path: str, name: str, extensions: Tuple[TSchemaFileFormat, ...]=SchemaFileExtensions) -> Schema:
         storage = FileStorage(path)
         for extension in extensions:
             file = SchemaStorage._file_name_in_store(name, extension)
             if storage.has_file(file):
                 parsed_schema = SchemaStorage._parse_schema_str(storage.load(file), extension)
-                return Schema.from_dict(parsed_schema)
+                schema = Schema.from_dict(parsed_schema)
+                if schema.name != name:
+                    raise UnexpectedSchemaName(name, path, schema.name)
+                return schema
         raise SchemaNotFoundError(name, path)
 
     @staticmethod
     def _parse_schema_str(schema_str: str, extension: TSchemaFileFormat) -> DictStrAny:
         if extension == "json":
             imported_schema: DictStrAny = json.loads(schema_str)
         elif extension == "yaml":
```

### Comparing `dlt-0.2.9a0/dlt/common/storages/versioned_storage.py` & `dlt-0.3.0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/time.py` & `dlt-0.3.0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/typing.py` & `dlt-0.3.0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/utils.py` & `dlt-0.3.0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/validation.py` & `dlt-0.3.0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/common/wei.py` & `dlt-0.3.0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.0/dlt/destinations/bigquery/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,16 @@
                     raise LoadJobNotExistsException(file_path)
                 elif reason in BQ_TERMINAL_REASONS:
                     raise LoadJobTerminalException(file_path)
                 else:
                     raise DestinationTransientException(gace)
         return job
 
-    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
-        job = super().start_file_load(table, file_path)
+    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+        job = super().start_file_load(table, file_path, load_id)
         if not job:
             try:
                 job = BigQueryLoadJob(
                     FileStorage.get_file_name_from_file_path(file_path),
                     self._create_load_job(table["name"], table["write_disposition"], file_path),
                     self.config.credentials
                 )
```

### Comparing `dlt-0.2.9a0/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.0/dlt/destinations/duckdb/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,18 +83,23 @@
         # do not set any paths for external database
         if self.database == ":external:":
             return
         # try the pipeline context
         is_default_path = False
         if self.database == ":pipeline:":
             self.database = self._path_in_pipeline(DEFAULT_DUCK_DB_NAME)
-        # if pipeline context was not present or database was not set
-        if not self.database:
-            # create database locally
-            self.database, is_default_path = self._path_from_pipeline(DEFAULT_DUCK_DB_NAME)
+        else:
+            # maybe get database
+            maybe_database, maybe_is_default_path = self._path_from_pipeline(DEFAULT_DUCK_DB_NAME)
+            # if pipeline context was not present or database was not set
+            if not self.database or not maybe_is_default_path:
+                # create database locally
+                is_default_path = maybe_is_default_path
+                self.database = maybe_database
+
         # always make database an abs path
         self.database = os.path.abspath(self.database)
         # do not save the default path into pipeline's local state
         if not is_default_path:
             self._path_to_pipeline(self.database)
 
     def _path_in_pipeline(self, rel_path: str) -> str:
```

### Comparing `dlt-0.2.9a0/dlt/destinations/duckdb/duck.py` & `dlt-0.3.0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/dummy/__init__.py` & `dlt-0.3.0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/dummy/configuration.py` & `dlt-0.3.0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/dummy/dummy.py` & `dlt-0.3.0/dlt/destinations/dummy/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def update_storage_schema(self, staging: bool = False, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
         applied_update = super().update_storage_schema(staging, only_tables, expected_update)
         if self.config.fail_schema_update:
             raise DestinationTransientException("Raise on schema update due to fail_schema_update config flag")
         return applied_update
 
-    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
+    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job_id = FileStorage.get_file_name_from_file_path(file_path)
         file_name = FileStorage.get_file_name_from_file_path(file_path)
         # return existing job if already there
         if job_id not in JOBS:
             JOBS[job_id] = self._create_job(file_name)
         else:
             job = JOBS[job_id]
```

### Comparing `dlt-0.2.9a0/dlt/destinations/exceptions.py` & `dlt-0.3.0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/insert_job_client.py` & `dlt-0.3.0/dlt/destinations/insert_job_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             if write_disposition == "replace":
                 insert_sql.append("DELETE FROM {};".format(qualified_table_name))
             while content := f.read(self._sql_client.capabilities.max_query_length // 2):
                 # write INSERT
                 insert_sql.extend([header.format(qualified_table_name), values_mark, content])
                 # read one more line in order to
                 # 1. complete the content which ends at "random" position, not an end line
-                # 2. to modify it's ending without a need to re-allocating the 8MB of "content"
+                # 2. to modify its ending without a need to re-allocating the 8MB of "content"
                 until_nl = f.readline()
                 # if until next line contains just '\n' try to take another line so we can finish content properly
                 # TODO: write test for this case (content ends with ",")
                 if until_nl == "\n":
                     until_nl = f.readline()
                 until_nl = until_nl.strip("\n")
                 # if there was anything left, until_nl contains the last line
@@ -83,16 +83,16 @@
             LoadJob: Always a restored job completed
         """
         job = super().restore_file_load(file_path)
         if not job:
             job = EmptyLoadJob.from_file_path(file_path, "completed")
         return job
 
-    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
-        job = super().start_file_load(table, file_path)
+    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+        job = super().start_file_load(table, file_path, load_id)
         if not job:
             # this is using sql_client internally and will raise a right exception
             job = InsertValuesLoadJob(table["name"], table["write_disposition"], file_path, self.sql_client)
         return job
 
     # TODO: implement indexes and primary keys for postgres
     def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
```

### Comparing `dlt-0.2.9a0/dlt/destinations/job_client_impl.py` & `dlt-0.3.0/dlt/destinations/job_client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 yield
         else:
             yield
 
     def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return SqlMergeJob.from_table_chain(table_chain, self.sql_client)
 
-    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
+    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         """Starts SqlLoadJob for files ending with .sql or returns None to let derived classes to handle their specific jobs"""
         if SqlLoadJob.is_sql_job(file_path):
             # execute sql load job
             return SqlLoadJob(file_path, self.sql_client)
         return None
 
     def restore_file_load(self, file_path: str) -> LoadJob:
```

### Comparing `dlt-0.2.9a0/dlt/destinations/job_impl.py` & `dlt-0.3.0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/postgres/__init__.py` & `dlt-0.3.0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/postgres/configuration.py` & `dlt-0.3.0/dlt/destinations/postgres/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import Final, ClassVar, Any, List
 from sqlalchemy.engine import URL
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ConnectionStringCredentials
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
+from dlt.common.typing import TSecretValue
 
 
 @configspec
 class PostgresCredentials(ConnectionStringCredentials):
     drivername: Final[str] = "postgresql"  # type: ignore
+    password: TSecretValue
+    host: str
     port: int = 5432
     connect_timeout: int = 15
 
     __config_gen_annotations__: ClassVar[List[str]] = ["port", "connect_timeout"]
 
     def parse_native_representation(self, native_value: Any) -> None:
         super().parse_native_representation(native_value)
```

### Comparing `dlt-0.2.9a0/dlt/destinations/postgres/postgres.py` & `dlt-0.3.0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/redshift/README.md` & `dlt-0.3.0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/redshift/__init__.py` & `dlt-0.3.0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/redshift/configuration.py` & `dlt-0.3.0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/redshift/redshift.py` & `dlt-0.3.0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/destinations/sql_client.py` & `dlt-0.3.0/dlt/destinations/sql_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self.fetchmany = curr.fetchmany  # type: ignore
         self.fetchone = curr.fetchone  # type: ignore
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self.native_cursor, name)
 
     def df(self, chunk_size: int = None, **kwargs: Any) -> Optional[DataFrame]:
-        from dlt.helpers.pandas import _wrap_result
+        from dlt.helpers.pandas_helper import _wrap_result
 
         columns = [c[0] for c in self.native_cursor.description]
         if chunk_size is None:
             return _wrap_result(self.native_cursor.fetchall(), columns, **kwargs)
         else:
             df = _wrap_result(self.native_cursor.fetchmany(chunk_size), columns, **kwargs)
             # if no rows return None
```

### Comparing `dlt-0.2.9a0/dlt/destinations/sql_merge_job.py` & `dlt-0.3.0/dlt/destinations/sql_merge_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         try:
             sql = cls.gen_merge_sql(table_chain, sql_client)
             job = cls(file_info.job_id(), "running")
             job._save_text_file("\n".join(sql))
         except Exception:
             # return failed job
             failed_text = "Tried to generate a merge sql job for the following tables:"
-            tables_str = cast(str, yaml.dump(table_chain, allow_unicode=True, default_flow_style=False, sort_keys=False))
+            tables_str = yaml.dump(table_chain, allow_unicode=True, default_flow_style=False, sort_keys=False)
             job = cls(file_info.job_id(), "failed", pretty_format_exception())
             job._save_text_file("\n".join([failed_text, tables_str]))
         return job
 
     @classmethod
     def _gen_key_table_clauses(cls, primary_keys: Sequence[str], merge_keys: Sequence[str])-> List[str]:
         """Generate sql clauses to select rows to delete via merge and primary key. Return select all clause if no keys defined."""
```

### Comparing `dlt-0.2.9a0/dlt/destinations/typing.py` & `dlt-0.3.0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/extract/decorators.py` & `dlt-0.3.0/dlt/extract/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dlt.common.source import _SOURCES, SourceInfo
 from dlt.common.schema.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TTableSchemaColumns, TWriteDisposition
 from dlt.common.storages.exceptions import SchemaNotFoundError
 from dlt.common.storages.schema_storage import SchemaStorage
 from dlt.common.typing import AnyFun, ParamSpec, Concatenate, TDataItem, TDataItems
 from dlt.common.utils import get_callable_name, get_module_name, is_inner_callable
-from dlt.extract.exceptions import InvalidTransformerDataTypeGeneratorFunctionRequired, ResourceFunctionExpected, ResourceInnerCallableConfigWrapDisallowed, SourceDataIsNone, SourceIsAClassTypeError, SourceNotAFunction, SourceSchemaNotAvailable
+from dlt.extract.exceptions import InvalidTransformerDataTypeGeneratorFunctionRequired, ResourceFunctionExpected, ResourceInnerCallableConfigWrapDisallowed, SourceDataIsNone, SourceIsAClassTypeError, ExplicitSourceNameInvalid, SourceNotAFunction, SourceSchemaNotAvailable
 from dlt.extract.incremental import IncrementalResourceWrapper
 
 from dlt.extract.typing import TTableHintTemplate
 from dlt.extract.source import DltResource, DltSource, TUnboundDltResource
 
 
 
@@ -98,15 +98,15 @@
     See https://dlthub.com/docs/general-usage/credentials for details.
 
     ### Args:
         func: A function that returns a dlt resource or a list of those or a list of any data items that can be loaded by `dlt`.
 
         name (str, optional): A name of the source which is also the name of the associated schema. If not present, the function name will be used.
 
-        section (str, optional): A name of configuration and state sections. If not present, the current python module name will be used.
+        section (str, optional): A name of configuration. If not present, the current python module name will be used.
 
         max_table_nesting (int, optional): A schema hint that sets the maximum depth of nested table above which the remaining nodes are loaded as structs or JSON.
 
         root_key (bool): Enables merging on all resources by propagating root foreign key to child tables. This option is most useful if you plan to change write disposition of a resource to disable/enable merge. Defaults to False.
 
         schema (Schema, optional): An explicit `Schema` instance to be associated with the source. If not present, `dlt` creates a new `Schema` object with provided `name`. If such `Schema` already exists in the same folder as the module containing the decorated function, such schema will be loaded from file.
 
@@ -124,43 +124,46 @@
 
         if not callable(f) or isinstance(f, DltResource):
             raise SourceNotAFunction(name or "<no name>", f, type(f))
 
         if inspect.isclass(f):
             raise SourceIsAClassTypeError(name or "<no name>", f)
 
-        # source name is passed directly or taken from decorated function name
-        name = name or get_callable_name(f)
-
         if not schema:
+            # source name is passed directly or taken from decorated function name
+            effective_name = name or get_callable_name(f)
             # load the schema from file with name_schema.yaml/json from the same directory, the callable resides OR create new default schema
-            schema = _maybe_load_schema_for_callable(f, name) or Schema(name, normalize_name=True)
+            schema = _maybe_load_schema_for_callable(f, effective_name) or Schema(effective_name, normalize_name=True)
+
+        if name and name != schema.name:
+            raise ExplicitSourceNameInvalid(name, schema.name)
+
+        # the name of the source must be identical to the name of the schema
+        name = schema.name
 
         # wrap source extraction function in configuration with section
         func_module = inspect.getmodule(f)
         source_section = section or _get_source_section_name(func_module)
         source_sections = (known_sections.SOURCES, source_section, name)
         conf_f = with_config(f, spec=spec, sections=source_sections)
 
         @wraps(conf_f)
         def _wrap(*args: Any, **kwargs: Any) -> DltSource:
             # make schema available to the source
             with Container().injectable_context(SourceSchemaInjectableContext(schema)):
                 # configurations will be accessed in this section in the source
                 proxy = Container()[PipelineContext]
                 pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
-                with inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=source_sections)):
+                with inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=source_sections, source_state_key=name)):
                     rv = conf_f(*args, **kwargs)
-
-            if rv is None:
-                raise SourceDataIsNone(name)
-
-            # if generator, consume it immediately
-            if inspect.isgenerator(rv):
-                rv = list(rv)
+                    if rv is None:
+                        raise SourceDataIsNone(name)
+                    # if generator, consume it immediately
+                    if inspect.isgenerator(rv):
+                        rv = list(rv)
 
             # convert to source
             s = DltSource.from_data(name, source_section, schema.clone(), rv)
             # apply hints
             if max_table_nesting is not None:
                 s.max_table_nesting = max_table_nesting
             # enable root propagation
@@ -484,14 +487,15 @@
 def _maybe_load_schema_for_callable(f: AnyFun, name: str) -> Optional[Schema]:
     if not inspect.isfunction(f):
         f = f.__class__
     try:
         file = inspect.getsourcefile(f)
         if file:
             return SchemaStorage.load_schema_file(os.path.dirname(file), name)
+
     except SchemaNotFoundError:
         pass
     return None
 
 
 def _get_source_section_name(m: ModuleType) -> str:
     if m is None:
```

### Comparing `dlt-0.2.9a0/dlt/extract/exceptions.py` & `dlt-0.3.0/dlt/extract/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,10 +231,17 @@
 
 
 class SourceSchemaNotAvailable(DltSourceException):
     def __init__(self) -> None:
         super().__init__("Current source schema is available only when called from a function decorated with dlt.source or dlt.resource")
 
 
+class ExplicitSourceNameInvalid(DltSourceException):
+    def __init__(self, source_name: str, schema_name: str) -> None:
+        self.source_name = source_name
+        self.schema_name = schema_name
+        super().__init__(f"Your explicit source name {source_name} is not a valid schema name. Please use a valid schema name ie. '{schema_name}'.")
+
+
 class IncrementalUnboundError(DltResourceException):
     def __init__(self, cursor_path: str) -> None:
         super().__init__("", f"The incremental definition with cursor path {cursor_path} is used without being bound to the resource. This most often happens when you create dynamic resource from a generator function that uses incremental. See https://dlthub.com/docs/general-usage/incremental-loading#incremental-loading-with-last-value for an example.")
```

### Comparing `dlt-0.2.9a0/dlt/extract/extract.py` & `dlt-0.3.0/dlt/extract/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     max_parallel_items: int,
     workers: int
 ) -> str:
     # generate extract_id to be able to commit all the sources together later
     extract_id = storage.create_extract_id()
     with Container().injectable_context(SourceSchemaInjectableContext(schema)):
         # inject the config section with the current source name
-        with inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, source.section, source.name))):
+        with inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, source.section, source.name), source_state_key=source.name)):
             # reset resource states
             for resource in source.resources.extracted.values():
                 with contextlib.suppress(DataItemRequiredForDynamicTableHints):
                     if resource.write_disposition == "replace":
                         _reset_resource_state(resource._name)
 
             extractor = extract(extract_id, source, storage, collector, max_parallel_items=max_parallel_items, workers=workers)
```

### Comparing `dlt-0.2.9a0/dlt/extract/incremental.py` & `dlt-0.3.0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/extract/pipe.py` & `dlt-0.3.0/dlt/extract/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     @configspec
     class PipeIteratorConfiguration(BaseConfiguration):
         max_parallel_items: int = 20
         workers: int = 5
         futures_poll_interval: float = 0.01
         copy_on_fork: bool = False
 
-        __sections__ = "extract"
+        __section__ = "extract"
 
     def __init__(self, max_parallel_items: int, workers: int, futures_poll_interval: float) -> None:
         self.max_parallel_items = max_parallel_items
         self.workers = workers
         self.futures_poll_interval = futures_poll_interval
 
         self._async_pool: asyncio.AbstractEventLoop = None
@@ -462,14 +462,15 @@
         yield_parents: bool = True,
         *,
         max_parallel_items: int = 20,
         workers: int = 5,
         futures_poll_interval: float = 0.01,
         copy_on_fork: bool = False
     ) -> "PipeIterator":
+        # print(f"max_parallel_items: {max_parallel_items} workers: {workers}")
         extract = cls(max_parallel_items, workers, futures_poll_interval)
         # clone all pipes before iterating (recursively) as we will fork them (this add steps) and evaluate gens
         pipes = PipeIterator.clone_pipes(pipes)
 
         def _fork_pipeline(pipe: Pipe) -> None:
             if pipe.parent:
                 # fork the parent pipe
```

### Comparing `dlt-0.2.9a0/dlt/extract/schema.py` & `dlt-0.3.0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/extract/source.py` & `dlt-0.3.0/dlt/extract/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 import contextlib
 from copy import copy
 import makefun
 import inspect
 from typing import AsyncIterable, AsyncIterator, ClassVar, Callable, ContextManager, Dict, Iterable, Iterator, List, Sequence, Tuple, Union, Any
 
 from dlt.common.configuration.resolve import inject_section
@@ -29,14 +30,16 @@
     """Marks `item` to be dispatched to table `table_name` when yielded from resource function."""
     return DataItemWithMeta(TableNameMeta(table_name), item)
 
 
 class DltResource(Iterable[TDataItem], DltResourceSchema):
 
     Empty: ClassVar["DltResource"] = None
+    source_name: str
+    """Name of the source that contains this instance of the source, set when added to DltResourcesDict"""
 
     def __init__(
         self,
         pipe: Pipe,
         table_schema_template: TTableSchemaTemplate,
         selected: bool,
         incremental: IncrementalResourceWrapper = None,
@@ -45,14 +48,15 @@
         self._name = pipe.name
         self.section = section
         self.selected = selected
         self._pipe = pipe
         self._bound = False
         if incremental and not self.incremental:
             self.add_step(incremental)
+        self.source_name = None
         super().__init__(self._name, table_schema_template)
 
     @classmethod
     def from_data(
         cls,
         data: Any,
         name: str = None,
@@ -270,43 +274,51 @@
 
     def bind(self, *args: Any, **kwargs: Any) -> "DltResource":
         """Binds the parametrized resource to passed arguments. Modifies resource pipe in place. Does not evaluate generators or iterators."""
         if self._bound:
             raise TypeError("Bound DltResource object is not callable")
         gen = self._pipe.bind_gen(*args, **kwargs)
         if isinstance(gen, DltResource):
-            # replace resource in place
+            # the resource returned resource: update in place
             old_pipe = self._pipe
             self.__dict__.clear()
             self.__dict__.update(gen.__dict__)
             # keep old pipe instance
             self._pipe = old_pipe
             self._pipe.__dict__.clear()
             # write props from new pipe instance
             self._pipe.__dict__.update(gen._pipe.__dict__)
         elif isinstance(gen, Pipe):
-            # just replace pipe
+            # the resource returned pipe: just replace pipe
             self._pipe.__dict__.clear()
             # write props from new pipe instance
             self._pipe.__dict__.update(gen.__dict__)
         else:
             self._bound = True
         return self
 
     @property
     def state(self) -> StrAny:
-        """Gets resource-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
+        """Gets resource-scoped state from the active pipeline. PipelineStateNotAvailable is raised if pipeline context is not available"""
         with self._get_config_section_context():
             return resource_state(self.name)
 
+    def clone(self, clone_pipe: bool = True, keep_pipe_id: bool = True) -> "DltResource":
+        """Creates a deep copy of a current resource, optionally cloning also pipe. Note that name of a containing source will not be cloned."""
+        pipe = self._pipe
+        if self._pipe and not self._pipe.is_empty and clone_pipe:
+            pipe = pipe._clone(keep_pipe_id=keep_pipe_id)
+        # incremental and parent are already in the pipe (if any)
+        return DltResource(pipe, self._table_schema_template, selected=self.selected, section=self.section)
+
     def __call__(self, *args: Any, **kwargs: Any) -> "DltResource":
         """Binds the parametrized resources to passed arguments. Creates and returns a bound resource. Generators and iterators are not evaluated."""
         if self._bound:
             raise TypeError("Bound DltResource object is not callable")
-        r = DltResource.from_data(self._pipe._clone(keep_pipe_id=False), self._name, self.section, self._table_schema_template, self.selected, self._pipe.parent)
+        r = self.clone(clone_pipe=True, keep_pipe_id=False)
         return r.bind(*args, **kwargs)
 
     def __or__(self, transform: Union["DltResource", AnyFun]) -> "DltResource":
         """Allows to pipe data from across resources and transform functions with | operator"""
         # print(f"{resource.name} | {self.name} -> {resource.name}[{resource.is_transformer}]")
         if isinstance(transform, DltResource):
             transform.pipe_data_from(self)
@@ -341,25 +353,42 @@
         pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
         _iter = map(lambda item: item.item, pipe_iterator)
         return flatten_list_or_items(_iter)
 
     def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
         container = Container()
         proxy = container[PipelineContext]
-        pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
+        pipeline = None if not proxy.is_active() else proxy.pipeline()
+        if pipeline:
+            pipeline_name = pipeline.pipeline_name
+        else:
+            pipeline_name = None
+        if pipeline:
+            default_schema_name = pipeline.default_schema_name
+        else:
+            default_schema_name = None
+        if not default_schema_name and pipeline_name:
+            default_schema_name = pipeline._make_schema_with_default_name().name
         return inject_section(
-            ConfigSectionContext(pipeline_name=pipeline_name, sections=(known_sections.SOURCES, self.section or pipeline_name or uniq_id(), self._name))
+            ConfigSectionContext(
+                pipeline_name=pipeline_name,
+                sections=(known_sections.SOURCES, self.section or default_schema_name or uniq_id(), self.source_name or default_schema_name or self._name),
+                source_state_key=self.source_name or default_schema_name or self.section or uniq_id()
+            )
         )
 
     def __str__(self) -> str:
-        info = f"DltResource {self._name}"
+        info = f"DltResource [{self._name}]"
         if self.section:
-            info += f" in section {self.section}:"
+            info += f" in section [{self.section}]"
+        if self.source_name:
+            info += f" added to source [{self.source_name}]:"
         else:
             info += ":"
+
         if self.is_transformer:
             info += f"\nThis resource is a transformer and takes data items from {self._pipe.parent.name}"
         else:
             if self._pipe.is_data_bound:
                 if self.requires_binding:
                     head_sig = inspect.signature(self._pipe.gen)  # type: ignore
                     info += f"\nThis resource is parametrized and takes the following arguments {head_sig}. You must call this resource before loading."
@@ -429,28 +458,29 @@
     @property
     def selected(self) -> Dict[str, DltResource]:
         """Returns a subset of all resources that will be extracted and loaded to the destination."""
         return {k:v for k,v in self.items() if v.selected}
 
     @property
     def extracted(self) -> Dict[str, DltResource]:
-        """Returns a dictionary of all resources that will be extracted. That includes selected resources and all their dependencies.
-        For dependencies that are not added explicitly to the source, a mock resource object is created that holds the parent pipe and derives the table
+        """Returns a dictionary of all resources that will be extracted. That includes selected resources and all their parents.
+        For parents that are not added explicitly to the source, a mock resource object is created that holds the parent pipe and derives the table
         schema from the child resource
         """
         extracted = self.selected
         for resource in self.selected.values():
             while (pipe := resource._pipe.parent) is not None:
                 if not pipe.is_empty:
                     try:
                         resource = self.find_by_pipe(pipe)
                     except KeyError:
                         # resource for pipe not found: return mock resource
                         mock_template = DltResourceSchema.new_table_template(pipe.name, write_disposition=resource._table_schema_template.get("write_disposition"))
                         resource = DltResource(pipe, mock_template, False, section=resource.section)
+                        resource.source_name = resource.source_name
                     extracted[resource._name] = resource
                 else:
                     break
         return extracted
 
     @property
     def selected_dag(self) -> List[Tuple[str, str]]:
@@ -509,14 +539,15 @@
             self.find_by_pipe(cloned)._pipe = cloned
         self._recently_added.clear()
 
     def __setitem__(self, resource_name: str, resource: DltResource) -> None:
         # make shallow copy of the resource
         resource = copy(resource)
         resource.section = self.source_section
+        resource.source_name = self.source_name
         # now set it in dict
         self._recently_added.append(resource)
         return super().__setitem__(resource_name, resource)
 
     def __delitem__(self, resource_name: str) -> None:
         raise DeletingResourcesNotSupported(self.source_name, resource_name)
 
@@ -537,14 +568,19 @@
     def __init__(self, name: str, section: str, schema: Schema, resources: Sequence[DltResource] = None) -> None:
         self.name = name
         self.section = section
         self.exhausted = False
         """Tells if iterator associated with a source is exhausted"""
         self._schema = schema
         self._resources: DltResourceDict = DltResourceDict(self.name, self.section)
+
+        if self.name != schema.name:
+            # raise ValueError(f"Schema name {schema.name} differs from source name {name}! The explicit source name argument is deprecated and will be soon removed.")
+            warnings.warn(f"Schema name {schema.name} differs from source name {name}! The explicit source name argument is deprecated and will be soon removed.")
+
         if resources:
             for resource in resources:
                 self._add_resource(resource._name, resource)
             self._resources.clone_new_pipes()
 
     @classmethod
     def from_data(cls, name: str, section: str, schema: Schema, data: Any) -> "DltSource":
@@ -665,15 +701,15 @@
     def run(self) -> SupportsPipelineRun:
         """A convenience method that will call `run` run on the currently active `dlt` pipeline. If pipeline instance is not found, one with default settings will be created."""
         self_run: SupportsPipelineRun = makefun.partial(Container()[PipelineContext].pipeline().run, *(), data=self)
         return self_run
 
     @property
     def state(self) -> StrAny:
-        """Gets source-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
+        """Gets source-scoped state from the active pipeline. PipelineStateNotAvailable is raised if no pipeline is active"""
         with self._get_config_section_context():
             return source_state()
 
     def clone(self) -> "DltSource":
         """Creates a deep copy of the source where copies of schema, resources and pipes are created"""
         # mind that resources and pipes are cloned when added to the DltResourcesDict in the source constructor
         return DltSource(self.name, self.section, self.schema.clone(), list(self._resources.values()))
@@ -701,15 +737,21 @@
         _iter = map(lambda item: item.item, pipe_iterator)
         self.exhausted = True
         return flatten_list_or_items(_iter)
 
     def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
         proxy = Container()[PipelineContext]
         pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
-        return inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=(known_sections.SOURCES, self.section, self.name)))
+        return inject_section(
+            ConfigSectionContext(
+                pipeline_name=pipeline_name,
+                sections=(known_sections.SOURCES, self.section, self.name),
+                source_state_key=self.name
+            )
+        )
 
     def _add_resource(self, name: str, resource: DltResource) -> None:
         if self.exhausted:
             raise SourceExhausted(self.name)
 
         if name in self._resources:
             # for resources with the same name try to add the resource as an another pipe
```

### Comparing `dlt-0.2.9a0/dlt/extract/typing.py` & `dlt-0.3.0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/extract/utils.py` & `dlt-0.3.0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/dbt/__init__.py` & `dlt-0.3.0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/dbt/configuration.py` & `dlt-0.3.0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/dbt/runner.py` & `dlt-0.3.0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/pandas.py` & `dlt-0.3.0/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/parquet.py` & `dlt-0.3.0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/helpers/streamlit.py` & `dlt-0.3.0/dlt/helpers/streamlit_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dlt.common import pendulum
 from dlt.common.typing import AnyFun
 from dlt.common.schema.typing import LOADS_TABLE_NAME, VERSION_TABLE_NAME
 from dlt.common.configuration.exceptions import ConfigFieldMissingException
 from dlt.common.exceptions import MissingDependencyException
 
-from dlt.helpers.pandas import pd
+from dlt.helpers.pandas_helper import pd
 from dlt.pipeline import Pipeline
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 from dlt.pipeline.state_sync import load_state_from_destination
 
 try:
     import streamlit as st
     # from streamlit import SECRETS_FILE_LOC, secrets
```

### Comparing `dlt-0.2.9a0/dlt/load/configuration.py` & `dlt-0.3.0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/load/exceptions.py` & `dlt-0.3.0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/load/load.py` & `dlt-0.3.0/dlt/load/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 job_info = self.load_storage.parse_job_file_name(file_path)
                 if job_info.file_format not in self.capabilities.supported_loader_file_formats:
                     raise LoadClientUnsupportedFileFormats(job_info.file_format, self.capabilities.supported_loader_file_formats, file_path)
                 logger.info(f"Will load file {file_path} with table name {job_info.table_name}")
                 table = self.get_load_table(schema, file_path)
                 if table["write_disposition"] not in ["append", "replace", "merge"]:
                     raise LoadClientUnsupportedWriteDisposition(job_info.table_name, table["write_disposition"], file_path)
-                job = client.start_file_load(table, self.load_storage.storage.make_full_path(file_path))
+                job = client.start_file_load(table, self.load_storage.storage.make_full_path(file_path), load_id)
         except (DestinationTerminalException, TerminalValueError):
             # if job irreversibly cannot be started, mark it as failed
             logger.exception(f"Terminal problem when adding job {file_path}")
             job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
         except (DestinationTransientException, Exception):
             # return no job so file stays in new jobs (root) folder
             logger.exception(f"Temporary problem when adding job {file_path}")
@@ -335,14 +335,14 @@
         dataset_name = None
         if isinstance(self.initial_client_config, DestinationClientDwhConfiguration):
             dataset_name = self.initial_client_config.dataset_name
 
         return LoadInfo(
             pipeline,
             self.initial_client_config.destination_name,
-            str(self.initial_client_config.credentials),
+            str(self.initial_client_config),
             dataset_name,
             list(load_ids),
             load_packages,
             started_at,
             pipeline.first_run
         )
```

### Comparing `dlt-0.2.9a0/dlt/normalize/configuration.py` & `dlt-0.3.0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/normalize/normalize.py` & `dlt-0.3.0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/pipeline/__init__.py` & `dlt-0.3.0/dlt/pipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,15 @@
         export_schema_path,
         full_refresh,
         progress,
         False,
         last_config(**kwargs),
         kwargs["runtime"])
     # set it as current pipeline
-    Container()[PipelineContext].activate(p)
-
+    p.activate()
     return p
 
 
 @with_config(spec=PipelineConfiguration, auto_pipeline_section=True)
 def attach(
     pipeline_name: str = None,
     pipelines_dir: str = None,
@@ -147,15 +146,15 @@
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
     progress = collector_from_name(progress)
     # create new pipeline instance
     p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
     # set it as current pipeline
-    Container()[PipelineContext].activate(p)
+    p.activate()
     return p
 
 
 def run(
     data: Any,
     *,
     destination: TDestinationReferenceArg = None,
```

### Comparing `dlt-0.2.9a0/dlt/pipeline/configuration.py` & `dlt-0.3.0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/pipeline/dbt.py` & `dlt-0.3.0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/pipeline/exceptions.py` & `dlt-0.3.0/dlt/pipeline/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,7 +50,12 @@
 class PipelineHasPendingDataException(PipelineException):
     def __init__(self, pipeline_name: str, pipelines_dir: str) -> None:
         msg = (
             f" Operation failed because pipeline with name {pipeline_name} in working directory {pipelines_dir} contains pending extracted files or load packages. "
             "Use `dlt pipeline sync` to reset the local state then run this operation again."
         )
         super().__init__(pipeline_name, msg)
+
+
+class PipelineNotActive(PipelineException):
+    def __init__(self, pipeline_name: str) -> None:
+        super().__init__(pipeline_name, f"Pipeline {pipeline_name} is not active so it cannot be deactivated")
```

### Comparing `dlt-0.2.9a0/dlt/pipeline/helpers.py` & `dlt-0.3.0/dlt/pipeline/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from collections import defaultdict
 import contextlib
-from typing import Callable, Tuple, Iterable, Optional, Any, cast, List, Iterator, Dict, Union, TypedDict
+from typing import Callable, Sequence, Iterable, Optional, Any, List, Iterator, Dict, Union, TypedDict
 from itertools import chain
 
 from dlt.common.jsonpath import resolve_paths, TAnyJsonPath, compile_paths
 
 from dlt.common.exceptions import TerminalException
 from dlt.common.schema.utils import get_child_tables, group_tables_by_resource, compile_simple_regexes, compile_simple_regex
 from dlt.common.schema.typing import TSimpleRegex
 from dlt.common.typing import REPattern
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
 from dlt.pipeline.exceptions import PipelineStepFailed, PipelineHasPendingDataException
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline import Pipeline
-from dlt.common.pipeline import TSourceState, _reset_resource_state, sources_state, _delete_source_state_keys, _get_matching_resources
+from dlt.common.pipeline import TSourceState, _reset_resource_state, _sources_state, _delete_source_state_keys, _get_matching_resources
 
 
-def retry_load(retry_on_pipeline_steps: Tuple[TPipelineStep, ...] = ("load",)) -> Callable[[Exception], bool]:
+def retry_load(retry_on_pipeline_steps: Sequence[TPipelineStep] = ("load",)) -> Callable[[BaseException], bool]:
     """A retry strategy for Tenacity that, with default setting, will repeat `load` step for all exceptions that are not terminal
 
     Use this condition with tenacity `retry_if_exception`. Terminal exceptions are exceptions that will not go away when operations is repeated.
     Examples: missing configuration values, Authentication Errors, terminally failed jobs exceptions etc.
 
     >>> data = source(...)
     >>> for attempt in Retrying(stop=stop_after_attempt(3), retry=retry_if_exception(retry_load(())), reraise=True):
     >>>     with attempt:
     >>>         p.run(data)
 
     Args:
         retry_on_pipeline_steps (Tuple[TPipelineStep, ...], optional): which pipeline steps are allowed to be repeated. Default: "load"
 
     """
-    def _retry_load(ex: Exception) -> bool:
+    def _retry_load(ex: BaseException) -> bool:
         # do not retry in normalize or extract stages
         if isinstance(ex, PipelineStepFailed) and ex.step not in retry_on_pipeline_steps:
             return False
         # do not retry on terminal exceptions
         if isinstance(ex, TerminalException) or (ex.__context__ is not None and isinstance(ex.__context__, TerminalException)):
             return False
         return True
@@ -136,15 +135,15 @@
     def _list_state_paths(self, source_state: Dict[str, Any]) -> List[str]:
         return resolve_paths(self.state_paths_to_drop, source_state)
 
     def _create_modified_state(self) -> Dict[str, Any]:
         state: TSourceState = self.pipeline.state  # type: ignore[assignment]
         if not self.drop_state:
             return state  # type: ignore[return-value]
-        source_states = sources_state(state).items()
+        source_states = _sources_state(state).items()
         for source_name, source_state in source_states:
             if self.drop_state:
                 for key in _get_matching_resources(self.resource_pattern, source_state):
                     self.info['resource_states'].append(key)
                     _reset_resource_state(key, source_state)
             resolved_paths = resolve_paths(self.state_paths_to_drop, source_state)
             if self.state_paths_to_drop and not resolved_paths:
```

### Comparing `dlt-0.2.9a0/dlt/pipeline/pipeline.py` & `dlt-0.3.0/dlt/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TSchemaTables, TWriteDisposition
 from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo
 from dlt.common.typing import TFun, TSecretValue
 from dlt.common.runners import pool_runner as runner
 from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, LoadStorage, SchemaStorage, FileStorage, NormalizeStorageConfiguration, SchemaStorageConfiguration, LoadStorageConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
-from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
+from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, PipelineContext, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
 from dlt.common.utils import is_interactive
 
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, SourceExhausted
 from dlt.extract.extract import ExtractorStorage, extract_with_schema
@@ -38,25 +38,27 @@
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load import Load
 
 from dlt.pipeline.configuration import PipelineConfiguration
 from dlt.pipeline.progress import _Collector, _NULL_COLLECTOR
-from dlt.pipeline.exceptions import CannotRestorePipelineException, InvalidPipelineName, PipelineConfigMissing, PipelineStepFailed, SqlClientNotAvailable
+from dlt.pipeline.exceptions import CannotRestorePipelineException, InvalidPipelineName, PipelineConfigMissing, PipelineNotActive, PipelineStepFailed, SqlClientNotAvailable
 from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, load_trace, merge_traces, start_trace, start_trace_step, end_trace_step, end_trace
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.state_sync import STATE_ENGINE_VERSION, load_state_from_destination, merge_state_if_changed, migrate_state, state_resource, json_encode_state, json_decode_state
 
 
 def with_state_sync(may_extract_state: bool = False) -> Callable[[TFun], TFun]:
 
     def decorator(f: TFun) -> TFun:
         @wraps(f)
         def _wrap(self: "Pipeline", *args: Any, **kwargs: Any) -> Any:
+            # activate pipeline so right state is always provided
+            self.activate()
             # backup and restore state
             should_extract_state = may_extract_state and self.config.restore_from_destination
             with self.managed_state(extract_state=should_extract_state) as state:
                 # add the state to container as a context
                 with self._container.injectable_context(StateInjectableContext(state=state)):
                     return f(self, *args, **kwargs)
 
@@ -214,15 +216,15 @@
             # we overwrite the state with the values from init
             self._set_destination(destination)  # changing the destination could be dangerous if pipeline has not loaded items
             self._set_dataset_name(dataset_name)
             self.credentials = credentials
             self._configure(import_schema_path, export_schema_path, must_attach_to_local_pipeline)
 
     def drop(self) -> "Pipeline":
-        """Deletes existing pipeline state, schemas and drops datasets at the destination if present"""
+        """Deletes local pipeline state, schemas and any working files"""
         # reset the pipeline working dir
         self._create_pipeline()
         # clone the pipeline
         return Pipeline(
             self.pipeline_name,
             self.pipelines_dir,
             self.pipeline_salt,
@@ -325,15 +327,14 @@
     ) -> LoadInfo:
         """Loads the packages prepared by `normalize` method into the `dataset_name` at `destination`, using provided `credentials`"""
         # set destination and default dataset if provided
         self._set_destination(destination)
         self._set_dataset_name(dataset_name)
         self.credentials = credentials or self.credentials
 
-
         # check if any schema is present, if not then no data was extracted
         if not self.default_schema_name:
             return None
 
         # make sure that destination is set and client is importable and can be instantiated
         client = self._get_destination_client(self.default_schema)
 
@@ -528,14 +529,42 @@
             if "_local" not in state:
                 state["_local"] = local_state
             self._props_to_state(state)
             self._save_state(state)
         except Exception as ex:
             raise PipelineStepFailed(self, "run", ex, None) from ex
 
+    def activate(self) -> None:
+        """Activates the pipeline
+
+        The active pipeline is used as a context for several `dlt` components. It provides state to sources and resources evaluated outside of
+        `pipeline.run` and `pipeline.extract` method. For example, if the source you use is accessing state in `dlt.source` decorated function, the state is provided
+        by active pipeline.
+
+        The name of active pipeline is used when resolving secrets and config values as the optional most outer section during value lookup. For example if pipeline
+        with name `chess_pipeline` is active and `dlt` looks for `BigQuery` configuration, it will look in `chess_pipeline.destination.bigquery.credentials` first and then in
+        `destination.bigquery.credentials`.
+
+        Active pipeline also provides the current DestinationCapabilitiesContext to other components ie. Schema instances. Among others, it sets the naming convention
+        and maximum identifier length.
+
+        Only one pipeline is active at a given time.
+
+        Pipeline created or attached with `dlt.pipeline`/'dlt.attach` is automatically activated. `run`, `load` and `extract` methods also activate pipeline.
+        """
+        Container()[PipelineContext].activate(self)
+
+    def deactivate(self) -> None:
+        """Deactivates the pipeline
+
+        Pipeline must be active in order to use this method. Please refer to `activate()` method for the explanation of active pipeline concept.
+        """
+        if not self.is_active:
+            raise PipelineNotActive(self.pipeline_name)
+        Container()[PipelineContext].deactivate()
 
     @property
     def has_data(self) -> bool:
         """Tells if the pipeline contains any data: schemas, extracted files, load packages or loaded packages in the destination"""
         return not self.first_run or bool(self.schema_names) or len(self.list_extracted_resources()) > 0 or len(self.list_normalized_load_packages()) > 0
 
     @property
@@ -625,14 +654,24 @@
         #     )
         if schema_name:
             schema = self.schemas[schema_name]
         else:
             schema = self.default_schema if self.default_schema_name else Schema(self.dataset_name)
         return self._sql_job_client(schema, credentials).sql_client
 
+    def _destination_client(self, schema_name: str = None, credentials: Any = None) -> JobClientBase:
+        """Get the destination job client for the configured destination"""
+        # TODO: duplicated code from self.sql_client()  ...
+        if schema_name:
+            schema = self.schemas[schema_name]
+        else:
+            schema = self.default_schema if self.default_schema_name else Schema(self.dataset_name)
+        client_config = self._get_destination_client_initial_config(credentials)
+        return self._get_destination_client(schema, client_config)
+
     def _sql_job_client(self, schema: Schema, credentials: Any = None) -> SqlJobClientBase:
         client_config = self._get_destination_client_initial_config(credentials)
         client = self._get_destination_client(schema , client_config)
         if isinstance(client, SqlJobClientBase):
             return client
         else:
             raise SqlClientNotAvailable(self.pipeline_name, self.destination.__name__)
@@ -742,15 +781,17 @@
                 _resources = data_item.resources.values()
                 for r in _resources:
                     apply_hint_args(r)
                 sources.append(data_item)
             elif isinstance(data_item, DltResource):
                 # apply hints
                 apply_hint_args(data_item)
-                sources.append(DltSource(data_item.name, data_item.section or self.pipeline_name, effective_schema, [data_item]))
+                sources.append(
+                    DltSource(effective_schema.name, data_item.section or self.pipeline_name, effective_schema, [data_item])
+                    )
             else:
                 # iterator/iterable/generator
                 # create resource first without table template
                 resource = DltResource.from_data(data_item, name=table_name, section=self.pipeline_name)
                 # apply hints
                 apply_hint_args(resource)
                 resources.append(resource)
@@ -849,16 +890,20 @@
     def _validate_pipeline_name(self) -> None:
         try:
             FileStorage.validate_file_name_component(self.pipeline_name)
         except ValueError as ve_ex:
             raise InvalidPipelineName(self.pipeline_name, str(ve_ex))
 
     def _make_schema_with_default_name(self) -> Schema:
-        # make a schema from the pipeline name using the name normalizer
-        return Schema(self.pipeline_name, normalize_name=True)
+        """Make a schema from the pipeline name using the name normalizer. "_pipeline" suffix is removed if present"""
+        if self.pipeline_name.endswith("_pipeline"):
+            schema_name = self.pipeline_name[:-9]
+        else:
+            schema_name = self.pipeline_name
+        return Schema(schema_name, normalize_name=True)
 
     def _validate_dataset_name(self, dataset_name: str) -> None:
         normalized_name = self._default_naming.normalize_identifier(dataset_name)
         if normalized_name != dataset_name:
             raise InvalidDatasetName(dataset_name, normalized_name)
 
     def _set_context(self, is_active: bool) -> None:
@@ -1046,15 +1091,14 @@
             backup_state = self._get_state()
             # do not compare local states
             local_state = state.pop("_local")
             backup_state.pop("_local")
 
             # check if any state element was changed
             merged_state = merge_state_if_changed(backup_state, state)
-
             # extract state only when there's change in the state or state was not yet extracted AND we actually want to do it
             if (merged_state or "_last_extracted_at" not in local_state) and extract_state:
                 # print(f'EXTRACT STATE merged: {bool(merged_state)} extracted timestamp in {"_last_extracted_at" not in local_state}')
                 merged_state = self._extract_state(merged_state or state)
                 local_state["_last_extracted_at"] = pendulum.now()
 
             # if state is modified and is not being extracted, mark it to be extracted next time
@@ -1091,15 +1135,15 @@
 
     def _save_state(self, state: TPipelineState) -> None:
         self._pipeline_storage.save(Pipeline.STATE_FILE, json_encode_state(state))
 
     def _extract_state(self, state: TPipelineState) -> TPipelineState:
         # this will extract the state into current load package and update the schema with the _dlt_pipeline_state table
         # note: the schema will be persisted because the schema saving decorator is over the state manager decorator for extract
-        state_source = DltSource("pipeline_state", self.pipeline_name, self.default_schema, [state_resource(state)])
+        state_source = DltSource(self.default_schema.name, self.pipeline_name, self.default_schema, [state_resource(state)])
         storage = ExtractorStorage(self._normalize_storage_config)
         extract_id = extract_with_schema(storage, state_source, self.default_schema, _NULL_COLLECTOR, 1, 1)
         storage.commit_extract_files(extract_id)
         return state
 
     def __getstate__(self) -> Any:
         # pickle only the SupportsPipeline protocol fields
```

### Comparing `dlt-0.2.9a0/dlt/pipeline/progress.py` & `dlt-0.3.0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/pipeline/state_sync.py` & `dlt-0.3.0/dlt/pipeline/state_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import base64
 import binascii
 from typing import Any, Optional, cast
 import binascii
 
 import pendulum
 
 import dlt
```

### Comparing `dlt-0.2.9a0/dlt/pipeline/trace.py` & `dlt-0.3.0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/pipeline/track.py` & `dlt-0.3.0/dlt/pipeline/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from dlt.common import pendulum
 from dlt.common import logger
 from dlt.common.runtime.exec_info import github_info
 from dlt.common.runtime.segment import track as dlthub_telemetry_track
 from dlt.common.runtime.slack import send_slack_message
 from dlt.common.pipeline import LoadInfo, SupportsPipeline
+from dlt.common.destination import DestinationReference
 
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace
 
 
 def _add_sentry_tags(span: Span, pipeline: SupportsPipeline) -> None:
     span.set_tag("pipeline_name", pipeline.pipeline_name)
@@ -78,15 +79,15 @@
     # disable automatic slack messaging until we can configure messages themselves
     # if step.step == "load":
     #     if pipeline.runtime_config.slack_incoming_hook and step.step_exception is None:
     #         slack_notify_load_success(pipeline.runtime_config.slack_incoming_hook, step_info, trace)
     dlthub_telemetry_track("pipeline", step.step, {
         "elapsed": (step.finished_at - trace.started_at).total_seconds(),
         "success": step.step_exception is None,
-        "destination_name": pipeline.destination.__name__.split(".")[-1] if pipeline.destination else None,
+        "destination_name": DestinationReference.to_name(pipeline.destination) if pipeline.destination else None,
         "transaction_id": trace.transaction_id
     })
 
 
 def on_end_trace(trace: PipelineTrace, pipeline: SupportsPipeline) -> None:
     if pipeline.runtime_config.sentry_dsn:
         # print(f"---END SENTRY TX: {trace.transaction_id} SCOPE: {Hub.current.scope}")
```

### Comparing `dlt-0.2.9a0/dlt/reflection/names.py` & `dlt-0.3.0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/reflection/script_inspector.py` & `dlt-0.3.0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/reflection/script_visitor.py` & `dlt-0.3.0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.0/dlt/sources/helpers/requests/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,37 +129,39 @@
     >>>         return False
     >>>     return response.text == 'error'
 
     The retry is triggered when either any of the predicates or the default conditions based on status code/exception are `True`.
 
     ### Args:
         timeout: Timeout for requests in seconds. May be passed as `timedelta` or `float/int` number of seconds.
+        max_connections: Max connections per host in the HTTPAdapter pool
         raise_for_status: Whether to raise exception on error status codes (using `response.raise_for_status()`)
         session: Optional `requests.Session` instance to add the retry handler to. A new session is created by default.
         status_codes: Retry when response has any of these status codes. Default `429` and all `5xx` codes. Pass an empty list to disable retry based on status.
         exceptions: Retry on exception of given type(s). Default `(requests.Timeout, requests.ConnectionError)`. Pass an empty list to disable retry on exceptions.
         max_attempts: Max number of retry attempts before giving up
         condition: A predicate or a list of predicates to decide whether to retry. If any predicate returns `True` the request is retried
         backoff_factor: Multiplier used for exponential delay between retries
         respect_retry_after_header: Whether to use the `Retry-After` response header (when available) to determine the retry delay
         **session_attrs: Extra attributes that will be set on the session instance, e.g. `headers: {'Authorization': 'api-key'}` (see `requests.sessions.Session` for possible attributes)
     """
     def __init__(
         self,
         timeout: Optional[TimedeltaSeconds] = DEFAULT_TIMEOUT,
+        max_connections: int = 50,
         raise_for_status: bool = True,
         status_codes: Sequence[int] = DEFAULT_RETRY_STATUS,
         exceptions: Sequence[Type[Exception]] = DEFAULT_RETRY_EXCEPTIONS,
         max_attempts: int = DEFAULT_RETRY_ATTEMPTS,
         condition: Union[RetryPredicate, Sequence[RetryPredicate], None] = None,
         backoff_factor: float = DEFAULT_BACKOFF_FACTOR,
         respect_retry_after_header: bool = True,
         **session_attrs: Any
     ) -> None:
-        self._adapter = HTTPAdapter()
+        self._adapter = HTTPAdapter(pool_maxsize=max_connections)
         self._local = local()
         self._session_kwargs = dict(timeout=timeout, raise_for_status=raise_for_status)
         self._retry_kwargs = dict(
             status_codes=status_codes,
             exceptions=exceptions,
             max_attempts=max_attempts,
             condition=condition,
```

### Comparing `dlt-0.2.9a0/dlt/sources/helpers/requests/session.py` & `dlt-0.3.0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/sources/helpers/transform.py` & `dlt-0.3.0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/dlt/version.py` & `dlt-0.3.0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9a0/pyproject.toml` & `dlt-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.9a0"
+version = "0.3.0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -65,15 +65,18 @@
 
 duckdb = {version = ">=0.6.1,<0.9.0", optional = true}
 
 dbt-core = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-redshift = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-bigquery = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-duckdb = {version = ">=1.3.0,<1.5.0", optional = true}
-psutil = "^5.9.5"
+s3fs = {version = "^2023.5.0", optional = true}
+gcsfs = {version = "^2023.5.0", optional = true}
+boto3 = {version = ">=1.26", optional = true}
+fsspec = "^2023.5.0"
 
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 mypy = "1.2.0"
 flake8 = "^5.0.0"
@@ -92,20 +95,23 @@
 flake8-tidy-imports = ">=4.8.0"
 flake8-encodings = "^0.5.0"
 flake8-builtins = "^1.5.3"
 types-SQLAlchemy = ">=1.4.53"
 
 [tool.poetry.extras]
 dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb"]
-gcp = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes"]
+gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
 # bigquery is alias on gcp extras
-bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes"]
+bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
 postgres = ["psycopg2-binary", "psycopg2cffi"]
 redshift = ["psycopg2-binary", "psycopg2cffi"]
 duckdb = ["duckdb"]
+filesystem = ["s3fs", "boto3"]
+s3 = ["s3fs", "boto3"]
+gs = ["gcsfs"]
 
 [tool.poetry.scripts]
 dlt = "dlt.cli._dlt:_main"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.10.0"
 types-click = "^7.1.8"
```

### Comparing `dlt-0.2.9a0/setup.py` & `dlt-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
  'dlt.common.runtime',
  'dlt.common.schema',
  'dlt.common.storages',
  'dlt.destinations',
  'dlt.destinations.bigquery',
  'dlt.destinations.duckdb',
  'dlt.destinations.dummy',
+ 'dlt.destinations.filesystem',
  'dlt.destinations.postgres',
  'dlt.destinations.redshift',
  'dlt.extract',
  'dlt.helpers',
  'dlt.helpers.dbt',
  'dlt.load',
  'dlt.normalize',
@@ -45,25 +46,25 @@
  'SQLAlchemy>=1.4.0',
  'astunparse>=1.6.3',
  'asyncstdlib>=3.10.5',
  'cachetools>=5.2.0',
  'click>=7.1',
  'cron-descriptor>=1.2.32',
  'deprecated>=1.2.13,<2.0.0',
+ 'fsspec>=2023.5.0,<2024.0.0',
  'gitpython>=3.1.29',
  'giturlparse>=0.10.0',
  'hexbytes>=0.2.2',
  'humanize>=4.4.0',
  'json-logging==1.4.1rc0',
  'jsonpath-ng>=1.5.3,<2.0.0',
  'makefun>=1.15.0',
  'pathvalidate>=2.5.2',
  'pendulum>=2.1.2',
  'pipdeptree>=2.3.3',
- 'psutil>=5.9.5,<6.0.0',
  'pytz>=2022.6',
  'requests>=2.26.0',
  'requirements-parser>=0.5.0',
  'semver>=2.13.0',
  'sentry-sdk>=1.4.3',
  'setuptools>=65.6.0',
  'simplejson>=3.17.5',
@@ -72,34 +73,40 @@
  'typing-extensions>=4.0.0',
  'tzdata>=2022.1']
 
 extras_require = \
 {':platform_python_implementation != "PyPy"': ['orjson>=3.8.6,<4.0.0'],
  'bigquery': ['grpcio>=1.50.0',
               'google-cloud-bigquery>=2.26.0',
-              'pyarrow>=8.0.0'],
+              'pyarrow>=8.0.0',
+              'gcsfs>=2023.5.0,<2024.0.0'],
  'dbt': ['dbt-core>=1.3.0,<1.5.0',
          'dbt-redshift>=1.3.0,<1.5.0',
          'dbt-bigquery>=1.3.0,<1.5.0',
          'dbt-duckdb>=1.3.0,<1.5.0'],
  'duckdb': ['duckdb>=0.6.1,<0.9.0'],
- 'gcp': ['grpcio>=1.50.0', 'google-cloud-bigquery>=2.26.0', 'pyarrow>=8.0.0'],
+ 'filesystem': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26'],
+ 'gcp': ['grpcio>=1.50.0',
+         'google-cloud-bigquery>=2.26.0',
+         'gcsfs>=2023.5.0,<2024.0.0'],
+ 'gs': ['gcsfs>=2023.5.0,<2024.0.0'],
  'postgres': ['psycopg2-binary>=2.9.1'],
  'postgres:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0'],
  'redshift': ['psycopg2-binary>=2.9.1'],
- 'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0']}
+ 'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0'],
+ 's3': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.2.9a0',
+    'version': '0.3.0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
-    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Pipelines and Destinations\n\nExplore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
+    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dlt-0.2.9a0/PKG-INFO` & `dlt-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.9a0
+Version: 0.3.0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -20,50 +20,56 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: bigquery
 Provides-Extra: dbt
 Provides-Extra: duckdb
+Provides-Extra: filesystem
 Provides-Extra: gcp
+Provides-Extra: gs
 Provides-Extra: postgres
 Provides-Extra: redshift
+Provides-Extra: s3
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: SQLAlchemy (>=1.4.0)
 Requires-Dist: astunparse (>=1.6.3)
 Requires-Dist: asyncstdlib (>=3.10.5)
+Requires-Dist: boto3 (>=1.26); extra == "filesystem" or extra == "s3"
 Requires-Dist: cachetools (>=5.2.0)
 Requires-Dist: click (>=7.1)
 Requires-Dist: cron-descriptor (>=1.2.32)
 Requires-Dist: dbt-bigquery (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-core (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-duckdb (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-redshift (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: duckdb (>=0.6.1,<0.9.0); extra == "duckdb"
+Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
+Requires-Dist: gcsfs (>=2023.5.0,<2024.0.0); extra == "gcp" or extra == "bigquery" or extra == "gs"
 Requires-Dist: gitpython (>=3.1.29)
 Requires-Dist: giturlparse (>=0.10.0)
 Requires-Dist: google-cloud-bigquery (>=2.26.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: grpcio (>=1.50.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: hexbytes (>=0.2.2)
 Requires-Dist: humanize (>=4.4.0)
 Requires-Dist: json-logging (==1.4.1rc0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: makefun (>=1.15.0)
 Requires-Dist: orjson (>=3.8.6,<4.0.0); platform_python_implementation != "PyPy"
 Requires-Dist: pathvalidate (>=2.5.2)
 Requires-Dist: pendulum (>=2.1.2)
 Requires-Dist: pipdeptree (>=2.3.3)
-Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1); extra == "postgres" or extra == "redshift"
 Requires-Dist: psycopg2cffi (>=2.9.0); (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
-Requires-Dist: pyarrow (>=8.0.0); extra == "gcp" or extra == "bigquery"
+Requires-Dist: pyarrow (>=8.0.0); extra == "bigquery"
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: requirements-parser (>=0.5.0)
+Requires-Dist: s3fs (>=2023.5.0,<2024.0.0); extra == "filesystem" or extra == "s3"
 Requires-Dist: semver (>=2.13.0)
 Requires-Dist: sentry-sdk (>=1.4.3)
 Requires-Dist: setuptools (>=65.6.0)
 Requires-Dist: simplejson (>=3.17.5)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tomlkit (>=0.11.3)
 Requires-Dist: typing-extensions (>=4.0.0)
@@ -131,17 +137,17 @@
 - **Easy Maintenance:** Clear data pipeline structure for updates.
 - **Rapid Exploration:** Quickly explore and gain insights from new data sources.
 - **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
 - **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
 - **Incremental Loading:** Load only new or changed data and avoid loading old records again.
 - **Open Source:** Free and Apache 2.0 Licensed.
 
-## Ready to use Pipelines and Destinations
+## Ready to use Sources and Destinations
 
-Explore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
+Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
 
 ## Documentation
 
 For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
 ## Examples
 
@@ -149,15 +155,15 @@
 
 ## Get Involved
 
 The dlt project is quickly growing, and we're excited to have you join our community! Here's how you can get involved:
 
 - **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)
 - **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.
-- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.
+- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.
 - **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.
 - **Improve documentation**: Help us enhance the dlt documentation.
 
 ## License
 
 DLT is released under the [Apache 2.0 License](LICENSE.txt).
```

