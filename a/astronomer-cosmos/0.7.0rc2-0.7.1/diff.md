# Comparing `tmp/astronomer_cosmos-0.7.0rc2.tar.gz` & `tmp/astronomer_cosmos-0.7.1.tar.gz`

## Comparing `astronomer_cosmos-0.7.0rc2.tar` & `astronomer_cosmos-0.7.1.tar`

### file list

```diff
@@ -1,76 +1,80 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0    13421 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/base.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/token.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/thrift.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/tests/test_base.py
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/base.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/warn_parsing.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/README.rst
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9047 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/virtualenv.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_virtualenv.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/base.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/token.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/thrift.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/base.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/test-connections.yaml
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/test_example_dags.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/cosmos/tests/utils.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/README.rst
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.1/PKG-INFO
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/core/airflow.py` & `astronomer_cosmos-0.7.1/cosmos/core/airflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,43 +64,35 @@
         super().__init__(*args, **kwargs)
 
         entities: Dict[str, Any] = {}
 
         # render all the entities in the group
         for ent in cosmos_group.entities:
             if isinstance(ent, Group):
-                entities[ent.id] = CosmosTaskGroup(
-                    cosmos_group=ent, dag=dag, parent_group=self
-                )
+                entities[ent.id] = CosmosTaskGroup(cosmos_group=ent, dag=dag, parent_group=self)
             elif isinstance(ent, Task):
                 entities[ent.id] = get_airflow_task(
                     task=ent,
                     dag=dag,
                     task_group=self,
                 )
 
         # add dependencies
         for ent in cosmos_group.entities:
             for upstream_id in ent.upstream_entity_ids:
                 if upstream_id not in entities:
-                    raise ValueError(
-                        f"Entity {upstream_id} is not in the group {cosmos_group.id}"
-                    )
+                    raise ValueError(f"Entity {upstream_id} is not in the group {cosmos_group.id}")
 
                 if ent.id not in entities:
-                    raise ValueError(
-                        f"Entity {ent.id} is not in the group {cosmos_group.id}"
-                    )
+                    raise ValueError(f"Entity {ent.id} is not in the group {cosmos_group.id}")
 
                 entities[upstream_id] >> entities[ent.id]
 
 
-def get_airflow_task(
-    task: Task, dag: DAG, task_group: Optional[TaskGroup] = None
-) -> BaseOperator:
+def get_airflow_task(task: Task, dag: DAG, task_group: Optional[TaskGroup] = None) -> BaseOperator:
     """
     Get the Airflow Operator class for a Task.
 
     :param task: The Task to get the Operator for
 
     :return: The Operator class
     :rtype: BaseOperator
@@ -115,12 +107,10 @@
         task_id=task.id,
         dag=dag,
         task_group=task_group,
         **task.arguments,
     )
 
     if not isinstance(airflow_task, BaseOperator):
-        raise TypeError(
-            f"Operator class {task.operator_class} is not a subclass of BaseOperator"
-        )
+        raise TypeError(f"Operator class {task.operator_class} is not a subclass of BaseOperator")
 
     return airflow_task
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.7.1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/core/tests/test_airflow.py` & `astronomer_cosmos-0.7.1/cosmos/core/tests/test_airflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,15 @@
             if isinstance(entity, Task):
                 expected[entity.id] = {
                     "operator_class": entity.operator_class,
                     "arguments": entity.arguments,
                     "upstream_entity_ids": entity.upstream_entity_ids + upstreams,
                 }
             elif isinstance(entity, Group):
-                flatten_entities(
-                    entity.entities, upstreams + entity.upstream_entity_ids
-                )
+                flatten_entities(entity.entities, upstreams + entity.upstream_entity_ids)
 
     flatten_entities(group.entities)
 
     ############################
     # CosmosDag
     ############################
     dag = CosmosDag(
@@ -240,17 +238,15 @@
         cosmos_task = expected[task_id]
 
         assert task_id in expected
 
         class_name = str(type(tg_task))
         assert class_name == f"<class '{cosmos_task['operator_class']}'>"
 
-        airflow_upstream_task_ids = [
-            id.split(".")[-1] for id in list(tg_task.upstream_task_ids)
-        ]
+        airflow_upstream_task_ids = [id.split(".")[-1] for id in list(tg_task.upstream_task_ids)]
         assert airflow_upstream_task_ids == cosmos_task["upstream_entity_ids"]
 
 
 def test_invalid_operator() -> None:
     """Tests that an invalid operator raises an error."""
     with pytest.raises(ValueError):
         group = Group(id="group_1")
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,33 +29,25 @@
         DbtSeedDockerOperator,
         DbtSnapshotDockerOperator,
         DbtTestDockerOperator,
     )
 except ImportError:
     from .core.operators.lazy_load import MissingPackage
 
-    DbtLSDockerOperator = MissingPackage(
-        "cosmos.providers.dbt.core.operators.docker.DbtLSDockerOperator", "docker"
-    )
-    DbtRunDockerOperator = MissingPackage(
-        "cosmos.providers.dbt.core.operators.docker.DbtRunDockerOperator", "docker"
-    )
+    DbtLSDockerOperator = MissingPackage("cosmos.providers.dbt.core.operators.docker.DbtLSDockerOperator", "docker")
+    DbtRunDockerOperator = MissingPackage("cosmos.providers.dbt.core.operators.docker.DbtRunDockerOperator", "docker")
     DbtRunOperationDockerOperator = MissingPackage(
         "cosmos.providers.dbt.core.operators.docker.DbtRunOperationDockerOperator",
         "docker",
     )
-    DbtSeedDockerOperator = MissingPackage(
-        "cosmos.providers.dbt.core.operators.docker.DbtSeedDockerOperator", "docker"
-    )
+    DbtSeedDockerOperator = MissingPackage("cosmos.providers.dbt.core.operators.docker.DbtSeedDockerOperator", "docker")
     DbtSnapshotDockerOperator = MissingPackage(
         "cosmos.providers.dbt.core.operators.docker.DbtSnapshotDockerOperator", "docker"
     )
-    DbtTestDockerOperator = MissingPackage(
-        "cosmos.providers.dbt.core.operators.docker.DbtTestDockerOperator", "docker"
-    )
+    DbtTestDockerOperator = MissingPackage("cosmos.providers.dbt.core.operators.docker.DbtTestDockerOperator", "docker")
 
 try:
     from .core.operators.kubernetes import (
         DbtLSKubernetesOperator,
         DbtRunKubernetesOperator,
         DbtRunOperationKubernetesOperator,
         DbtSeedKubernetesOperator,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/dag.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param execution_mode: The execution mode in which the dbt project should be run.
-        Options are "local", "docker", and "kubernetes".
+        Options are "local", "virtualenv", "docker", and "kubernetes".
         Defaults to "local"
     :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     def __init__(
         self,
@@ -49,15 +49,15 @@
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
-        execution_mode: Literal["local", "docker", "kubernetes"] = "local",
+        execution_mode: Literal["local", "docker", "kubernetes", "virtualenv"] = "local",
         on_warning_callback: Optional[Callable] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         # add additional args to the dbt_args
         dbt_args = {
             **dbt_args,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,15 @@
         dbt_snapshots_dir=dbt_snapshots_dir,
         dbt_seeds_dir=dbt_seeds_dir,
         project_name=dbt_project_name,
     )
 
     # this is the group that will be returned
     base_group = Group(id=dbt_project_name)
-    entities: Dict[
-        str, CosmosEntity
-    ] = {}  # this is a dict of all the entities we create
+    entities: Dict[str, CosmosEntity] = {}  # this is a dict of all the entities we create
 
     # add project_dir arg to task_args
     if execution_mode == "local":
         task_args["project_dir"] = project.project_dir
 
     # ensures the same tag isn't in select & exclude
     if "tags" in select and "tags" in exclude:
@@ -99,36 +97,27 @@
                 f"Can't specify the same path in `select` and `include`: "
                 f"{set(select['paths']).intersection(exclude['paths'])}"
             )
 
     # if task_args has a schema, add it to the profile args and add a deprecated warning
     if "schema" in task_args:
         profile_args["schema"] = task_args["schema"]
-        logger.warning(
-            "Specifying a schema in the task_args is deprecated. Please use the profile_args instead."
-        )
+        logger.warning("Specifying a schema in the task_args is deprecated. Please use the profile_args instead.")
 
     # iterate over each model once to create the initial tasks
-    for model_name, model in itertools.chain(
-        project.models.items(), project.snapshots.items(), project.seeds.items()
-    ):
+    for model_name, model in itertools.chain(project.models.items(), project.snapshots.items(), project.seeds.items()):
         # filters down to a path within the project_dir
         if "paths" in select:
-            root_directories = [
-                project.project_dir / path.strip("/")
-                for path in select.get("paths", [])
-            ]
+            root_directories = [project.project_dir / path.strip("/") for path in select.get("paths", [])]
             if not set(root_directories).intersection(model.path.parents):
                 continue
 
         # filters out any specified paths
         if "paths" in exclude:
-            root_directories = [
-                project.project_dir / path.strip("/") for path in exclude.get("paths")
-            ]
+            root_directories = [project.project_dir / path.strip("/") for path in exclude.get("paths")]
             if set(root_directories).intersection(model.path.parents):
                 continue
 
         if "configs" in select:
             # TODO: coverme
             if not set(select["configs"]).intersection(model.config.config_selectors):
                 continue
@@ -189,15 +178,16 @@
                     execution_mode=execution_mode,
                     dbt_class="DbtSeed",
                 ),
                 arguments=run_args,
             )
         else:
             # TODO: coverme
-            logger.error("Unknown DBT type.")
+            logger.error("Unknown dbt type.")
+            continue
 
         # if test_behavior isn't "after_each", we can just add the task to the
         # base group and do nothing else for now
         if test_behavior != "after_each":
             entities[model_name] = run_task
             base_group.add_entity(entity=run_task)
             continue
@@ -226,26 +216,22 @@
 
         # all other non-run tasks don't need to be grouped with test tasks
         else:
             entities[model_name] = run_task
             base_group.add_entity(entity=run_task)
 
     # add dependencies now that we have all the entities
-    for model_name, model in itertools.chain(
-        project.models.items(), project.snapshots.items(), project.seeds.items()
-    ):
+    for model_name, model in itertools.chain(project.models.items(), project.snapshots.items(), project.seeds.items()):
         upstream_deps = model.config.upstream_models
         for upstream_model_name in upstream_deps:
             try:
                 dep_task = entities[upstream_model_name]
                 entities[model_name].add_upstream(dep_task)
             except KeyError:
-                logger.error(
-                    f"Dependency {upstream_model_name} not found for model {model}"
-                )
+                logger.error(f"Dependency {upstream_model_name} not found for model {model}")
     if test_behavior == "after_all":
         # make a test task
         test_task = Task(
             id=f"{dbt_project_name}_test",
             operator_class=calculate_operator_class(
                 execution_mode=execution_mode,
                 dbt_class="DbtTest",
@@ -256,17 +242,15 @@
 
         # add it to the base group
         base_group.add_entity(test_task)
 
         # add it as an upstream to all the models that don't have downstream tasks
         # since we don't have downstream info readily available, we have to iterate
         # start with all models, and remove them as we find downstream tasks
-        models_with_no_downstream_tasks = [
-            model_name for model_name, model in project.models.items()
-        ]
+        models_with_no_downstream_tasks = [model_name for model_name, model in project.models.items()]
 
         # iterate over all models
         for model_name, model in project.models.items():
             # iterate over all upstream models
             for upstream_model_name in model.config.upstream_models:
                 # remove the upstream model from the list of models with no downstream tasks
                 try:
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/task_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param execution_mode: The execution mode in which the dbt project should be run.
-        Options are "local", "docker", and "kubernetes".
+        Options are "local", "virtualenv", "docker", and "kubernetes".
         Defaults to "local"
     :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     def __init__(
         self,
@@ -51,15 +51,15 @@
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_snapshots_dir: str = "snapshots",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
-        execution_mode: Literal["local", "docker", "kubernetes"] = "local",
+        execution_mode: Literal["local", "docker", "kubernetes", "virtualenv"] = "local",
         on_warning_callback: Optional[Callable] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         # add additional args to the dbt_args
         dbt_args = {
             **dbt_args,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .local import DbtDepsLocalOperator as DbtDepsOperator
+from .local import DbtDocsAzureStorageLocalOperator as DbtDocsAzureStorageOperator
 from .local import DbtDocsLocalOperator as DbtDocsOperator
+from .local import DbtDocsS3LocalOperator as DbtDocsS3Operator
 from .local import DbtLSLocalOperator as DbtLSOperator
 from .local import DbtRunLocalOperator as DbtRunOperator
 from .local import DbtRunOperationLocalOperator as DbtRunOperationOperator
 from .local import DbtSeedLocalOperator as DbtSeedOperator
 from .local import DbtSnapshotLocalOperator as DbtSnapshotOperator
 from .local import DbtTestLocalOperator as DbtTestOperator
 
@@ -12,8 +14,10 @@
     "DbtSeedOperator",
     "DbtSnapshotOperator",
     "DbtRunOperator",
     "DbtTestOperator",
     "DbtRunOperationOperator",
     "DbtDepsOperator",
     "DbtDocsOperator",
+    "DbtDocsS3Operator",
+    "DbtDocsAzureStorageOperator",
 ]
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         "no_version_check",
         "cache_selected_only",
         "fail_fast",
         "quiet",
         "warn_error",
     )
 
-    include_system_env = False
     intercept_flag = True
 
     def __init__(
         self,
         project_dir: str,
         conn_id: str,
         base_cmd: str | list[str] = None,
@@ -129,43 +128,60 @@
         elif dbt_executable_path == "dbt":
             self.dbt_executable_path = shutil.which("dbt")
         else:
             self.dbt_executable_path = dbt_executable_path
         self.dbt_cmd_flags = dbt_cmd_flags
         super().__init__(**kwargs)
 
-    def get_env(self, context: Context, profile_vars: dict[str, str]) -> dict[str, str]:
+    def get_env(self, context: Context) -> dict[str, str | bytes | os.PathLike]:
         """
         Builds the set of environment variables to be exposed for the bash command.
+
         The order of determination is:
-            1. The env parameter passed to the Operator
+            1. If append_env is True, the current process environment.
             2. The Airflow context as environment variables.
-            3. The profile variables from the dbt profile file.
-        If a user accidentally uses a key that is found earlier in the determination order then it is overwritten.
+            3. The env parameter passed to the Operator
+
+        Note that this also filters out any invalid types that cannot be cast to strings.
         """
         env: dict[str, Any] = {}
 
-        # env parameter passed to the Operator
-        if self.env and isinstance(self.env, dict):
-            env.update(self.env)
+        if self.append_env:
+            env.update(os.environ)
 
         # Airflow context as environment variables
         airflow_context_vars = context_to_airflow_vars(context, in_env_var_format=True)
         env.update(airflow_context_vars)
 
-        # profile variables from the dbt profile file
-        env.update(profile_vars)
+        # env parameter passed to the Operator
+        if self.env and isinstance(self.env, dict):
+            env.update(self.env)
 
-        # filter out invalid types
+        # filter out invalid types and give a warning when a value is removed
         accepted_types = (str, bytes, os.PathLike)
-        filtered_env = {
-            k: v
-            for k, v in env.items()
-            if all((isinstance(k, accepted_types), isinstance(v, accepted_types)))
-        }
+
+        filtered_env: dict[str, str | bytes | os.PathLike] = {}
+
+        for key, val in env.items():
+            if isinstance(key, accepted_types) and isinstance(val, accepted_types):
+                filtered_env[key] = val
+            else:
+                if isinstance(key, accepted_types):
+                    logger.warning(
+                        "Env var %s was ignored because its key is not a valid type. Must be one of %s",
+                        key,
+                        accepted_types,
+                    )
+
+                if isinstance(val, accepted_types):
+                    logger.warning(
+                        "Env var %s was ignored because its value is not a valid type. Must be one of %s",
+                        key,
+                        accepted_types,
+                    )
 
         return filtered_env
 
     def add_global_flags(self) -> list[str]:
         flags = []
         for global_flag in self.global_flags:
             # for now, skip the project_dir flag
@@ -196,10 +212,10 @@
         else:
             dbt_cmd.extend(self.base_cmd)
         dbt_cmd.extend(self.add_global_flags())
         # add command specific flags
         if cmd_flags:
             dbt_cmd.extend(cmd_flags)
 
-        env = self.get_env(context, profile_vars={})
+        env = self.get_env(context)
 
         return dbt_cmd, env
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 
 class DbtDockerBaseOperator(DockerOperator, DbtBaseOperator):
     """
     Executes a dbt core cli command in a Docker container.
 
     """
 
-    template_fields: Sequence[str] = (
-        DbtBaseOperator.template_fields + DockerOperator.template_fields
-    )
+    template_fields: Sequence[str] = DbtBaseOperator.template_fields + DockerOperator.template_fields
 
     intercept_flag = False
 
     def __init__(
         self,
         image: str,  # Make image a required argument since it's required by DockerOperator
         **kwargs,
@@ -131,17 +129,15 @@
 class DbtTestDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core test command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(
-        self, on_warning_callback: Optional[Callable] = None, **kwargs
-    ) -> None:
+    def __init__(self, on_warning_callback: Optional[Callable] = None, **kwargs) -> None:
         super().__init__(**kwargs)
         self.base_cmd = "test"
         # as of now, on_warning_callback in docker executor does nothing
         self.on_warning_callback = on_warning_callback
 
     def execute(self, context: Context):
         return self.build_and_run_cmd(context=context)
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 
 class DbtKubernetesBaseOperator(KubernetesPodOperator, DbtBaseOperator):
     """
     Executes a dbt core cli command in a Kubernetes Pod.
 
     """
 
-    template_fields: Sequence[str] = (
-        DbtBaseOperator.template_fields + KubernetesPodOperator.template_fields
-    )
+    template_fields: Sequence[str] = DbtBaseOperator.template_fields + KubernetesPodOperator.template_fields
 
     intercept_flag = False
 
     def __init__(
         self,
         **kwargs,
     ) -> None:
@@ -141,17 +139,15 @@
 class DbtTestKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core test command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(
-        self, on_warning_callback: Optional[Callable] = None, **kwargs
-    ) -> None:
+    def __init__(self, on_warning_callback: Optional[Callable] = None, **kwargs) -> None:
         super().__init__(**kwargs)
         self.base_cmd = "test"
         # as of now, on_warning_callback in kubernetes executor does nothing
         self.on_warning_callback = on_warning_callback
 
     def execute(self, context: Context):
         return self.build_and_run_cmd(context=context)
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/local.py`

 * *Files 26% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
