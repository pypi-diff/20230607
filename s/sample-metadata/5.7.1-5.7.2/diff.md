# Comparing `tmp/sample_metadata-5.7.1.tar.gz` & `tmp/sample_metadata-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample_metadata-5.7.1.tar", last modified: Fri Apr 14 03:02:10 2023, max compression
+gzip compressed data, was "sample_metadata-5.7.2.tar", last modified: Wed Jun  7 03:30:15 2023, max compression
```

## Comparing `sample_metadata-5.7.1.tar` & `sample_metadata-5.7.2.tar`

### file list

```diff
@@ -1,109 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.535205 sample_metadata-5.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-14 03:02:10.535205 sample_metadata-5.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.523204 sample_metadata-5.7.1/sample_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.527205 sample_metadata-5.7.1/sample_metadata/api/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61864 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42202 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28316 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/sequence_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.527205 sample_metadata-5.7.1/sample_metadata/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.527205 sample_metadata-5.7.1/sample_metadata/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/sample_metadata/graphql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.531205 sample_metadata-5.7.1/sample_metadata/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/analysis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/analysis_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/body_get_sequences_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/nested_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/nested_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/new_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/new_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/participant_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/participant_upsert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/project_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sample_batch_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sample_batch_upsert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sample_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sequence_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sequence_technology.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sequence_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/sequence_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82237 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.531205 sample_metadata-5.7.1/sample_metadata/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.531205 sample_metadata-5.7.1/sample_metadata/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/sample_metadata/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/sample_metadata/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    32263 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/sample_metadata/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    49608 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/sample_metadata/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/sample_metadata/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-14 03:00:10.000000 sample_metadata-5.7.1/sample_metadata/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.523204 sample_metadata-5.7.1/sample_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-14 03:02:10.000000 sample_metadata-5.7.1/sample_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-14 03:02:10.000000 sample_metadata-5.7.1/sample_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:02:10.000000 sample_metadata-5.7.1/sample_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:02:10.000000 sample_metadata-5.7.1/sample_metadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 03:02:10.000000 sample_metadata-5.7.1/sample_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 03:02:10.000000 sample_metadata-5.7.1/sample_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:02:10.535205 sample_metadata-5.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:02:10.535205 sample_metadata-5.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_add_samples_for_joint_calling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_joint_calling_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    27410 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-14 02:57:55.000000 sample_metadata-5.7.1/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.377246 sample_metadata-5.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-06-07 03:30:15.377246 sample_metadata-5.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.345246 sample_metadata-5.7.2/sample_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.349246 sample_metadata-5.7.2/sample_metadata/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61864 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47667 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28316 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/sequence_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.349246 sample_metadata-5.7.2/sample_metadata/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.353246 sample_metadata-5.7.2/sample_metadata/audit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/audit/delete_sequence_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27730 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/audit/generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.353246 sample_metadata-5.7.2/sample_metadata/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/graphql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.365246 sample_metadata-5.7.2/sample_metadata/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/analysis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/analysis_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/body_get_sequences_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/nested_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/nested_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/new_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/new_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/participant_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/participant_upsert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/project_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sample_batch_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sample_batch_upsert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sample_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sequence_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sequence_technology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sequence_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/sequence_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-07 03:28:04.000000 sample_metadata-5.7.2/sample_metadata/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82237 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.365246 sample_metadata-5.7.2/sample_metadata/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.369246 sample_metadata-5.7.2/sample_metadata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49676 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/sample_metadata/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-06-07 03:28:05.000000 sample_metadata-5.7.2/sample_metadata/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.345246 sample_metadata-5.7.2/sample_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-06-07 03:30:15.000000 sample_metadata-5.7.2/sample_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-07 03:30:15.000000 sample_metadata-5.7.2/sample_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:30:15.000000 sample_metadata-5.7.2/sample_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:30:15.000000 sample_metadata-5.7.2/sample_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 03:30:15.000000 sample_metadata-5.7.2/sample_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 03:30:15.000000 sample_metadata-5.7.2/sample_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:30:15.377246 sample_metadata-5.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:30:15.377246 sample_metadata-5.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_add_samples_for_joint_calling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_existing_cohort_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_joint_calling_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27410 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-07 03:25:44.000000 sample_metadata-5.7.2/test/testbase.py
```

### Comparing `sample_metadata-5.7.1/LICENSE` & `sample_metadata-5.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/PKG-INFO` & `sample_metadata-5.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample_metadata
-Version: 5.7.1
+Version: 5.7.2
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sample_metadata-5.7.1/README.md` & `sample_metadata-5.7.2/README.md`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/sample_metadata/__init__.py` & `sample_metadata-5.7.2/sample_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/analysis_api.py` & `sample_metadata-5.7.2/sample_metadata/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/default_api.py` & `sample_metadata-5.7.2/sample_metadata/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/family_api.py` & `sample_metadata-5.7.2/sample_metadata/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/import_api.py` & `sample_metadata-5.7.2/sample_metadata/api/import_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/participant_api.py` & `sample_metadata-5.7.2/sample_metadata/api/participant_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -519,14 +519,79 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
+        self.update_participant_family_async = async_wrap(self.update_participant_family)
+        self.update_participant_family_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [
+                    'HTTPBearer'
+                ],
+                'endpoint_path': '/api/v1/participant/{participant_id}/update-participant-family',
+                'operation_id': 'update_participant_family',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'participant_id',
+                    'old_family_id',
+                    'new_family_id',
+                ],
+                'required': [
+                    'participant_id',
+                    'old_family_id',
+                    'new_family_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'participant_id':
+                        (int,),
+                    'old_family_id':
+                        (int,),
+                    'new_family_id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'participant_id': 'participant_id',
+                    'old_family_id': 'old_family_id',
+                    'new_family_id': 'new_family_id',
+                },
+                'location_map': {
+                    'participant_id': 'path',
+                    'old_family_id': 'query',
+                    'new_family_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
     def batch_upsert_participants(
         self,
         project,
         participant_upsert_body,
         **kwargs
     ):
         """Batch Upsert Participants  # noqa: E501
@@ -1106,7 +1171,86 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['participant_id'] = \
             participant_id
         kwargs['participant_update_model'] = \
             participant_update_model
         return self.update_participant_endpoint.call_with_http_info(**kwargs)
 
+    def update_participant_family(
+        self,
+        participant_id,
+        old_family_id,
+        new_family_id,
+        **kwargs
+    ):
+        """Update Participant Family  # noqa: E501
+
+        Change a participants family from old_family_id to new_family_id, maintaining all other fields. The new_family_id must already exist.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_participant_family(participant_id, old_family_id, new_family_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            participant_id (int):
+            old_family_id (int):
+            new_family_id (int):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['participant_id'] = \
+            participant_id
+        kwargs['old_family_id'] = \
+            old_family_id
+        kwargs['new_family_id'] = \
+            new_family_id
+        return self.update_participant_family_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/project_api.py` & `sample_metadata-5.7.2/sample_metadata/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/sample_api.py` & `sample_metadata-5.7.2/sample_metadata/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/seqr_api.py` & `sample_metadata-5.7.2/sample_metadata/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/sequence_api.py` & `sample_metadata-5.7.2/sample_metadata/api/sequence_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api/web_api.py` & `sample_metadata-5.7.2/sample_metadata/api/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/api_client.py` & `sample_metadata-5.7.2/sample_metadata/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `sample_metadata-5.7.1/sample_metadata/apis/__init__.py` & `sample_metadata-5.7.2/sample_metadata/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/sample_metadata/configuration.py` & `sample_metadata-5.7.2/sample_metadata/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -401,15 +401,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 5.7.1\n"\
+               "Version of the API: 5.7.2\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `sample_metadata-5.7.1/sample_metadata/exceptions.py` & `sample_metadata-5.7.2/sample_metadata/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `sample_metadata-5.7.1/sample_metadata/graphql/__init__.py` & `sample_metadata-5.7.2/sample_metadata/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/sample_metadata/model/analysis_model.py` & `sample_metadata-5.7.2/sample_metadata/model/analysis_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/analysis_query_model.py` & `sample_metadata-5.7.2/sample_metadata/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/analysis_status.py` & `sample_metadata-5.7.2/sample_metadata/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/analysis_type.py` & `sample_metadata-5.7.2/sample_metadata/model/analysis_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/analysis_update_model.py` & `sample_metadata-5.7.2/sample_metadata/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py` & `sample_metadata-5.7.2/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/body_get_participants.py` & `sample_metadata-5.7.2/sample_metadata/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/body_get_samples.py` & `sample_metadata-5.7.2/sample_metadata/model/body_get_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/body_get_sequences_by_criteria.py` & `sample_metadata-5.7.2/sample_metadata/model/body_get_sequences_by_criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/error_response.py` & `sample_metadata-5.7.2/sample_metadata/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/export_type.py` & `sample_metadata-5.7.2/sample_metadata/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/extra_participant_importer_handler.py` & `sample_metadata-5.7.2/sample_metadata/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/family_search_response_data.py` & `sample_metadata-5.7.2/sample_metadata/model/family_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/family_update_model.py` & `sample_metadata-5.7.2/sample_metadata/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/http_validation_error.py` & `sample_metadata-5.7.2/sample_metadata/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/meta_search_entity_prefix.py` & `sample_metadata-5.7.2/sample_metadata/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/nested_family.py` & `sample_metadata-5.7.2/sample_metadata/model/nested_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/nested_participant.py` & `sample_metadata-5.7.2/sample_metadata/model/nested_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/nested_sample.py` & `sample_metadata-5.7.2/sample_metadata/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/nested_sequence.py` & `sample_metadata-5.7.2/sample_metadata/model/nested_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/new_sample.py` & `sample_metadata-5.7.2/sample_metadata/model/new_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/new_sequence.py` & `sample_metadata-5.7.2/sample_metadata/model/new_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/paging_links.py` & `sample_metadata-5.7.2/sample_metadata/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/participant_search_response_data.py` & `sample_metadata-5.7.2/sample_metadata/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/participant_update_model.py` & `sample_metadata-5.7.2/sample_metadata/model/participant_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/participant_upsert.py` & `sample_metadata-5.7.2/sample_metadata/model/participant_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/participant_upsert_body.py` & `sample_metadata-5.7.2/sample_metadata/model/participant_upsert_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/project.py` & `sample_metadata-5.7.2/sample_metadata/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/project_summary_response.py` & `sample_metadata-5.7.2/sample_metadata/model/project_summary_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sample_batch_upsert.py` & `sample_metadata-5.7.2/sample_metadata/model/sample_batch_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sample_batch_upsert_body.py` & `sample_metadata-5.7.2/sample_metadata/model/sample_batch_upsert_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sample_search_response_data.py` & `sample_metadata-5.7.2/sample_metadata/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sample_type.py` & `sample_metadata-5.7.2/sample_metadata/model/sample_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sample_update_model.py` & `sample_metadata-5.7.2/sample_metadata/model/sample_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/search_item.py` & `sample_metadata-5.7.2/sample_metadata/model/search_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/search_response.py` & `sample_metadata-5.7.2/sample_metadata/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/search_response_model.py` & `sample_metadata-5.7.2/sample_metadata/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/search_response_type.py` & `sample_metadata-5.7.2/sample_metadata/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sequence_status.py` & `sample_metadata-5.7.2/sample_metadata/model/sequence_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sequence_technology.py` & `sample_metadata-5.7.2/sample_metadata/model/sequence_technology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sequence_type.py` & `sample_metadata-5.7.2/sample_metadata/model/sequence_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sequence_update_model.py` & `sample_metadata-5.7.2/sample_metadata/model/sequence_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/sequence_upsert.py` & `sample_metadata-5.7.2/sample_metadata/model/sequence_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/validation_error.py` & `sample_metadata-5.7.2/sample_metadata/model/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model/web_project.py` & `sample_metadata-5.7.2/sample_metadata/model/web_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.7.1/sample_metadata/model_utils.py` & `sample_metadata-5.7.2/sample_metadata/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `sample_metadata-5.7.1/sample_metadata/models/__init__.py` & `sample_metadata-5.7.2/sample_metadata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/sample_metadata/parser/cloudhelper.py` & `sample_metadata-5.7.2/sample_metadata/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/sample_metadata/parser/generic_metadata_parser.py` & `sample_metadata-5.7.2/sample_metadata/parser/generic_metadata_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=R0904,too-many-instance-attributes,too-many-locals,unused-argument,wrong-import-order,unused-argument,too-many-arguments,unused-import
 import asyncio
 import logging
 import re
 import shlex
 from functools import reduce
 from io import StringIO
-from typing import Dict, List, Optional, Any, Tuple, Union
+from typing import Dict, List, Optional, Any, Union
 
 import click
 
 from sample_metadata.model.sample_type import SampleType
 from sample_metadata.model.sequence_status import SequenceStatus
 from sample_metadata.model.sequence_technology import SequenceTechnology
 from sample_metadata.model.sequence_type import SequenceType
@@ -733,22 +733,38 @@
 @click.option(
     '--project',
     required=True,
     help='The sample-metadata project ($DATASET) to import manifest into',
 )
 @click.option('--sample-name-column', required=True)
 @click.option(
+    '--participant-column',
+    help='Column where the external participant id is held',
+)
+@click.option(
     '--reads-column',
     help='Column where the reads information is held, comma-separated if multiple',
 )
 @click.option(
     '--gvcf-column',
     help='Column where the reads information is held, comma-separated if multiple',
 )
 @click.option(
+    '--reported-sex-column',
+    help='Column where the reported sex is held',
+)
+@click.option(
+    '--reported-gender-column',
+    help='Column where the reported gender is held',
+)
+@click.option(
+    '--karyotype-column',
+    help='Column where the karyotype is held',
+)
+@click.option(
     '--qc-meta-field-map',
     nargs=2,
     multiple=True,
     help='Two arguments per listing, eg: --qc-meta-field "name-in-manifest" "name-in-analysis.meta"',
 )
 @click.option(
     '--participant-meta-field',
@@ -789,26 +805,30 @@
     '--confirm', is_flag=True, help='Confirm with user input before updating server'
 )
 @click.option('--search-path', multiple=True, required=True)
 @click.argument('manifests', nargs=-1)
 @run_as_sync
 async def main(
     manifests,
-    search_path: List[str],
+    search_path: list[str],
     project,
     sample_name_column: str,
-    participant_meta_field: List[str],
-    participant_meta_field_map: List[Tuple[str, str]],
-    sample_meta_field: List[str],
-    sample_meta_field_map: List[Tuple[str, str]],
-    sequence_meta_field: List[str],
-    sequence_meta_field_map: List[Tuple[str, str]],
-    qc_meta_field_map: List[Tuple[str, str]] = None,
+    participant_meta_field: list[str],
+    participant_meta_field_map: list[tuple[str, str]],
+    sample_meta_field: list[str],
+    sample_meta_field_map: list[tuple[str, str]],
+    sequence_meta_field: list[str],
+    sequence_meta_field_map: list[tuple[str, str]],
+    qc_meta_field_map: list[tuple[str, str]] = None,
     reads_column: Optional[str] = None,
     gvcf_column: Optional[str] = None,
+    participant_column: Optional[str] = None,
+    reported_sex_column: Optional[str] = None,
+    reported_gender_column: Optional[str] = None,
+    karyotype_column: Optional[str] = None,
     default_sample_type='blood',
     default_sequence_type='wgs',
     confirm=False,
 ):
     """Run script from CLI arguments"""
     if not manifests:
         raise ValueError('Expected at least 1 manifest')
@@ -834,20 +854,24 @@
         sequence_meta_map.update(dict(sequence_meta_field_map))
     if sequence_meta_field:
         sequence_meta_map.update({k: k for k in sequence_meta_field})
 
     parser = GenericMetadataParser(
         project=project,
         sample_name_column=sample_name_column,
+        participant_column=participant_column,
         participant_meta_map=participant_meta_map,
         sample_meta_map=sample_meta_map,
         sequence_meta_map=sequence_meta_map,
         qc_meta_map=qc_meta_map,
         reads_column=reads_column,
         gvcf_column=gvcf_column,
+        reported_sex_column=reported_sex_column,
+        reported_gender_column=reported_gender_column,
+        karyotype_column=karyotype_column,
         default_sample_type=default_sample_type,
         default_sequence_type=default_sequence_type,
         search_locations=search_path,
     )
     for manifest in manifests:
         logger.info(f'Importing {manifest}')
```

