# Comparing `tmp/aqueduct-ml-0.3.5.tar.gz` & `tmp/aqueduct-ml-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.3.5.tar", last modified: Wed May 31 20:27:13 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.3.6.tar", last modified: Wed Jun  7 04:48:27 2023, max compression
```

## Comparing `aqueduct-ml-0.3.5.tar` & `aqueduct-ml-0.3.6.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.521709 aqueduct-ml-0.3.5/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.525709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.525709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.525709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.529709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.537709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2886 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1820 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16596 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5201 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9602 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7001 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.537709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2725 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.545709 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.545709 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1276 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.549709 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.549709 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.549709 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7519 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9245 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5795 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-31 20:27:13.000000 aqueduct-ml-0.3.5/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29947 2023-05-31 18:17:41.000000 aqueduct-ml-0.3.5/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-31 18:17:41.000000 aqueduct-ml-0.3.5/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 20:27:13.553709 aqueduct-ml-0.3.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-31 17:37:48.000000 aqueduct-ml-0.3.5/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-31 18:17:41.000000 aqueduct-ml-0.3.5/version
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.274980 aqueduct-ml-0.3.6/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       40 2023-05-03 19:36:09.000000 aqueduct-ml-0.3.6/MANIFEST.in
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7719 2023-06-07 04:48:27.274691 aqueduct-ml-0.3.6/PKG-INFO
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.223003 aqueduct-ml-0.3.6/aqueduct_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.223192 aqueduct-ml-0.3.6/aqueduct_executor/migrators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.225015 aqueduct-ml-0.3.6/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.226734 aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.229253 aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.229595 aqueduct-ml-0.3.6/aqueduct_executor/operators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.231111 aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3092 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      485 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.231475 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.243794 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/athena.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3970 2023-05-24 17:09:38.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      658 2023-05-09 17:09:45.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/common.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2886 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1820 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/connector.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    16596 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5201 2023-05-24 17:09:38.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/extract.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      725 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/load.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1258 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-05-09 17:09:45.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/models.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1742 2023-05-24 17:09:38.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/parameters.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/relational.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9602 2023-05-12 21:06:08.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7001 2023-05-12 21:06:08.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.244742 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5379 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5463 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2725 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.250214 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.256484 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    17252 2023-05-03 19:36:09.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1276 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1501 2023-05-03 19:36:09.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.258869 aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1097 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.261642 aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2683 2023-05-03 19:36:09.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/execute_data.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1020 2023-05-03 19:36:09.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/execute_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.263879 aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1105 2023-05-23 00:44:06.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.267969 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/enums.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      462 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/exceptions.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7519 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/execution.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.271719 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/file.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/parse.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/storage.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/timer.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9245 2023-06-06 20:20:00.000000 aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.273352 aqueduct-ml-0.3.6/aqueduct_ml.egg-info/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7719 2023-06-07 04:48:27.000000 aqueduct-ml-0.3.6/aqueduct_ml.egg-info/PKG-INFO
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5795 2023-06-07 04:48:27.000000 aqueduct-ml-0.3.6/aqueduct_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-06-07 04:48:27.000000 aqueduct-ml-0.3.6/aqueduct_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      248 2023-06-07 04:48:27.000000 aqueduct-ml-0.3.6/aqueduct_ml.egg-info/requires.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-06-07 04:48:27.000000 aqueduct-ml-0.3.6/aqueduct_ml.egg-info/top_level.txt
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-06-07 04:48:27.273632 aqueduct-ml-0.3.6/bin/
+-rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29947 2023-06-06 20:21:12.000000 aqueduct-ml-0.3.6/bin/aqueduct
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      228 2023-05-03 19:36:09.000000 aqueduct-ml-0.3.6/requirements.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-06-07 04:48:27.275063 aqueduct-ml-0.3.6/setup.cfg
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1053 2023-05-09 17:09:45.000000 aqueduct-ml-0.3.6/setup.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        6 2023-06-06 20:21:12.000000 aqueduct-ml-0.3.6/version
```

### Comparing `aqueduct-ml-0.3.5/PKG-INFO` & `aqueduct-ml-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.5
+Version: 0.3.6
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.3.6/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.3.6/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/load.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/parameters.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/main.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/main.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_data.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/execute_function.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/execute_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/main.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.3.6/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.3.6/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.5
+Version: 0.3.6
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.5/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.3.6/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.5/bin/aqueduct` & `aqueduct-ml-0.3.6/bin/aqueduct`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import distro
 import requests
 import yaml
 from packaging.version import parse as parse_version
 from tqdm import tqdm
 
-SCHEMA_VERSION = "27"
+SCHEMA_VERSION = "28"
 CHUNK_SIZE = 4096
 
 # Connector Package Version Bounds
 PYMONGO_VERSION_BOUND = "<=4.3.3"
 PSYCOPG2_VERSION_BOUND = "<=2.9.5"
 BIGQUERY_VERSION_BOUND = "<=3.5.0"
 DB_DTYPES_VERSION_BOUND = "<=1.1.1"
@@ -34,15 +34,15 @@
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.3.5"
+package_version = "0.3.6"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
```

### Comparing `aqueduct-ml-0.3.5/setup.py` & `aqueduct-ml-0.3.6/setup.py`

 * *Files identical despite different names*