-    include_system_env = True
 
     def __init__(
         self,
         install_deps: bool = False,
         callback: Optional[Callable[[str], None]] = None,
         profile_args: dict[str, str] = {},
         **kwargs,
@@ -61,26 +60,23 @@
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
 
     def exception_handling(self, result: FullOutputSubprocessResult):
         if self.skip_exit_code is not None and result.exit_code == self.skip_exit_code:
-            raise AirflowSkipException(
-                f"dbt command returned exit code {self.skip_exit_code}. Skipping."
-            )
+            raise AirflowSkipException(f"dbt command returned exit code {self.skip_exit_code}. Skipping.")
         elif result.exit_code != 0:
             raise AirflowException(
-                f"dbt command failed. The command returned a non-zero exit code {result.exit_code}."
+                f"dbt command failed. The command returned a non-zero exit code {result.exit_code}. Details: ",
+                *result.full_output,
             )
 
     @provide_session
-    def store_compiled_sql(
-        self, tmp_project_dir: str, context: Context, session: Session = NEW_SESSION
-    ) -> None:
+    def store_compiled_sql(self, tmp_project_dir: str, context: Context, session: Session = NEW_SESSION) -> None:
         """
         Takes the compiled SQL files from the dbt run and stores them in the compiled_sql rendered template.
         Gets called after every dbt run.
         """
         compiled_queries = {}
         # dbt compiles sql files and stores them in the target directory
         for root, _, files in os.walk(os.path.join(tmp_project_dir, "target")):
@@ -109,33 +105,50 @@
         session.query(RenderedTaskInstanceFields).filter(
             RenderedTaskInstanceFields.dag_id == self.dag_id,
             RenderedTaskInstanceFields.task_id == self.task_id,
             RenderedTaskInstanceFields.run_id == ti.run_id,
         ).delete()
         session.add(rtif)
 
+    def run_subprocess(self, *args, **kwargs):
+        return self.subprocess_hook.run_command(*args, **kwargs)
+
     def run_command(
         self,
         cmd: list[str],
         env: dict[str, str],
         context: Context,
     ) -> FullOutputSubprocessResult:
         """
         Copies the dbt project to a temporary directory and runs the command.
         """
         with tempfile.TemporaryDirectory() as tmp_dir:
+            logger.info(
+                "Cloning project to writable temp directory %s from %s",
+                tmp_dir,
+                self.project_dir,
+            )
+
             # need a subfolder because shutil.copytree will fail if the destination dir already exists
             tmp_project_dir = os.path.join(tmp_dir, "dbt_project")
             shutil.copytree(
                 self.project_dir,
                 tmp_project_dir,
             )
 
             # get the profile name from the dbt_project.yml file
             dbt_project_path = os.path.join(tmp_project_dir, "dbt_project.yml")
+
+            # if there's no dbt_project.yml file, we're not in a dbt project
+            # and need to raise an error
+            if not os.path.exists(dbt_project_path):
+                raise AirflowException(
+                    f"dbt project directory {self.project_dir} does not contain a dbt_project.yml file."
+                )
+
             with open(dbt_project_path, encoding="utf-8") as f:
                 dbt_project = yaml.safe_load(f)
 
             profile_name = dbt_project.get("profile")
 
             # need to write the profile to a file because dbt requires a profile file
             # and doesn't accept a profile as a string
@@ -147,58 +160,54 @@
                 profile_name=profile_name,
             )
             profile_file_path = os.path.join(tmp_project_dir, "profiles.yml")
             with open(profile_file_path, "w", encoding="utf-8") as f:
                 f.write(profile_file_contents)
 
             # we also need to get the env from the profile mapping
