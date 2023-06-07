# Comparing `tmp/pilot-platform-common-0.4.0.tar.gz` & `tmp/pilot-platform-common-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.4.0.tar", last modified: Mon May 22 14:33:27 2023, max compression
+gzip compressed data, was "pilot-platform-common-0.4.1.tar", last modified: Wed Jun  7 19:37:00 2023, max compression
```

## Comparing `pilot-platform-common-0.4.0.tar` & `pilot-platform-common-0.4.1.tar`

### file list

```diff
@@ -1,67 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/
--rw-r--r--   0 runner    (1001) docker     (122)     1265 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/geid/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (122)     4295 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/jwt_handler_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/jwt_handler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/entity_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/lineage/lineage_object.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.780512 pilot-platform-common-0.4.0/common/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/models/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/permissions/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/project/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8179 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/common/vault/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-22 14:33:27.000000 pilot-platform-common-0.4.0/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.784512 pilot-platform-common-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8103 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:33:27.788512 pilot-platform-common-0.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-22 14:32:31.000000 pilot-platform-common-0.4.0/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.095242 pilot-platform-common-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-07 19:37:00.095242 pilot-platform-common-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.075242 pilot-platform-common-0.4.1/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.075242 pilot-platform-common-0.4.1/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.079242 pilot-platform-common-0.4.1/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (122)     4295 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/jwt_handler/jwt_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/jwt_handler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.079242 pilot-platform-common-0.4.1/common/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/lineage/entity_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/lineage/lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/lineage/lineage_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.079242 pilot-platform-common-0.4.1/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.083242 pilot-platform-common-0.4.1/common/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.083242 pilot-platform-common-0.4.1/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17100 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.087242 pilot-platform-common-0.4.1/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/permissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4381 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/permissions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3985 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/permissions/permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/permissions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.087242 pilot-platform-common-0.4.1/common/project/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8179 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.087242 pilot-platform-common-0.4.1/common/services/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/services/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.087242 pilot-platform-common-0.4.1/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.091242 pilot-platform-common-0.4.1/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-07 19:37:00.000000 pilot-platform-common-0.4.1/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-06-07 19:37:00.000000 pilot-platform-common-0.4.1/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 19:37:00.000000 pilot-platform-common-0.4.1/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-07 19:37:00.000000 pilot-platform-common-0.4.1/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-07 19:37:00.000000 pilot-platform-common-0.4.1/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 19:37:00.095242 pilot-platform-common-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.095242 pilot-platform-common-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8103 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.095242 pilot-platform-common-0.4.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/fixtures/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:37:00.095242 pilot-platform-common-0.4.1/tests/permissions/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/permissions/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12829 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/permissions/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4460 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/permissions/test_permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-07 19:35:58.000000 pilot-platform-common-0.4.1/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.4.0/PKG-INFO` & `pilot-platform-common-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.4.0/README.md` & `pilot-platform-common-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/__init__.py` & `pilot-platform-common-0.4.1/common/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .object_storage_adaptor import TokenError
 from .object_storage_adaptor import get_boto3_admin_client
 from .object_storage_adaptor import get_boto3_client
 from .object_storage_adaptor import get_minio_policy_client
 from .permissions import get_project_role
 from .permissions import has_file_permission
 from .permissions import has_permission
+from .permissions import has_permissions
 from .project import ProjectClient
 from .project import ProjectClientSync
 from .project import ProjectException
 from .project import ProjectNotFoundException
 from .vault import VaultClient
 
 __all__ = [
@@ -29,13 +30,14 @@
     'get_boto3_client',
     'get_minio_policy_client',
     'TokenError',
     'NotFoundError',
     'get_project_role',
     'has_file_permission',
     'has_permission',
+    'has_permissions',
     'ProjectClient',
     'ProjectClientSync',
     'ProjectException',
     'ProjectNotFoundException',
     'VaultClient',
 ]
