# Comparing `tmp/encord-0.1.80.tar.gz` & `tmp/encord-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.80.tar", max compression
+gzip compressed data, was "encord-0.1.81.tar", max compression
```

## Comparing `encord-0.1.80.tar` & `encord-0.1.81.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    11330 2023-06-07 13:15:03.082148 encord-0.1.80/LICENSE
--rw-r--r--   0        0        0     2037 2023-06-07 13:15:03.082148 encord-0.1.80/README.md
--rw-r--r--   0        0        0       84 2023-06-07 13:15:03.082148 encord-0.1.80/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-06-07 13:15:03.102149 encord-0.1.80/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-06-07 13:15:03.102149 encord-0.1.80/encord/_version.py
--rw-r--r--   0        0        0    49796 2023-06-07 13:15:03.102149 encord-0.1.80/encord/client.py
--rw-r--r--   0        0        0    10843 2023-06-07 13:15:03.102149 encord-0.1.80/encord/configs.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/enums.py
--rw-r--r--   0        0        0     3293 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-06-07 13:15:03.102149 encord-0.1.80/encord/dataset.py
--rw-r--r--   0        0        0     6351 2023-06-07 13:15:03.102149 encord-0.1.80/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/limits.py
--rw-r--r--   0        0        0     7928 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/classification.py
--rw-r--r--   0        0        0    31069 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/frames.py
--rw-r--r--   0        0        0    21035 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   142513 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/project.py
--rw-r--r--   0        0        0     1289 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-06-07 13:15:03.106149 encord-0.1.80/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/api_key.py
--rw-r--r--   0        0        0     5335 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32800 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      175 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/model.py
--rw-r--r--   0        0        0      823 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/ontology.py
--rw-r--r--   0        0        0     8885 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/workflow.py
--rw-r--r--   0        0        0    39203 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    28768 2023-06-07 13:15:03.106149 encord-0.1.80/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1944 2023-06-07 13:15:03.106149 encord-0.1.80/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.80/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-06-07 16:04:02.858859 encord-0.1.81/LICENSE
+-rw-r--r--   0        0        0     2037 2023-06-07 16:04:02.858859 encord-0.1.81/README.md
+-rw-r--r--   0        0        0       84 2023-06-07 16:04:02.858859 encord-0.1.81/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-07 16:04:02.878859 encord-0.1.81/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-07 16:04:02.878859 encord-0.1.81/encord/_version.py
+-rw-r--r--   0        0        0    49810 2023-06-07 16:04:02.878859 encord-0.1.81/encord/client.py
+-rw-r--r--   0        0        0    10843 2023-06-07 16:04:02.878859 encord-0.1.81/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/enums.py
+-rw-r--r--   0        0        0     3293 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-06-07 16:04:02.878859 encord-0.1.81/encord/dataset.py
+-rw-r--r--   0        0        0     6351 2023-06-07 16:04:02.878859 encord-0.1.81/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/limits.py
+-rw-r--r--   0        0        0     7928 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-06-07 16:04:02.882859 encord-0.1.81/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-06-07 16:04:02.882859 encord-0.1.81/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/classification.py
+-rw-r--r--   0        0        0    31614 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/frames.py
+-rw-r--r--   0        0        0    21035 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   142513 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/project.py
+-rw-r--r--   0        0        0     1289 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-06-07 16:04:02.882859 encord-0.1.81/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5335 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32800 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      175 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/model.py
+-rw-r--r--   0        0        0      823 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8885 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/workflow.py
+-rw-r--r--   0        0        0    39431 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    28768 2023-06-07 16:04:02.886859 encord-0.1.81/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1944 2023-06-07 16:04:02.886859 encord-0.1.81/pyproject.toml
+-rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.81/PKG-INFO
```

### Comparing `encord-0.1.80/LICENSE` & `encord-0.1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/README.md` & `encord-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/client.py` & `encord-0.1.81/encord/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,15 +707,15 @@
 
 
 class EncordClientProject(EncordClient):
     """
     DEPRECATED - prefer using the :class:`encord.project.Project` instead
     """
 