-            env.update(profile_mapping.get_env_vars())
+            env.update(profile_mapping.env_vars)
 
             # if we need to install deps, do so
             if self.install_deps:
-                self.subprocess_hook.run_command(
+                self.run_subprocess(
                     command=[self.dbt_executable_path, "deps"],
                     env=env,
                     output_encoding=self.output_encoding,
                     cwd=tmp_project_dir,
                 )
 
-            result = self.subprocess_hook.run_command(
+            logger.info("Trying to run the command:\n %s\nFrom %s", cmd, tmp_project_dir)
+
+            result = self.run_subprocess(
                 command=cmd,
                 env=env,
                 output_encoding=self.output_encoding,
                 cwd=tmp_project_dir,
             )
 
             self.exception_handling(result)
             self.store_compiled_sql(tmp_project_dir, context)
             if self.callback:
                 self.callback(tmp_project_dir)
 
             return result
 
-    def build_and_run_cmd(
-        self, context: Context, cmd_flags: list[str] | None = None
-    ) -> FullOutputSubprocessResult:
+    def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None) -> FullOutputSubprocessResult:
         dbt_cmd, env = self.build_cmd(context=context, cmd_flags=cmd_flags)
         return self.run_command(cmd=dbt_cmd, env=env, context=context)
 
     def execute(self, context: Context) -> str:
         # TODO is this going to put loads of unnecessary stuff in to xcom?
         return self.build_and_run_cmd(context=context).output
 
     def on_kill(self) -> None:
         if self.cancel_query_on_kill:
             self.subprocess_hook.log.info("Sending SIGINT signal to process group")
-            if self.subprocess_hook.sub_process and hasattr(
-                self.subprocess_hook.sub_process, "pid"
-            ):
-                os.killpg(
-                    os.getpgid(self.subprocess_hook.sub_process.pid), signal.SIGINT
-                )
+            if self.subprocess_hook.sub_process and hasattr(self.subprocess_hook.sub_process, "pid"):
+                os.killpg(os.getpgid(self.subprocess_hook.sub_process.pid), signal.SIGINT)
         else:
             self.subprocess_hook.send_sigterm()
 
 
 class DbtLSLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core ls command.
@@ -304,17 +313,15 @@
         and on_warning_callback is set, then function returns True.
 
         :param result: The output from the build and run command.
         """
 
         return self.on_warning_callback and no_tests_message not in result.output
 
-    def _handle_warnings(
-        self, result: FullOutputSubprocessResult, context: Context
-    ) -> None:
+    def _handle_warnings(self, result: FullOutputSubprocessResult, context: Context) -> None:
         """
          Handles warnings by extracting log issues, creating additional context, and calling the
          on_warning_callback with the updated context.
 
         :param result: The result object from the build and run command.
         :param context: The original airflow context in which the build and run command was executed.
         """
@@ -374,28 +381,150 @@
     """
     Executes `dbt docs generate` command.
     Use the `callback` parameter to specify a callback function to run after the command completes.
     """
 
     ui_color = "#8194E0"
 
+    required_files = ["index.html", "manifest.json", "graph.gpickle", "catalog.json"]
+
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self.base_cmd = ["docs", "generate"]
 
     def execute(self, context: Context):
         result = self.build_and_run_cmd(context=context)
         return result.output
 
 
+class DbtDocsS3LocalOperator(DbtDocsLocalOperator):
+    """
+    Executes `dbt docs generate` command and upload to S3 storage. Returns the S3 path to the generated documentation.
+
+    :param aws_conn_id: S3's Airflow connection ID
+    :param bucket_name: S3's bucket name
+    :param folder_dir: This can be used to specify under which directory the generated DBT documentation should be
+        uploaded.
+    """
+
+    ui_color = "#FF9900"
+
+    def __init__(
+        self,
+        aws_conn_id: str,
+        bucket_name: str,
+        folder_dir: str | None = None,
+        **kwargs,
+    ) -> None:
+        "Initializes the operator."
+        self.aws_conn_id = aws_conn_id
+        self.bucket_name = bucket_name
+        self.folder_dir = folder_dir
+
+        super().__init__(**kwargs)
+
+        # override the callback with our own
+        self.callback = self.upload_to_s3
+
+    def upload_to_s3(self, project_dir: str) -> None:
+        "Uploads the generated documentation to S3."
+        logger.info(
+            'Attempting to upload generated docs to S3 using S3Hook("%s")',
+            self.aws_conn_id,
+        )
+
+        from airflow.providers.amazon.aws.hooks.s3 import S3Hook
+
+        target_dir = f"{project_dir}/target"
+
+        hook = S3Hook(
+            self.aws_conn_id,
+            extra_args={
+                "ContentType": "text/html",
+            },
+        )
+
+        for filename in self.required_files:
+            logger.info("Uploading %s to %s", filename, f"s3://{self.bucket_name}/{filename}")
+
+            key = f"{self.folder_dir}/{filename}" if self.folder_dir else filename
+
+            hook.load_file(
+                filename=f"{target_dir}/{filename}",
+                bucket_name=self.bucket_name,
+                key=key,
+                replace=True,
+            )
+
+
+class DbtDocsAzureStorageLocalOperator(DbtDocsLocalOperator):
+    """
+    Executes `dbt docs generate` command and upload to Azure Blob Storage.
+
+    :param azure_conn_id: Azure Blob Storage's Airflow connection ID
+    :param container_name: Azure Blob Storage's bucket name
+    :param folder_dir: This can be used to specify under which directory the generated DBT documentation should be
+        uploaded.
+    """
+
+    ui_color = "#007FFF"
+
+    def __init__(
+        self,
+        azure_conn_id: str,
+        container_name: str,
+        folder_dir: str | None = None,
+        **kwargs,
+    ) -> None:
+        "Initializes the operator."
+        self.azure_conn_id = azure_conn_id
+        self.container_name = container_name
+        self.folder_dir = folder_dir
+
+        super().__init__(**kwargs)
+
+        # override the callback with our own
+        self.callback = self.upload_to_azure
+
+    def upload_to_azure(self, project_dir: str) -> None:
+        "Uploads the generated documentation to Azure Blob Storage."
+        logger.info(
+            'Attempting to upload generated docs to Azure Blob Storage using WasbHook(conn_id="%s")',
+            self.azure_conn_id,
+        )
+
+        from airflow.providers.microsoft.azure.hooks.wasb import WasbHook
+
+        target_dir = f"{project_dir}/target"
+
+        hook = WasbHook(
+            self.azure_conn_id,
+        )
+
+        for filename in self.required_files:
+            logger.info(
+                "Uploading %s to %s",
+                filename,
+                f"wasb://{self.container_name}/{filename}",
+            )
+
+            blob_name = f"{self.folder_dir}/{filename}" if self.folder_dir else filename
+
+            hook.load_file(
+                file_path=f"{target_dir}/{filename}",
+                container_name=self.container_name,
+                blob_name=blob_name,
+                overwrite=True,
+            )
+
+
 class DbtDepsLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core deps command.
     """
 
     ui_color = "#8194E0"
 
     def __init__(self, **kwargs) -> None:
         raise DeprecationWarning(
-            "The DbtDepsOperator has been deprecated. "
-            "Please use the `install_deps` flag in dbt_args instead."
+            "The DbtDepsOperator has been deprecated. " "Please use the `install_deps` flag in dbt_args instead."
         )
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_docker.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,34 +50,20 @@
         "some_path": Path(__file__),
         "retries": 3,
         ("tuple", "key"): "some_value",
     }
     p_context_to_airflow_vars.return_value = {"START_DATE": "2023-02-15 12:30:00"}
     env = dbt_base_operator.get_env(
         Context(execution_date=datetime(2023, 2, 15, 12, 30)),
-        profile_vars={
-            "SNOWFLAKE_USER": "my_user_id",
-            "SNOWFLAKE_PASSWORD": "supersecure123",
-            "SNOWFLAKE_ACCOUNT": "my_account",
-            "SNOWFLAKE_ROLE": None,
-            "SNOWFLAKE_DATABASE": "my_database",
-            "SNOWFLAKE_WAREHOUSE": None,
-            "SNOWFLAKE_SCHEMA": "jaffle_shop",
-        },
     )
     expected_env = {
         "start_date": "20220101",
         "end_date": "20220102",
         "some_path": Path(__file__),
         "START_DATE": "2023-02-15 12:30:00",
-        "SNOWFLAKE_USER": "my_user_id",
-        "SNOWFLAKE_PASSWORD": "supersecure123",
-        "SNOWFLAKE_ACCOUNT": "my_account",
-        "SNOWFLAKE_DATABASE": "my_database",
-        "SNOWFLAKE_SCHEMA": "jaffle_shop",
     }
     assert env == expected_env
 
 
 base_kwargs = {
     "conn_id": "my_airflow_connection",
     "task_id": "my-task",
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,34 +50,20 @@
         "some_path": Path(__file__),
         "retries": 3,
         ("tuple", "key"): "some_value",
     }
     p_context_to_airflow_vars.return_value = {"START_DATE": "2023-02-15 12:30:00"}
     env = dbt_kube_operator.get_env(
         Context(execution_date=datetime(2023, 2, 15, 12, 30)),
-        profile_vars={
-            "SNOWFLAKE_USER": "my_user_id",
-            "SNOWFLAKE_PASSWORD": "supersecure123",
-            "SNOWFLAKE_ACCOUNT": "my_account",
-            "SNOWFLAKE_ROLE": None,
-            "SNOWFLAKE_DATABASE": "my_database",
-            "SNOWFLAKE_WAREHOUSE": None,
-            "SNOWFLAKE_SCHEMA": "jaffle_shop",
-        },
     )
     expected_env = {
         "start_date": "20220101",
         "end_date": "20220102",
         "some_path": Path(__file__),
         "START_DATE": "2023-02-15 12:30:00",
-        "SNOWFLAKE_USER": "my_user_id",
-        "SNOWFLAKE_PASSWORD": "supersecure123",
-        "SNOWFLAKE_ACCOUNT": "my_account",
-        "SNOWFLAKE_DATABASE": "my_database",
-        "SNOWFLAKE_SCHEMA": "jaffle_shop",
     }
     assert env == expected_env
 
 
 base_kwargs = {
     "conn_id": "my_airflow_connection",
     "task_id": "my-task",
@@ -138,15 +124,14 @@
             "generation": None,
             "labels": {
                 "airflow_kpo_in_cluster": "False",
                 "airflow_version": pod_obj.metadata.labels["airflow_version"],
             },
             "managed_fields": None,
             "name": pod_obj.metadata.name,
-            "namespace": "foo",
             "owner_references": None,
             "resource_version": None,
             "self_link": None,
             "uid": None,
         },
         "spec": {
             "active_deadline_seconds": None,
@@ -220,8 +205,10 @@
             "termination_grace_period_seconds": None,
             "tolerations": [],
             "topology_spread_constraints": None,
             "volumes": [],
         },
         "status": None,
     }