```

### Comparing `pilot-platform-common-0.4.0/common/geid/geid_client.py` & `pilot-platform-common-0.4.1/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-0.4.1/common/jwt_handler/JWTHandler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/jwt_handler/models.py` & `pilot-platform-common-0.4.1/common/jwt_handler/models.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/lineage/entity_object.py` & `pilot-platform-common-0.4.1/common/lineage/entity_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/lineage/lineage_client.py` & `pilot-platform-common-0.4.1/common/lineage/lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/lineage/lineage_object.py` & `pilot-platform-common-0.4.1/common/lineage/lineage_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/logging/formatter.py` & `pilot-platform-common-0.4.1/common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/logging/logging.py` & `pilot-platform-common-0.4.1/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/models/config_center_policy.py` & `pilot-platform-common-0.4.1/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-0.4.1/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-0.4.1/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-0.4.1/common/object_storage_adaptor/boto3_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Copyright (C) 2022-2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import json
 import os
+from datetime import datetime
+from datetime import timedelta
+from datetime import timezone
 from typing import Any
 from typing import List
 from typing import Optional
+from typing import Union
 
 import aioboto3
 import httpx
 import xmltodict
 from botocore.client import Config
 
 from common.object_storage_adaptor.base_client import BaseClient
@@ -298,38 +302,45 @@
         async with self._session.client('s3', endpoint_url=self.endpoint, config=self._config) as s3:
             presigned_url = await s3.generate_presigned_url(
                 'get_object', Params={'Bucket': bucket, 'Key': key}, ExpiresIn=duration
             )
 
         return presigned_url
 
-    async def prepare_multipart_upload(self, bucket: str, keys: List[str]) -> List[str]:
+    async def prepare_multipart_upload(
+        self, bucket: str, keys: List[str], expire_time: Union[datetime, None] = None
+    ) -> List[str]:
         """
         Summary:
             The function is the boto3 wrapup to generate a multipart upload presigned url.
             This is the first step to do the multipart upload.
 
             NOTE: The api has been changed to adapot the batch operation. The prepare
             upload api is a batch operation to create all jobs and lock in advance. If
             not, the performance will decrease that every iteration will try to connect
             with endpoints
 
         Parameter:
             - bucket(str): the bucket name
             - keys(list of str): the object path of file
+            - expire_time(datetime): when the multipart upload will expire
 
         return:
             - upload_id(list): list of upload id will be used in later two apis
         """
         self.logger.info('Prepare multipart upload for bucket: %s, keys: %s', bucket, str(keys))
 
+        # add the default expire time as utc now + 1 day
+        if expire_time is None:
+            expire_time = datetime.now(tz=timezone.utc) + timedelta(days=1)
+
         upload_id_list = []
         async with self._session.client('s3', endpoint_url=self.endpoint, config=self._config) as s3:
             for key in keys:
-                res = await s3.create_multipart_upload(Bucket=bucket, Key=key)
+                res = await s3.create_multipart_upload(Bucket=bucket, Key=key, Expires=expire_time)
                 upload_id_list.append(res.get('UploadId'))
 
         self.logger.info('Result upload ids: %s', str(upload_id_list))
 
         return upload_id_list
 
     async def part_upload(self, bucket: str, key: str, upload_id: str, part_number: int, content: str) -> dict:
```

### Comparing `pilot-platform-common-0.4.0/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-0.4.1/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/project/project_client.py` & `pilot-platform-common-0.4.1/common/project/project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/project/project_exceptions.py` & `pilot-platform-common-0.4.1/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/common/vault/vault_client.py` & `pilot-platform-common-0.4.1/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-0.4.1/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.4.0/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-0.4.1/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,18 +21,23 @@
 common/models/service_id_generator.py
 common/object_storage_adaptor/__init__.py
 common/object_storage_adaptor/base_client.py
 common/object_storage_adaptor/boto3_admin_client.py
 common/object_storage_adaptor/boto3_client.py
 common/object_storage_adaptor/minio_policy_client.py
 common/permissions/__init__.py
+common/permissions/exceptions.py
 common/permissions/permissions.py
+common/permissions/permissions_manager.py
+common/permissions/schemas.py
 common/project/__init__.py
 common/project/project_client.py
 common/project/project_exceptions.py
+common/services/__init__.py
+common/services/auth_client.py
 common/vault/__init__.py
 common/vault/vault_client.py
 common/vault/vault_exception.py
 pilot_platform_common.egg-info/PKG-INFO
 pilot_platform_common.egg-info/SOURCES.txt
 pilot_platform_common.egg-info/dependency_links.txt
 pilot_platform_common.egg-info/requires.txt
