# Comparing `tmp/google-cloud-discoveryengine-0.8.0.tar.gz` & `tmp/google-cloud-discoveryengine-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-discoveryengine-0.8.0.tar", last modified: Thu May 25 18:06:43 2023, max compression
+gzip compressed data, was "google-cloud-discoveryengine-0.8.1.tar", last modified: Wed Jun  7 15:37:20 2023, max compression
```

## Comparing `google-cloud-discoveryengine-0.8.0.tar` & `google-cloud-discoveryengine-0.8.1.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.130235 google-cloud-discoveryengine-0.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-05-25 18:06:43.130235 google-cloud-discoveryengine-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3663 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.094227 google-cloud-discoveryengine-0.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.094227 google-cloud-discoveryengine-0.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.098228 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine/
--rw-rw-r--   0 root         (0)     1003     5697 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.098228 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/
--rw-rw-r--   0 root         (0)     1003     4020 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8490 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.098228 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.098228 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17074 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26167 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.098228 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6703 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13608 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13816 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23102 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.102229 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47501 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58096 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5885 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.102229 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10026 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22476 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22924 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    60840 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.102229 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38042 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48349 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5793 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.102229 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8545 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18663 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19066 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    49720 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.106230 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17593 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28224 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5721 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.106230 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6595 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13393 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13611 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22989 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.106230 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27405 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37270 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.106230 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8157 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17214 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17552 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41428 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.110231 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/
--rw-rw-r--   0 root         (0)     1003     3050 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3977 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     4614 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6357 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/document.py
--rw-rw-r--   0 root         (0)     1003     9309 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    21849 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4073 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003     2392 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/schema.py
--rw-rw-r--   0 root         (0)     1003     8915 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    18461 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27255 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3424 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.110231 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003     4372 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     9266 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.110231 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.110231 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17110 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26203 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.114232 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6711 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13616 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13824 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22926 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.114232 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47829 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58424 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5921 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.114232 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10042 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23048 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    60520 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.114232 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17422 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27322 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.114232 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6712 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13617 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13829 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23083 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.118233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38222 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48529 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5829 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.118233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8553 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18711 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19114 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    49372 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.118233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17633 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28264 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5757 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.118233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6603 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13401 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13619 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22813 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.122233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27473 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37338 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.122233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8165 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17230 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17568 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41036 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.122233 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3197 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5368 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003     4646 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6373 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/document.py
--rw-rw-r--   0 root         (0)     1003     9481 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    22061 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/import_config.py
--rw-rw-r--   0 root         (0)     1003     4085 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/purge_config.py
--rw-rw-r--   0 root         (0)     1003    10788 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
--rw-rw-r--   0 root         (0)     1003     2396 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/schema.py
--rw-rw-r--   0 root         (0)     1003     9031 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    37375 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27718 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3436 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.126234 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    10665 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-25 18:06:43.000000 google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-25 18:06:43.130235 google-cloud-discoveryengine-0.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.126234 google-cloud-discoveryengine-0.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.126234 google-cloud-discoveryengine-0.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.126234 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.126234 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    83160 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201237 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_document_service.py
--rw-rw-r--   0 root         (0)     1003   168146 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93087 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119289 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-25 18:06:43.130235 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    83584 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   201685 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
--rw-rw-r--   0 root         (0)     1003    86195 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
--rw-rw-r--   0 root         (0)     1003   168594 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93887 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119713 2023-05-25 18:04:06.000000 google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3663 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.670532 google-cloud-discoveryengine-0.8.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.674532 google-cloud-discoveryengine-0.8.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.674532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/
+-rw-rw-r--   0 root         (0)     1003     5697 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/
+-rw-rw-r--   0 root         (0)     1003     4020 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8490 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17074 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26167 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6703 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13608 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13816 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23102 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.678532 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47501 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58096 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5885 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10026 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22476 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22924 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60840 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38042 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48349 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5793 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8545 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18663 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19066 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    49720 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17593 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28224 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5721 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.682533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6595 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13393 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13611 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22989 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.686533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27405 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37270 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.686533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8157 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17214 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17552 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41428 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.686533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3050 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3977 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4614 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6357 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9309 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    21849 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4073 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003     2392 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     8915 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    16487 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27255 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3424 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4372 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9266 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17110 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26203 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6711 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13824 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22926 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47829 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58424 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.690533 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10042 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23048 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60520 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17422 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27322 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6712 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13617 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13829 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23083 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38222 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48529 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.694534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8553 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18711 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19114 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    49372 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17633 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28264 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6603 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13401 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13619 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22813 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27473 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37338 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.698534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8165 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17230 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17568 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41036 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3197 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5368 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4646 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6373 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9481 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    22061 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4085 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003    10788 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003     2396 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     9031 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    37375 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27718 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3436 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    10665 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-07 15:37:20.000000 google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.702534 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83160 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   201237 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003   168146 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93087 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119289 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-07 15:37:20.706534 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   201685 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003    86195 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003   168594 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93887 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119713 2023-06-07 15:34:36.000000 google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
```

### Comparing `google-cloud-discoveryengine-0.8.0/LICENSE` & `google-cloud-discoveryengine-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/MANIFEST.in` & `google-cloud-discoveryengine-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/PKG-INFO` & `google-cloud-discoveryengine-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.8.0/README.rst` & `google-cloud-discoveryengine-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine/gapic_version.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.8.0"  # {x-release-please-version}
+__version__ = "0.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/gapic_metadata.json` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/gapic_version.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.8.0"  # {x-release-please-version}
+__version__ = "0.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/common.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/completion_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/document.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/document_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/import_config.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/purge_config.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/schema.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/schema_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/search_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/search_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -235,17 +235,14 @@
         r"""The specification that configs the desired behavior of the
         UCS content search.
 
         Attributes:
             snippet_spec (google.cloud.discoveryengine_v1.types.SearchRequest.ContentSearchSpec.SnippetSpec):
                 If there is no snippet spec provided, there
                 will be no snippet in the search result.
-            summary_spec (google.cloud.discoveryengine_v1.types.SearchRequest.ContentSearchSpec.SummarySpec):
-                If there is no summary spec provided, there
-                will be no summary in the search response.
         """
 
         class SnippetSpec(proto.Message):
             r"""The specification that configs the snippet in the search
             results.
 
             Attributes:
@@ -265,44 +262,19 @@
                 number=1,
             )
             reference_only: bool = proto.Field(
                 proto.BOOL,
                 number=2,
             )
 
-        class SummarySpec(proto.Message):
-            r"""The specification that configs the summary in the search
-            response.
-
-            Attributes:
-                summary_result_count (int):
-                    The number of top results the summary should be generated
-                    from. If the number of returned results is less than
-                    summary_result_count, then the summary would be derived from
-                    all the results; otherwise, the summary would be derived
-                    from the top results.
-
-                    At most 5 results can be used for generating summary.
-            """
-
-            summary_result_count: int = proto.Field(
-                proto.INT32,
-                number=1,
-            )
-
         snippet_spec: "SearchRequest.ContentSearchSpec.SnippetSpec" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="SearchRequest.ContentSearchSpec.SnippetSpec",
         )
-        summary_spec: "SearchRequest.ContentSearchSpec.SummarySpec" = proto.Field(
-            proto.MESSAGE,
-            number=2,
-            message="SearchRequest.ContentSearchSpec.SummarySpec",
-        )
 
     serving_config: str = proto.Field(
         proto.STRING,
         number=1,
     )
     branch: str = proto.Field(
         proto.STRING,
@@ -392,19 +364,14 @@
             to retrieve the next page. If this field is omitted, there
             are no subsequent pages.
         corrected_query (str):
             Contains the spell corrected query, if found. If the spell
             correction type is AUTOMATIC, then the search results are
             based on corrected_query. Otherwise the original query is
             used for search.
-        summary (google.cloud.discoveryengine_v1.types.SearchResponse.Summary):
-            A summary as part of the search results. This field is only
-            returned if
-            [SearchRequest.ContentSearchSpec.summary_spec][google.cloud.discoveryengine.v1.SearchRequest.ContentSearchSpec.summary_spec]
-            is set.
     """
 
     class SearchResult(proto.Message):
         r"""Represents the search results.
 
         Attributes:
             id (str):
@@ -423,28 +390,14 @@
         )
         document: gcd_document.Document = proto.Field(
             proto.MESSAGE,
             number=2,
             message=gcd_document.Document,
         )
 
-    class Summary(proto.Message):
-        r"""Summary of the top N search result specified by the summary
-        spec.
-
-        Attributes:
-            summary_text (str):
-                The summary content.
-        """
-
-        summary_text: str = proto.Field(
-            proto.STRING,
-            number=1,
-        )
-
     @property
     def raw_page(self):
         return self
 
     results: MutableSequence[SearchResult] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
@@ -462,15 +415,10 @@
         proto.STRING,
         number=5,
     )
     corrected_query: str = proto.Field(
         proto.STRING,
         number=7,
     )
-    summary: Summary = proto.Field(
-        proto.MESSAGE,
-        number=9,
-        message=Summary,
-    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/user_event.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1/types/user_event_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/gapic_version.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.8.0"  # {x-release-please-version}
+__version__ = "0.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/__init__.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/common.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/completion_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/document.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/document_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/import_config.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/purge_config.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/purge_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/schema.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/schema_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/search_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/user_event.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py` & `google-cloud-discoveryengine-0.8.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/PKG-INFO` & `google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.8.0/google_cloud_discoveryengine.egg-info/SOURCES.txt` & `google-cloud-discoveryengine-0.8.1/google_cloud_discoveryengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/setup.py` & `google-cloud-discoveryengine-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/__init__.py` & `google-cloud-discoveryengine-0.8.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/__init__.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/__init__.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/__init__.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_completion_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_document_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_schema_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_search_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1/test_user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.8.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py` & `google-cloud-discoveryengine-0.8.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py`

 * *Files identical despite different names*