-    assert pod_obj.to_dict() == expected_result
+    computed_result = pod_obj.to_dict()
+    computed_result["metadata"].pop("namespace")
+    assert computed_result == expected_result
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/base.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 This module contains a base class that other profile mappings should
 inherit from to ensure consistency.
 """
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
+
 from logging import getLogger
 from typing import Any
 
+from typing import TYPE_CHECKING
 import yaml
-from typing_extensions import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from airflow.models import Connection
 
 logger = getLogger(__name__)
 
 
-class BaseProfileMapping:
+class BaseProfileMapping(ABC):
     """
     A base class that other profile mappings should inherit from to ensure consistency.
     Responsible for mapping Airflow connections to dbt profiles.
     """
 
     airflow_connection_type: str = "generic"
     is_community: bool = False
@@ -55,39 +57,40 @@
                     self.__class__.__name__,
                     field,
                 )
                 return False
 
         return True
 
-    def get_profile(self) -> dict[str, Any]:
+    @property
+    @abstractmethod
+    def profile(self) -> dict[str, Any]:
         """
         Return a dbt profile based on the Airflow connection.
         """
         raise NotImplementedError
 
-    def get_env_vars(self) -> dict[str, str]:
+    @property
+    def env_vars(self) -> dict[str, str]:
         "Returns a dictionary of environment variables that should be set based on self.secret_fields."
         env_vars = {}
 
         for field in self.secret_fields:
             env_var_name = self.get_env_var_name(field)
             value = self.get_dbt_value(field)
             if value is not None:
                 env_vars[env_var_name] = str(value)
 
         return env_vars
 
-    def get_profile_file_contents(
-        self, profile_name: str, target_name: str = "cosmos_target"
-    ) -> str:
+    def get_profile_file_contents(self, profile_name: str, target_name: str = "cosmos_target") -> str:
         """
         Translates the profile into a string that can be written to a profiles.yml file.
         """
-        profile_vars = self.get_profile()
+        profile_vars = self.profile
 
         # filter out any null values
         profile_vars = {k: v for k, v in profile_vars.items() if v is not None}
 
         profile_contents = {
             profile_name: {
                 "target": target_name,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 
 
 class GoogleCloudServiceAccountFileProfileMapping(BaseProfileMapping):
     """
     Maps Airflow GCP connections to dbt BigQuery profiles if they use a service account file.
 
     https://docs.getdbt.com/reference/warehouse-setups/bigquery-setup#service-account-file
-    https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/connections/databricks.html
+    https://airflow.apache.org/docs/apache-airflow-providers-google/stable/connections/gcp.html
     """
 
-    airflow_connection_type: str = "google-cloud-platform"
+    airflow_connection_type: str = "google_cloud_platform"
 
     required_fields = [
         "project",
         "dataset",
         "keyfile",
     ]
 
     airflow_param_mapping = {
         "project": "extra.project",
         "dataset": "dataset",
         "keyfile": "extra.key_path",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Generates profile. Defaults `threads` to 1."
         return {
             "type": "bigquery",
             "method": "service-account",
             "project": self.project,
             "dataset": self.dataset,
             "threads": self.profile_args.get("threads") or 1,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     extra = {
         "project": "my_project",
         "key_path": "my_key_path.json",
     }
     conn = Connection(
         conn_id="my_bigquery_connection",
-        conn_type="google-cloud-platform",
+        conn_type="google_cloud_platform",
         extra=json.dumps(extra),
     )
 
     with patch("airflow.hooks.base.BaseHook.get_connection", return_value=conn):
         yield conn
 
 
@@ -48,43 +48,39 @@
 
     # if we're missing any of the values, it shouldn't claim
     for key in extra:
         values = extra.copy()
         del values[key]
         conn = Connection(
             conn_id="my_bigquery_connection",
-            conn_type="google-cloud-platform",
+            conn_type="google_cloud_platform",
             extra=json.dumps(values),
         )
 
         print("testing with", values)
 
-        profile_mapping = GoogleCloudServiceAccountFileProfileMapping(
-            conn, {"dataset": "my_dataset"}
-        )
+        profile_mapping = GoogleCloudServiceAccountFileProfileMapping(conn, {"dataset": "my_dataset"})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(
         conn_id="my_bigquery_connection",
-        conn_type="google-cloud-platform",
+        conn_type="google_cloud_platform",
         extra=json.dumps(extra),
     )
     profile_mapping = GoogleCloudServiceAccountFileProfileMapping(conn, {})
     assert not profile_mapping.can_claim_connection()
 
     # if we have them all, it should claim
     conn = Connection(
         conn_id="my_bigquery_connection",
-        conn_type="google-cloud-platform",
+        conn_type="google_cloud_platform",
         extra=json.dumps(extra),
     )
-    profile_mapping = GoogleCloudServiceAccountFileProfileMapping(
-        conn, {"dataset": "my_dataset"}
-    )
+    profile_mapping = GoogleCloudServiceAccountFileProfileMapping(conn, {"dataset": "my_dataset"})
     assert profile_mapping.can_claim_connection()
 
 
 def test_bigquery_mapping_selected(
     mock_bigquery_conn: Connection,
 ) -> None:
     """
@@ -109,15 +105,15 @@
             "dataset": "my_dataset",
         },
     )
     assert profile_mapping.profile_args == {
         "dataset": "my_dataset",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "bigquery",
         "method": "service-account",
         "project": mock_bigquery_conn.extra_dejson.get("project"),
         "keyfile": mock_bigquery_conn.extra_dejson.get("key_path"),
         "dataset": "my_dataset",
         "threads": 1,
     }
@@ -141,15 +137,15 @@
     assert profile_mapping.profile_args == {
         "dataset": "my_dataset",
         "threads": 2,
         "project": "my_project_override",
         "keyfile": "my_keyfile_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "bigquery",
         "method": "service-account",
         "project": "my_project_override",
         "keyfile": "my_keyfile_override",
         "dataset": "my_dataset",
         "threads": 2,
     }
@@ -161,8 +157,8 @@
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_bigquery_conn.conn_id,
         profile_args={"dataset": "my_dataset"},
     )
-    assert profile_mapping.get_env_vars() == {}
+    assert profile_mapping.env_vars == {}
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/token.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     airflow_param_mapping = {
         "host": "host",
         "schema": "schema",
         "token": ["password", "extra.token"],
         "http_path": "extra.http_path",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Generates profile. The token is stored in an environment variable."
         return {
             "type": "databricks",
             "schema": self.schema,
             "host": self.host,
             "http_path": self.http_path,
             **self.profile_args,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         },
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
         "catalog": "my_catalog",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_databricks_conn.conn_type,
         "host": mock_databricks_conn.host.replace("https://", ""),
         "token": "{{ env_var('COSMOS_CONN_DATABRICKS_TOKEN') }}",
         "http_path": mock_databricks_conn.extra_dejson.get("http_path"),
         "schema": "my_schema",
         "catalog": "my_catalog",
     }
@@ -125,16 +125,15 @@
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
         "http_path": "http_path_override",
         "host": "my_host_override",
     }
 
-    print("profile_mapping.get_profile()", profile_mapping.get_profile())
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_databricks_conn.conn_type,
         "host": "my_host_override",
         "token": "{{ env_var('COSMOS_CONN_DATABRICKS_TOKEN') }}",
         "http_path": "http_path_override",
         "schema": "my_schema",
     }
 
