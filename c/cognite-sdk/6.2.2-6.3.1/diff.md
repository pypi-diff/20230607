# Comparing `tmp/cognite_sdk-6.2.2.tar.gz` & `tmp/cognite_sdk-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.2.2.tar", max compression
+gzip compressed data, was "cognite_sdk-6.3.1.tar", max compression
```

## Comparing `cognite_sdk-6.2.2.tar` & `cognite_sdk-6.3.1.tar`

### file list

```diff
@@ -1,100 +1,112 @@
--rw-r--r--   0        0        0    11349 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/README.md
--rw-r--r--   0        0        0      503 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/assets.py
--rw-r--r--   0        0        0      573 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/data_modeling.py
--rw-r--r--   0        0        0    11025 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-05 09:54:54.642897 cognite_sdk-6.2.2/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17320 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45329 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49915 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     6483 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/spaces.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    37531 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/config.py
--rw-r--r--   0        0        0    18062 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/credentials.py
--rw-r--r--   0        0        0     8901 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-06-05 09:54:54.646897 cognite_sdk-6.2.2/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14299 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0     1753 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/spaces.py
--rw-r--r--   0        0        0    16814 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/py.typed
--rw-r--r--   0        0        0     8434 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7277 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-05 09:54:54.650897 cognite_sdk-6.2.2/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2133 2023-06-05 09:54:54.654897 cognite_sdk-6.2.2/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/README.md
+-rw-r--r--   0        0        0      574 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1013 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7924 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8454 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     6468 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7894 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17320 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45329 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49915 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    37481 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      178 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/config.py
+-rw-r--r--   0        0        0    18062 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     2935 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12346 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7240 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3651 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     3877 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0     2524 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14625 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6682 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14299 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/py.typed
+-rw-r--r--   0        0        0     8865 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7422 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2132 2023-06-07 13:19:35.605548 cognite_sdk-6.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.3.1/PKG-INFO
```

### Comparing `cognite_sdk-6.2.2/LICENSE` & `cognite_sdk-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/README.md` & `cognite_sdk-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/annotations.py` & `cognite_sdk-6.3.1/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/assets.py` & `cognite_sdk-6.3.1/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/data_sets.py` & `cognite_sdk-6.3.1/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.3.1/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/datapoints.py` & `cognite_sdk-6.3.1/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/diagrams.py` & `cognite_sdk-6.3.1/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.3.1/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/events.py` & `cognite_sdk-6.3.1/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.3.1/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/files.py` & `cognite_sdk-6.3.1/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/functions.py` & `cognite_sdk-6.3.1/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/geospatial.py` & `cognite_sdk-6.3.1/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/iam.py` & `cognite_sdk-6.3.1/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/labels.py` & `cognite_sdk-6.3.1/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/raw.py` & `cognite_sdk-6.3.1/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/relationships.py` & `cognite_sdk-6.3.1/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/sequences.py` & `cognite_sdk-6.3.1/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/spaces.py` & `cognite_sdk-6.3.1/cognite/client/_api/data_modeling/spaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 from __future__ import annotations
 
-from typing import Iterator, Optional, Sequence, cast, overload
+from typing import Iterator, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import LIST_LIMIT_DEFAULT
-from cognite.client.data_classes import Space, SpaceList
+from cognite.client.data_classes.data_modeling.spaces import Space, SpaceApply, SpaceList
 from cognite.client.utils._identifier import DataModelingIdentifierSequence
 
 
 class SpacesAPI(APIClient):
     _RESOURCE_PATH = "/models/spaces"
 
+    @overload
+    def __call__(
+        self,
+        chunk_size: None = None,
+        limit: int = None,
+    ) -> Iterator[Space]:
+        ...
+
+    @overload
+    def __call__(
+        self,
+        chunk_size: int,
+        limit: int = None,
+    ) -> Iterator[SpaceList]:
+        ...
+
     def __call__(
         self,
         chunk_size: int = None,
         limit: int = None,
     ) -> Iterator[Space] | Iterator[SpaceList]:
         """Iterate over spaces
 
@@ -41,56 +57,46 @@
         Fetches spaces as they are iterated over, so you keep a limited number of spaces in memory.
 
         Yields:
             Space: yields Spaces one by one.
         """
         return cast(Iterator[Space], self())
 