### Comparing `sample_metadata-5.7.1/sample_metadata/parser/generic_parser.py` & `sample_metadata-5.7.2/sample_metadata/parser/generic_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,17 +392,16 @@
         return AnalysisType(self.default_analysis_type)
 
     # @abstractmethod
     def get_analysis_status(self, sample_id: str, row: GroupedRow) -> AnalysisStatus:
         """Get analysis status from row"""
         return AnalysisStatus(self.default_analysis_status)
 
-    @staticmethod
     def get_existing_external_sequence_ids(
-        participant_map: Dict[str, Dict[Any, List[Any]]]
+        self, participant_map: Dict[str, Dict[Any, List[Any]]]
     ):
         """Pulls external sequence IDs from participant map"""
         external_sequence_ids: list[str] = []
         for participant in participant_map:
             for sample in participant_map[participant]:
                 for sequence in participant_map[participant][sample]:
                     external_sequence_ids.append((sequence.get('Sequence ID')))
@@ -499,14 +498,15 @@
         sample_args: Dict[str, Any] = {
             'meta': collapsed_sample_meta.meta,
             'external_id': external_sample_id,
             'type': self.get_sample_type(rows),
             'sequences': sequences_to_upsert,
         }
         if cpg_sample_id:
+            # If we have a CPG ID, we can update
             sample_args['id'] = cpg_sample_id
 
         sample_to_upsert = SampleBatchUpsert(**sample_args)
 
         if collapsed_analyses:
             analyses_to_add.extend(collapsed_analyses)
 