@@ -145,10 +144,10 @@
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_databricks_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_DATABRICKS_TOKEN": mock_databricks_conn.password,
     }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         "encryption": "extra.encryption",
         "compression": "extra.compression",
         "connection_timeout": "extra.connection_timeout",
         "socket_timeout": "extra.socket_timeout",
         "protocol_version": "extra.protocol_version",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile. The password is stored in an environment variable."
         profile_vars = {
             "type": "exasol",
             "threads": self.threads,
             "dsn": self.dsn,
             "user": self.user,
             "dbname": self.dbname,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,46 +56,40 @@
     for key in potential_values:
         values = potential_values.copy()
         del values[key]
         conn = Connection(**values)  # type: ignore
 
         print("testing with", values)
 
-        profile_mapping = ExasolUserPasswordProfileMapping(
-            conn, {"schema": "my_schema", "threads": 1}
-        )
+        profile_mapping = ExasolUserPasswordProfileMapping(conn, {"schema": "my_schema", "threads": 1})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = ExasolUserPasswordProfileMapping(conn, {"threads": 1})
     assert not profile_mapping.can_claim_connection()
 
     # also test when there's no threads
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = ExasolUserPasswordProfileMapping(conn, {"schema": "my_schema"})
     assert not profile_mapping.can_claim_connection()
 
     # if we have them all, it should claim
     conn = Connection(**potential_values)  # type: ignore
-    profile_mapping = ExasolUserPasswordProfileMapping(
-        conn, {"schema": "my_schema", "threads": 1}
-    )
+    profile_mapping = ExasolUserPasswordProfileMapping(conn, {"schema": "my_schema", "threads": 1})
     assert profile_mapping.can_claim_connection()
 
 
 def test_profile_mapping_selected(
     mock_exasol_connection: Connection,
 ) -> None:
     """
     Tests that the correct profile mapping is selected.
     """
-    profile_mapping = get_profile_mapping(
-        mock_exasol_connection.conn_id, {"schema": "my_schema", "threads": 1}
-    )
+    profile_mapping = get_profile_mapping(mock_exasol_connection.conn_id, {"schema": "my_schema", "threads": 1})
     assert isinstance(profile_mapping, ExasolUserPasswordProfileMapping)
 
 
 def test_profile_args(
     mock_exasol_connection: Connection,
 ) -> None:
     """
@@ -106,15 +100,15 @@
         profile_args={"schema": "my_schema", "threads": 1},
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
         "threads": 1,
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_exasol_connection.conn_type,
         "dsn": f"{mock_exasol_connection.host}:{mock_exasol_connection.port}",
         "user": mock_exasol_connection.login,
         "password": "{{ env_var('COSMOS_CONN_EXASOL_PASSWORD') }}",
         "dbname": mock_exasol_connection.schema,
         "schema": "my_schema",
         "threads": 1,
@@ -146,15 +140,15 @@
         "password": "my_password_override",
         "schema": "my_schema",
         "dbname": "my_db_override",
         "threads": 1,
         "protocol_version": "2",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_exasol_connection.conn_type,
         "dsn": "my_dsn_override",
         "user": "my_user_override",
         "password": "{{ env_var('COSMOS_CONN_EXASOL_PASSWORD') }}",
         "dbname": "my_db_override",
         "schema": "my_schema",
         "threads": 1,
@@ -168,15 +162,15 @@
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_exasol_connection.conn_id,
         profile_args={"schema": "my_schema", "threads": 1},
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_EXASOL_PASSWORD": mock_exasol_connection.password,
     }
 
 
 def test_dsn_formatting() -> None:
     """
     Tests that the DSN gets set correctly when a user specifies a port.
@@ -187,42 +181,36 @@
         conn_type="exasol",
         host="my_host:1000",
         login="my_user",
         password="my_password",
         schema="my_database",
     )
 
-    profile_mapping = ExasolUserPasswordProfileMapping(
-        conn, {"schema": "my_schema", "threads": 1}
-    )
+    profile_mapping = ExasolUserPasswordProfileMapping(conn, {"schema": "my_schema", "threads": 1})
     assert profile_mapping.dsn == "my_host:1000"
 
     # next, test with a host that doesn't include a port
     conn = Connection(
         conn_id="my_exasol_connection",
         conn_type="exasol",
         host="my_host",
         login="my_user",
         password="my_password",
         schema="my_database",
     )
 
-    profile_mapping = ExasolUserPasswordProfileMapping(
-        conn, {"schema": "my_schema", "threads": 1}
-    )
+    profile_mapping = ExasolUserPasswordProfileMapping(conn, {"schema": "my_schema", "threads": 1})
     assert profile_mapping.dsn == "my_host:8563"  # should default to 8563
 
     # lastly, test with a port override
     conn = Connection(
         conn_id="my_exasol_connection",
         conn_type="exasol",
         host="my_host",
         login="my_user",
         password="my_password",
         port=1000,  # different than the default
         schema="my_database",
     )
 
-    profile_mapping = ExasolUserPasswordProfileMapping(
-        conn, {"schema": "my_schema", "threads": 1}
-    )
+    profile_mapping = ExasolUserPasswordProfileMapping(conn, {"schema": "my_schema", "threads": 1})
     assert profile_mapping.dsn == "my_host:1000"
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         "password": "password",
         "port": "port",
         "dbname": "schema",
         "keepalives_idle": "extra.keepalives_idle",
         "sslmode": "extra.sslmode",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile. The password is stored in an environment variable."
         profile = {
             "type": "postgres",
             "host": self.conn.host,
             "user": self.conn.login,
             "port": self.conn.port or self.default_port,
             "dbname": self.dbname,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,15 @@
     for key in potential_values:
         values = potential_values.copy()
         del values[key]
         conn = Connection(**values)  # type: ignore
 
         print("testing with", values)
 
-        profile_mapping = PostgresUserPasswordProfileMapping(
-            conn, {"schema": "my_schema"}
-        )
+        profile_mapping = PostgresUserPasswordProfileMapping(conn, {"schema": "my_schema"})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = PostgresUserPasswordProfileMapping(conn, {})
     assert not profile_mapping.can_claim_connection()
 
@@ -99,15 +97,15 @@
         mock_postgres_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_postgres_conn.conn_type,
         "host": mock_postgres_conn.host,
         "user": mock_postgres_conn.login,
         "password": "{{ env_var('COSMOS_CONN_POSTGRES_PASSWORD') }}",
         "port": mock_postgres_conn.port,
         "dbname": mock_postgres_conn.schema,
         "schema": "my_schema",
@@ -125,15 +123,15 @@
         profile_args={"schema": "my_schema", "dbname": "my_db_override"},
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
         "dbname": "my_db_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_postgres_conn.conn_type,
         "host": mock_postgres_conn.host,
         "user": mock_postgres_conn.login,
         "password": "{{ env_var('COSMOS_CONN_POSTGRES_PASSWORD') }}",
         "port": mock_postgres_conn.port,
         "dbname": "my_db_override",
         "schema": "my_schema",
@@ -146,10 +144,10 @@
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_postgres_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_POSTGRES_PASSWORD": mock_postgres_conn.password,
     }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         "port": "port",
         "dbname": "schema",
         "timeout": "extra.timeout",
         "sslmode": "extra.sslmode",
         "region": "extra.region",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile = {
             "type": "redshift",
             "host": self.host,
             "user": self.user,
             "password": self.get_env_var_format("password"),
             "port": self.port or self.default_port,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         values = potential_values.copy()
         del values[key]
         conn = Connection(**values)  # type: ignore
 
         print("testing with", values)
 
         # should raise an InvalidMappingException
-        profile_mapping = RedshiftUserPasswordProfileMapping(
-            conn, {"schema": "my_schema"}
-        )
+        profile_mapping = RedshiftUserPasswordProfileMapping(conn, {"schema": "my_schema"})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = RedshiftUserPasswordProfileMapping(conn, {})
     assert not profile_mapping.can_claim_connection()
 
@@ -98,15 +96,15 @@
         mock_redshift_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_redshift_conn.conn_type,
         "host": mock_redshift_conn.host,
         "user": mock_redshift_conn.login,
         "password": "{{ env_var('COSMOS_CONN_REDSHIFT_PASSWORD') }}",
         "port": mock_redshift_conn.port,
         "dbname": mock_redshift_conn.schema,
         "schema": "my_schema",
@@ -124,15 +122,15 @@
         profile_args={"schema": "my_schema", "dbname": "my_db_override"},
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
         "dbname": "my_db_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_redshift_conn.conn_type,
         "host": mock_redshift_conn.host,
         "user": mock_redshift_conn.login,
         "password": "{{ env_var('COSMOS_CONN_REDSHIFT_PASSWORD') }}",
         "port": mock_redshift_conn.port,
         "dbname": "my_db_override",
         "schema": "my_schema",
@@ -145,10 +143,10 @@
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_redshift_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_REDSHIFT_PASSWORD": mock_redshift_conn.password,
     }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,38 +36,34 @@
         "password": "password",
         "database": "extra.database",
         "warehouse": "extra.warehouse",
         "schema": "schema",
         "role": "extra.role",
     }
 
-    def __init__(
-        self, conn: Connection, profile_args: dict[str, Any | None] | None = None
-    ) -> None:
+    def __init__(self, conn: Connection, profile_args: dict[str, Any | None] | None = None) -> None:
         """
         Snowflake can be odd because the fields used to be stored with keys in the format
         'extra__snowflake__account', but now are stored as 'account'.
 
         This standardizes the keys to be 'account', 'database', etc.
         """
         conn_dejson = conn.extra_dejson
 
         if conn_dejson.get("extra__snowflake__account"):