@@ -40,12 +45,15 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_formatter.py
 tests/test_geid_client.py
 tests/test_jwt_handler.py
 tests/test_lineage_client.py
 tests/test_logging.py
-tests/test_permissions.py
 tests/test_project_client.py
 tests/test_vault_client.py
 tests/fixtures/__init__.py
-tests/fixtures/fake.py
+tests/fixtures/fake.py
+tests/permissions/__init__.py
+tests/permissions/test_auth_client.py
+tests/permissions/test_permissions.py
+tests/permissions/test_permissions_manager.py
```

### Comparing `pilot-platform-common-0.4.0/pyproject.toml` & `pilot-platform-common-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Indoc Research"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = ">=0.19.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
@@ -12,14 +12,15 @@
 xmltodict = "^0.13.0"
 minio = "^7.1.8"
 httpx = "^0.23.0"
 pyjwt = "2.6.0"
 redis = "^4.5"
 starlette = "^0.25.0"
 cryptography = "39.0.0"
+pydantic = "^1.10.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 pytest-asyncio = "0.20.3"
 pytest-cov = "4.0.0"
 pytest-httpx = "0.21.3"
 pytest-mock = "3.10.0"
```

### Comparing `pilot-platform-common-0.4.0/setup.py` & `pilot-platform-common-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.4.0',
+    version='0.4.1',
     author='Indoc Research',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pilot-platform-common-0.4.0/tests/conftest.py` & `pilot-platform-common-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/tests/test_formatter.py` & `pilot-platform-common-0.4.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/tests/test_jwt_handler.py` & `pilot-platform-common-0.4.1/tests/test_jwt_handler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/tests/test_lineage_client.py` & `pilot-platform-common-0.4.1/tests/test_lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/tests/test_logging.py` & `pilot-platform-common-0.4.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/tests/test_permissions.py` & `pilot-platform-common-0.4.1/tests/permissions/test_permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import pytest
 
 from common import get_project_role
 from common import has_file_permission
 from common import has_permission
+from common import has_permissions
+from common.permissions.exceptions import ProjectRoleNotFound
 
 
 class TestPermissions:
     @pytest.mark.asyncio
     async def test_has_permission_true(self, httpx_mock):
         current_identity = {
             'username': 'test',
@@ -265,7 +267,38 @@
         current_identity = {
             'username': 'test',
             'role': 'member',
             'realm_roles': ['test_project-customrole'],
         }
         result = await get_project_role('test_project', current_identity)
         assert result == 'customrole'
+
+
+class TestBulkPermissions:
+    auth_service_url = 'http://auth_service/v1/'
+    permission_request = [
+        {'role': 'admin', 'zone': 'greenroom', 'resource': 'file_any', 'operation': 'copy'},
+        {'role': 'admin', 'zone': 'greenroom', 'resource': 'file_any', 'operation': 'view'},
+    ]
+    current_identity = {'role': 'collaborator', 'realm_roles': ['test_project-collaborator']}
+
+    async def test_has_permissions_return_mapped_assertions(self, httpx_mock):
+        granted = {'has_permission': True}
+        mapped_result = {'greenroom_file_any_copy': True, 'greenroom_file_any_view': True}
+
+        httpx_mock.add_response(
+            method='POST',
+            url=f'{self.auth_service_url}authorize',
+            status_code=200,
+            json=granted,
+        )
+        mapped = await has_permissions(
+            self.auth_service_url, 'test_project', self.permission_request, self.current_identity
+        )
+
+        assert mapped == mapped_result
+
+    async def test_has_permissions_raise_project_role_not_found_exception_for_invalid_role(self, httpx_mock):
+        identity = self.current_identity
+        identity['realm_roles'] = ['invalidproject-collaborator']
+        with pytest.raises(ProjectRoleNotFound):
+            await has_permissions(self.auth_service_url, 'test_project', self.permission_request, identity)
```

### Comparing `pilot-platform-common-0.4.0/tests/test_project_client.py` & `pilot-platform-common-0.4.1/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.4.0/tests/test_vault_client.py` & `pilot-platform-common-0.4.1/tests/test_vault_client.py`

 * *Files identical despite different names*

