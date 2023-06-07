# Comparing `tmp/encord-0.1.79.tar.gz` & `tmp/encord-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.79.tar", max compression
+gzip compressed data, was "encord-0.1.80.tar", max compression
```

## Comparing `encord-0.1.79.tar` & `encord-0.1.80.tar`

### file list

```diff
@@ -1,74 +1,76 @@
--rw-r--r--   0        0        0    11330 2023-05-31 16:24:21.757835 encord-0.1.79/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-31 16:24:21.757835 encord-0.1.79/README.md
--rw-r--r--   0        0        0       84 2023-05-31 16:24:21.757835 encord-0.1.79/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-05-31 16:24:21.777835 encord-0.1.79/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-05-31 16:24:21.777835 encord-0.1.79/encord/_version.py
--rw-r--r--   0        0        0    49096 2023-05-31 16:24:21.777835 encord-0.1.79/encord/client.py
--rw-r--r--   0        0        0    10843 2023-05-31 16:24:21.777835 encord-0.1.79/encord/configs.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/enums.py
--rw-r--r--   0        0        0     3293 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-05-31 16:24:21.777835 encord-0.1.79/encord/dataset.py
--rw-r--r--   0        0        0     6351 2023-05-31 16:24:21.777835 encord-0.1.79/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/limits.py
--rw-r--r--   0        0        0     7928 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/__init__.py
--rw-r--r--   0        0        0      182 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/classification.py
--rw-r--r--   0        0        0    30906 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/common.py
--rw-r--r--   0        0        0      149 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   140605 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-05-31 16:24:21.777835 encord-0.1.79/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/api_key.py
--rw-r--r--   0        0        0     5335 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32204 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      175 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/model.py
--rw-r--r--   0        0        0      823 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/ontology.py
--rw-r--r--   0        0        0     8885 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    39203 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    28739 2023-05-31 16:24:21.777835 encord-0.1.79/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-05-31 16:24:21.777835 encord-0.1.79/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-05-31 16:24:21.777835 encord-0.1.79/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1944 2023-05-31 16:24:21.781835 encord-0.1.79/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.79/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-06-07 13:15:03.082148 encord-0.1.80/LICENSE
+-rw-r--r--   0        0        0     2037 2023-06-07 13:15:03.082148 encord-0.1.80/README.md
+-rw-r--r--   0        0        0       84 2023-06-07 13:15:03.082148 encord-0.1.80/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-07 13:15:03.102149 encord-0.1.80/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-07 13:15:03.102149 encord-0.1.80/encord/_version.py
+-rw-r--r--   0        0        0    49796 2023-06-07 13:15:03.102149 encord-0.1.80/encord/client.py
+-rw-r--r--   0        0        0    10843 2023-06-07 13:15:03.102149 encord-0.1.80/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/enums.py
+-rw-r--r--   0        0        0     3293 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-07 13:15:03.102149 encord-0.1.80/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-06-07 13:15:03.102149 encord-0.1.80/encord/dataset.py
+-rw-r--r--   0        0        0     6351 2023-06-07 13:15:03.102149 encord-0.1.80/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/limits.py
+-rw-r--r--   0        0        0     7928 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-06-07 13:15:03.102149 encord-0.1.80/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/classification.py
+-rw-r--r--   0        0        0    31069 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/frames.py
+-rw-r--r--   0        0        0    21035 2023-06-07 13:15:03.102149 encord-0.1.80/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   142513 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/project.py
+-rw-r--r--   0        0        0     1289 2023-06-07 13:15:03.106149 encord-0.1.80/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-06-07 13:15:03.106149 encord-0.1.80/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5335 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32800 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      175 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/model.py
+-rw-r--r--   0        0        0      823 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8885 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-06-07 13:15:03.106149 encord-0.1.80/encord/orm/workflow.py
+-rw-r--r--   0        0        0    39203 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-06-07 13:15:03.106149 encord-0.1.80/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    28768 2023-06-07 13:15:03.106149 encord-0.1.80/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-06-07 13:15:03.106149 encord-0.1.80/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1944 2023-06-07 13:15:03.106149 encord-0.1.80/pyproject.toml
+-rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.80/PKG-INFO
```

### Comparing `encord-0.1.79/LICENSE` & `encord-0.1.80/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/README.md` & `encord-0.1.80/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/client.py` & `encord-0.1.80/encord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,19 @@
 from encord.orm.project import Project as OrmProject
 from encord.orm.project import (
     ProjectCopy,
     ProjectCopyOptions,
     ProjectDataset,
     ProjectUsers,
 )
+from encord.orm.workflow import (
+    LabelWorkflowGraphNode,
+    LabelWorkflowGraphNodePayload,
+    WorkflowAction,
+)
 from encord.project_ontology.classification_type import ClassificationType
 from encord.project_ontology.object_type import ObjectShape
 from encord.project_ontology.ontology import Ontology
 from encord.utilities.client_utilities import optional_set_to_list, parse_datetime
 from encord.utilities.project_user import ProjectUser, ProjectUserRole
 
 LONG_POLLING_RESPONSE_RETRY_N = 3
@@ -702,27 +707,30 @@
 
 
 class EncordClientProject(EncordClient):
     """
     DEPRECATED - prefer using the :class:`encord.project.Project` instead
     """
 
-    def get_project(self):
+    def get_project(self, include_labels_metadata=True):
         """
         Retrieve project info (pointers to data, labels).
 
+        Args:
+            include_labels_metadata: if false, label row metadata information will not be returned.
+
         Returns:
             OrmProject: A project record instance.
 
         Raises:
             AuthorisationError: If the project API key is invalid.
             ResourceNotFoundError: If no project exists by the specified project EntityId.
             UnknownError: If an error occurs while retrieving the project.
         """