@@ -1227,23 +1227,25 @@
             if not _checksum:
                 md5_filename = self.file_path(filename + '.md5')
                 if await self.file_exists(md5_filename):
                     contents = await self.file_contents(md5_filename)
                     if contents:
                         _checksum = f'md5:{contents.strip()}'
 
-            file_size, datetime_added = await asyncio.gather(self.file_size(filename), self.datetime_added(filename))
+            file_size, datetime_added = await asyncio.gather(
+                self.file_size(filename), self.datetime_added(filename)
+            )
 
         d = {
             'location': self.file_path(filename),
             'basename': os.path.basename(filename),
             'class': 'File',
             'checksum': _checksum,
             'size': file_size,
-            'datetime_added': datetime_added.isoformat() if datetime_added else None
+            'datetime_added': datetime_added.isoformat() if datetime_added else None,
         }
 
         if secondary_files:
             d['secondaryFiles'] = secondary_files
 
         return d
```

### Comparing `sample_metadata-5.7.1/sample_metadata/parser/sample_file_map_parser.py` & `sample_metadata-5.7.2/sample_metadata/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/sample_metadata/rest.py` & `sample_metadata-5.7.2/sample_metadata/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.7.1
+    The version of the OpenAPI document: 5.7.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `sample_metadata-5.7.1/sample_metadata.egg-info/PKG-INFO` & `sample_metadata-5.7.2/sample_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-metadata
-Version: 5.7.1
+Version: 5.7.2
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sample_metadata-5.7.1/sample_metadata.egg-info/SOURCES.txt` & `sample_metadata-5.7.2/sample_metadata.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 sample_metadata/api/participant_api.py
 sample_metadata/api/project_api.py
 sample_metadata/api/sample_api.py
 sample_metadata/api/seqr_api.py
 sample_metadata/api/sequence_api.py
 sample_metadata/api/web_api.py
 sample_metadata/apis/__init__.py
+sample_metadata/audit/__init__.py
+sample_metadata/audit/audit_upload_bucket.py
+sample_metadata/audit/audithelper.py
+sample_metadata/audit/delete_sequence_files_from_audit.py
+sample_metadata/audit/generic_auditor.py
 sample_metadata/graphql/__init__.py
 sample_metadata/model/__init__.py
 sample_metadata/model/analysis_model.py
 sample_metadata/model/analysis_query_model.py
 sample_metadata/model/analysis_status.py
 sample_metadata/model/analysis_type.py
 sample_metadata/model/analysis_update_model.py
@@ -77,21 +82,24 @@
 sample_metadata/parser/__init__.py
 sample_metadata/parser/cloudhelper.py
 sample_metadata/parser/generic_metadata_parser.py
 sample_metadata/parser/generic_parser.py
 sample_metadata/parser/sample_file_map_parser.py
 test/test_add_samples_for_joint_calling.py
 test/test_analysis.py
+test/test_existing_cohort_parser.py
+test/test_generic_auditor.py
 test/test_get_participants.py
 test/test_import_individual_metadata.py
 test/test_joint_calling_workflow.py
 test/test_parse_file_map.py
 test/test_parse_generic_metadata.py
 test/test_parse_ont_processor.py
 test/test_parse_ont_sheet.py
 test/test_pedigree.py
 test/test_sample.py
 test/test_search.py
 test/test_sequence.py
+test/test_update_participant_family.py
 test/test_upsert.py
 test/test_web.py
 test/testbase.py
```

