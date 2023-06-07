# Comparing `tmp/SQLAlchemy-Continuum-1.3.7.tar.gz` & `tmp/SQLAlchemy-Continuum-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SQLAlchemy-Continuum-1.3.7.tar", last modified: Sun Jan 13 14:25:14 2019, max compression
+gzip compressed data, was "dist/SQLAlchemy-Continuum-1.3.9.tar", last modified: Tue Mar 19 13:32:22 2019, max compression
```

## Comparing `SQLAlchemy-Continuum-1.3.7.tar` & `SQLAlchemy-Continuum-1.3.9.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/
--rw-r--r--   0 konsta     (501) staff       (20)    16256 2019-01-13 14:09:23.000000 SQLAlchemy-Continuum-1.3.7/CHANGES.rst
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/docs/
--rw-r--r--   0 konsta     (501) staff       (20)    12292 2014-09-02 12:34:50.000000 SQLAlchemy-Continuum-1.3.7/docs/.DS_Store
--rw-r--r--   0 konsta     (501) staff       (20)      544 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/docs/alembic.rst
--rw-r--r--   0 konsta     (501) staff       (20)      757 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/docs/api.rst
--rw-r--r--   0 konsta     (501) staff       (20)     8420 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/docs/conf.py
--rw-r--r--   0 konsta     (501) staff       (20)     5375 2014-12-09 15:05:34.000000 SQLAlchemy-Continuum-1.3.7/docs/configuration.rst
--rw-r--r--   0 konsta     (501) staff       (20)      297 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.7/docs/index.rst
--rw-r--r--   0 konsta     (501) staff       (20)     3377 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.7/docs/intro.rst
--rw-r--r--   0 konsta     (501) staff       (20)       41 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/docs/license.rst
--rw-r--r--   0 konsta     (501) staff       (20)     6729 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/docs/make.bat
--rw-r--r--   0 konsta     (501) staff       (20)     6818 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/docs/Makefile
--rw-r--r--   0 konsta     (501) staff       (20)     1068 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.7/docs/native_versioning.rst
--rw-r--r--   0 konsta     (501) staff       (20)      801 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.7/docs/plugins.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1714 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/docs/queries.rst
--rw-r--r--   0 konsta     (501) staff       (20)     2209 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/docs/revert.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1898 2014-04-24 08:21:06.000000 SQLAlchemy-Continuum-1.3.7/docs/schema.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1877 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.7/docs/transactions.rst
--rw-r--r--   0 konsta     (501) staff       (20)      892 2014-08-27 09:58:16.000000 SQLAlchemy-Continuum-1.3.7/docs/utilities.rst
--rw-r--r--   0 konsta     (501) staff       (20)     6020 2014-04-24 09:58:30.000000 SQLAlchemy-Continuum-1.3.7/docs/version_objects.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1437 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/LICENSE
--rw-r--r--   0 konsta     (501) staff       (20)      193 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.7/MANIFEST.in
--rw-r--r--   0 konsta     (501) staff       (20)     1079 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)     2977 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.7/README.rst
--rw-r--r--   0 konsta     (501) staff       (20)       38 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/setup.cfg
--rw-r--r--   0 konsta     (501) staff       (20)     2413 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.7/setup.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/
--rw-r--r--   0 konsta     (501) staff       (20)     3258 2019-01-13 14:09:28.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     6758 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/builder.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/dialects/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-08-14 14:08:11.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/dialects/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)    15324 2014-12-06 10:19:14.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/dialects/postgresql.py
--rw-r--r--   0 konsta     (501) staff       (20)      152 2014-04-29 12:36:20.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/exc.py
--rw-r--r--   0 konsta     (501) staff       (20)      975 2015-07-24 06:47:20.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/expression_reflector.py
--rw-r--r--   0 konsta     (501) staff       (20)      407 2014-09-04 12:34:32.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/factory.py
--rw-r--r--   0 konsta     (501) staff       (20)     5799 2014-07-10 11:45:57.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/fetcher.py
--rw-r--r--   0 konsta     (501) staff       (20)    18570 2018-07-30 12:47:07.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/manager.py
--rw-r--r--   0 konsta     (501) staff       (20)     9348 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/model_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     2840 2014-07-16 13:16:55.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/operation.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/
--rw-r--r--   0 konsta     (501) staff       (20)      322 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)    10395 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/activity.py
--rw-r--r--   0 konsta     (501) staff       (20)     1866 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/base.py
--rw-r--r--   0 konsta     (501) staff       (20)     2188 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/flask.py
--rw-r--r--   0 konsta     (501) staff       (20)      987 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/null_delete.py
--rw-r--r--   0 konsta     (501) staff       (20)     2487 2014-08-19 08:18:11.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/property_mod_tracker.py
--rw-r--r--   0 konsta     (501) staff       (20)     3193 2014-12-30 15:57:18.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/transaction_changes.py
--rw-r--r--   0 konsta     (501) staff       (20)     3172 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/transaction_meta.py
--rw-r--r--   0 konsta     (501) staff       (20)    12506 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/relationship_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     4464 2015-09-27 08:54:29.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/reverter.py
--rw-r--r--   0 konsta     (501) staff       (20)     5593 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/schema.py
--rw-r--r--   0 konsta     (501) staff       (20)     4752 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/table_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     5872 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/transaction.py
--rw-r--r--   0 konsta     (501) staff       (20)    11266 2015-07-24 07:20:58.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/unit_of_work.py
--rw-r--r--   0 konsta     (501) staff       (20)    11830 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/utils.py
--rw-r--r--   0 konsta     (501) staff       (20)     2095 2017-11-05 16:02:23.000000 SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/version.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/
--rw-r--r--   0 konsta     (501) staff       (20)        1 2019-01-13 14:25:13.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/dependency_links.txt
--rw-r--r--   0 konsta     (501) staff       (20)        1 2014-02-10 07:59:41.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/not-zip-safe
--rw-r--r--   0 konsta     (501) staff       (20)     1079 2019-01-13 14:25:13.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)      411 2019-01-13 14:25:13.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/requires.txt
--rw-r--r--   0 konsta     (501) staff       (20)     4049 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/SOURCES.txt
--rw-r--r--   0 konsta     (501) staff       (20)       21 2019-01-13 14:25:13.000000 SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/top_level.txt
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/
--rw-r--r--   0 konsta     (501) staff       (20)     6431 2017-01-30 16:37:55.000000 SQLAlchemy-Continuum-1.3.7/tests/__init__.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/builders/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/builders/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)      259 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/builders/test_model_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     1146 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/builders/test_relationship_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     3550 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.7/tests/builders/test_table_builder.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/dialects/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.7/tests/dialects/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2045 2014-10-13 19:41:57.000000 SQLAlchemy-Continuum-1.3.7/tests/dialects/test_triggers.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)      940 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_common_base_class.py
--rw-r--r--   0 konsta     (501) staff       (20)     3272 2014-06-16 09:20:44.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_concrete_inheritance.py
--rw-r--r--   0 konsta     (501) staff       (20)     7059 2015-09-27 08:36:34.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_join_table_inheritance.py
--rw-r--r--   0 konsta     (501) staff       (20)     1646 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_multi_level_inheritance.py
--rw-r--r--   0 konsta     (501) staff       (20)     2980 2014-08-18 13:30:03.000000 SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_single_table_inheritance.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     5680 2014-08-14 13:56:49.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_activity.py
--rw-r--r--   0 konsta     (501) staff       (20)     8766 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_flask.py
--rw-r--r--   0 konsta     (501) staff       (20)     1000 2014-08-14 13:56:49.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_null_delete.py
--rw-r--r--   0 konsta     (501) staff       (20)     1070 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_plugin_collection.py
--rw-r--r--   0 konsta     (501) staff       (20)     5881 2014-08-26 11:51:22.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_property_mod_tracker.py
--rw-r--r--   0 konsta     (501) staff       (20)     2473 2014-12-30 16:00:18.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_transaction_changes.py
--rw-r--r--   0 konsta     (501) staff       (20)     1253 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/plugins/test_transaction_meta.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2048 2018-06-03 11:24:04.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_association_table_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     2035 2015-07-24 07:48:10.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_custom_condition_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     3029 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_dynamic_relationships.py
--rw-r--r--   0 konsta     (501) staff       (20)    14534 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_many_to_many_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     3291 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_non_versioned_classes.py
--rw-r--r--   0 konsta     (501) staff       (20)     9110 2014-12-28 13:06:15.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_one_to_many_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     2882 2014-07-10 11:45:57.000000 SQLAlchemy-Continuum-1.3.7/tests/relationships/test_one_to_one_relations.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/revert/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/revert/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2112 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/revert/test_deep_relationships.py
--rw-r--r--   0 konsta     (501) staff       (20)     2806 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/revert/test_many_to_many_relationships.py
--rw-r--r--   0 konsta     (501) staff       (20)     1817 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/revert/test_one_to_one_relationship.py
--rw-r--r--   0 konsta     (501) staff       (20)     2127 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/revert/test_one_to_one_with_secondary_table.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/schema/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/schema/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2129 2014-10-01 13:34:49.000000 SQLAlchemy-Continuum-1.3.7/tests/schema/test_update_end_transaction_id.py
--rw-r--r--   0 konsta     (501) staff       (20)     2946 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/schema/test_update_property_mod_flags.py
--rw-r--r--   0 konsta     (501) staff       (20)     8343 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.7/tests/test_accessors.py
--rw-r--r--   0 konsta     (501) staff       (20)     3470 2017-11-05 16:02:23.000000 SQLAlchemy-Continuum-1.3.7/tests/test_changeset.py
--rw-r--r--   0 konsta     (501) staff       (20)     1935 2014-04-21 09:09:53.000000 SQLAlchemy-Continuum-1.3.7/tests/test_column_aliases.py
--rw-r--r--   0 konsta     (501) staff       (20)     3661 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.7/tests/test_column_inclusion_and_exclusion.py
--rw-r--r--   0 konsta     (501) staff       (20)     2456 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/test_composite_primary_key.py
--rw-r--r--   0 konsta     (501) staff       (20)     3713 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.7/tests/test_configuration.py
--rw-r--r--   0 konsta     (501) staff       (20)     2057 2014-10-01 09:31:26.000000 SQLAlchemy-Continuum-1.3.7/tests/test_custom_schema.py
--rw-r--r--   0 konsta     (501) staff       (20)     1114 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.7/tests/test_custom_version_base_class.py
--rw-r--r--   0 konsta     (501) staff       (20)     1356 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.7/tests/test_delete.py
--rw-r--r--   0 konsta     (501) staff       (20)     1068 2014-07-16 13:11:49.000000 SQLAlchemy-Continuum-1.3.7/tests/test_exotic_listener_chaining.py
--rw-r--r--   0 konsta     (501) staff       (20)     2509 2015-07-24 07:16:05.000000 SQLAlchemy-Continuum-1.3.7/tests/test_exotic_operation_combos.py
--rw-r--r--   0 konsta     (501) staff       (20)     2602 2017-01-30 17:14:23.000000 SQLAlchemy-Continuum-1.3.7/tests/test_i18n.py
--rw-r--r--   0 konsta     (501) staff       (20)     2647 2015-07-24 10:14:05.000000 SQLAlchemy-Continuum-1.3.7/tests/test_insert.py
--rw-r--r--   0 konsta     (501) staff       (20)     2336 2014-04-22 15:07:31.000000 SQLAlchemy-Continuum-1.3.7/tests/test_mapper_args.py
--rw-r--r--   0 konsta     (501) staff       (20)      976 2014-10-01 13:34:49.000000 SQLAlchemy-Continuum-1.3.7/tests/test_raw_sql.py
--rw-r--r--   0 konsta     (501) staff       (20)     6000 2015-09-27 08:54:29.000000 SQLAlchemy-Continuum-1.3.7/tests/test_revert.py
--rw-r--r--   0 konsta     (501) staff       (20)     1540 2014-09-02 06:42:43.000000 SQLAlchemy-Continuum-1.3.7/tests/test_savepoints.py
--rw-r--r--   0 konsta     (501) staff       (20)     2170 2018-07-30 12:47:07.000000 SQLAlchemy-Continuum-1.3.7/tests/test_sessions.py
--rw-r--r--   0 konsta     (501) staff       (20)     2654 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.7/tests/test_transaction.py
--rw-r--r--   0 konsta     (501) staff       (20)     3414 2015-07-24 06:49:15.000000 SQLAlchemy-Continuum-1.3.7/tests/test_update.py
--rw-r--r--   0 konsta     (501) staff       (20)     1707 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.7/tests/test_vacuum.py
--rw-r--r--   0 konsta     (501) staff       (20)     3640 2014-09-02 06:44:39.000000 SQLAlchemy-Continuum-1.3.7/tests/test_validity_strategy.py
--rw-r--r--   0 konsta     (501) staff       (20)      669 2014-04-09 15:04:22.000000 SQLAlchemy-Continuum-1.3.7/tests/test_versions.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-01-13 14:25:14.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-25 11:06:55.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)      869 2014-04-25 11:08:20.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_changeset.py
--rw-r--r--   0 konsta     (501) staff       (20)     1079 2014-08-27 09:54:26.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_count_versions.py
--rw-r--r--   0 konsta     (501) staff       (20)      877 2014-12-06 08:57:22.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_is_modified.py
--rw-r--r--   0 konsta     (501) staff       (20)      440 2014-04-25 11:12:06.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_parent_class.py
--rw-r--r--   0 konsta     (501) staff       (20)      477 2014-04-25 11:22:10.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_transaction_class.py
--rw-r--r--   0 konsta     (501) staff       (20)      824 2014-04-25 11:21:06.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_tx_column_name.py
--rw-r--r--   0 konsta     (501) staff       (20)      887 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.7/tests/utils/test_version_class.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/
+-rw-r--r--   0 konsta     (501) staff       (20)    16466 2019-03-19 13:10:38.000000 SQLAlchemy-Continuum-1.3.9/CHANGES.rst
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/docs/
+-rw-r--r--   0 konsta     (501) staff       (20)    12292 2014-09-02 12:34:50.000000 SQLAlchemy-Continuum-1.3.9/docs/.DS_Store
+-rw-r--r--   0 konsta     (501) staff       (20)      544 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/alembic.rst
+-rw-r--r--   0 konsta     (501) staff       (20)      757 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/docs/api.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     8420 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/conf.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5375 2014-12-09 15:05:34.000000 SQLAlchemy-Continuum-1.3.9/docs/configuration.rst
+-rw-r--r--   0 konsta     (501) staff       (20)      297 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/docs/index.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     3377 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.9/docs/intro.rst
+-rw-r--r--   0 konsta     (501) staff       (20)       41 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/license.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     6729 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/make.bat
+-rw-r--r--   0 konsta     (501) staff       (20)     6818 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/Makefile
+-rw-r--r--   0 konsta     (501) staff       (20)     1068 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/docs/native_versioning.rst
+-rw-r--r--   0 konsta     (501) staff       (20)      801 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.9/docs/plugins.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     1714 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/docs/queries.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     2209 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/revert.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     1898 2014-04-24 08:21:06.000000 SQLAlchemy-Continuum-1.3.9/docs/schema.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     1877 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.9/docs/transactions.rst
+-rw-r--r--   0 konsta     (501) staff       (20)      892 2014-08-27 09:58:16.000000 SQLAlchemy-Continuum-1.3.9/docs/utilities.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     6020 2014-04-24 09:58:30.000000 SQLAlchemy-Continuum-1.3.9/docs/version_objects.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     1437 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/LICENSE
+-rw-r--r--   0 konsta     (501) staff       (20)      193 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/MANIFEST.in
+-rw-r--r--   0 konsta     (501) staff       (20)     1079 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)     2977 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.9/README.rst
+-rw-r--r--   0 konsta     (501) staff       (20)       38 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/setup.cfg
+-rw-r--r--   0 konsta     (501) staff       (20)     2413 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.9/setup.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/
+-rw-r--r--   0 konsta     (501) staff       (20)     3258 2019-03-19 12:18:33.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     6758 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/builder.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-08-14 14:08:11.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)    15324 2014-12-06 10:19:14.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/postgresql.py
+-rw-r--r--   0 konsta     (501) staff       (20)      152 2014-04-29 12:36:20.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/exc.py
+-rw-r--r--   0 konsta     (501) staff       (20)      975 2015-07-24 06:47:20.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/expression_reflector.py
+-rw-r--r--   0 konsta     (501) staff       (20)      407 2014-09-04 12:34:32.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/factory.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5799 2014-07-10 11:45:57.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/fetcher.py
+-rw-r--r--   0 konsta     (501) staff       (20)    18570 2018-07-30 12:47:07.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/manager.py
+-rw-r--r--   0 konsta     (501) staff       (20)     9348 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/model_builder.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2840 2014-07-16 13:16:55.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/operation.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/
+-rw-r--r--   0 konsta     (501) staff       (20)      322 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)    10395 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/activity.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1866 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/base.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2188 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/flask.py
+-rw-r--r--   0 konsta     (501) staff       (20)      987 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/null_delete.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2487 2014-08-19 08:18:11.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/property_mod_tracker.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3193 2014-12-30 15:57:18.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_changes.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3172 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_meta.py
+-rw-r--r--   0 konsta     (501) staff       (20)    12507 2019-03-19 12:18:33.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/relationship_builder.py
+-rw-r--r--   0 konsta     (501) staff       (20)     4464 2015-09-27 08:54:29.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/reverter.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5593 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/schema.py
+-rw-r--r--   0 konsta     (501) staff       (20)     4752 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/table_builder.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5497 2019-03-19 13:08:16.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/transaction.py
+-rw-r--r--   0 konsta     (501) staff       (20)    11266 2015-07-24 07:20:58.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/unit_of_work.py
+-rw-r--r--   0 konsta     (501) staff       (20)    12240 2019-02-27 15:07:50.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/utils.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2095 2017-11-05 16:02:23.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/version.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/dependency_links.txt
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2014-02-10 07:59:41.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/not-zip-safe
+-rw-r--r--   0 konsta     (501) staff       (20)     1079 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)      411 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/requires.txt
+-rw-r--r--   0 konsta     (501) staff       (20)     4049 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/SOURCES.txt
+-rw-r--r--   0 konsta     (501) staff       (20)       21 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/top_level.txt
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/
+-rw-r--r--   0 konsta     (501) staff       (20)     6588 2019-02-27 15:22:36.000000 SQLAlchemy-Continuum-1.3.9/tests/__init__.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)      259 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/test_model_builder.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1146 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/test_relationship_builder.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3550 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/test_table_builder.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/dialects/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/tests/dialects/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2045 2014-10-13 19:41:57.000000 SQLAlchemy-Continuum-1.3.9/tests/dialects/test_triggers.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)      940 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_common_base_class.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3272 2014-06-16 09:20:44.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_concrete_inheritance.py
+-rw-r--r--   0 konsta     (501) staff       (20)     7059 2015-09-27 08:36:34.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_join_table_inheritance.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1646 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_multi_level_inheritance.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2980 2014-08-18 13:30:03.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_single_table_inheritance.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5680 2014-08-14 13:56:49.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_activity.py
+-rw-r--r--   0 konsta     (501) staff       (20)     8766 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_flask.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1000 2014-08-14 13:56:49.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_null_delete.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1070 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_plugin_collection.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5881 2014-08-26 11:51:22.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_property_mod_tracker.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2473 2014-12-30 16:00:18.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_changes.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1253 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_meta.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2048 2018-06-03 11:24:04.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_association_table_relations.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2035 2015-07-24 07:48:10.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_custom_condition_relations.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3029 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_dynamic_relationships.py
+-rw-r--r--   0 konsta     (501) staff       (20)    14534 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_many_to_many_relations.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3291 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_non_versioned_classes.py
+-rw-r--r--   0 konsta     (501) staff       (20)     9110 2014-12-28 13:06:15.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_many_relations.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2882 2014-07-10 11:45:57.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_one_relations.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2112 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_deep_relationships.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2806 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_many_to_many_relationships.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1817 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_relationship.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2127 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_with_secondary_table.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2129 2014-10-01 13:34:49.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_end_transaction_id.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2946 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_property_mod_flags.py
+-rw-r--r--   0 konsta     (501) staff       (20)     8343 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.9/tests/test_accessors.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3470 2017-11-05 16:02:23.000000 SQLAlchemy-Continuum-1.3.9/tests/test_changeset.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1935 2014-04-21 09:09:53.000000 SQLAlchemy-Continuum-1.3.9/tests/test_column_aliases.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3661 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.9/tests/test_column_inclusion_and_exclusion.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2456 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/test_composite_primary_key.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3713 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/tests/test_configuration.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2057 2014-10-01 09:31:26.000000 SQLAlchemy-Continuum-1.3.9/tests/test_custom_schema.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1114 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/test_custom_version_base_class.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1356 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/tests/test_delete.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1068 2014-07-16 13:11:49.000000 SQLAlchemy-Continuum-1.3.9/tests/test_exotic_listener_chaining.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2509 2015-07-24 07:16:05.000000 SQLAlchemy-Continuum-1.3.9/tests/test_exotic_operation_combos.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2602 2017-01-30 17:14:23.000000 SQLAlchemy-Continuum-1.3.9/tests/test_i18n.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2647 2015-07-24 10:14:05.000000 SQLAlchemy-Continuum-1.3.9/tests/test_insert.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2336 2014-04-22 15:07:31.000000 SQLAlchemy-Continuum-1.3.9/tests/test_mapper_args.py
+-rw-r--r--   0 konsta     (501) staff       (20)      976 2014-10-01 13:34:49.000000 SQLAlchemy-Continuum-1.3.9/tests/test_raw_sql.py
+-rw-r--r--   0 konsta     (501) staff       (20)     6000 2015-09-27 08:54:29.000000 SQLAlchemy-Continuum-1.3.9/tests/test_revert.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1540 2014-09-02 06:42:43.000000 SQLAlchemy-Continuum-1.3.9/tests/test_savepoints.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2170 2018-07-30 12:47:07.000000 SQLAlchemy-Continuum-1.3.9/tests/test_sessions.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2654 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/tests/test_transaction.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3414 2015-07-24 06:49:15.000000 SQLAlchemy-Continuum-1.3.9/tests/test_update.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1707 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.9/tests/test_vacuum.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3640 2014-09-02 06:44:39.000000 SQLAlchemy-Continuum-1.3.9/tests/test_validity_strategy.py
+-rw-r--r--   0 konsta     (501) staff       (20)      669 2014-04-09 15:04:22.000000 SQLAlchemy-Continuum-1.3.9/tests/test_versions.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-25 11:06:55.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)      869 2014-04-25 11:08:20.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_changeset.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1079 2014-08-27 09:54:26.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_count_versions.py
+-rw-r--r--   0 konsta     (501) staff       (20)      877 2014-12-06 08:57:22.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_is_modified.py
+-rw-r--r--   0 konsta     (501) staff       (20)      440 2014-04-25 11:12:06.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_parent_class.py
+-rw-r--r--   0 konsta     (501) staff       (20)      477 2014-04-25 11:22:10.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_transaction_class.py
+-rw-r--r--   0 konsta     (501) staff       (20)      824 2014-04-25 11:21:06.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_tx_column_name.py
+-rw-r--r--   0 konsta     (501) staff       (20)      887 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_version_class.py
```

### Comparing `SQLAlchemy-Continuum-1.3.7/CHANGES.rst` & `SQLAlchemy-Continuum-1.3.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 Changelog
 ---------
 
 Here you can see the full list of changes between each SQLAlchemy-Continuum release.
 
 