-    def retrieve(self, space: str) -> Optional[Space]:
-        """`Retrieve a single space by id. <https://docs.cognite.com/api/v1/#tag/Spaces/operation/bySpaceIdsSpaces>`_
+    @overload
+    def retrieve(self, space: str) -> Space | None:  # type: ignore[misc]
+        ...
+
+    @overload
+    def retrieve(self, space: Sequence[str]) -> SpaceList:
+        ...
+
+    def retrieve(self, space: str | Sequence[str]) -> Space | SpaceList | None:
+        """`Retrieve space by id. <https://docs.cognite.com/api/v1/#tag/Spaces/operation/bySpaceIdsSpaces>`_
 
         Args:
             space (str): Space ID
 
         Returns:
             Optional[Space]: Requested space or None if it does not exist.
 
         Examples:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.spaces.retrieve(space='mySpace')
 
-        """
-        identifier = DataModelingIdentifierSequence.load_spaces(spaces=space).as_singleton()
-        return self._retrieve_multiple(list_cls=SpaceList, resource_cls=Space, identifiers=identifier)
-
-    def retrieve_multiple(
-        self,
-        spaces: Sequence[str],
-    ) -> SpaceList:
-        """`Retrieve multiple spaces by id. <https://docs.cognite.com/api/v1/#tag/Spaces/operation/bySpaceIdsSpaces>`_
-
-        Args:
-            spaces (Sequence[str]): Space IDs.
-
-        Returns:
-            SpaceList: The requested spaces.
-
-        Examples:
-
-            Get spaces by id::
+         Get multiple spaces by id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
-                >>> res = c.data_modeling.spaces.retrieve_multiple(spaces=["MySpace", "MyAwesomeSpace", "MyOtherSpace"])
+                >>> res = c.data_modeling.spaces.retrieve(spaces=["MySpace", "MyAwesomeSpace", "MyOtherSpace"])
 
         """
-        identifiers = DataModelingIdentifierSequence.load_spaces(spaces=spaces)
-        return self._retrieve_multiple(list_cls=SpaceList, resource_cls=Space, identifiers=identifiers)
+        identifier = DataModelingIdentifierSequence.load_spaces(spaces=space)
+        return self._retrieve_multiple(list_cls=SpaceList, resource_cls=Space, identifiers=identifier)
 
     def delete(self, space: str | Sequence[str]) -> list[str]:
         """`Delete one or more spaces <https://docs.cognite.com/api/v1/#tag/Spaces/operation/deleteSpacesV3>`_
 
         Args:
             space (str | Sequence[str]): ID or ID list ids of spaces.
         Returns:
@@ -150,35 +156,35 @@
             list_cls=SpaceList,
             resource_cls=Space,
             method="GET",
             limit=limit,
         )
 
     @overload
-    def apply(self, space: Sequence[Space]) -> SpaceList:
+    def apply(self, space: Sequence[SpaceApply]) -> SpaceList:
         ...
 
     @overload
-    def apply(self, space: Space) -> Space:
+    def apply(self, space: SpaceApply) -> Space:
         ...
 
-    def apply(self, space: Space | Sequence[Space]) -> Space | SpaceList:
+    def apply(self, space: SpaceApply | Sequence[SpaceApply]) -> Space | SpaceList:
         """`Create or patch one or more spaces. <https://docs.cognite.com/api/v1/#tag/Spaces/operation/ApplySpaces>`_
 
         Args:
             space (space: Space | Sequence[Space]): Space or spaces of spacesda to create or update.
 
         Returns:
             Space | SpaceList: Created space(s)
 
         Examples:
 
-            Create new spacesda::
+            Create new spaces:
 
                 >>> from cognite.client import CogniteClient
-                >>> from cognite.client.data_classes import Space
+                >>> from cognite.client.data_classes.data_modeling import SpaceApply
                 >>> c = CogniteClient()
-                >>> spaces = [Space(space="mySpace", description="My first space", name="My Space"),
-                ... Space(space="myOtherSpace", description="My second space", name="My Other Space")]
-                >>> res = c.data_modeling.spaces.create(spaces)
+                >>> spaces = [SpaceApply(space="mySpace", description="My first space", name="My Space"),
+                ... SpaceApply(space="myOtherSpace", description="My second space", name="My Other Space")]
+                >>> res = c.data_modeling.spaces.apply(spaces)
         """
         return self._create_multiple(list_cls=SpaceList, resource_cls=Space, items=space)