### Comparing `sample_metadata-5.7.1/setup.py` & `sample_metadata-5.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='5.7.1',
+    version='5.7.2',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `sample_metadata-5.7.1/test/test_add_samples_for_joint_calling.py` & `sample_metadata-5.7.2/test/test_add_samples_for_joint_calling.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_analysis.py` & `sample_metadata-5.7.2/test/test_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=invalid-overridden-method
 from datetime import date, timedelta
 
 from test.testbase import DbIsolatedTest, run_as_sync
 
 from models.enums.sequencing import SequenceType
 from models.enums import AnalysisType, AnalysisStatus
+from models.models.analysis import Analysis
 
 from db.python.layers.analysis import AnalysisLayer
 from db.python.layers.sample import SampleLayer, SampleType
 
 
 class TestAnalysis(DbIsolatedTest):
     """Test sample class"""
@@ -48,14 +49,48 @@
 
         self.assertEqual(1, len(analyses))
 
         self.assertEqual(1, analysis_samples[0]['sample_id'])
         self.assertEqual(analyses[0]['id'], analysis_samples[0]['analysis_id'])
 
     @run_as_sync
+    async def test_get_analysis(self):
+        """
+        Test adding an analysis of type ANALYSIS_RUNNER
+        """
+
+        await self.al.insert_analysis(
+            analysis_type=AnalysisType.ANALYSIS_RUNNER,
+            status=AnalysisStatus.UNKNOWN,
+            # no sample IDs to check join
+            sample_ids=[],
+            meta={},
+        )
+
+        analyses = await self.al.query_analysis(
+            project_ids=[1], analysis_type=AnalysisType.ANALYSIS_RUNNER
+        )
+        expected = [
+            Analysis(
+                id=3,
+                type=AnalysisType.ANALYSIS_RUNNER,
+                status=AnalysisStatus.UNKNOWN,
+                sample_ids=[],
+                output=None,
+                timestamp_completed=None,
+                project=1,
+                meta={},
+                active=True,
+                author='testuser',
+            )
+        ]
+
+        self.assertEqual(analyses, expected)
+
+    @run_as_sync
     async def test_get_sample_file_sizes(self):
         """
         Test retrieval of sample file sizes over time
         """
 
         result = await self.al.get_sample_file_sizes(project_ids=[1])
         expected = [
```