-        return self._querier.basic_getter(OrmProject)
+        return self._querier.basic_getter(OrmProject, payload={"include_labels_metadata": include_labels_metadata})
 
     def list_label_rows(
         self,
         edited_before: Optional[Union[str, datetime]] = None,
         edited_after: Optional[Union[str, datetime]] = None,
         label_statuses: Optional[List[AnnotationTaskStatus]] = None,
         shadow_data_state: Optional[ShadowDataState] = None,
@@ -1291,16 +1299,25 @@
         payload = {"editor": ontology.to_dict()}
         return self._querier.basic_setter(OrmProject, uid=None, payload=payload)
 
     def workflow_reopen(self, label_hashes: List[str]) -> None:
         """
         This function is documented in :meth:`encord.objects.LabelRowV2.workflow_reopen`.
         """
+        self._querier.basic_setter(
+            LabelWorkflowGraphNode,
+            label_hashes,
+            payload=LabelWorkflowGraphNodePayload({"action": WorkflowAction.REOPEN.value}),
+        )
 
-        # Workaround to make basic_setter generate proper api call
-        class LabelWorkflowGraphNode:
-            pass
-
-        self._querier.basic_setter(LabelWorkflowGraphNode, label_hashes, payload=None)
+    def workflow_complete(self, label_hashes: List[str]) -> None:
+        """
+        This function is documented in :meth:`encord.objects.LabelRowV2.workflow_complete`.
+        """
+        self._querier.basic_setter(
+            LabelWorkflowGraphNode,
+            label_hashes,
+            payload=LabelWorkflowGraphNodePayload({"action": WorkflowAction.COMPLETE.value}),
+        )
 
 
 CordClientProject = EncordClientProject
```

### Comparing `encord-0.1.79/encord/configs.py` & `encord-0.1.80/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/constants/enums.py` & `encord-0.1.80/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/constants/model.py` & `encord-0.1.80/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/constants/model_weights.py` & `encord-0.1.80/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/constants/string_constants.py` & `encord-0.1.80/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/constants/test/test_enums.py` & `encord-0.1.80/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/dataset.py` & `encord-0.1.80/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/exceptions.py` & `encord-0.1.80/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/bundle.py` & `encord-0.1.80/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/constants.py` & `encord-0.1.80/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/error_utils.py` & `encord-0.1.80/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/querier.py` & `encord-0.1.80/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/query_methods.py` & `encord-0.1.80/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/request.py` & `encord-0.1.80/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/http/utils.py` & `encord-0.1.80/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/objects/common.py` & `encord-0.1.80/encord/objects/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from enum import Enum, auto
-from typing import Any, List, Optional, Tuple, Type, TypeVar, Union
+from enum import Enum
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 from encord.exceptions import OntologyError
 from encord.objects.utils import (
     _decode_nested_uid,
     check_type,
     filter_by_type,
     short_uuid_str,
 )
 from encord.orm.project import StringEnum
 
 NestedID = List[int]
 
 
-class PropertyType(StringEnum):
-    RADIO = "radio"
-    TEXT = "text"
-    CHECKLIST = "checklist"
-
-
 class Shape(StringEnum):
     BOUNDING_BOX = "bounding_box"
     POLYGON = "polygon"
     POINT = "point"
     SKELETON = "skeleton"
     POLYLINE = "polyline"
     ROTATABLE_BOUNDING_BOX = "rotatable_bounding_box"
+    BITMASK = "bitmask"
 
 
-@dataclass
 class Attribute(ABC):
     """
     Base class for shared Attribute fields
     """
 
     uid: NestedID
     feature_node_hash: str
@@ -45,203 +50,214 @@
     required: bool
     dynamic: bool
     """
     The `dynamic` member is part of every attribute. However it can only be true for top level (not nested) attributes
     that are part of an :class:`encord.objects.ontology_object.Object`.
     """
 
+    def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
+        self.uid = uid
+        self.feature_node_hash = feature_node_hash
+        self.name = name
+        self.required = required
+        self.dynamic = dynamic
+
+    @property
+    def options(self) -> Sequence[Option]:
+        return []
+
+    @staticmethod
     @abstractmethod
-    def get_property_type(self) -> PropertyType:
+    def _get_property_type_name() -> str:
         pass
 
-    @classmethod
     @abstractmethod
-    def has_options_field(cls) -> bool:
+    def _encode_options(self) -> Optional[List[dict]]:
         pass
 
     @abstractmethod
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
         raise NotImplementedError("This method is not implemented for this class")
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the child node. Only a node that matches this type will be returned.
         """
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
+    def to_dict(self) -> Dict[str, Any]:
+        ret = self._encode_base()
+
+        options = self._encode_options()
+        if options is not None:
+            ret["options"] = options
+
+        return ret
+
     @abstractmethod
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         raise NotImplementedError("This method is not implemented for this class")
 
-    def to_dict(self) -> dict:
-        ret = self._encode_base()
-
-        options = self._encode_options()
-        if options is not None:
-            ret["options"] = options
-
-        return ret
-
     @classmethod
-    def from_dict(cls, d: dict) -> Attribute:
+    def from_dict(cls, d: Dict[str, Any]) -> Attribute:
         property_type = d["type"]
         common_attribute_fields = cls._decode_common_attribute_fields(d)
-        if property_type == "radio":
-            options_ret: List[NestableOption] = list()
-            if "options" in d:
-                for options_dict in d["options"]:
-                    options_ret.append(NestableOption.from_dict(options_dict))
-
+        if property_type == RadioAttribute._get_property_type_name():
             return RadioAttribute(
                 **common_attribute_fields,
-                options=options_ret,
+                options=[NestableOption.from_dict(x) for x in d.get("options", [])],
             )
 
-        elif property_type == "checklist":
-            options_ret: List[FlatOption] = list()
-            if "options" in d:
-                for options_dict in d["options"]:
-                    options_ret.append(FlatOption.from_dict(options_dict))
-
+        elif property_type == ChecklistAttribute._get_property_type_name():
             return ChecklistAttribute(
                 **common_attribute_fields,
-                options=options_ret,
+                options=[FlatOption.from_dict(x) for x in d.get("options", [])],
             )
 
-        elif property_type == "text":
+        elif property_type == TextAttribute._get_property_type_name():
             return TextAttribute(
                 **common_attribute_fields,
             )
 
         raise TypeError(
             f"Attribute is ill-formed: '{d}'. Expected to see either "
             f"attribute specific fields or option specific fields. Got both or none of them."
         )
 
-    def _encode_base(self) -> dict:
-        ret = dict()
+    def _encode_base(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = dict()
         ret["id"] = _decode_nested_uid(self.uid)
         ret["name"] = self.name
-        ret["type"] = self.get_property_type().value
+        ret["type"] = self._get_property_type_name()
         ret["featureNodeHash"] = self.feature_node_hash
         ret["required"] = self.required
         ret["dynamic"] = self.dynamic
 
         return ret
 
-    def _encode_options(self) -> Optional[list]:
-        # pylint: disable-next=no-member
-        if not self.has_options_field() or not self.options:
-            return None
-
-        self: OptionAttribute
-
-        ret = list()
-        for option in self.options:
-            ret.append(option.to_dict())
-        return ret
-
     @staticmethod
-    def _decode_common_attribute_fields(attribute_dict: dict) -> dict:
+    def _decode_common_attribute_fields(attribute_dict: Dict[str, Any]) -> Dict[str, Any]:
         return {
             "uid": _attribute_id_from_json_str(attribute_dict["id"]),
             "feature_node_hash": attribute_dict["featureNodeHash"],
             "name": attribute_dict["name"],
             "required": attribute_dict["required"],
             "dynamic": attribute_dict.get("dynamic", False),
         }
 
+    def __eq__(self, other: object):
+        return (
+            isinstance(other, Attribute) and self.uid == other.uid and self.feature_node_hash == other.feature_node_hash
+        )
+
 
-@dataclass
 class RadioAttribute(Attribute):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
-    options: List[NestableOption] = field(default_factory=list)
+    _options: List[NestableOption]
 
-    def get_property_type(self) -> PropertyType:
-        return PropertyType.RADIO
+    def __init__(
+        self,
+        uid: NestedID,
+        feature_node_hash: str,
+        name: str,
+        required: bool,
+        dynamic: bool,
+        options: Optional[List[NestableOption]] = None,
+    ):
+        super().__init__(uid, feature_node_hash, name, required, dynamic)
+        self._options = options if options is not None else []
 
-    @classmethod
-    def has_options_field(cls) -> bool:
-        return True
+    @property
+    def options(self) -> Sequence[Option]:
+        return self._options
+
+    @staticmethod
+    def _get_property_type_name() -> str:
+        return "radio"
+
+    def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
+        if len(self._options) == 0:
+            return None
+        return [option.to_dict() for option in self._options]
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
-        found_item = _get_option_by_hash(feature_node_hash, self.options)
+        found_item = _get_option_by_hash(feature_node_hash, self._options)
         if found_item is None:
             raise OntologyError("Item not found.")
         check_type(found_item, type_)
         return found_item
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         found_items = _get_options_by_title(title, self.options)
-        return filter_by_type(found_items, type_)  # noqa
+        return filter_by_type(found_items, type_)
 
     def add_option(
         self,
         label: str,
         value: Optional[str] = None,
         local_uid: Optional[int] = None,
         feature_node_hash: Optional[str] = None,
@@ -254,107 +270,122 @@
                     omit this unless the aim is to create an exact clone of existing ontology
             feature_node_hash: global identifier of the option. Normally auto-generated;
                     omit this unless the aim is to create an exact clone of existing ontology
 
         Returns:
             a `NestableOption` instance attached to the attribute. This can be further specified by adding nested attributes.
         """
-        return _add_option(self.options, NestableOption, label, self.uid, local_uid, feature_node_hash, value)
+        return _add_option(self._options, NestableOption, label, self.uid, local_uid, feature_node_hash, value)
 
 
-@dataclass
 class ChecklistAttribute(Attribute):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
-    options: List[FlatOption] = field(default_factory=list)
+    _options: List[FlatOption]
+
+    def __init__(
+        self,
+        uid: NestedID,
+        feature_node_hash: str,
+        name: str,
+        required: bool,
+        dynamic: bool,
+        options: Optional[List[FlatOption]] = None,
+    ):
+        super().__init__(uid, feature_node_hash, name, required, dynamic)
+        self._options = options if options is not None else []
+
+    @staticmethod
+    def _get_property_type_name() -> str:
+        return "checklist"
 
-    def get_property_type(self) -> PropertyType:
-        return PropertyType.CHECKLIST
+    def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
+        if len(self._options) == 0:
+            return None
+        return [option.to_dict() for option in self._options]
 
-    @classmethod
-    def has_options_field(cls) -> bool:
-        return True
+    @property
+    def options(self) -> Sequence[Option]:
+        return self._options
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
-        found_item = _get_option_by_hash(feature_node_hash, self.options)
+        found_item = _get_option_by_hash(feature_node_hash, self._options)
         if found_item is None:
             raise OntologyError("Item not found.")
         check_type(found_item, type_)
         return found_item
 
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+    def get_children_by_title(self, title: str, type_: Optional[OntologyElementType] = None) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         found_items = _get_options_by_title(title, self.options)
-        return filter_by_type(found_items, type_)  # noqa
+        return filter_by_type(found_items, type_)
 
     def add_option(
         self,
         label: str,
         value: Optional[str] = None,
         local_uid: Optional[int] = None,
         feature_node_hash: Optional[str] = None,
-    ):
+    ) -> FlatOption:
         """
         Args:
             label: user-visible name of the option
             value: internal unique value; optional; normally mechanically constructed from the label
             local_uid: integer identifier of the option. Normally auto-generated;
                     omit this unless the aim is to create an exact clone of existing ontology
             feature_node_hash: global identifier of the option. Normally auto-generated;
                     omit this unless the aim is to create an exact clone of existing ontology
         Returns:
             a `FlatOption` instance attached to the attribute.
         """
-        return _add_option(self.options, FlatOption, label, self.uid, local_uid, feature_node_hash, value)
+        return _add_option(self._options, FlatOption, label, self.uid, local_uid, feature_node_hash, value)
 
 
-@dataclass
 class TextAttribute(Attribute):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
-    def get_property_type(self) -> PropertyType:
-        return PropertyType.TEXT
+    def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
+        super().__init__(uid, feature_node_hash, name, required, dynamic)
 
-    @classmethod
-    def has_options_field(cls) -> bool:
-        return False
+    @staticmethod
+    def _get_property_type_name() -> str:
+        return "text"
+
+    def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
+        return None
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         For TextAttributes this will always throw as they have no children.
 
@@ -363,126 +394,116 @@
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
         raise OntologyError("No nested options available for text attributes.")
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         For TextAttributes this will always return an empty list.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         return []
 
 
-OptionAttribute = Union[RadioAttribute, ChecklistAttribute]
 """
 This class is currently in BETA. Its API might change in future minor version releases. 
 """
 
 
 def _attribute_id_from_json_str(attribute_id: str) -> NestedID:
     nested_ids = attribute_id.split(".")
     return [int(x) for x in nested_ids]
 
 
-def attribute_from_dict(d: dict) -> Attribute:
+def attribute_from_dict(d: Dict[str, Any]) -> Attribute:
     """Convenience functions as you cannot call static member on union types."""
     return Attribute.from_dict(d)
 
 
 def attributes_to_list_dict(attributes: List[Attribute]) -> list:
     attributes_list = list()
     for attribute in attributes:
         attributes_list.append(attribute.to_dict())
 
     return attributes_list
 
 
-class OptionType(Enum):
-    FLAT = auto()
-    NESTABLE = auto()
-
-
 @dataclass
 class Option(ABC):
     """
     Base class for shared Option fields
     """
 
     uid: NestedID
     feature_node_hash: str
     label: str
     value: str
 
     @abstractmethod