+1.3.9 (2019-03-19)
+^^^^^^^^^^^^^^^^^^
+
+- Added SA 1.3 support
+- Reverted trigger creation from 1.3.7
+
+
+1.3.8 (2019-02-27)
+^^^^^^^^^^^^^^^^^^
+
+- Fixed revert to ignore non-columns (#197, courtesy of mauler)
+
+
 1.3.7 (2019-01-13)
 ^^^^^^^^^^^^^^^^^^
 
-Fix trigger creation during alembic migrations (#209, courtesy of lyndsysimon)
+- Fix trigger creation during alembic migrations (#209, courtesy of lyndsysimon)
 
 
 1.3.6 (2018-07-30)
 ^^^^^^^^^^^^^^^^^^
 
 - Fixed ResourceClosedErrors from connections leaking when using an external transaction (#196, courtesy of vault)
```

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/.DS_Store` & `SQLAlchemy-Continuum-1.3.9/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/alembic.rst` & `SQLAlchemy-Continuum-1.3.9/docs/alembic.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/api.rst` & `SQLAlchemy-Continuum-1.3.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/conf.py` & `SQLAlchemy-Continuum-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/configuration.rst` & `SQLAlchemy-Continuum-1.3.9/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/intro.rst` & `SQLAlchemy-Continuum-1.3.9/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/make.bat` & `SQLAlchemy-Continuum-1.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/Makefile` & `SQLAlchemy-Continuum-1.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/native_versioning.rst` & `SQLAlchemy-Continuum-1.3.9/docs/native_versioning.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/plugins.rst` & `SQLAlchemy-Continuum-1.3.9/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/queries.rst` & `SQLAlchemy-Continuum-1.3.9/docs/queries.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/revert.rst` & `SQLAlchemy-Continuum-1.3.9/docs/revert.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/schema.rst` & `SQLAlchemy-Continuum-1.3.9/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/transactions.rst` & `SQLAlchemy-Continuum-1.3.9/docs/transactions.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/utilities.rst` & `SQLAlchemy-Continuum-1.3.9/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/docs/version_objects.rst` & `SQLAlchemy-Continuum-1.3.9/docs/version_objects.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/LICENSE` & `SQLAlchemy-Continuum-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/PKG-INFO` & `SQLAlchemy-Continuum-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SQLAlchemy-Continuum
-Version: 1.3.7
+Version: 1.3.9
 Summary: Versioning and auditing extension for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-continuum
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         SQLAlchemy-Continuum
```

### Comparing `SQLAlchemy-Continuum-1.3.7/README.rst` & `SQLAlchemy-Continuum-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/setup.py` & `SQLAlchemy-Continuum-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/__init__.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     transaction_class,
     tx_column_name,
     vacuum,
     version_class,
 )
 
 
-__version__ = '1.3.7'
+__version__ = '1.3.9'
 
 
 versioning_manager = VersioningManager()
 
 
 def make_versioned(
     mapper=sa.orm.mapper,
```

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/builder.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/dialects/postgresql.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/expression_reflector.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/expression_reflector.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/fetcher.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/fetcher.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/manager.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/manager.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/model_builder.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/model_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/operation.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/operation.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/activity.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/activity.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/base.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/base.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/flask.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/flask.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/null_delete.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/null_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/property_mod_tracker.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/property_mod_tracker.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/transaction_changes.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_changes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/plugins/transaction_meta.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_meta.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/relationship_builder.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/relationship_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
                 not self.manager.is_excluded_property(
                     self.model, self.property.key)):
             self.build_association_version_tables()
 
             # store remote cls to association table column pairs
             self.remote_to_association_column_pairs = []
             for column_pair in self.property.local_remote_pairs:
-                if column_pair[0] in self.property.table.c.values():
+                if column_pair[0] in self.property.target.c.values():
                     self.remote_to_association_column_pairs.append(column_pair)
 
         setattr(
             self.local_cls,
             self.property.key,
             self.reflected_relationship
         )
```

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/reverter.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/reverter.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/schema.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/table_builder.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/table_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/transaction.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,46 +70,32 @@
     RETURN NEW;
 END;
 $$
 LANGUAGE plpgsql
 """
 
 
-def _after_create(cls, ddl):
-    """Execute DDL after a table is created
-
-    This is required for compatibility with alembic, as the `after_create` event
-    does not fire during alembic migrations"""
-    def listener(tablename, ddl, table, bind, **kw):
-        if table.name == tablename:
-            ddl(table, bind, **kw)
-
-    sa.event.listen(
-        sa.Table,
-       'after_create',
-       partial(listener, cls.__table__.name, ddl)
-    )
-
-
 def create_triggers(cls):
-    _after_create(
-        cls,
+    sa.event.listen(
+        cls.__table__,
+        'after_create',
         sa.schema.DDL(
             procedure_sql.format(
                 temporary_transaction_sql=CreateTemporaryTransactionTableSQL(),
                 insert_temporary_transaction_sql=(
                     InsertTemporaryTransactionSQL(
                         transaction_id_values='NEW.id'
                     )
                 ),
             )
         )
     )
-    _after_create(
-        cls,
+    sa.event.listen(
+        cls.__table__,
+        'after_create',
         sa.schema.DDL(str(TransactionTriggerSQL(cls)))
     )
     sa.event.listen(
         cls.__table__,
         'after_drop',
         sa.schema.DDL(
             'DROP FUNCTION IF EXISTS transaction_temp_table_generator()'
```

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/unit_of_work.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/utils.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -198,15 +198,19 @@
     :param obj: SQLAlchemy declarative model object
     """
     manager = get_versioning_manager(obj_or_class)
 
     cls = obj_or_class if isclass(obj_or_class) else obj_or_class.__class__
 
     mapper = sa.inspect(cls)
-    for key in mapper.columns.keys():
+    for key, column in mapper.columns.items():
+        # Ignores non table columns
+        if not is_table_column(column):
+            continue
+
         if not manager.is_excluded_property(obj_or_class, key):
             yield getattr(mapper.attrs, key)
 
 
 def versioned_relationships(obj, versioned_column_keys):
     """
     Return all versioned relationships for given versioned SQLAlchemy
@@ -258,14 +262,24 @@
             prev_version = versions[version_id][-1]
             if naturally_equivalent(prev_version, version):
                 session.delete(version)
         else:
             versions[version_id].append(version)
 
 
+def is_table_column(column):
+    """
+    Return wheter of not give field is a column over the database table.
+
+    :param column: SQLAclhemy model field.
+    :rtype: bool
+    """
+    return isinstance(column, sa.Column)
+
+
 def is_internal_column(model, column_name):
     """
     Return whether or not given column of given SQLAlchemy declarative classs
     is considered an internal column (a column whose purpose is mainly
     for SA-Continuum's internal use).
 
     :param version_obj: SQLAlchemy declarative class
@@ -402,15 +416,18 @@
         # {'name': [u'Some article', None]}
 
     :param obj: SQLAlchemy declarative model object
     """
     data = {}
     session = sa.orm.object_session(obj)
     if session and obj in session.deleted:
-        for column in sa.inspect(obj.__class__).columns.values():
+        columns = [c for c in sa.inspect(obj.__class__).columns.values()
+                   if is_table_column(c)]
+
+        for column in columns:
             if not column.primary_key:
                 value = getattr(obj, column.key)
                 if value is not None:
                     data[column.key] = [None, getattr(obj, column.key)]
     else:
         for prop in obj.__mapper__.iterate_properties:
             history = get_history(obj, prop.key)
```

### Comparing `SQLAlchemy-Continuum-1.3.7/sqlalchemy_continuum/version.py` & `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/version.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/PKG-INFO` & `SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SQLAlchemy-Continuum
-Version: 1.3.7
+Version: 1.3.9
 Summary: Versioning and auditing extension for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-continuum
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         SQLAlchemy-Continuum
```

### Comparing `SQLAlchemy-Continuum-1.3.7/SQLAlchemy_Continuum.egg-info/SOURCES.txt` & `SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/__init__.py` & `SQLAlchemy-Continuum-1.3.9/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+
 from copy import copy
 import inspect
 import itertools as it
 import os
 import warnings
 import sqlalchemy as sa
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import sessionmaker, column_property
 from sqlalchemy_continuum import (
     ClassNotVersioned,
     version_class,
     make_versioned,
     versioning_manager,
     remove_versioning
 )
@@ -144,14 +145,17 @@
             __versioned__ = copy(self.options)
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255), nullable=False)
             content = sa.Column(sa.UnicodeText)
             description = sa.Column(sa.UnicodeText)
 
+            # Dynamic column cotaining all text content data
+            fulltext_content = column_property(name + content + description)
+
         class Tag(self.Model):
             __tablename__ = 'tag'
             __versioned__ = copy(self.options)
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255))
             article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
```

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/builders/test_relationship_builder.py` & `SQLAlchemy-Continuum-1.3.9/tests/builders/test_relationship_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/builders/test_table_builder.py` & `SQLAlchemy-Continuum-1.3.9/tests/builders/test_table_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/dialects/test_triggers.py` & `SQLAlchemy-Continuum-1.3.9/tests/dialects/test_triggers.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_common_base_class.py` & `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_common_base_class.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_concrete_inheritance.py` & `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_concrete_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_join_table_inheritance.py` & `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_join_table_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_multi_level_inheritance.py` & `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_multi_level_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/inheritance/test_single_table_inheritance.py` & `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_single_table_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_activity.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_activity.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_flask.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_flask.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_null_delete.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_null_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_plugin_collection.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_property_mod_tracker.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_property_mod_tracker.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_transaction_changes.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_changes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/plugins/test_transaction_meta.py` & `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_meta.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_association_table_relations.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_association_table_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_custom_condition_relations.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_custom_condition_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_dynamic_relationships.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_dynamic_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_many_to_many_relations.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_many_to_many_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_non_versioned_classes.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_non_versioned_classes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_one_to_many_relations.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_many_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/relationships/test_one_to_one_relations.py` & `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_one_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/revert/test_deep_relationships.py` & `SQLAlchemy-Continuum-1.3.9/tests/revert/test_deep_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/revert/test_many_to_many_relationships.py` & `SQLAlchemy-Continuum-1.3.9/tests/revert/test_many_to_many_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/revert/test_one_to_one_relationship.py` & `SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_relationship.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/revert/test_one_to_one_with_secondary_table.py` & `SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_with_secondary_table.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/schema/test_update_end_transaction_id.py` & `SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_end_transaction_id.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/schema/test_update_property_mod_flags.py` & `SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_property_mod_flags.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_accessors.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_changeset.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_changeset.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_column_aliases.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_column_aliases.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_column_inclusion_and_exclusion.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_column_inclusion_and_exclusion.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_composite_primary_key.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_composite_primary_key.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_configuration.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_custom_schema.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_custom_schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_custom_version_base_class.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_custom_version_base_class.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_delete.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_exotic_listener_chaining.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_exotic_listener_chaining.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_exotic_operation_combos.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_exotic_operation_combos.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_i18n.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_insert.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_mapper_args.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_mapper_args.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_raw_sql.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_raw_sql.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_revert.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_revert.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_savepoints.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_savepoints.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_sessions.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_transaction.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_update.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_vacuum.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_validity_strategy.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_validity_strategy.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/test_versions.py` & `SQLAlchemy-Continuum-1.3.9/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/utils/test_changeset.py` & `SQLAlchemy-Continuum-1.3.9/tests/utils/test_changeset.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/utils/test_count_versions.py` & `SQLAlchemy-Continuum-1.3.9/tests/utils/test_count_versions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/utils/test_is_modified.py` & `SQLAlchemy-Continuum-1.3.9/tests/utils/test_is_modified.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/utils/test_tx_column_name.py` & `SQLAlchemy-Continuum-1.3.9/tests/utils/test_tx_column_name.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.7/tests/utils/test_version_class.py` & `SQLAlchemy-Continuum-1.3.9/tests/utils/test_version_class.py`

 * *Files identical despite different names*