### Comparing `sample_metadata-5.7.1/test/test_get_participants.py` & `sample_metadata-5.7.2/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_import_individual_metadata.py` & `sample_metadata-5.7.2/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_joint_calling_workflow.py` & `sample_metadata-5.7.2/test/test_joint_calling_workflow.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_parse_file_map.py` & `sample_metadata-5.7.2/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_parse_generic_metadata.py` & `sample_metadata-5.7.2/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_parse_ont_processor.py` & `sample_metadata-5.7.2/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_parse_ont_sheet.py` & `sample_metadata-5.7.2/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_pedigree.py` & `sample_metadata-5.7.2/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_sample.py` & `sample_metadata-5.7.2/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_search.py` & `sample_metadata-5.7.2/test/test_search.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_sequence.py` & `sample_metadata-5.7.2/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_upsert.py` & `sample_metadata-5.7.2/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.7.1/test/test_web.py` & `sample_metadata-5.7.2/test/test_web.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,14 +269,15 @@
                                                 'location': '/path/to/sample_id002.filename-R2.fastq.gz',
                                                 'size': 112,
                                             },
                                         ]
                                     ],
                                     'reads_type': 'fastq',
                                     'batch': 'M001',
+                                    'field with spaces': 'some entry',
                                 },
                             },
                         ],
                     }
                 ],
             },
         ]