-            conn_dejson = {
-                key.replace("extra__snowflake__", ""): value
-                for key, value in conn_dejson.items()
-            }
+            conn_dejson = {key.replace("extra__snowflake__", ""): value for key, value in conn_dejson.items()}
 
         conn.extra = json.dumps(conn_dejson)
 
         self.conn = conn
         self.profile_args = profile_args or {}
         super().__init__(conn, profile_args)
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile_vars = {
             "type": "snowflake",
             "account": self.account,
             "user": self.user,
             "schema": self.schema,
             "database": self.database,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     """
     Tests that the profile values get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_snowflake_conn.conn_id,
     )
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_snowflake_conn.conn_type,
         "user": mock_snowflake_conn.login,
         "password": "{{ env_var('COSMOS_CONN_SNOWFLAKE_PASSWORD') }}",
         "schema": mock_snowflake_conn.schema,
         "account": mock_snowflake_conn.extra_dejson.get("account"),
         "database": mock_snowflake_conn.extra_dejson.get("database"),
         "warehouse": mock_snowflake_conn.extra_dejson.get("warehouse"),
@@ -134,15 +134,15 @@
         mock_snowflake_conn.conn_id,
         profile_args={"database": "my_db_override"},
     )
     assert profile_mapping.profile_args == {
         "database": "my_db_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": mock_snowflake_conn.conn_type,
         "user": mock_snowflake_conn.login,
         "password": "{{ env_var('COSMOS_CONN_SNOWFLAKE_PASSWORD') }}",
         "schema": mock_snowflake_conn.schema,
         "account": mock_snowflake_conn.extra_dejson.get("account"),
         "database": "my_db_override",
         "warehouse": mock_snowflake_conn.extra_dejson.get("warehouse"),
@@ -154,15 +154,15 @@
 ) -> None:
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_snowflake_conn.conn_id,
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_SNOWFLAKE_PASSWORD": mock_snowflake_conn.password,
     }
 
 
 def test_old_snowflake_format() -> None:
     """
     Tests that the old format still works.
@@ -179,15 +179,15 @@
                 "extra__snowflake__database": "my_database",
                 "extra__snowflake__warehouse": "my_warehouse",
             }
         ),
     )
 
     profile_mapping = SnowflakeUserPasswordProfileMapping(conn)
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": conn.conn_type,
         "user": conn.login,
         "password": "{{ env_var('COSMOS_CONN_SNOWFLAKE_PASSWORD') }}",
         "schema": conn.schema,
         "account": conn.extra_dejson.get("account"),
         "database": conn.extra_dejson.get("database"),
         "warehouse": conn.extra_dejson.get("warehouse"),
@@ -211,15 +211,15 @@
                 "database": "my_database",
                 "warehouse": "my_warehouse",
             }
         ),
     )
 
     profile_mapping = SnowflakeUserPasswordProfileMapping(conn)
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": conn.conn_type,
         "user": conn.login,
         "password": "{{ env_var('COSMOS_CONN_SNOWFLAKE_PASSWORD') }}",
         "schema": conn.schema,
         "account": f"{conn.extra_dejson.get('account')}.{conn.extra_dejson.get('region')}",
         "database": conn.extra_dejson.get("database"),
         "warehouse": conn.extra_dejson.get("warehouse"),
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/thrift.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/thrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         "host",
     ]
 
     airflow_param_mapping = {
         "host": "host",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         """
         Return a dbt Spark profile based on the Airflow Spark connection.
         """
         profile_vars = {
             "type": "spark",
             "method": "thrift",
             "schema": self.schema,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         mock_spark_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "spark",
         "method": "thrift",
         "schema": "my_schema",
         "host": "my_host",
     }
 
 
@@ -107,15 +107,15 @@
     )
     assert profile_mapping.profile_args == {
         "schema": "my_schema",
         "host": "my_host_override",
         "user": "my_user",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "spark",
         "method": "thrift",
         "schema": "my_schema",
         "host": "my_host_override",
         "user": "my_user",
     }
 
@@ -126,8 +126,8 @@
     """
     Tests that the environment variables get set correctly.
     """
     profile_mapping = get_profile_mapping(
         mock_spark_conn.conn_id,
         profile_args={"schema": "my_schema"},
     )
-    assert profile_mapping.get_env_vars() == {}
+    assert profile_mapping.env_vars == {}
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/base.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
     airflow_param_mapping = {
         "host": "host",
         "port": "port",
         "session_properties": "extra.session_properties",
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile_vars = {
             "type": "trino",
             "host": self.host,
             "port": self.port,
             "database": self.database,
             "schema": self.schema,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/certificate.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/certificate.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 
     airflow_param_mapping = {
         "client_certificate": "extra.certs__client_cert_path",
         "client_private_key": "extra.certs__client_key_path",
         **TrinoBaseProfileMapping.airflow_param_mapping,
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile."
-        common_profile_vars = super().get_profile()
+        common_profile_vars = super().profile
         profile_vars = {
             **common_profile_vars,
             "method": "certificate",
             "client_certificate": self.client_certificate,
             "client_private_key": self.client_private_key,
             **self.profile_args,
         }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/jwt.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/jwt.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         "jwt_token",
     ]
     airflow_param_mapping = {
         "jwt_token": "extra.jwt__token",
         **TrinoBaseProfileMapping.airflow_param_mapping,
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         "Gets profile."
-        common_profile_vars = super().get_profile()
+        common_profile_vars = super().profile
 
         # need to remove jwt from profile_args because it will be set as an environment variable
         profile_args = self.profile_args.copy()
         profile_args.pop("jwt", None)
 
         profile_vars = {
             **common_profile_vars,
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/ldap.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,20 @@
     ]
     airflow_param_mapping = {
         "user": "login",
         "password": "password",
         **TrinoBaseProfileMapping.airflow_param_mapping,
     }
 
-    def get_profile(self) -> dict[str, Any | None]:
+    @property
+    def profile(self) -> dict[str, Any | None]:
         """
         Returns a dbt Trino profile based on the Airflow Trino connection.
         """
-        common_profile_vars = super().get_profile()
+        common_profile_vars = super().profile
         profile_vars = {
             **common_profile_vars,
             "method": "ldap",
             "user": self.user,
             "password": self.get_env_var_format("password"),
             **self.profile_args,
         }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         },
     )
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host",
         "port": 8080,
         "session_properties": {"my_property": "my_value"},
     }
@@ -67,15 +67,15 @@
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host_override",
         "session_properties": {"my_property": "my_value_override"},
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host_override",
         "port": 8080,
         "session_properties": {"my_property": "my_value_override"},
     }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,15 @@
     for key in potential_values:
         values = potential_values.copy()
         del values[key]
         conn = Connection(**values)  # type: ignore
 
         print("testing with", values)
 
-        profile_mapping = TrinoCertificateProfileMapping(
-            conn, {"database": "my_database", "schema": "my_schema"}
-        )
+        profile_mapping = TrinoCertificateProfileMapping(conn, {"database": "my_database", "schema": "my_schema"})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = TrinoCertificateProfileMapping(
         conn,
         {
@@ -134,15 +132,15 @@
         },
     )
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "method": "certificate",
         "host": "my_host",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
         "client_certificate": "/path/to/client_cert",
@@ -168,15 +166,15 @@
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host_override",
         "client_private_key": "my_client_private_key_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "method": "certificate",
         "host": "my_host_override",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
         "client_certificate": "/path/to/client_cert",
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,15 @@
     for key in potential_values:
         values = potential_values.copy()
         del values[key]
         conn = Connection(**values)  # type: ignore
 
         print("testing with", values)
 
-        profile_mapping = TrinoJWTProfileMapping(
-            conn, {"database": "my_database", "schema": "my_schema"}
-        )
+        profile_mapping = TrinoJWTProfileMapping(conn, {"database": "my_database", "schema": "my_schema"})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = TrinoJWTProfileMapping(
         conn,
         {
@@ -129,15 +127,15 @@
         },
     )
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "method": "jwt",
         "host": "my_host",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
         "jwt_token": "{{ env_var('COSMOS_CONN_TRINO_JWT_TOKEN') }}",
@@ -162,15 +160,15 @@
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host_override",
         "jwt_token": "my_jwt_token_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "method": "jwt",
         "host": "my_host_override",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
         "jwt_token": "{{ env_var('COSMOS_CONN_TRINO_JWT_TOKEN') }}",
@@ -186,10 +184,10 @@
     profile_mapping = get_profile_mapping(
         mock_trino_conn.conn_id,
         profile_args={
             "database": "my_database",
             "schema": "my_schema",
         },
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_TRINO_JWT_TOKEN": "my_jwt_token",
     }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,15 @@
     for key in potential_values:
         values = potential_values.copy()
         del values[key]
         conn = Connection(**values)  # type: ignore
 
         print("testing with", values)
 
-        profile_mapping = TrinoLDAPProfileMapping(
-            conn, {"database": "my_database", "schema": "my_schema"}
-        )
+        profile_mapping = TrinoLDAPProfileMapping(conn, {"database": "my_database", "schema": "my_schema"})
         assert not profile_mapping.can_claim_connection()
 
     # also test when there's no schema
     conn = Connection(**potential_values)  # type: ignore
     profile_mapping = TrinoLDAPProfileMapping(
         conn,
         {
@@ -123,15 +121,15 @@
         },
     )
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "method": "ldap",
         "host": "my_host",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
         "user": "my_login",
@@ -157,15 +155,15 @@
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host_override",
         "user": "my_user_override",
     }
 