```

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.3.1/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/templates.py` & `cognite_sdk-6.3.1/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/three_d.py` & `cognite_sdk-6.3.1/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/time_series.py` & `cognite_sdk-6.3.1/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.3.1/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.3.1/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.3.1/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.3.1/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.3.1/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api/vision.py` & `cognite_sdk-6.3.1/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_api_client.py` & `cognite_sdk-6.3.1/cognite/client/_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,28 +597,28 @@
         limit: Optional[int] = None,
     ) -> T_CogniteResourceList:
         ...
 
     @overload
     def _create_multiple(
         self,
-        items: Union[T_CogniteResource, Dict[str, Any]],
+        items: Union[CogniteResource, Dict[str, Any]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
     ) -> T_CogniteResource:
         ...
 
     def _create_multiple(
         self,
-        items: Union[Sequence[T_CogniteResource], Sequence[Dict[str, Any]], T_CogniteResource, Dict[str, Any]],
+        items: Union[Sequence[CogniteResource], Sequence[Dict[str, Any]], CogniteResource, Dict[str, Any]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
@@ -687,16 +687,15 @@
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"],
             task_list_element_unwrap_fn=utils._auxiliary.unwrap_identifer,
         )
         if returns_items:
-            deleted_spaces = summary.joined_results(lambda res: res.json()["items"])
-            return deleted_spaces
+            return summary.joined_results(lambda res: res.json()["items"])
         else:
             return None
 
     @overload
     def _update_multiple(
         self,
         items: Union[CogniteResource, CogniteUpdate],
```

### Comparing `cognite_sdk-6.2.2/cognite/client/_cognite_client.py` & `cognite_sdk-6.3.1/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_http_client.py` & `cognite_sdk-6.3.1/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.3.1/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/config.py` & `cognite_sdk-6.3.1/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/credentials.py` & `cognite_sdk-6.3.1/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,18 +122,14 @@
     AggregateUniqueValuesResult,
     GeoLocation,
     GeoLocationFilter,
     Geometry,
     GeometryFilter,
     TimestampRange,
 )
-from cognite.client.data_classes.spaces import (
-    Space,
-    SpaceList,
-)
 from cognite.client.data_classes.templates import (
     ConstantResolver,
     Source,
     TemplateGroup,
     TemplateGroupList,
     TemplateGroupVersion,
     TemplateGroupVersionList,
@@ -353,10 +349,8 @@
     "FeatureTypePatch",
     "FeatureAggregate",
     "FeatureTypeUpdate",
     "FeatureAggregateList",
     "FeatureTypeUpdateList",
     "CoordinateReferenceSystemList",
     "CoordinateReferenceSystem",
-    "Space",
-    "SpaceList",
 ]
```

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/_base.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/assets.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/events.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/files.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/functions.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/iam.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/labels.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/raw.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/shared.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/spaces.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,83 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, cast
-
 from cognite.client.data_classes._base import (
-    CogniteResource,
     CogniteResourceList,
 )
+from cognite.client.data_classes.data_modeling._core import DataModelingResource
+from cognite.client.data_classes.data_modeling._validation import validate_data_modeling_identifier
 
-if TYPE_CHECKING:
-    from cognite.client import CogniteClient
 
-_RESERVED_SPACE_IDS = frozenset({"space", "cdf", "dms", "pg3", "shared", "system", "node", "edge"})
+class SpaceCore(DataModelingResource):
+    """A workspace for data models and instances.
 
+    Args:
+        space (str): A unique identifier for space.
+        description (str): Textual description of the space
+        name (str): Human readable name for the space.
+    """
 
-class Space(CogniteResource):
-    """A workspace for data models and instances.
+    def __init__(
+        self,
+        space: str,
+        description: str = None,
+        name: str = None,
+        **_: dict,
+    ):
+        validate_data_modeling_identifier(space)
+        self.space = space
+        self.description = description
+        self.name = name
+
+
+class SpaceApply(SpaceCore):
+    """A workspace for data models and instances. This is the write version"""
+
+    ...
+
+
+class Space(SpaceCore):
+    """A workspace for data models and instances. This is the read version.
 
     Args:
         space (str): a unique identifier for the space.
         description (str): Textual description of the space
         name (str): Human readable name for the space.
+        is_global (bool): Whether the space is global or not.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
     """
 
     def __init__(
         self,
-        space: str = None,
+        space: str,
+        is_global: bool,
+        last_updated_time: int,
+        created_time: int,
         description: str = None,
         name: str = None,
-        last_updated_time: int = None,
-        created_time: int = None,
-        cognite_client: CogniteClient = None,
     ):
-        if space in _RESERVED_SPACE_IDS:
-            raise ValueError(f"The space ID: {space} is reserved. Please use another ID.")
-        self.space = space
-        self.description = description
-        self.name = name
+        super().__init__(space, description, name)
+        self.is_global = is_global
         self.last_updated_time = last_updated_time
         self.created_time = created_time
-        self._cognite_client = cast("CogniteClient", cognite_client)
 
-    def __repr__(self) -> str:
-        space = self.space
-        return f"{type(self).__name__}({space=}) at 0x{hex(id(self)).upper().zfill(16)}"
+    def as_apply(self) -> SpaceApply:
+        return SpaceApply(
+            space=self.space,
+            description=self.description,
+            name=self.name,
+        )
+
+
+class SpaceApplyList(CogniteResourceList):
+    _RESOURCE = SpaceApply
 
 
 class SpaceList(CogniteResourceList):
     _RESOURCE = Space
+
+    def to_space_apply_list(self) -> SpaceApplyList:
+        return SpaceApplyList(
+            resources=[item.as_apply() for item in self.items],
+            cognite_client=self._cognite_client,
+        )
```

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/templates.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/exceptions.py` & `cognite_sdk-6.3.1/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/testing.py` & `cognite_sdk-6.3.1/cognite/client/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from typing import Any, Iterator
 from unittest.mock import MagicMock
 
 from cognite.client import CogniteClient
 from cognite.client._api.annotations import AnnotationsAPI
 from cognite.client._api.assets import AssetsAPI
 from cognite.client._api.data_modeling import DataModelingAPI