@@ -342,14 +343,15 @@
                 ('external_id', 'External Sample ID'),
                 ('created_date', 'Created date'),
             ],
             sequence_keys=[
                 ('type', 'type'),
                 ('technology', 'technology'),
                 ('meta.batch', 'batch'),
+                ('meta.field with spaces', 'field with spaces'),
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
 
         two_samples_result = await self.webl.get_project_summary(
@@ -414,14 +416,15 @@
                 ('external_id', 'External Sample ID'),
                 ('created_date', 'Created date'),
             ],
             sequence_keys=[
                 ('type', 'type'),
                 ('technology', 'technology'),
                 ('meta.batch', 'batch'),
+                ('meta.field with spaces', 'field with spaces'),
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
 
         two_samples_result_filtered = await self.webl.get_project_summary(
@@ -437,7 +440,23 @@
                 )
             ],
         )
 
         self.assertEqual(
             expected_data_two_samples_filtered, two_samples_result_filtered
         )
+
+        test_field_with_space = await self.webl.get_project_summary(
+            token=0,
+            grid_filter=[
+                SearchItem(
+                    **{
+                        'model_type': MetaSearchEntityPrefix.SEQUENCE,
+                        'query': 'some',
+                        'field': 'field with spaces',
+                        'is_meta': True,
+                    }
+                )
+            ],
+        )
+
+        self.assertEqual(expected_data_two_samples_filtered, test_field_with_space)
```

### Comparing `sample_metadata-5.7.1/test/testbase.py` & `sample_metadata-5.7.2/test/testbase.py`

 * *Files identical despite different names*