-    assert profile_mapping.get_profile() == {
+    assert profile_mapping.profile == {
         "type": "trino",
         "method": "ldap",
         "host": "my_host_override",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
         "user": "my_user_override",
@@ -182,10 +180,10 @@
     profile_mapping = get_profile_mapping(
         mock_trino_conn.conn_id,
         profile_args={
             "database": "my_database",
             "schema": "my_schema",
         },
     )
-    assert profile_mapping.get_env_vars() == {
+    assert profile_mapping.env_vars == {
         "COSMOS_CONN_TRINO_PASSWORD": "my_password",
     }
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 import signal
 from collections import namedtuple
 from subprocess import PIPE, STDOUT, Popen
 from tempfile import TemporaryDirectory, gettempdir
 
 from airflow.hooks.base import BaseHook
 
-FullOutputSubprocessResult = namedtuple(
-    "FullOutputSubprocessResult", ["exit_code", "output", "full_output"]
-)
+FullOutputSubprocessResult = namedtuple("FullOutputSubprocessResult", ["exit_code", "output", "full_output"])
 
 
 class FullOutputSubprocessHook(BaseHook):
     """Hook for running processes with the ``subprocess`` module."""
 
     def __init__(self) -> None:
         self.sub_process: Popen[bytes] | None = None
@@ -79,30 +77,24 @@
             self.log.info("Output:")
             line = ""
 
             if self.sub_process is None:
                 raise RuntimeError("The subprocess should be created here and is None!")
             if self.sub_process.stdout is not None:
                 for raw_line in iter(self.sub_process.stdout.readline, b""):
-                    line = raw_line.decode(
-                        output_encoding, errors="backslashreplace"
-                    ).rstrip()
+                    line = raw_line.decode(output_encoding, errors="backslashreplace").rstrip()
                     # storing the warn & error lines to be used later
                     log_lines.append(line)
                     self.log.info("%s", line)
 
             self.sub_process.wait()
 
-            self.log.info(
-                "Command exited with return code %s", self.sub_process.returncode
-            )
+            self.log.info("Command exited with return code %s", self.sub_process.returncode)
             return_code: int = self.sub_process.returncode
 
-        return FullOutputSubprocessResult(
-            exit_code=return_code, output=line, full_output=log_lines
-        )
+        return FullOutputSubprocessResult(exit_code=return_code, output=line, full_output=log_lines)
 
     def send_sigterm(self):
         """Sends SIGTERM signal to ``self.sub_process`` if one exists."""
         self.log.info("Sending SIGTERM signal to process group")
         if self.sub_process and hasattr(self.sub_process, "pid"):
             os.killpg(os.getpgid(self.sub_process.pid), signal.SIGTERM)
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/warn_parsing.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/warn_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Tuple
 
 from airflow.hooks.subprocess import SubprocessResult
 
 
 def parse_output(result: SubprocessResult, keyword: str) -> int:
     """
-    Parses the DBT test output message and returns the number of errors or warnings.
+    Parses the dbt test output message and returns the number of errors or warnings.
 
     :param result: String containing the output to be parsed.
     :param keyword: String representing the keyword to search for in the output (WARN, ERROR).
     :return: An integer value associated with the keyword, or 0 if parsing fails.
 
     Usage:
     -----
@@ -31,18 +31,18 @@
     return num
 
 
 def extract_log_issues(log_list: List[str]) -> Tuple[List[str], List[str]]:
     """
     Extracts warning messages from the log list and returns them as a formatted string.
 
-    This function searches for warning messages in DBT test. It reverses the log list for performance
+    This function searches for warning messages in dbt test. It reverses the log list for performance
     improvement. It extracts and formats the relevant information and appends it to a list of warnings.
 
-    :param log_list: List of strings, where each string is a log line from DBT test.
+    :param log_list: List of strings, where each string is a log line from dbt test.
     :return: two lists of strings, the first one containing the test names and the second one
         containing the test results.
     """
 
     def clean_line(line: str) -> str:
         return line.replace("\x1b[33m", "").replace("\x1b[0m", "").strip()
 
@@ -57,15 +57,13 @@
         if "Finished running" in cleaned_line:
             # No need to keep checking the log lines once all warnings are found
             break
 
         if "Warning in test" in cleaned_line:
             test_name = pattern1.sub(r"\1", cleaned_line)
             # test_result is on the next line by default
-            test_result = pattern2.sub(
-                r"\1", clean_line(log_list[-(line_index + 1) + 1])
-            )
+            test_result = pattern2.sub(r"\1", clean_line(log_list[-(line_index + 1) + 1]))
 
             test_names.append(test_name)
             test_results.append(test_result)
 
     return test_names, test_results
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,12 @@
     [
         (
             "my_connection",
             "jaffle_shop",
             "orders",
             Dataset("DBT://MY_CONNECTION/JAFFLE_SHOP/ORDERS"),
         ),
-        pytest.param(
-            "my_connection", "jafflé_shop", "orders", None, marks=pytest.mark.xfail
-        ),
+        pytest.param("my_connection", "jafflé_shop", "orders", None, marks=pytest.mark.xfail),
     ],
 )
-def test_get_dbt_dataset(
-    connection_id: str, project_name: str, model_name: str, expected_dataset: Dataset
-) -> None:
+def test_get_dbt_dataset(connection_id: str, project_name: str, model_name: str, expected_dataset: Dataset) -> None:
     assert get_dbt_dataset(connection_id, project_name, model_name) == expected_dataset
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import yaml  # type: ignore
 
 logger = logging.getLogger(__name__)
 
 
 class DbtModelType(Enum):
     """
-    Represents type of DBT unit (model, snapshot, seed)
+    Represents type of dbt unit (model, snapshot, seed)
     """
 
     DBT_MODEL = 1
     DBT_SNAPSHOT = 2
     DBT_SEED = 3
 
 
@@ -71,23 +71,19 @@
 
         for config in properties_configs:
             # identify the config_type and its associated value (i.e. materialized:table)
             config_type, value = config.split(":")
             # if the config_type matches is even in a list of prefixes then
             if config_type in prefixes:
                 # make sure that it's prefix doesn't already exist in the sql configs
-                if not any(
-                    [element.startswith(config_type) for element in sql_configs]
-                ):
+                if not any([element.startswith(config_type) for element in sql_configs]):
                     # if it does let's double-check against each prefix and add it
                     for prefix in prefixes:
                         # if the actual config doesn't exist in the sql_configs then add it
-                        if not any(
-                            [element.startswith(prefix) for element in sql_configs]
-                        ):
+                        if not any([element.startswith(prefix) for element in sql_configs]):
                             sql_configs.add(config)
             else:
                 sql_configs.add(config)
 
         return sql_configs
 
 
@@ -144,21 +140,17 @@
                         config.upstream_models.add(first_arg.value)
 
                 # check if we have a config - this could contain tags
                 if base_node.node.name == "config":
                     # if it is, check if any kwargs are tags
                     for kwarg in base_node.kwargs:
                         for selector in self.config.config_types:
-                            extracted_config = self._extract_config(
-                                kwarg=kwarg, config_name=selector
-                            )
+                            extracted_config = self._extract_config(kwarg=kwarg, config_name=selector)
                             config.config_selectors |= (
-                                set(extracted_config)
-                                if isinstance(extracted_config, (str, List))
-                                else set()
+                                set(extracted_config) if isinstance(extracted_config, (str, List)) else set()
                             )
 
         # set the config and set the parsed file flag to true
         self.config = config
 
     # TODO following needs coverage:
     def _extract_config(self, kwarg, config_name: str):
@@ -172,17 +164,15 @@
                 if isinstance(value, str):
                     value = [f"{config_name}:{value}"]
 
                 return value
 
             except Exception as e:
                 # if we can't convert it to a constant, we can't do anything with it
-                logger.warning(
-                    f"Could not parse {config_name} from config in {self.path}: {e}"
-                )
+                logger.warning(f"Could not parse {config_name} from config in {self.path}: {e}")
                 pass
 
     def __repr__(self) -> str:
         """
         Returns the string representation of the model.
         """
         return f"DbtModel(name='{self.name}', type='{self.type}', path='{self.path}', config={self.config})"
@@ -302,28 +292,20 @@
             config_selectors = []
             for selector in self.models[model_name].config.config_types:
                 config_value = model.get("config", {}).get(selector)
                 if config_value:
                     if isinstance(config_value, str):
                         config_selectors.append(f"{selector}:{config_value}")
                     else:
-                        [
-                            config_selectors.append(f"{selector}:{item}")
-                            for item in config_value
-                            if item
-                        ]
+                        [config_selectors.append(f"{selector}:{item}") for item in config_value if item]
 
             # dbt default ensures "materialized:view" is set for all models if nothing is specified so that it will
             # work in a select/exclude list
             config_types = [
-                selector_name
-                for selector in config_selectors
-                for selector_name in [selector.split(":")[0]]
+                selector_name for selector in config_selectors for selector_name in [selector.split(":")[0]]
             ]
             if "materialized" not in config_types:
                 config_selectors.append("materialized:view")
 
             # then, get the model and merge the configs
             model = self.models[model_name]
-            model.config = model.config + DbtModelConfig(
-                config_selectors=set(config_selectors)
-            )
+            model.config = model.config + DbtModelConfig(config_selectors=set(config_selectors))
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/tests/test_project.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/parser/tests/test_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,40 +90,33 @@
 @pytest.mark.parametrize(
     "input_tags,expected_config_selectors",
     [
         ("some_tag", {"materialized:view", "tags:some_tag"}),
         (["tag1", "tag2"], {"materialized:view", "tags:tag1", "tags:tag2"}),
     ],
 )
-def test_dbtproject__handle_config_file_with_selector(
-    input_tags, expected_config_selectors
-):
+def test_dbtproject__handle_config_file_with_selector(input_tags, expected_config_selectors):
     dbt_project = DbtProject(
         project_name="jaffle_shop",
         dbt_root_path=DBT_PROJECT_PATH,
     )
     assert dbt_project.models["orders"].config.config_selectors == {"materialized:view"}
 
     with NamedTemporaryFile("w") as tmp_fp:
         yaml_data = {"models": [{"name": "orders", "config": {"tags": input_tags}}]}
         yaml.dump(yaml_data, tmp_fp)
         tmp_fp.flush()
 
         sample_config_file_path = Path(tmp_fp.name)
         dbt_project._handle_config_file(sample_config_file_path)
-        assert (
-            dbt_project.models["orders"].config.config_selectors
-            == expected_config_selectors
-        )
+        assert dbt_project.models["orders"].config.config_selectors == expected_config_selectors
 
 
 def test_dbtmodelconfig___repr__():
-    dbt_model = DbtModel(
-        name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH
-    )
+    dbt_model = DbtModel(name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH)
     expected_start = (
         "DbtModel(name='some_name', type='DbtModelType.DBT_MODEL', "
         "path='dev/dags/dbt/jaffle_shop/models/customers.sql', config=DbtModelConfig(config_selectors=set(), "
         "upstream_models={'stg_"
     )
     assert str(dbt_model).startswith(expected_start)
 
@@ -144,52 +137,44 @@
 @dataclass
 class KeywordArg:
     key: str
     value: KeywordArgValue | List
 
 
 def test_dbtmodelconfig_extract_config_non_kwarg():
-    dbt_model = DbtModel(
-        name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH
-    )
+    dbt_model = DbtModel(name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH)
     kwarg = {}
     config_name = "abc"
     computed = dbt_model._extract_config(kwarg, config_name)
     assert computed is None
 
 
 def test_dbtmodelconfig_extract_config_with_kwarg_list_without_as_const(caplog):
-    dbt_model = DbtModel(
-        name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH
-    )
+    dbt_model = DbtModel(name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH)
     kwarg = KeywordArg(key="some_conf", value=[1, 2])
     config_name = "some_conf"
     with caplog.at_level(logging.WARN):
         computed = dbt_model._extract_config(kwarg, config_name)
     assert computed is None
     expected_log = (
         "Could not parse some_conf from config in dev/dags/dbt/jaffle_shop/models/customers.sql: "
         "'list' object has no attribute 'as_const'"
     )
     assert expected_log in caplog.text
 
 
 def test_dbtmodelconfig_extract_config_with_kwarg_list():
-    dbt_model = DbtModel(
-        name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH
-    )
+    dbt_model = DbtModel(name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH)
     kwarg = KeywordArg(key="some_conf", value=KeywordArgValueList([1, 2]))
     config_name = "some_conf"
     computed = dbt_model._extract_config(kwarg, config_name)
     expected = ["some_conf:1", "some_conf:2"]
     assert computed == expected
 
 
 def test_dbtmodelconfig_extract_config_with_kwarg_str():
-    dbt_model = DbtModel(
-        name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH
-    )
+    dbt_model = DbtModel(name="some_name", type=DbtModelType.DBT_MODEL, path=SAMPLE_MODEL_SQL_PATH)
     kwarg = KeywordArg(key="some_conf", value=KeywordArgValueStr("abc"))
     config_name = "some_conf"
     computed = dbt_model._extract_config(kwarg, config_name)
     expected = ["some_conf:abc"]
     assert computed == expected
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_dataset.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_export.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,15 @@
     docker_operators,
 )
 def test_failed_docker_import(operator: str, reset_docker_operators: None) -> None:
     """
     Test that the docker operators are not imported when docker is not installed.
     Should raise a RuntimeError.
     """
-    with mock.patch.dict(
-        sys.modules, {"airflow.providers.docker.operators.docker": None}
-    ):
+    with mock.patch.dict(sys.modules, {"airflow.providers.docker.operators.docker": None}):
         with pytest.raises(RuntimeError):
             from cosmos.providers import dbt
 
             importlib.reload(dbt)
             getattr(dbt, operator)()
 
 
@@ -66,17 +64,15 @@
             del sys.modules[key]
 
 
 @pytest.mark.parametrize(
     "operator",
     kubernetes_operators,
 )
-def test_failed_kubernetes_import(
-    operator: str, reset_kubernetes_operators: None
-) -> None:
+def test_failed_kubernetes_import(operator: str, reset_kubernetes_operators: None) -> None:
     """
     Test that the kubernetes operators are not imported when kubernetes is not installed.
     Should raise a RuntimeError.
     """
     with mock.patch.dict(
         sys.modules,
         {
```

### Comparing `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_render.py` & `astronomer_cosmos-0.7.1/cosmos/providers/dbt/tests/test_render.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 from cosmos.core.graph.entities import Group
 from cosmos.providers.dbt.render import calculate_operator_class, render_project
 
 DBT_PROJECT_PATH = Path(__name__).parent.parent.parent.parent.parent / "dev/dags/dbt/"
 
 
 def test_calculate_operator_class():
-    class_module_import_path = calculate_operator_class(
-        execution_mode="kubernetes", dbt_class="Seed"
-    )
-    assert (
-        class_module_import_path
-        == "cosmos.providers.dbt.core.operators.kubernetes.SeedKubernetesOperator"
-    )
+    class_module_import_path = calculate_operator_class(execution_mode="kubernetes", dbt_class="Seed")
+    assert class_module_import_path == "cosmos.providers.dbt.core.operators.kubernetes.SeedKubernetesOperator"
 
 
 def test_render_project_default():
-    computed = render_project(
-        dbt_project_name="jaffle_shop", dbt_root_path=DBT_PROJECT_PATH
-    )
+    computed = render_project(dbt_project_name="jaffle_shop", dbt_root_path=DBT_PROJECT_PATH)
     assert isinstance(computed, Group)
     assert computed.id == "jaffle_shop"
     assert len(computed.entities) == 8
     entities_ids = [entity.id for entity in computed.entities]
     expected_ids = [
         "customers",
         "orders",
```

### Comparing `astronomer_cosmos-0.7.0rc2/.gitignore` & `astronomer_cosmos-0.7.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -138,9 +138,18 @@
 
 # pycharm
 .DS_Store
 
 # dbt
 logs/
 
-# Airflow connections file
-test-connections.yaml
+# integration tests
+dev/dags/.airflowignore
+
+# Local Airflow standalone
+airflow.cfg
+airflow.db
+standalone_admin_password.txt
+webserver_config.py
+
+# VI
+*.sw[a-z]
```

### Comparing `astronomer_cosmos-0.7.0rc2/LICENSE` & `astronomer_cosmos-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc2/README.rst` & `astronomer_cosmos-0.7.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
 
     with DAG(
         dag_id="extract_dag",
         start_date=datetime(2022, 11, 27),
         schedule="@daily",
     ):
-
         e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
             dbt_project_name="jaffle_shop",
             conn_id="airflow_db",
             profile_args={
                 "schema": "public",
@@ -68,14 +67,17 @@
 
         e1 >> dbt_tg >> e2
 
 This will generate an Airflow Task Group that looks like this:
 
 .. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
 
+Community
+_________
+- Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1vo1rxgc3-EfsbdDzqrV51fddWOc6GOQ>`_ at #airflow-dbt
 
 Changelog
 _________
 
 We follow `Semantic Versioning <https://semver.org/>`_ for releases.
 Check `CHANGELOG.rst <https://github.com/astronomer/astronomer-cosmos/blob/main/CHANGELOG.rst>`_
 for the latest changes.
```

### Comparing `astronomer_cosmos-0.7.0rc2/pyproject.toml` & `astronomer_cosmos-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,18 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "apache-airflow>=2.3.0",
+    "importlib-metadata; python_version < '3.8'",
     "Jinja2>=3.0.0",
     "typing-extensions; python_version < '3.8'",
+    "virtualenv",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
     "dbt-bigquery",
     "dbt-databricks",
     "dbt-exasol",
@@ -83,14 +85,15 @@
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx-autobuild",
     "sphinx-tabs",
     "sphinx-autoapi"
 ]
 tests = [
+    "packaging",
     "pytest>=6.0",
     "pytest-split",
     "pytest-dotenv",
     "requests-mock",
     "pytest-cov",
     "pytest-describe",
     "types-requests",
@@ -147,24 +150,26 @@
     { value = "apache-airflow==2.4", if = ["2.4"] },
     { value = "apache-airflow==2.5", if = ["2.5"] },
     { value = "apache-airflow==2.6", if = ["2.6"] },
 ]
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
-test = "pytest ."
-test-cov = "pytest --cov=cosmos --cov-report=term-missing --cov-report=xml ."
+test = 'pytest -vv --durations=0 . -m "not integration"'
+test-cov = 'pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 . -m "not integration"'
+test-integration = "pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m integration"
 
-######################################
-# PYTEST
-######################################
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
+minversion = "6.0"
+markers = [
+    "integration"
+]
 
 ######################################
 # DOCS
 ######################################
 
 [tool.hatch.envs.docs]
 dependencies = [
@@ -178,14 +183,17 @@
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs docs/_build"
 serve = "sphinx-autobuild docs docs/_build"
 
 ######################################
 # THIRD PARTY TOOLS
 ######################################
+[tool.black]
+line-length = 120
+target-version = ['py37', 'py38', 'py39', 'py310']
 
 [tool.isort]
 profile = "black"
 known_third_party = ["airflow", "jinja2"]
 
 [tool.mypy]
 strict = true
```

### Comparing `astronomer_cosmos-0.7.0rc2/PKG-INFO` & `astronomer_cosmos-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.7.0rc2
+Version: 0.7.1
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -19,16 +19,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: apache-airflow>=2.3.0
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: typing-extensions; python_version < '3.8'
+Requires-Dist: virtualenv
 Provides-Extra: all
 Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
 Provides-Extra: dbt-all
 Requires-Dist: astronomer-cosmos[dbt-openlineage]; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
 Requires-Dist: dbt-databricks; extra == 'dbt-all'
 Requires-Dist: dbt-exasol; extra == 'dbt-all'
@@ -61,14 +63,15 @@
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-tabs; extra == 'docs'
 Provides-Extra: kubernetes
 Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
 Provides-Extra: tests
 Requires-Dist: mypy; extra == 'tests'
+Requires-Dist: packaging; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
 Requires-Dist: pytest-dotenv; extra == 'tests'
 Requires-Dist: pytest-split; extra == 'tests'
 Requires-Dist: pytest>=6.0; extra == 'tests'
 Requires-Dist: requests-mock; extra == 'tests'
 Requires-Dist: sqlalchemy-stubs; extra == 'tests'
@@ -126,15 +129,14 @@
 
 
     with DAG(
         dag_id="extract_dag",
         start_date=datetime(2022, 11, 27),
         schedule="@daily",
     ):
-
         e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
             dbt_project_name="jaffle_shop",
             conn_id="airflow_db",
             profile_args={
                 "schema": "public",
@@ -145,14 +147,17 @@
 
         e1 >> dbt_tg >> e2
 
 This will generate an Airflow Task Group that looks like this:
 
 .. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
 
+Community
+_________
+- Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1vo1rxgc3-EfsbdDzqrV51fddWOc6GOQ>`_ at #airflow-dbt
 
 Changelog
 _________
 
 We follow `Semantic Versioning <https://semver.org/>`_ for releases.
 Check `CHANGELOG.rst <https://github.com/astronomer/astronomer-cosmos/blob/main/CHANGELOG.rst>`_
 for the latest changes.
```