+from cognite.client._api.data_modeling.containers import ContainersAPI
+from cognite.client._api.data_modeling.data_models import DataModelsAPI
+from cognite.client._api.data_modeling.spaces import SpacesAPI
+from cognite.client._api.data_modeling.views import ViewsAPI
 from cognite.client._api.data_sets import DataSetsAPI
 from cognite.client._api.datapoints import DatapointsAPI
 from cognite.client._api.diagrams import DiagramsAPI
 from cognite.client._api.entity_matching import EntityMatchingAPI
 from cognite.client._api.events import EventsAPI
 from cognite.client._api.extractionpipelines import (
     ExtractionPipelineConfigsAPI,
@@ -22,15 +26,14 @@
 from cognite.client._api.functions import FunctionCallsAPI, FunctionsAPI, FunctionSchedulesAPI
 from cognite.client._api.geospatial import GeospatialAPI
 from cognite.client._api.iam import IAMAPI, GroupsAPI, SecurityCategoriesAPI, SessionsAPI, TokenAPI
 from cognite.client._api.labels import LabelsAPI
 from cognite.client._api.raw import RawAPI, RawDatabasesAPI, RawRowsAPI, RawTablesAPI
 from cognite.client._api.relationships import RelationshipsAPI
 from cognite.client._api.sequences import SequencesAPI, SequencesDataAPI
-from cognite.client._api.spaces import SpacesAPI
 from cognite.client._api.synthetic_time_series import SyntheticDatapointsAPI
 from cognite.client._api.templates import (
     TemplateGroupsAPI,
     TemplateGroupVersionsAPI,
     TemplateInstancesAPI,
     TemplatesAPI,
     TemplateViewsAPI,
@@ -70,15 +73,18 @@
         #   - Add spacing above and below
         #   - Use `spec=MyAPI` only for "top level"
         #   - Use `spec_set=MyNestedAPI` for all nested APIs
         self.annotations = MagicMock(spec_set=AnnotationsAPI)
         self.assets = MagicMock(spec_set=AssetsAPI)
 
         self.data_modeling = MagicMock(spec=DataModelingAPI)
+        self.data_modeling.containers = MagicMock(spec_set=ContainersAPI)
+        self.data_modeling.data_models = MagicMock(spec_set=DataModelsAPI)
         self.data_modeling.spaces = MagicMock(spec_set=SpacesAPI)
+        self.data_modeling.views = MagicMock(spec_set=ViewsAPI)
 
         self.data_sets = MagicMock(spec_set=DataSetsAPI)
 
         self.diagrams = MagicMock(spec_set=DiagramsAPI)
         self.entity_matching = MagicMock(spec_set=EntityMatchingAPI)
         self.events = MagicMock(spec_set=EventsAPI)
```

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/__init__.py` & `cognite_sdk-6.3.1/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.3.1/cognite/client/utils/_auxiliary.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,7 +242,15 @@
     seen: Set[THashable] = set()
     add = seen.add  # skip future attr lookups for perf
     return {x for x in seq if x in seen or add(x)}
 
 
 def exactly_one_is_not_none(*args: Any) -> bool:
     return sum(1 if a is not None else 0 for a in args) == 1
+
+
+def rename_and_exclude_keys(
+    dct: dict[str, Any], aliases: dict[str, str] = None, exclude: set[str] = None
+) -> dict[str, Any]:
+    aliases = aliases or {}
+    exclude = exclude or set()
+    return {aliases.get(k, k): v for k, v in dct.items() if k not in exclude}
```

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.3.1/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_graph.py` & `cognite_sdk-6.3.1/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_identifier.py` & `cognite_sdk-6.3.1/cognite/client/utils/_identifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,24 +74,27 @@
         return {self.name(camel_case): self.__value}
 
     def as_tuple(self, camel_case: bool = True) -> Tuple[str, T_ID]:
         return self.name(camel_case), self.__value
 
 
 class DataModelingIdentifier:
-    def __init__(self, space: str, external_id: str | None = None):
+    def __init__(self, space: str, external_id: str | None = None, version: str | None = None):
         self.__space = space
         self.__external_id = external_id
+        self.__version = version
 
     def as_dict(self, camel_case: bool = True) -> dict[str, str]:
         output = {"space": self.__space}
-        if self.__external_id is None:
-            return output
-        key = "externalId" if camel_case else "external_id"
-        return {**output, key: self.__external_id}
+        if self.__external_id is not None:
+            key = "externalId" if camel_case else "external_id"
+            output[key] = self.__external_id
+        if self.__version is not None:
+            output["version"] = self.__version
+        return output
 
     def as_primitive(self) -> NoReturn:
         raise AttributeError(f"Not supported for {type(self).__name__} implementation")
 
 
 class ExternalId(Identifier[str]):
     ...
```

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_logging.py` & `cognite_sdk-6.3.1/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.3.1/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.3.1/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.3.1/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_text.py` & `cognite_sdk-6.3.1/cognite/client/utils/_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import random
 import re
 import string
 from functools import lru_cache
 from typing import Any, Dict, Iterator, Sequence
 
 
@@ -35,14 +37,38 @@
         yield from map(to_snake_case, seq)
 
 
 def convert_all_keys_to_camel_case(dct: Dict[str, Any]) -> Dict[str, Any]:
     return dict(zip(map(to_camel_case, dct.keys()), dct.values()))
 
 
+def convert_all_keys_to_camel_case_recursive(dct: dict[str, Any]) -> dict[str, Any]:
+    """Converts all the dictionary keys from snake to camel cases included nested objects.
+    >>> convert_all_keys_to_camel_case_recursive({"my_key": {"my_key": 1}})
+    {'myKey': {'myKey': 1}}
+    """
+    return {
+        to_camel_case(k): (convert_all_keys_to_camel_case_recursive(v) if isinstance(v, dict) else v)
+        for k, v in dct.items()
+    }
+
+
+def convert_all_keys_recursive(dct: dict[str, Any], camel_case: bool = False) -> dict[str, Any]:
+    """Converts all the dictionary keys from snake to camel cases included nested objects.
+    >>> convert_all_keys_recursive({"my_key": {"my_key": 1}}, camel_case=True)
+    {'myKey': {'myKey': 1}}
+    """
+    return {
+        (to_camel_case(k) if camel_case else k): (
+            convert_all_keys_recursive(v, camel_case) if isinstance(v, dict) else v
+        )
+        for k, v in dct.items()
+    }
+
+
 def convert_all_keys_to_snake_case(dct: Dict[str, Any]) -> Dict[str, Any]:
     return dict(zip(map(to_snake_case, dct.keys()), dct.values()))
 
 
 def convert_dict_to_case(dct: Dict[str, Any], camel_case: bool) -> Dict[str, Any]:
     if camel_case:
         return convert_all_keys_to_camel_case(dct)
```

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_time.py` & `cognite_sdk-6.3.1/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_validation.py` & `cognite_sdk-6.3.1/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.3.1/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.2.2/pyproject.toml` & `cognite_sdk-6.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.2.2"
-
+version = "6.3.1"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.2.2/PKG-INFO` & `cognite_sdk-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.2.2
+Version: 6.3.1
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.2.2 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.3.1 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