-    def get_project(self, include_labels_metadata=True):
+    def get_project(self, include_labels_metadata=True) -> OrmProject:
         """
         Retrieve project info (pointers to data, labels).
 
         Args:
             include_labels_metadata: if false, label row metadata information will not be returned.
 
         Returns:
```

### Comparing `encord-0.1.80/encord/configs.py` & `encord-0.1.81/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/constants/enums.py` & `encord-0.1.81/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/constants/model.py` & `encord-0.1.81/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/constants/model_weights.py` & `encord-0.1.81/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/constants/string_constants.py` & `encord-0.1.81/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/constants/test/test_enums.py` & `encord-0.1.81/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/dataset.py` & `encord-0.1.81/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/exceptions.py` & `encord-0.1.81/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/bundle.py` & `encord-0.1.81/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/constants.py` & `encord-0.1.81/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/error_utils.py` & `encord-0.1.81/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/querier.py` & `encord-0.1.81/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/query_methods.py` & `encord-0.1.81/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/request.py` & `encord-0.1.81/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/http/utils.py` & `encord-0.1.81/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/bitmask.py` & `encord-0.1.81/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/common.py` & `encord-0.1.81/encord/objects/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     short_uuid_str,
 )
 from encord.orm.project import StringEnum
 
 NestedID = List[int]
 
 
+class PropertyType(StringEnum):
+    RADIO = "radio"
+    TEXT = "text"
+    CHECKLIST = "checklist"
+
+
 class Shape(StringEnum):
     BOUNDING_BOX = "bounding_box"
     POLYGON = "polygon"
     POINT = "point"
     SKELETON = "skeleton"
     POLYLINE = "polyline"
     ROTATABLE_BOUNDING_BOX = "rotatable_bounding_box"
@@ -63,14 +69,19 @@
 
     @property
     def options(self) -> Sequence[Option]:
         return []
 
     @staticmethod
     @abstractmethod
+    def get_property_type() -> PropertyType:
+        pass
+
+    @staticmethod
+    @abstractmethod
     def _get_property_type_name() -> str:
         pass
 
     @abstractmethod
     def _encode_options(self) -> Optional[List[dict]]:
         pass
 
@@ -207,16 +218,20 @@
         self._options = options if options is not None else []
 
     @property
     def options(self) -> Sequence[Option]:
         return self._options
 
     @staticmethod
+    def get_property_type() -> PropertyType:
+        return PropertyType.RADIO
+
+    @staticmethod
     def _get_property_type_name() -> str:
-        return "radio"
+        return PropertyType.RADIO.value
 
     def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
         if len(self._options) == 0:
             return None
         return [option.to_dict() for option in self._options]
 
     def get_child_by_hash(
@@ -293,16 +308,20 @@
         dynamic: bool,
         options: Optional[List[FlatOption]] = None,
     ):
         super().__init__(uid, feature_node_hash, name, required, dynamic)
         self._options = options if options is not None else []
 
     @staticmethod
+    def get_property_type() -> PropertyType:
+        return PropertyType.CHECKLIST
+
+    @staticmethod
     def _get_property_type_name() -> str:
-        return "checklist"
+        return PropertyType.CHECKLIST.value
 
     def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
         if len(self._options) == 0:
             return None
         return [option.to_dict() for option in self._options]
 
     @property
@@ -367,16 +386,20 @@
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
     def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
         super().__init__(uid, feature_node_hash, name, required, dynamic)
 
     @staticmethod
+    def get_property_type() -> PropertyType:
+        return PropertyType.TEXT
+
+    @staticmethod
     def _get_property_type_name() -> str:
-        return "text"
+        return PropertyType.TEXT.value
 
     def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
         return None
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
```

### Comparing `encord-0.1.80/encord/objects/coordinates.py` & `encord-0.1.81/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/frames.py` & `encord-0.1.81/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/internal_helpers.py` & `encord-0.1.81/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/ontology_labels_impl.py` & `encord-0.1.81/encord/objects/ontology_labels_impl.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/project.py` & `encord-0.1.81/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/objects/utils.py` & `encord-0.1.81/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/ontology.py` & `encord-0.1.81/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/api_key.py` & `encord-0.1.81/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/base_orm.py` & `encord-0.1.81/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/dataset.py` & `encord-0.1.81/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/dataset_with_user_role.py` & `encord-0.1.81/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/label_log.py` & `encord-0.1.81/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/label_row.py` & `encord-0.1.81/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/labeling_algorithm.py` & `encord-0.1.81/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/model.py` & `encord-0.1.81/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/ontology.py` & `encord-0.1.81/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/project.py` & `encord-0.1.81/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/project_api_key.py` & `encord-0.1.81/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/project_with_user_role.py` & `encord-0.1.81/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/orm/test/test_dataset.py` & `encord-0.1.81/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/project.py` & `encord-0.1.81/encord/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,27 +113,30 @@
         project_instance = self._get_project_instance()
         return project_instance.datasets
 
     @property
     def label_rows(self) -> dict:
         """
         Get the label rows.
-
-        Prefer using the :meth:`encord.orm.label_row.LabelRowMetadata` class to work with the data.
+        DEPRECATED: Prefer using :meth:`list_label_row_v2()` method and :meth:`LabelRowV2` class to work with the data.
 
         .. code::
 
             from encord.orm.label_row import LabelRowMetadata
 
             project = user_client.get_project("<project_hash>")
 
             label_rows = LabelRowMetadata.from_list(project.label_rows)
 
         """
         project_instance = self._get_project_instance()
+        if project_instance.label_rows is None:
+            project_descriptor = self._client.get_project(include_labels_metadata=True)
+            project_instance.label_rows = project_descriptor.label_rows
+
         return project_instance.label_rows
 
     def refetch_data(self) -> None:
         """
         The Project class will only fetch its properties once. Use this function if you suspect the state of those
         properties to be dirty.
         """
```

### Comparing `encord-0.1.80/encord/project_ontology/classification_attribute.py` & `encord-0.1.81/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/project_ontology/classification_option.py` & `encord-0.1.81/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/project_ontology/ontology.py` & `encord-0.1.81/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/project_ontology/ontology_classification.py` & `encord-0.1.81/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/project_ontology/ontology_object.py` & `encord-0.1.81/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/user_client.py` & `encord-0.1.81/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/utilities/client_utilities.py` & `encord-0.1.81/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/utilities/label_utilities.py` & `encord-0.1.81/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/encord/utilities/project_user.py` & `encord-0.1.81/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.80/pyproject.toml` & `encord-0.1.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.80"
+version = "0.1.81"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.80/PKG-INFO` & `encord-0.1.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.80
+Version: 0.1.81
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.80 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.81 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