-    def get_option_type(self) -> OptionType:
+    def is_nestable(self) -> bool:
         pass
 
     @abstractmethod
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
         raise NotImplementedError("This method is not implemented for this class")
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the child node. Only a node that matches this type will be returned.
         """
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
     @abstractmethod
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+    def get_children_by_title(self, title: str, type_: Optional[OntologyElementType] = None) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         raise NotImplementedError("This method is not implemented for this class")
 
-    def to_dict(self) -> dict:
-        ret = dict()
+    def to_dict(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = dict()
         ret["id"] = _decode_nested_uid(self.uid)
         ret["label"] = self.label
         ret["value"] = self.value
         ret["featureNodeHash"] = self.feature_node_hash
 
         nested_options = self._encode_nested_options()
         if nested_options:
@@ -491,37 +512,37 @@
         return ret
 
     @abstractmethod
     def _encode_nested_options(self) -> list:
         pass
 
     @staticmethod
-    def _decode_common_option_fields(option_dict: dict) -> dict:
+    def _decode_common_option_fields(option_dict: Dict[str, Any]) -> Dict[str, Any]:
         return {
             "uid": _attribute_id_from_json_str(option_dict["id"]),
             "label": option_dict["label"],
             "value": option_dict["value"],
             "feature_node_hash": option_dict["featureNodeHash"],
         }
 
 
 @dataclass
 class FlatOption(Option):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
-    def get_option_type(self) -> OptionType:
-        return OptionType.FLAT
+    def is_nestable(self) -> bool:
+        return False
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         For FlatOptions this will always throw as they have no children.
 
@@ -530,16 +551,16 @@
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
         raise OntologyError("No nested attributes for flat options.")
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         For FlatOptions this will always return an empty list.
 
         Args:
@@ -560,22 +581,22 @@
 class NestableOption(Option):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
     nested_options: List[Attribute] = field(default_factory=list)
 
-    def get_option_type(self) -> OptionType:
-        return OptionType.NESTABLE
+    def is_nestable(self) -> bool:
+        return True
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
@@ -586,26 +607,26 @@
             raise OntologyError("Item not found.")
         check_type(found_item, type_)
         return found_item
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         found_items = _get_attributes_by_title(title, self.nested_options)
-        return filter_by_type(found_items, type_)  # noqa
+        return filter_by_type(found_items, type_)
 
     def _encode_nested_options(self) -> list:
         return attributes_to_list_dict(self.nested_options)
 
     @classmethod
     def from_dict(cls, d: dict) -> NestableOption:
         nested_options_ret: List[Attribute] = list()
@@ -646,15 +667,15 @@
         return _add_attribute(self.nested_options, cls, name, self.uid, local_uid, feature_node_hash, required)
 
     def __hash__(self):
         return hash(self.feature_node_hash)
 
 
 def __build_identifiers(
-    existent_items: Union[Attribute, Option],
+    existent_items: Iterable[OntologyElement],
     local_uid: Optional[int] = None,
     feature_node_hash: Optional[str] = None,
 ) -> Tuple[int, str]:
     if local_uid is None:
         if existent_items:
             local_uid = max([item.uid[-1] for item in existent_items]) + 1
         else:
@@ -681,35 +702,27 @@
     parent_uid: List[int],
     local_uid: Optional[int] = None,
     feature_node_hash: Optional[str] = None,
     required: bool = False,
     dynamic: bool = False,
 ) -> T:
     local_uid, feature_node_hash = __build_identifiers(attributes, local_uid, feature_node_hash)
+    attr = cls(
+        name=name, uid=parent_uid + [local_uid], feature_node_hash=feature_node_hash, required=required, dynamic=dynamic
+    )
 
-    constructor_params = {
-        "name": name,
-        "uid": parent_uid + [local_uid],
-        "feature_node_hash": feature_node_hash,
-        "required": required,
-        "dynamic": dynamic,
-    }
-
-    if cls.has_options_field():
-        constructor_params["options"] = []
-    attr = cls(**constructor_params)
     attributes.append(attr)
     return attr
 
 
 OT = TypeVar("OT", bound=Option)
 
 
 def _add_option(
-    options: List[Option],
+    options: List[OT],
     cls: Type[OT],
     label: str,
     parent_uid: List[int],
     local_uid: Optional[int] = None,
     feature_node_hash: Optional[str] = None,
     value: Optional[str] = None,
 ) -> OT:
@@ -717,95 +730,91 @@
     if not value:
         value = re.sub(r"[\s]", "_", label).lower()
     option = cls(parent_uid + [local_uid], feature_node_hash, label, value)
     options.append(option)
     return option
 
 
-def _get_option_by_hash(
-    feature_node_hash: str, options: List[Option]
-) -> Union[RadioAttribute, ChecklistAttribute, TextAttribute, NestableOption, FlatOption, None]:
+def _get_option_by_hash(feature_node_hash: str, options: Iterable[Option]) -> Optional[OntologyElement]:
     for option_ in options:
         if option_.feature_node_hash == feature_node_hash:
             return option_
 
-        if option_.get_option_type() == OptionType.NESTABLE:
+        if option_.is_nestable():
             found_item = _get_attribute_by_hash(feature_node_hash, option_.nested_options)
             if found_item is not None:
                 return found_item
 
     return None
 
 
-def _get_attribute_by_hash(
-    feature_node_hash: str, attributes: List[Attribute]
-) -> Union[RadioAttribute, ChecklistAttribute, TextAttribute, NestableOption, FlatOption, None]:
+def _get_attribute_by_hash(feature_node_hash: str, attributes: List[Attribute]) -> Optional[OntologyElement]:
     for attribute in attributes:
         if attribute.feature_node_hash == feature_node_hash:
             return attribute
 
-        if attribute.has_options_field():
-            found_item = _get_option_by_hash(feature_node_hash, attribute.options)
-            if found_item is not None:
-                return found_item
+        found_item = _get_option_by_hash(feature_node_hash, attribute.options)
+        if found_item is not None:
+            return found_item
     return None
 
 
-def _get_options_by_title(
-    title: str, options: List[Option]
-) -> List[Union[RadioAttribute, ChecklistAttribute, TextAttribute, NestableOption, FlatOption]]:
-    ret = []
+def _get_options_by_title(title: str, options: Iterable[Option]) -> List[OntologyElement]:
+    ret: List[OntologyElement] = []
     for option_ in options:
         if option_.label == title:
             ret.append(option_)
 
-        if option_.get_option_type() == OptionType.NESTABLE:
+        if option_.is_nestable():
             found_items = _get_attributes_by_title(title, option_.nested_options)
             ret.extend(found_items)
 
     return ret
 
 
-def _get_attributes_by_title(
-    title: str, attributes: List[Attribute]
-) -> List[Union[RadioAttribute, ChecklistAttribute, TextAttribute, NestableOption, FlatOption]]:
-    ret = []
+def _get_attributes_by_title(title: str, attributes: List[Attribute]) -> List[OntologyElement]:
+    ret: List[OntologyElement] = []
     for attribute in attributes:
         if attribute.name == title:
             ret.append(attribute)
 
-        if attribute.has_options_field():
-            found_items = _get_options_by_title(title, attribute.options)
-            ret.extend(found_items)
+        found_items = _get_options_by_title(title, attribute.options)
+        ret.extend(found_items)
     return ret
 
 
 def _handle_wrong_number_of_found_items(
-    found_items: List[Union[RadioAttribute, ChecklistAttribute, TextAttribute, NestableOption, FlatOption]],
+    found_items: List[OntologyElement],
     title: str,
     type_: Any,
 ) -> None:
     if len(found_items) == 0:
         raise OntologyError(f"No item was found in the ontology with the given title `{title}` and type `{type_}`")
     elif len(found_items) > 1:
         raise OntologyError(
             f"More than one item was found in the ontology with the given title `{title}` and type `{type_}`. "
             f"Use the `get_children_by_title` or `get_child_by_hash` function instead. "
             f"The found items are `{found_items}`."
         )
 
 
+OptionAttribute = Union[RadioAttribute, ChecklistAttribute]
+OntologyElement = Union[Attribute, Option]
 AttributeTypes = Union[
     Type[RadioAttribute],
     Type[ChecklistAttribute],
     Type[TextAttribute],
     Type[Attribute],
 ]
-AttributeClasses = Union[RadioAttribute, ChecklistAttribute, TextAttribute, Attribute]
 OptionTypes = Union[Type[FlatOption], Type[NestableOption], Type[Option]]
+OntologyElementType = Union[AttributeTypes, OptionTypes]
+
+# Two types below are kept for the backwards compatibility
+# Please don't use them, as they are going to be removed in the future versions
+AttributeClasses = Union[RadioAttribute, ChecklistAttribute, TextAttribute, Attribute]
 OptionClasses = Union[FlatOption, NestableOption, Option]
 
 
 class DeidentifyRedactTextMode(Enum):
     REDACT_ALL_TEXT = "REDACT_ALL_TEXT"
     REDACT_NO_TEXT = "REDACT_NO_TEXT"
     REDACT_SENSITIVE_TEXT = "REDACT_SENSITIVE_TEXT"
@@ -818,29 +827,29 @@
 
 @dataclass
 class SaveDeidentifiedDicomConditionIn:
     value: List[str]
     dicom_tag: str
     condition_type: SaveDeidentifiedDicomConditionType = SaveDeidentifiedDicomConditionType.IN
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> Dict[str, Any]:
         return {
             "value": self.value,
             "dicom_tag": self.dicom_tag,
             "condition_type": self.condition_type.value,
         }
 
 
 @dataclass
 class SaveDeidentifiedDicomConditionNotSubstr:
     value: str
     dicom_tag: str
     condition_type: SaveDeidentifiedDicomConditionType = SaveDeidentifiedDicomConditionType.NOT_SUBSTR
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> Dict[str, Any]:
         return {
             "value": self.value,
             "dicom_tag": self.dicom_tag,
             "condition_type": self.condition_type.value,
         }
```

### Comparing `encord-0.1.79/encord/objects/coordinates.py` & `encord-0.1.80/encord/objects/coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Flag, auto
 from typing import Dict, List, Optional, Type, Union
 
+from encord.objects.bitmask import BitmaskCoordinates
 from encord.objects.common import Shape
 
 
 @dataclass(frozen=True)
 class BoundingBoxCoordinates:
     """All the values are percentages relative to the total image size."""
 
@@ -182,16 +183,18 @@
 Coordinates = Union[
     BoundingBoxCoordinates,
     RotatableBoundingBoxCoordinates,
     PointCoordinate,
     PolygonCoordinates,
     PolylineCoordinates,
     SkeletonCoordinates,
+    BitmaskCoordinates,
 ]
 ACCEPTABLE_COORDINATES_FOR_ONTOLOGY_ITEMS: Dict[Shape, Type[Coordinates]] = {
     Shape.BOUNDING_BOX: BoundingBoxCoordinates,
     Shape.ROTATABLE_BOUNDING_BOX: RotatableBoundingBoxCoordinates,
     Shape.POINT: PointCoordinate,
     Shape.POLYGON: PolygonCoordinates,
     Shape.POLYLINE: PolylineCoordinates,
     Shape.SKELETON: SkeletonCoordinates,
+    Shape.BITMASK: BitmaskCoordinates,
 }
```

### Comparing `encord-0.1.79/encord/objects/frames.py` & `encord-0.1.80/encord/objects/frames.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Collection, List, Union
+from typing import Collection, List, Union, cast
 
 
 @dataclass
 class Range:
     start: int
     end: int
 
@@ -119,14 +119,14 @@
     """
     if isinstance(frames_class, int):
         return [frames_class]
     elif isinstance(frames_class, Range):
         return range_to_frames(frames_class)
     elif isinstance(frames_class, list):
         if all([isinstance(x, int) for x in frames_class]):
-            return sorted(list(set(frames_class)))
+            return cast(List[int], sorted(list(set(frames_class))))
         elif all([isinstance(x, Range) for x in frames_class]):
-            return ranges_to_frames(frames_class)
+            return ranges_to_frames(cast(List[Range], frames_class))
         else:
             raise RuntimeError("Unexpected type for frames.")
     else:
         raise RuntimeError("Unexpected type for frames.")
```

### Comparing `encord-0.1.79/encord/objects/internal_helpers.py` & `encord-0.1.80/encord/objects/internal_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from encord.exceptions import LabelRowError
 from encord.objects.common import (
     Attribute,
     ChecklistAttribute,
     FlatOption,
     NestableOption,
     Option,
-    OptionType,
-    PropertyType,
     RadioAttribute,
     TextAttribute,
     _get_option_by_hash,
 )
 from encord.objects.constants import DEFAULT_MANUAL_ANNOTATION
 from encord.objects.frames import Ranges, ranges_to_list
 from encord.objects.utils import _lower_snake_case, short_uuid_str
@@ -62,49 +60,49 @@
     def ontology_attribute(self):
         return deepcopy(self._ontology_attribute)
 
     @ontology_attribute.setter
     def ontology_attribute(self, v: Any) -> NoReturn:
         raise RuntimeError("Cannot reset the ontology attribute of an instantiated answer.")
 
-    def to_encord_dict(self, ranges: Optional[Ranges] = None) -> Optional[Dict]:
+    def to_encord_dict(self, ranges: Optional[Ranges] = None) -> Optional[Dict[str, Any]]:
         """
         A low level helper to convert to the Encord JSON format.
         For most use cases the `get_answer` function should be used instead.
         """
         if not self.is_answered():
             return None
 
         ret = self._to_encord_dict_impl(self.is_dynamic)
         if self.is_dynamic:
             ret.update(self._get_encord_dynamic_fields(ranges))
 
         return ret
 
     @abstractmethod
-    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict:
+    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         pass
 
     @abstractmethod
-    def from_dict(self, d: Dict) -> None:
+    def from_dict(self, d: Dict[str, Any]) -> None:
         pass
 
-    def _get_encord_dynamic_fields(self, ranges: Ranges) -> Dict:
+    def _get_encord_dynamic_fields(self, ranges: Ranges) -> Dict[str, Any]:
         return {
             "dynamic": True,
             "range": ranges_to_list(ranges),
             "shouldPropagate": self._should_propagate,
             "trackHash": self._track_hash,
         }
 
 
 class TextAnswer(Answer):
     def __init__(self, ontology_attribute: TextAttribute):
         super().__init__(ontology_attribute)
-        self._value = None
+        self._value: Optional[str] = None
 
     def set(self, value: str) -> TextAnswer:
         """Returns the object itself"""
         if not isinstance(value, str):
             raise ValueError("TextAnswer can only be set to a string.")
         self._value = value
         self._answered = True
@@ -124,42 +122,42 @@
         other_is_answered = text_answer.is_answered()
         if not other_is_answered:
             self.unset()
         else:
             other_answer = text_answer.get_value()
             self.set(other_answer)
 
-    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict:
+    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         return {
             "name": self.ontology_attribute.name,
             "value": _lower_snake_case(self.ontology_attribute.name),
             "answers": self._value,
             "featureHash": self.ontology_attribute.feature_node_hash,
             "manualAnnotation": self.is_manual_annotation,
         }
 
-    def from_dict(self, d: Dict) -> None:
+    def from_dict(self, d: Dict[str, Any]) -> None:
         if d["featureHash"] != self.ontology_attribute.feature_node_hash:
             raise ValueError("Cannot set the value of a TextAnswer based on a different ontology attribute.")
 
         self._answered = True
         self.set(d["answers"])
         self.is_manual_annotation = d["manualAnnotation"]
 
     def __hash__(self):
         return hash((self._ontology_attribute.feature_node_hash, self._value, type(self).__name__))
 
-    def __eq__(self, other: TextAnswer) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, TextAnswer):
             return False
-        else:
-            return (
-                self._ontology_attribute.feature_node_hash == other._ontology_attribute.feature_node_hash
-                and self._value == other._value
-            )
+
+        return (
+            self._ontology_attribute.feature_node_hash == other._ontology_attribute.feature_node_hash
+            and self._value == other._value
+        )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._value})"
 
 
 @dataclass
 class RadioAnswer(Answer):
@@ -197,15 +195,15 @@
         other_is_answered = radio_answer.is_answered()
         if not other_is_answered:
             self.unset()
         else:
             other_answer = radio_answer.get_value()
             self.set(other_answer)
 
-    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Optional[Dict]:
+    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         nestable_option = self._value
 
         return {
             "name": self.ontology_attribute.name,
             "value": _lower_snake_case(self.ontology_attribute.name),
             "answers": [
                 {
@@ -231,22 +229,22 @@
         nestable_option = _get_option_by_hash(answer["featureHash"], self.ontology_attribute.options)
         self.set(nestable_option)
         self.is_manual_annotation = d["manualAnnotation"]
 
     def __hash__(self):
         return hash((self.ontology_attribute.feature_node_hash, self._value, type(self).__name__))
 
-    def __eq__(self, other: RadioAnswer) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, RadioAnswer):
             return False
-        else:
-            return (
-                self._ontology_attribute.feature_node_hash == other._ontology_attribute.feature_node_hash
-                and self._value == other._value
-            )
+
+        return (
+            self._ontology_attribute.feature_node_hash == other._ontology_attribute.feature_node_hash
+            and self._value == other._value
+        )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._value})"
 
 
 @dataclass
 class ChecklistAnswer(Answer):
@@ -328,15 +326,15 @@
     def _verify_flat_option(self, value: FlatOption) -> None:
         if value.feature_node_hash not in self._ontology_options_feature_hashes:
             raise RuntimeError(
                 f"The supplied FlatOption `{value}` is not a child of the ChecklistAttribute that "
                 f"is associated with this class: `{self._ontology_attribute}`"
             )
 
-    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Optional[Dict]:
+    def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         checked_options = []
         ontology_attribute: ChecklistAttribute = self._ontology_attribute
         for option in ontology_attribute.options:
             if self.get_value(option):
                 checked_options.append(option)
 
         answers = []
@@ -352,15 +350,15 @@
             "name": self.ontology_attribute.name,
             "value": _lower_snake_case(self.ontology_attribute.name),
             "answers": answers,
             "featureHash": self.ontology_attribute.feature_node_hash,
             "manualAnnotation": self.is_manual_annotation,
         }
 
-    def from_dict(self, d: Dict) -> None:
+    def from_dict(self, d: Dict[str, Any]) -> None:
         if d["featureHash"] != self.ontology_attribute.feature_node_hash:
             raise ValueError("Cannot set the value of a ChecklistAnswer based on a different ontology attribute.")
 
         answers = d["answers"]
         if len(answers) == 0:
             return
 
@@ -372,34 +370,33 @@
         self._answered = True
 
     def __hash__(self):
         flat_values = [(key, value) for key, value in self._feature_hash_to_answer_map.items()]
         flat_values.sort()
         return hash((tuple(flat_values), type(self).__name__))
 
-    def __eq__(self, other: ChecklistAnswer) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, ChecklistAnswer):
             return False
-        else:
-            flat_values = {(key, value) for key, value in self._feature_hash_to_answer_map.items()}
-            other_flat_values = {(key, value) for key, value in other._feature_hash_to_answer_map.items()}
-            return flat_values == other_flat_values
+
+        flat_values = {(key, value) for key, value in self._feature_hash_to_answer_map.items()}
+        other_flat_values = {(key, value) for key, value in other._feature_hash_to_answer_map.items()}
+        return flat_values == other_flat_values
 
     def __repr__(self):
         flat_values = [(key, value) for key, value in self._feature_hash_to_answer_map.items()]
         return f"{self.__class__.__name__}({flat_values})"
 
 
 def get_default_answer_from_attribute(attribute: Attribute) -> Answer:
-    property_type = attribute.get_property_type()
-    if property_type == PropertyType.TEXT:
+    if isinstance(attribute, TextAttribute):
         return TextAnswer(attribute)
-    elif property_type == PropertyType.RADIO:
+    elif isinstance(attribute, RadioAttribute):
         return RadioAnswer(attribute)
-    elif property_type == PropertyType.CHECKLIST:
+    elif isinstance(attribute, ChecklistAttribute):
         return ChecklistAnswer(attribute)
     else:
         raise RuntimeError(f"Got an attribute with an unexpected property type: {attribute}")
 
 
 def set_answer_for_object(answer_object: Answer, answer_value: Union[str, Option, Iterable[Option]]) -> None:
     attribute = answer_object.ontology_attribute
@@ -428,19 +425,18 @@
 def _get_default_static_answers_from_attributes(attributes: List[Attribute]) -> List[Answer]:
     ret: List[Answer] = list()
     for attribute in attributes:
         if not attribute.dynamic:
             answer = get_default_answer_from_attribute(attribute)
             ret.append(answer)
 
-        if attribute.has_options_field():
-            for option in attribute.options:
-                if option.get_option_type() == OptionType.NESTABLE:
-                    other_attributes = _get_default_static_answers_from_attributes(option.nested_options)
-                    ret.extend(other_attributes)
+        for option in attribute.options:
+            if option.is_nestable():
+                other_attributes = _get_default_static_answers_from_attributes(option.nested_options)
+                ret.extend(other_attributes)
 
     return ret
 
 
 def _get_static_answer_map(attributes: List[Attribute]) -> Dict[str, Answer]:
     answers = _get_default_static_answers_from_attributes(attributes)
     answer_map = {answer.ontology_attribute.feature_node_hash: answer for answer in answers}
@@ -469,34 +465,33 @@
                     return True
 
     return False
 
 
 def _search_for_parent(passed_option: Option, attributes: List[Attribute]) -> Optional[Attribute]:
     for attribute in attributes:
-        if attribute.has_options_field():
-            for option in attribute.options:
-                if option == passed_option:
-                    return attribute
-                if option.get_option_type() == OptionType.NESTABLE:
-                    attribute_opt = _search_for_parent(passed_option, option.nested_options)
-                    if attribute_opt is not None:
-                        return attribute_opt
+        for option in attribute.options:
+            if option == passed_option:
+                return attribute
+            if option.is_nestable():
+                attribute_opt = _search_for_parent(passed_option, option.nested_options)
+                if attribute_opt is not None:
+                    return attribute_opt
     return None
 
 
 def _search_for_text_attributes(attributes: List[Attribute]) -> List[Attribute]:
     text_attributes: List[Attribute] = list()
     for attribute in attributes:
-        if attribute.get_property_type() == PropertyType.TEXT:
+        if isinstance(attribute, TextAttribute):
             text_attributes.append(attribute)
-        elif attribute.has_options_field():
-            for option in attribute.options:
-                if option.get_option_type() == OptionType.NESTABLE:
-                    text_attributes.extend(_search_for_text_attributes(option.nested_options))
+
+        for option in attribute.options:
+            if option.is_nestable():
+                text_attributes.extend(_search_for_text_attributes(option.nested_options))
     return text_attributes
 
 
 def _infer_attribute_from_answer(
     attributes: List[Attribute], answer: Union[str, Option, Sequence[Option]]
 ) -> Attribute:
     if isinstance(answer, Option):
```

### Comparing `encord-0.1.79/encord/objects/ontology_labels_impl.py` & `encord-0.1.80/encord/objects/ontology_labels_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,24 @@
 from encord.exceptions import LabelRowError, OntologyError, WrongProjectTypeError
 from encord.http.bundle import Bundle, BundleResultHandler, BundleResultMapper
 from encord.http.limits import (
     LABEL_ROW_BUNDLE_CREATE_LIMIT,
     LABEL_ROW_BUNDLE_GET_LIMIT,
     LABEL_ROW_BUNDLE_SAVE_LIMIT,
 )
+from encord.objects.common import AttributeClasses  # pylint: disable=unused-import
+from encord.objects.common import AttributeTypes  # pylint: disable=unused-import
+from encord.objects.common import OptionClasses  # pylint: disable=unused-import
+from encord.objects.common import OptionTypes  # pylint: disable=unused-import
 from encord.objects.common import (
     Attribute,
-    AttributeClasses,
-    AttributeTypes,
     ChecklistAttribute,
+    OntologyElement,
+    OntologyElementType,
     Option,
-    OptionClasses,
-    OptionTypes,
     RadioAttribute,
     Shape,
     TextAttribute,
     _add_attribute,
     _get_attribute_by_hash,
     _get_attributes_by_title,
     _get_option_by_hash,
@@ -56,14 +58,15 @@
 from encord.objects.constants import (
     DATETIME_LONG_STRING_FORMAT,
     DEFAULT_CONFIDENCE,
     DEFAULT_MANUAL_ANNOTATION,
 )
 from encord.objects.coordinates import (
     ACCEPTABLE_COORDINATES_FOR_ONTOLOGY_ITEMS,
+    BitmaskCoordinates,
     BoundingBoxCoordinates,
     Coordinates,
     PointCoordinate,
     PolygonCoordinates,
     PolylineCoordinates,
     RotatableBoundingBoxCoordinates,
 )
@@ -119,16 +122,16 @@
     def create_instance(self) -> ObjectInstance:
         """Create a :class:`encord.objects.ObjectInstance` to be used with a label row."""
         return ObjectInstance(self)
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
@@ -139,16 +142,16 @@
             raise OntologyError("Item not found.")
         check_type(found_item, type_)
         return found_item
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
@@ -157,26 +160,26 @@
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         found_items = _get_attributes_by_title(title, self.attributes)
-        return filter_by_type(found_items, type_)  # noqa
+        return filter_by_type(found_items, type_)
 
     @classmethod
     def from_dict(cls, d: dict) -> Object:
         shape_opt = Shape.from_string(d["shape"])
         if shape_opt is None:
             raise TypeError(f"The shape '{d['shape']}' of the object '{d}' is not recognised")
 
@@ -192,16 +195,16 @@
             shape=shape_opt,
             feature_node_hash=d["featureNodeHash"],
             attributes=attributes_ret,
         )
 
         return object_ret
 
-    def to_dict(self) -> dict:
-        ret = dict()
+    def to_dict(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = dict()
         ret["id"] = str(self.uid)
         ret["name"] = self.name
         ret["color"] = self.color
         ret["shape"] = self.shape.value
         ret["featureNodeHash"] = self.feature_node_hash
 
         attributes_list = attributes_to_list_dict(self.attributes)
@@ -259,16 +262,16 @@
     def create_instance(self) -> ClassificationInstance:
         """Create a :class:`encord.objects.ClassificationInstance` to be used with a label row."""
         return ClassificationInstance(self)
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
@@ -279,16 +282,16 @@
             raise OntologyError("Item not found.")
         check_type(found_item, type_)
         return found_item
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Union[OptionTypes, AttributeTypes, None] = None,
-    ) -> Union[AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
@@ -297,41 +300,41 @@
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[OptionTypes, AttributeTypes, None] = None,
-    ) -> List[Union[AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         found_items = _get_attributes_by_title(title, self.attributes)
-        return filter_by_type(found_items, type_)  # noqa
+        return filter_by_type(found_items, type_)
 
     @classmethod
     def from_dict(cls, d: dict) -> Classification:
         attributes_ret: List[Attribute] = list()
         for attribute_dict in d["attributes"]:
             attributes_ret.append(attribute_from_dict(attribute_dict))
 
         return Classification(
             uid=int(d["id"]),
             feature_node_hash=d["featureNodeHash"],
             attributes=attributes_ret,
         )
 
-    def to_dict(self) -> dict:
-        ret = dict()
+    def to_dict(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = dict()
         ret["id"] = str(self.uid)
         ret["featureNodeHash"] = self.feature_node_hash
 
         attributes_list = attributes_to_list_dict(self.attributes)
         if attributes_list:
             ret["attributes"] = attributes_list
 
@@ -423,16 +426,16 @@
 
     def set_for_frames(
         self,
         frames: Frames = 0,
         *,
         overwrite: bool = False,
         created_at: Optional[datetime] = None,
-        created_by: str = None,
-        confidence: int = DEFAULT_CONFIDENCE,
+        created_by: Optional[str] = None,
+        confidence: float = DEFAULT_CONFIDENCE,
         manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION,
         last_edited_at: Optional[datetime] = None,
         last_edited_by: Optional[str] = None,
         reviews: Optional[List[dict]] = None,
     ) -> None:
         """
         Places the classification onto the specified frame. If the classification already exists on the frame and
@@ -734,15 +737,15 @@
 
         @manual_annotation.setter
         def manual_annotation(self, manual_annotation: bool) -> None:
             self._check_if_frame_view_valid()
             self._get_object_frame_instance_data().manual_annotation = manual_annotation
 
         @property
-        def reviews(self) -> List[dict]:
+        def reviews(self) -> Optional[List[dict]]:
             """
             A read only property about the reviews that happened for this object on this frame.
             """
             self._check_if_frame_view_valid()
             return self._get_object_frame_instance_data().reviews
 
         def _check_if_frame_view_valid(self) -> None:
@@ -754,15 +757,15 @@
         def _get_object_frame_instance_data(self) -> ClassificationInstance.FrameData:
             return self._classification_instance._frames_to_data[self._frame]
 
     @dataclass
     class FrameData:
         created_at: datetime = field(default_factory=datetime.now)
         created_by: Optional[str] = None
-        confidence: int = DEFAULT_CONFIDENCE
+        confidence: float = DEFAULT_CONFIDENCE
         manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION
         last_edited_at: datetime = field(default_factory=datetime.now)
         last_edited_by: Optional[str] = None
         reviews: Optional[List[dict]] = None
 
         @staticmethod
         def from_dict(d: dict) -> ClassificationInstance.FrameData:
@@ -781,15 +784,15 @@
                 reviews=d.get("reviews"),
             )
 
         def update_from_optional_fields(
             self,
             created_at: Optional[datetime] = None,
             created_by: Optional[str] = None,
-            confidence: Optional[int] = None,
+            confidence: Optional[float] = None,
             manual_annotation: Optional[bool] = None,
             last_edited_at: Optional[datetime] = None,
             last_edited_by: Optional[str] = None,
             reviews: Optional[List[dict]] = None,
         ) -> None:
             self.created_at = created_at or self.created_at
             if created_by is not None:
@@ -807,15 +810,15 @@
     def _set_frame_and_frame_data(
         self,
         frame,
         *,
         overwrite: bool = False,
         created_at: Optional[datetime] = None,
         created_by: Optional[str] = None,
-        confidence: Optional[int] = None,
+        confidence: Optional[float] = None,
         manual_annotation: Optional[bool] = None,
         last_edited_at: Optional[datetime] = None,
         last_edited_by: Optional[str] = None,
         reviews: Optional[List[dict]] = None,
     ):
         existing_frame_data = self._frames_to_data.get(frame)
         if overwrite is False and existing_frame_data is not None:
@@ -1046,15 +1049,15 @@
     def ontology_structure(self) -> OntologyStructure:
         """Get the corresponding ontology structure"""
         return self._ontology.structure
 
     @property
     def is_labelling_initialised(self) -> bool:
         """
-        Whether you can start labelling or not. If this is `False`, call the member `.initialise_labels()` to
+        Whether you can start labelling or not. If this is `False`, call the member :meth:`.initialise_labels()` to
         read or write specific ObjectInstances or ClassificationInstances.
         """
         return self._is_labelling_initialised
 
     @property
     def __is_tms2_project(self) -> bool:
         return self.workflow_graph_node is not None
@@ -1136,28 +1139,28 @@
         include_classification_feature_hashes,
         include_reviews,
     ):
         if self.label_hash is None:
             bundle.add(
                 operation=self._project_client.create_label_rows,
                 request_reducer=self._bundle_create_rows_reducer,
-                result_mapper=BundleResultMapper(
+                result_mapper=BundleResultMapper[OrmLabelRow](
                     result_mapping_predicate=self._bundle_create_rows_mapping_predicate,
                     result_handler=BundleResultHandler(predicate=self.data_hash, handler=self.from_labels_dict),
                 ),
                 payload=BundledCreateRowsPayload(
                     uids=[self.data_hash],
                 ),
                 limit=LABEL_ROW_BUNDLE_CREATE_LIMIT,
             )
         else:
             bundle.add(
                 operation=self._project_client.get_label_rows,
                 request_reducer=self._bundle_get_rows_reducer,
-                result_mapper=BundleResultMapper(
+                result_mapper=BundleResultMapper[OrmLabelRow](
                     result_mapping_predicate=self._bundle_get_rows_mapping_predicate,
                     result_handler=BundleResultHandler(predicate=self.label_hash, handler=self.from_labels_dict),
                 ),
                 payload=BundledGetRowsPayload(
                     uids=[uid],
                     get_signed_url=get_signed_url,
                     include_object_feature_hashes=include_object_feature_hashes,
@@ -1201,18 +1204,18 @@
         Args:
             label_row_dict: The dictionary of all labels as expected by the Encord format.
         """
         self._is_labelling_initialised = True
 
         self._label_row_read_only_data = self._parse_label_row_dict(label_row_dict)
         self._frame_to_hashes = defaultdict(set)
-        self._classifications_to_frames: defaultdict[Classification, Set[int]] = defaultdict(set)
+        self._classifications_to_frames = defaultdict(set)
 
-        self._objects_map: Dict[str, ObjectInstance] = dict()
-        self._classifications_map: Dict[str, ClassificationInstance] = dict()
+        self._objects_map = dict()
+        self._classifications_map = dict()
         self._parse_labels_from_dict(label_row_dict)
 
     def get_image_hash(self, frame_number: int) -> Optional[str]:
         """
         Get the corresponding image hash of the frame number. Return `None` if the frame number is out of bounds.
         Raise an error if this function is used for non-image data types.
         """
@@ -1231,15 +1234,15 @@
         """
         self._check_labelling_is_initalised()
 
         if self.data_type not in (DataType.IMAGE, DataType.IMG_GROUP):
             raise LabelRowError("This function is only supported for label rows of image or image group data types.")
         return self._label_row_read_only_data.image_hash_to_frame[image_hash]
 
-    def save(self, bundle: Bundle = None) -> None:
+    def save(self, bundle: Optional[Bundle] = None) -> None:
         """
         Upload the created labels with the Encord server. This will overwrite any labels that someone has created
         in the platform in the meantime.
 
         Args:
             bundle: if not passed, save is executed immediately. If passed, it is executed as a part of the bundle
         """
@@ -1488,22 +1491,22 @@
 
         self._objects_map.pop(object_instance.object_hash)
         self._remove_from_frame_to_hashes_map(
             _frame_views_to_frame_numbers(object_instance.get_annotations()), object_instance.object_hash
         )
         object_instance._parent = None
 
-    def to_encord_dict(self) -> dict:
+    def to_encord_dict(self) -> Dict[str, Any]:
         """
         This is an internal helper function. Likely this should not be used by a user. To upload labels use the
         :meth:`.save()` function.
         """
         self._check_labelling_is_initalised()
 
-        ret = {}
+        ret: Dict[str, Any] = {}
         read_only_data = self._label_row_read_only_data
 
         ret["label_hash"] = read_only_data.label_hash
         ret["created_at"] = read_only_data.created_at
         ret["last_edited_at"] = read_only_data.last_edited_at
         ret["data_hash"] = read_only_data.data_hash
         ret["dataset_hash"] = read_only_data.dataset_hash
@@ -1518,25 +1521,45 @@
         ret["label_status"] = read_only_data.label_status.value
         ret["data_units"] = self._to_encord_data_units()
 
         return ret
 
     def workflow_reopen(self) -> None:
         """
-        A label row is returned to the first annotation stage for re-labeling. No data is lost during the call.
+        A label row is returned to the first annotation stage for re-labeling.
         No data will be lost during this call.
-        This method is only relevant for the projects that use the Encord Task Management System 2,
-        and does nothing for other types of projects
+
+        This method is only relevant for the projects that use the :ref:`Workflow <tutorials/workflows:Workflows>`
+        feature, and will raise an error for pre-workflow projects.
         """
         if self.label_hash is None:
             # Label has not yet moved from the initial state, nothing to do
             return
 
         self._project_client.workflow_reopen([self.label_hash])
 
+    def workflow_complete(self) -> None:
+        """
+         A label row is moved to the final workflow node, marking it as 'Complete'.
+
+         This method can be called only for labels for which :meth:`.initialise_labels()` was called at least ance, and
+         consequentially the "label_hash" field is not `None`.
+        Please note that labels need not be initialized every time the workflow_complete() method is called.
+
+         This method is only relevant for the projects that use the :ref:`Workflow <tutorials/workflows:Workflows>`
+         feature, and will raise an error for projects that don't use Workflows.
+        """
+        if self.label_hash is None:
+            raise LabelRowError(
+                "For this operation you will need to initialise labelling first. Call the .initialise_labels() "
+                "to do so first."
+            )
+
+        self._project_client.workflow_complete([self.label_hash])
+
     class FrameView:
         """
         This class can be used to inspect what object/classification instances are on a given frame or
         what metadata, such as a image file size, is on a given frame.
         """
 
         def __init__(
@@ -1625,16 +1648,16 @@
 
         def add_classification_instance(
             self,
             classification_instance: ClassificationInstance,
             *,
             overwrite: bool = False,
             created_at: Optional[datetime] = None,
-            created_by: str = None,
-            confidence: int = DEFAULT_CONFIDENCE,
+            created_by: Optional[str] = None,
+            confidence: float = DEFAULT_CONFIDENCE,
             manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION,
             last_edited_at: Optional[datetime] = None,
             last_edited_by: Optional[str] = None,
         ) -> None:
             if created_at is None:
                 created_at = datetime.now()
 
@@ -1733,38 +1756,38 @@
         width: Optional[int]
         height: Optional[int]
         data_link: Optional[str]
         frame_level_data: Dict[int, LabelRowV2.FrameLevelImageGroupData] = field(default_factory=dict)
         image_hash_to_frame: Dict[str, int] = field(default_factory=dict)
         frame_to_image_hash: Dict[int, str] = field(default_factory=dict)
 
-    def _to_object_answers(self) -> dict:
-        ret = {}
+    def _to_object_answers(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
         for obj in self._objects_map.values():
             all_static_answers = self._get_all_static_answers(obj)
             ret[obj.object_hash] = {
                 "classifications": list(reversed(all_static_answers)),
                 "objectHash": obj.object_hash,
             }
         return ret
 
-    def _to_object_actions(self) -> dict:
-        ret = {}
+    def _to_object_actions(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
         for obj in self._objects_map.values():
             all_static_answers = self._dynamic_answers_to_encord_dict(obj)
             if len(all_static_answers) == 0:
                 continue
             ret[obj.object_hash] = {
                 "actions": list(reversed(all_static_answers)),
                 "objectHash": obj.object_hash,
             }
         return ret
 
-    def _to_classification_answers(self) -> dict:
-        ret = {}
+    def _to_classification_answers(self) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
         for classification in self._classifications_map.values():
             classifications = []
 
             all_static_answers = classification.get_all_static_answers()
             for answer in all_static_answers:
                 if answer.is_answered():
                     classifications.append(answer.to_encord_dict())
@@ -1772,42 +1795,42 @@
             ret[classification.classification_hash] = {
                 "classifications": list(reversed(classifications)),
                 "classificationHash": classification.classification_hash,
             }
         return ret
 
     @staticmethod
-    def _get_all_static_answers(object_instance: ObjectInstance) -> List[dict]:
+    def _get_all_static_answers(object_instance: ObjectInstance) -> List[Dict[str, Any]]:
         """Essentially convert to the JSON format of all the static answers."""
         ret = []
         for answer in object_instance._get_all_static_answers():
             d_opt = answer.to_encord_dict()
             if d_opt is not None:
                 ret.append(d_opt)
         return ret
 
     @staticmethod
-    def _dynamic_answers_to_encord_dict(object_instance: ObjectInstance) -> List[dict]:
+    def _dynamic_answers_to_encord_dict(object_instance: ObjectInstance) -> List[Dict[str, Any]]:
         ret = []
         for answer, ranges in object_instance._get_all_dynamic_answers():
             d_opt = answer.to_encord_dict(ranges)
             if d_opt is not None:
                 ret.append(d_opt)
         return ret
 
-    def _to_encord_data_units(self) -> dict:
+    def _to_encord_data_units(self) -> Dict[str, Any]:
         ret = {}
         frame_level_data = self._label_row_read_only_data.frame_level_data
         for value in frame_level_data.values():
             ret[value.image_hash] = self._to_encord_data_unit(value)
 
         return ret
 
-    def _to_encord_data_unit(self, frame_level_data: FrameLevelImageGroupData) -> dict:
-        ret = {}
+    def _to_encord_data_unit(self, frame_level_data: FrameLevelImageGroupData) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
 
         data_type = self._label_row_read_only_data.data_type
         if data_type == DataType.IMG_GROUP:
             data_sequence = str(frame_level_data.frame_number)
         elif data_type in (DataType.VIDEO, DataType.DICOM, DataType.IMAGE):
             data_sequence = frame_level_data.frame_number
         else:
@@ -1828,30 +1851,30 @@
         if self._label_row_read_only_data.duration is not None:
             ret["data_duration"] = self._label_row_read_only_data.duration
         if self._label_row_read_only_data.fps is not None:
             ret["data_fps"] = self._label_row_read_only_data.fps
 
         return ret
 
-    def _to_encord_labels(self, frame_level_data: FrameLevelImageGroupData) -> dict:
-        ret = {}
+    def _to_encord_labels(self, frame_level_data: FrameLevelImageGroupData) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
         data_type = self._label_row_read_only_data.data_type
 
         if data_type in [DataType.IMAGE, DataType.IMG_GROUP]:
             frame = frame_level_data.frame_number
             ret.update(self._to_encord_label(frame))
 
         elif data_type in [DataType.VIDEO, DataType.DICOM]:
             for frame in self._frame_to_hashes.keys():
                 ret[str(frame)] = self._to_encord_label(frame)
 
         return ret
 
-    def _to_encord_label(self, frame: int) -> dict:
-        ret = {}
+    def _to_encord_label(self, frame: int) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
 
         ret["objects"] = self._to_encord_objects_list(frame)
         ret["classifications"] = self._to_encord_classifications_list(frame)
 
         return ret
 
     def _to_encord_objects_list(self, frame: int) -> list:
@@ -1864,16 +1887,16 @@
             ret.append(encord_object)
         return ret
 
     def _to_encord_object(
         self,
         object_: ObjectInstance,
         frame: int,
-    ) -> dict:
-        ret = {}
+    ) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
 
         object_instance_annotation = object_.get_annotation(frame)
         coordinates = object_instance_annotation.coordinates
         ontology_hash = object_.ontology_item.feature_node_hash
         ontology_object = self._ontology.structure.get_child_by_hash(ontology_hash)
 
         ret["name"] = ontology_object.name
@@ -1890,44 +1913,54 @@
         if object_instance_annotation.last_edited_at is not None:
             ret["lastEditedAt"] = object_instance_annotation.last_edited_at.strftime(DATETIME_LONG_STRING_FORMAT)
         if object_instance_annotation.last_edited_by is not None:
             ret["lastEditedBy"] = object_instance_annotation.last_edited_by
         if object_instance_annotation.is_deleted is not None:
             ret["isDeleted"] = object_instance_annotation.is_deleted
 
-        self._add_coordinates_to_encord_object(coordinates, ret)
+        self._add_coordinates_to_encord_object(coordinates, frame, ret)
 
         return ret
 
-    def _add_coordinates_to_encord_object(self, coordinates: Coordinates, encord_object: dict) -> None:
+    def _add_coordinates_to_encord_object(
+        self, coordinates: Coordinates, frame: int, encord_object: Dict[str, Any]
+    ) -> None:
         if isinstance(coordinates, BoundingBoxCoordinates):
             encord_object["boundingBox"] = coordinates.to_dict()
         elif isinstance(coordinates, RotatableBoundingBoxCoordinates):
             encord_object["rotatableBoundingBox"] = coordinates.to_dict()
         elif isinstance(coordinates, PolygonCoordinates):
             encord_object["polygon"] = coordinates.to_dict()
         elif isinstance(coordinates, PolylineCoordinates):
             encord_object["polyline"] = coordinates.to_dict()
         elif isinstance(coordinates, PointCoordinate):
             encord_object["point"] = coordinates.to_dict()
+        elif isinstance(coordinates, BitmaskCoordinates):
+            frame_view = self.get_frame_view(frame)
+            if not (
+                frame_view.height == coordinates._encoded_bitmask.height
+                and frame_view.width == coordinates._encoded_bitmask.width
+            ):
+                raise ValueError("Bitmask resolution doesn't match the media resolution")
+            encord_object["bitmask"] = coordinates.to_dict()
         else:
             raise NotImplementedError(f"adding coordinatees for this type not yet implemented {type(coordinates)}")
 
     def _to_encord_classifications_list(self, frame: int) -> list:
-        ret: List[dict] = []
+        ret: List[Dict[str, Any]] = []
 
         classifications = self.get_classification_instances(filter_frames=frame)
         for classification in classifications:
             encord_classification = self._to_encord_classification(classification, frame)
             ret.append(encord_classification)
 
         return ret
 
-    def _to_encord_classification(self, classification: ClassificationInstance, frame: int) -> dict:
-        ret = {}
+    def _to_encord_classification(self, classification: ClassificationInstance, frame: int) -> Dict[str, Any]:
+        ret: Dict[str, Any] = {}
 
         annotation = classification.get_annotation(frame)
         classification_feature_hash = classification.ontology_item.feature_node_hash
         ontology_classification = self._ontology.structure.get_child_by_hash(classification_feature_hash)
         attribute_hash = classification.ontology_item.attributes[0].feature_node_hash
         ontology_attribute = self._ontology.structure.get_child_by_hash(attribute_hash)
 
@@ -2141,14 +2174,16 @@
             return PolygonCoordinates.from_dict(frame_object_label)
         elif "point" in frame_object_label:
             return PointCoordinate.from_dict(frame_object_label)
         elif "polyline" in frame_object_label:
             return PolylineCoordinates.from_dict(frame_object_label)
         elif "skeleton" in frame_object_label:
             raise NotImplementedError("Got a skeleton object, which is not supported yet")
+        elif "bitmask" in frame_object_label:
+            return BitmaskCoordinates.from_dict(frame_object_label)
         else:
             raise NotImplementedError(f"Getting coordinates for `{frame_object_label}` is not supported yet.")
 
     def _add_classification_instances_from_classifications(
         self, classifications_list: List[dict], classification_answers: dict, frame: int
     ):
         for frame_classification_label in classifications_list:
@@ -2663,23 +2698,23 @@
 
         @manual_annotation.setter
         def manual_annotation(self, manual_annotation: bool) -> None:
             self._check_if_frame_view_is_valid()
             self._get_object_frame_instance_data().object_frame_instance_info.manual_annotation = manual_annotation
 
         @property
-        def reviews(self) -> List[dict]:
+        def reviews(self) -> Optional[List[Dict[str, Any]]]:
             """
             A read only property about the reviews that happened for this object on this frame.
             """
             self._check_if_frame_view_is_valid()
             return self._get_object_frame_instance_data().object_frame_instance_info.reviews
 
         @property
-        def is_deleted(self) -> bool:
+        def is_deleted(self) -> Optional[bool]:
             """This property is only relevant for internal use."""
             self._check_if_frame_view_is_valid()
             return self._get_object_frame_instance_data().object_frame_instance_info.is_deleted
 
         def _get_object_frame_instance_data(self) -> ObjectInstance.FrameData:
             return self._object_instance._frames_to_instance_data[self._frame]
 
@@ -2724,15 +2759,15 @@
             self,
             created_at: Optional[datetime] = None,
             created_by: Optional[str] = None,
             last_edited_at: Optional[datetime] = None,
             last_edited_by: Optional[str] = None,
             confidence: Optional[float] = None,
             manual_annotation: Optional[bool] = None,
-            reviews: Optional[List[dict]] = None,
+            reviews: Optional[List[Dict[str, Any]]] = None,
             is_deleted: Optional[bool] = None,
         ) -> None:
             """Return a new instance with the specified fields updated."""
             self.created_at = created_at or self.created_at
             if created_by is not None:
                 self.created_by = created_by
             self.last_edited_at = last_edited_at or self.last_edited_at
@@ -2946,15 +2981,15 @@
         ret: Set[Answer] = set()
         for attribute in self._object_instance.ontology_item.attributes:
             if attribute.dynamic:
                 answer = get_default_answer_from_attribute(attribute)
                 ret.add(answer)
         return ret
 
-    def __eq__(self, other: DynamicAnswerManager) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, DynamicAnswerManager):
             return False
         return (
             self._frames_to_answers == other._frames_to_answers and self._answers_to_frames == other._answers_to_frames
         )
 
     def __hash__(self) -> int:
@@ -3008,16 +3043,16 @@
 
     objects: List[Object] = field(default_factory=list)
     classifications: List[Classification] = field(default_factory=list)
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Union[OntologyTypes, AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[OntologyClasses, AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
@@ -3042,16 +3077,16 @@
                 return found_item
 
         raise OntologyError("Item not found.")
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Union[OntologyTypes, AttributeTypes, OptionTypes, None] = None,
-    ) -> Union[OntologyClasses, AttributeClasses, OptionClasses]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> OntologyElement:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
@@ -3060,25 +3095,25 @@
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Union[OntologyTypes, AttributeTypes, OptionTypes, None] = None,
-    ) -> List[Union[OntologyClasses, AttributeClasses, OptionClasses]]:
+        type_: Optional[OntologyElementType] = None,
+    ) -> List[OntologyElement]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
-        ret = []
+        ret: List[OntologyElement] = []
         for object_ in self.objects:
             if object_.name == title:
                 if does_type_match(object_, type_):
                     ret.append(object_)
             found_items = _get_attributes_by_title(title, object_.attributes)
             filtered_items = filter_by_type(found_items, type_)
             ret.extend(filtered_items)
@@ -3090,15 +3125,15 @@
             found_items = _get_attributes_by_title(title, classification.attributes)
             filtered_items = filter_by_type(found_items, type_)
             ret.extend(filtered_items)
 
         return ret
 
     @classmethod
-    def from_dict(cls, d: dict) -> OntologyStructure:
+    def from_dict(cls, d: Dict[str, Any]) -> OntologyStructure:
         """
         Args:
             d: a JSON blob of an "ontology structure" (e.g. from Encord web app)
 
         Raises:
             KeyError: If the dict is missing a required field.
         """
@@ -3108,29 +3143,29 @@
 
         classifications_ret: List[Classification] = list()
         for classification_dict in d["classifications"]:
             classifications_ret.append(Classification.from_dict(classification_dict))
 
         return OntologyStructure(objects=objects_ret, classifications=classifications_ret)
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> Dict[str, List[Dict[str, Any]]]:
         """
         Returns:
             The dict equivalent to the ontology.
 
         Raises:
             KeyError: If the dict is missing a required field.
         """
-        ret = dict()
-        ontology_objects = list()
+        ret: Dict[str, List[Dict[str, Any]]] = dict()
+        ontology_objects: List[Dict[str, Any]] = list()
         ret["objects"] = ontology_objects
         for ontology_object in self.objects:
             ontology_objects.append(ontology_object.to_dict())
 
-        ontology_classifications = list()
+        ontology_classifications: List[Dict[str, Any]] = list()
         ret["classifications"] = ontology_classifications
         for ontology_classification in self.classifications:
             ontology_classifications.append(ontology_classification.to_dict())
 
         return ret
 
     def add_object(
```

### Comparing `encord-0.1.79/encord/objects/project.py` & `encord-0.1.80/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/objects/utils.py` & `encord-0.1.80/encord/objects/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import base64
 import re
 import uuid
-from typing import Any, List, Optional, TypeVar
+from typing import Any, Iterable, List, Optional, Type, TypeVar
 
 
 def _decode_nested_uid(nested_uid: list) -> str:
     return ".".join([str(uid) for uid in nested_uid])
 
 
 def short_uuid_str() -> str:
@@ -15,31 +15,31 @@
     return base64.b64encode(uuid.uuid4().bytes[:6]).decode("utf-8")
 
 
 def _lower_snake_case(s: str):
     return s.lower().replace(" ", "_")
 
 
-def check_type(obj: object, type_: Any) -> None:
+def check_type(obj: Any, type_: Optional[Type[Any]]) -> None:
     if not does_type_match(obj, type_):
         raise TypeError(f"Expected {type_}, got {type(obj)}")
 
 
-def does_type_match(obj: object, type_: Any) -> bool:
+def does_type_match(obj: Any, type_: Optional[Type[Any]]) -> bool:
     if type_ is None:
         return True
     if not isinstance(obj, type_):
         return False
     return True
 
 
 T = TypeVar("T")
 
 
-def filter_by_type(objects: List[object], type_: Optional[T]) -> List[T]:
+def filter_by_type(objects: Iterable[Any], type_: Optional[Type[T]]) -> List[T]:
     return [object_ for object_ in objects if does_type_match(object_, type_)]
 
 
 def is_valid_email(email: str) -> bool:
     """
     Validate that an email is a valid one
     """
```

### Comparing `encord-0.1.79/encord/ontology.py` & `encord-0.1.80/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/api_key.py` & `encord-0.1.80/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/base_orm.py` & `encord-0.1.80/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/dataset.py` & `encord-0.1.80/encord/orm/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,26 +311,26 @@
         self["client_metadata"] = new_client_metadata
 
     @property
     def width(self) -> Optional[int]:
         """
         An actual width of the data asset. This is `None` for data types of
         :meth:`DataType.IMG_GROUP <encord.constants.enums.DataType.IMG_GROUP>` where
-        :meth:`is_optimised_image_group <encord.data.DataRow.is_optimised_image_group>` is `False`, because
+        :meth:`is_image_sequence <encord.data.DataRow.is_image_sequence>` is `False`, because
         each image in this group can have a different dimension. Inspect the
         :meth:`images <encord.data.DataRow.images>` to get the height of individual images.
         """
         return self["width"]
 
     @property
     def height(self) -> Optional[int]:
         """
         An actual height of the data asset. This is `None` for data types of
         :meth:`DataType.IMG_GROUP <encord.constants.enums.DataType.IMG_GROUP>` where
-        :meth:`is_optimised_image_group <encord.data.DataRow.is_optimised_image_group>` is `False`, because
+        :meth:`is_image_sequence <encord.data.DataRow.is_image_sequence>` is `False`, because
         each image in this group can have a different dimension. Inspect the
         :meth:`images <encord.data.DataRow.images>` to get the height of individual images.
         """
         return self["height"]
 
     @property
     def last_edited_at(self) -> datetime:
@@ -384,14 +384,28 @@
         return self["images_data"]
 
     @property
     def is_optimised_image_group(self) -> Optional[bool]:
         """
         If the data type is an :meth:`DataType.IMG_GROUP <encord.constants.enums.DataType.IMG_GROUP>`,
         returns whether this is a performance optimised image group. Returns `None` for other data types.
+
+        DEPRECATED: This method is deprecated and will be removed in uplocming library version.
+        Please usie :meth:`.is_image_sequence` instead
+        """
+        return self.is_image_sequence
+
+    @property
+    def is_image_sequence(self) -> Optional[bool]:
+        """
+        If the data type is an :meth:`DataType.IMG_GROUP <encord.constants.enums.DataType.IMG_GROUP>`,
+        returns whether this is an image sequence. Returns `None` for other data types.
+
+        For more details refer to the
+        :ref:`documentation on image sequnces <https://docs.encord.com/datasets/supported-data/#image-sequences>`
         """
         return self["is_optimised_image_group"]
 
     def refetch_data(
         self,
         *,
         signed_url: bool = False,
```

### Comparing `encord-0.1.79/encord/orm/dataset_with_user_role.py` & `encord-0.1.80/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/label_log.py` & `encord-0.1.80/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/label_row.py` & `encord-0.1.80/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/labeling_algorithm.py` & `encord-0.1.80/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/model.py` & `encord-0.1.80/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/ontology.py` & `encord-0.1.80/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/project.py` & `encord-0.1.80/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/project_api_key.py` & `encord-0.1.80/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/project_with_user_role.py` & `encord-0.1.80/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/orm/test/test_dataset.py` & `encord-0.1.80/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/project.py` & `encord-0.1.80/encord/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/project_ontology/classification_attribute.py` & `encord-0.1.80/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/project_ontology/classification_option.py` & `encord-0.1.80/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/project_ontology/ontology.py` & `encord-0.1.80/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/project_ontology/ontology_classification.py` & `encord-0.1.80/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/project_ontology/ontology_object.py` & `encord-0.1.80/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/user_client.py` & `encord-0.1.80/encord/user_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         Args:
             project_hash: The Project ID
         """
         config = SshConfig(self.user_config, resource_type=TYPE_PROJECT, resource_id=project_hash)
         querier = Querier(config)
         client = EncordClientProject(querier=querier, config=config)
 
-        orm_project = client.get_project()
+        orm_project = client.get_project(include_labels_metadata=False)
 
         # Querying ontology using project querier to avoid permission error,
         # as there might be only read-only ontology structure access in scope of the project,
         # not full access, that is implied by get_ontology method
         ontology_hash = orm_project["ontology_hash"]
         config = SshConfig(self.user_config, resource_type=TYPE_ONTOLOGY, resource_id=ontology_hash)
         project_ontology = Ontology(querier, config)
```

### Comparing `encord-0.1.79/encord/utilities/client_utilities.py` & `encord-0.1.80/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/utilities/label_utilities.py` & `encord-0.1.80/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/encord/utilities/project_user.py` & `encord-0.1.80/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.79/pyproject.toml` & `encord-0.1.80/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.79"
+version = "0.1.80"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.79/PKG-INFO` & `encord-0.1.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.79
+Version: 0.1.80
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
-Metadata-Version: 2.1 Name: encord Version: 0.1.79 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.80 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

