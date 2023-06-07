# Comparing `tmp/bpkio_python_sdk-1.2.0.tar.gz` & `tmp/bpkio_python_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_python_sdk-1.2.0.tar", max compression
+gzip compressed data, was "bpkio_python_sdk-1.3.0.tar", max compression
```

## Comparing `bpkio_python_sdk-1.2.0.tar` & `bpkio_python_sdk-1.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.2.0/README.md
--rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.2.0/bpkio_api/__init__.py
--rw-r--r--   0        0        0     5308 2023-05-21 17:03:47.808287 bpkio_python_sdk-1.2.0/bpkio_api/api.py
--rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.2.0/bpkio_api/caching.py
--rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.2.0/bpkio_api/credential_provider.py
--rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.2.0/bpkio_api/defaults.py
--rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/__init__.py
--rw-r--r--   0        0        0     4521 2023-05-20 12:34:42.082005 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/categories.py
--rw-r--r--   0        0        0      666 2023-05-20 12:34:42.082634 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/consumption.py
--rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/enums.py
--rw-r--r--   0        0        0    21988 2023-05-20 12:34:42.083318 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/services.py
--rw-r--r--   0        0        0    21622 2023-05-20 12:34:42.084047 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/sources.py
--rw-r--r--   0        0        0     2675 2023-05-20 12:34:42.084780 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/tenants.py
--rw-r--r--   0        0        0     5879 2023-05-20 12:34:42.085269 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/transcoding_profiles.py
--rw-r--r--   0        0        0     2627 2023-05-20 12:34:42.085823 bpkio_python_sdk-1.2.0/bpkio_api/endpoints/users.py
--rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.2.0/bpkio_api/exceptions.py
--rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.2.0/bpkio_api/helpers/codecstrings.py
--rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/__init__.py
--rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/dash.py
--rw-r--r--   0        0        0     3644 2023-06-02 14:52:57.666804 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/factory.py
--rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/generic.py
--rw-r--r--   0        0        0     4431 2023-06-02 14:35:26.107648 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/hls.py
--rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/jpeg.py
--rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/mp4.py
--rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/png.py
--rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vast.py
--rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vmap.py
--rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/xml.py
--rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.2.0/bpkio_api/helpers/list.py
--rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.2.0/bpkio_api/helpers/objects.py
--rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/__init__.py
--rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/analyser.py
--rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/dash.py
--rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/hls.py
--rw-r--r--   0        0        0     1587 2023-05-23 22:08:22.519293 bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/profile_generator.py
--rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/__init__.py
--rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/curl.py
--rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/exporter.py
--rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/markdown.py
--rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/postman.py
--rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/session_items.py
--rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/session_recorder.py
--rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/text.py
--rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.2.0/bpkio_api/helpers/search.py
--rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.2.0/bpkio_api/helpers/source_type.py
--rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.2.0/bpkio_api/helpers/times.py
--rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.2.0/bpkio_api/mappings.py
--rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.2.0/bpkio_api/models/Categories.py
--rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.2.0/bpkio_api/models/Consumption.py
--rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.2.0/bpkio_api/models/Services.py
--rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.2.0/bpkio_api/models/Slots.py
--rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.2.0/bpkio_api/models/Sources.py
--rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.2.0/bpkio_api/models/Tenants.py
--rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.2.0/bpkio_api/models/TranscodingProfiles.py
--rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.2.0/bpkio_api/models/Users.py
--rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.2.0/bpkio_api/models/__init__.py
--rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.2.0/bpkio_api/models/common.py
--rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.2.0/bpkio_api/models/model_graph.py
--rw-r--r--   0        0        0     1941 2023-05-21 20:52:58.371698 bpkio_python_sdk-1.2.0/bpkio_api/response_handler.py
--rw-r--r--   0        0        0     1195 2023-06-05 14:46:01.091632 bpkio_python_sdk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.3.0/README.md
+-rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.3.0/bpkio_api/__init__.py
+-rw-r--r--   0        0        0     5766 2023-06-07 13:10:20.655016 bpkio_python_sdk-1.3.0/bpkio_api/api.py
+-rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.3.0/bpkio_api/caching.py
+-rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.3.0/bpkio_api/credential_provider.py
+-rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.3.0/bpkio_api/defaults.py
+-rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4521 2023-05-20 12:34:42.082005 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/categories.py
+-rw-r--r--   0        0        0      700 2023-06-07 09:05:39.402150 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/consumption.py
+-rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/enums.py
+-rw-r--r--   0        0        0    21988 2023-05-20 12:34:42.083318 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/services.py
+-rw-r--r--   0        0        0    21622 2023-05-20 12:34:42.084047 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/sources.py
+-rw-r--r--   0        0        0     2675 2023-05-20 12:34:42.084780 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/tenants.py
+-rw-r--r--   0        0        0     5972 2023-06-07 15:09:04.450220 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/transcoding_profiles.py
+-rw-r--r--   0        0        0     2627 2023-05-20 12:34:42.085823 bpkio_python_sdk-1.3.0/bpkio_api/endpoints/users.py
+-rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.3.0/bpkio_api/exceptions.py
+-rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.3.0/bpkio_api/helpers/codecstrings.py
+-rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/__init__.py
+-rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/dash.py
+-rw-r--r--   0        0        0     3986 2023-06-07 12:31:03.185367 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/factory.py
+-rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/generic.py
+-rw-r--r--   0        0        0     4501 2023-06-06 15:17:48.082443 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/hls.py
+-rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/jpeg.py
+-rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/mp4.py
+-rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/png.py
+-rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vast.py
+-rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vmap.py
+-rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/xml.py
+-rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.3.0/bpkio_api/helpers/list.py
+-rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.3.0/bpkio_api/helpers/objects.py
+-rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/analyser.py
+-rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/dash.py
+-rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/hls.py
+-rw-r--r--   0        0        0     1587 2023-05-23 22:08:22.519293 bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/profile_generator.py
+-rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/__init__.py
+-rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/curl.py
+-rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/exporter.py
+-rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/markdown.py
+-rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/postman.py
+-rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_items.py
+-rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_recorder.py
+-rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/text.py
+-rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.3.0/bpkio_api/helpers/search.py
+-rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.3.0/bpkio_api/helpers/source_type.py
+-rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.3.0/bpkio_api/helpers/times.py
+-rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.3.0/bpkio_api/mappings.py
+-rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.3.0/bpkio_api/models/Categories.py
+-rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.3.0/bpkio_api/models/Consumption.py
+-rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.3.0/bpkio_api/models/Services.py
+-rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.3.0/bpkio_api/models/Slots.py
+-rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.3.0/bpkio_api/models/Sources.py
+-rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.3.0/bpkio_api/models/Tenants.py
+-rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.3.0/bpkio_api/models/TranscodingProfiles.py
+-rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.3.0/bpkio_api/models/Users.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.3.0/bpkio_api/models/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.3.0/bpkio_api/models/common.py
+-rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.3.0/bpkio_api/models/model_graph.py
+-rw-r--r--   0        0        0     1941 2023-05-21 20:52:58.371698 bpkio_python_sdk-1.3.0/bpkio_api/response_handler.py
+-rw-r--r--   0        0        0     1195 2023-06-07 15:37:33.376880 bpkio_python_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.3.0/PKG-INFO
```

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/api.py` & `bpkio_python_sdk-1.3.0/bpkio_api/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import json
 import os
 from typing import Optional
+from urllib.parse import urlparse
 
 from uplink import Consumer
 from uplink.auth import BearerToken
 
 from bpkio_api.caching import init_cache
 from bpkio_api.credential_provider import TenantProfile, TenantProfileProvider
 from bpkio_api.defaults import DEFAULT_FQDN
@@ -34,14 +35,17 @@
         use_cache: bool = True,
         session_file: Optional[str] = None,
         **kwargs,
     ):
         if tenant and api_key:
             raise ValueError("You can't specify both tenant and api_key")
 
+        if fqdn and fqdn != DEFAULT_FQDN:
+            fqdn = BroadpeakIoApi.normalise_fqdn(fqdn)
+
         tp = TenantProfileProvider()
 
         if tenant:
             if isinstance(tenant, str):
                 t = tp.get_tenant_profile(tenant)
             if isinstance(tenant, TenantProfile):
                 t = tenant
@@ -145,19 +149,32 @@
     def fqdn(self):
         return self._fqdn
 
     def uses_default_fqdn(self):
         return self._fqdn == DEFAULT_FQDN
 
     @staticmethod
-    def is_correct_entrypoint(url: str, api_key: str) -> bool:
+    def normalise_fqdn(url):
+        """A function to allow extraction and normalisation of a FQDN from a full URL"""
+        fqdn = url
+        if url.startswith("http"):
+            fqdn = urlparse(url).netloc
+
+        if fqdn.startswith("app"):
+            fqdn = "api" + fqdn[3:]
+
+        return fqdn
+
+    @staticmethod
+    def is_correct_entrypoint(url: str, api_key: str) -> bool | str:
         """Checks that the URL is a valid Broadpeak.io entrypoint"""
+
         try:
             api = BroadpeakIoApi(api_key=api_key, fqdn=url)
             api.get_self_tenant()
             return True
-        except Exception as e:
+        except Exception:
             return False
 
     def root_endpoint_for_resource(self, resource: object) -> object:
         """Returns the root endpoint for a given resource"""
         return model_to_endpoint(api=self, model=type(resource))
```

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/caching.py` & `bpkio_python_sdk-1.3.0/bpkio_api/caching.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/credential_provider.py` & `bpkio_python_sdk-1.3.0/bpkio_api/credential_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/categories.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/consumption.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/consumption.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 
     @returns.json()
     @get("consumption")
     def retrieve(
         self,
         start_time: Query("start-time"),  # type: ignore
         end_time: Query("end-time"),  # type: ignore
+        tenant: Query("tenantId")
     ) -> ConsumptionData:  # type: ignore
         """Get the consumption data between 2 dates"""
```

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/services.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/sources.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/tenants.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/tenants.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/transcoding_profiles.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/transcoding_profiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Tuple
+from typing import Any, List, Optional, Tuple
 
 from uplink import (
     Body,
     Consumer,
     Query,
     delete,
     get,
@@ -31,22 +31,22 @@
 class TranscodingProfilesApi(Consumer):
     def __init__(self, base_url="", **kwargs):
         super().__init__(base_url, **kwargs)
 
     @returns.json()
     @get("transcoding-profiles")
     def get_page(
-        self, offset: Query = 0, limit: Query = 50, tenantId: Query = None
+        self, offset: Query = 0, limit: Query = 50, tenant_id: Query("tenantId") = None
     ) -> List[TranscodingProfile]:  # type: ignore
         """List all transcoding profiles"""
 
     @returns.json()
     @get("transcoding-profiles/{transcoding_profile_id}")
     def retrieve(
-        self, transcoding_profile_id, tenantId: Query = None
+        self, transcoding_profile_id, tenant_id: Query("tenantId") = None
     ) -> TranscodingProfile:
         """Get a single transcoding profile, by ID"""
 
     @json
     @returns.json()
     @post("transcoding-profiles")
     def create(self, profile: Body(type=TranscodingProfileIn)) -> TranscodingProfile:  # type: ignore
@@ -61,24 +61,24 @@
     @delete("transcoding-profiles/{transcoding_profile_id}")
     def delete(self, transcoding_profile_id):
         """Delete a single transcoding profile, by ID"""
 
     # === Helpers ===
 
     @cache_api_results("list_profiles")
-    def list(self, tenantId: int = None):
-        return get_all_with_pagination(self.get_page, tenantId=tenantId)
+    def list(self, tenant_id: int = None):
+        return get_all_with_pagination(self.get_page, tenant_id=tenant_id)
 
     def search(
         self,
         value: Any | None = None,
         field: str | None = None,
         method: SearchMethod = SearchMethod.STRING_SUB,
         filters: List[Tuple[Any, str | None, SearchMethod | None]] | None = None,
-        tenantId: int = None,
+        tenant_id: int = None,
     ) -> List[TranscodingProfile]:
         """Searches the list of transcoding profiles for those matching a particular filter query
 
         You can search for full or partial matches in all or specific fields.
         All searches are done as string matches (regarding of the actual type of each field)
 
         Args:
@@ -96,21 +96,22 @@
 
         Returns:
             List[Svc.SourceSpare]: List of matching sources
         """
         if not filters:
             filters = [(value, field, method)]
 
-        profiles = self.list(tenantId=tenantId)
+        profiles = self.list(tenant_id=tenant_id)
         return search_array_with_filters(profiles, filters=filters)
 
     def upsert(
         self,
         profile: TranscodingProfileIn,
         if_exists: str = "retrieve",
+        tenant_id: Optional[int] = None,
     ) -> Tuple[TranscodingProfile | TranscodingProfileIn, UpsertOperationType]:  # type: ignore
         """Creates a transcoding profile with adaptable behaviour if it already exist.
 
         Args:
             profile (TranscodingProfileIn): The payload for the source to create
             if_exists (str): What action to take if it exists:
               `error` (default) returns an error;
@@ -127,23 +128,23 @@
 
         try:
             return (self.create(profile), UpsertOperationType.CREATED)
         except ResourceExistsError as e:
             if if_exists == "error":
                 return (profile, UpsertOperationType.ERROR)
 
-            unique_fields = list(set("name"))
+            unique_fields = ["name"]
             for fld in unique_fields:
                 # single field
                 if isinstance(fld, str):
                     fld = (fld,)
 
                 # find duplicates
                 dupes = find_duplicates_of(
-                    obj=profile, in_list=self.list(), by_fields=fld
+                    obj=profile, in_list=self.list(tenant_id=tenant_id), by_fields=fld
                 )
                 if dupes:
                     existing_resource = self.retrieve(dupes[0][1].id)
 
                     if if_exists == "retrieve":
                         return (existing_resource, UpsertOperationType.RETRIEVED)
                     elif if_exists == "update":
```

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/endpoints/users.py` & `bpkio_python_sdk-1.3.0/bpkio_api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/exceptions.py` & `bpkio_python_sdk-1.3.0/bpkio_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/codecstrings.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/codecstrings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/dash.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/factory.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import re
 from urllib.parse import urlparse
 
 import requests
 
 from bpkio_api import __version__
@@ -20,14 +21,19 @@
 
 # Registry for subclasses
 _registry = {}
 
 # Main headers
 headers = {"User-Agent": f"bpkio-python-sdk/{__version__}"}
 
+# Timeout for HEAD
+timeout = 2
+
+logger = logging.getLogger(__name__)
+
 
 def all_subclasses(cls):
     return set(cls.__subclasses__()).union(
         [s for c in cls.__subclasses__() for s in all_subclasses(c)]
     )
 
 
@@ -55,16 +61,22 @@
     return content
 
 
 def create_handler(url, get_full_content=False, from_url_only=False):
     try:
         content_type = ""
         if not from_url_only:
-            response = requests.head(url, allow_redirects=True, headers=headers)
-            content_type = response.headers.get("content-type")
+            try:
+                response = requests.head(
+                    url, allow_redirects=True, headers=headers, timeout=timeout
+                )
+                content_type = response.headers.get("content-type")
+            except requests.exceptions.Timeout:
+                logger.debug(f"HTTP HEAD takes more than {timeout} seconds, skipping.")
+                content_type = "Unknown"
 
         match = re.search(r"/(\.\w+)$", url)
         if match:
             # Special handling of Unified Streaming URLs
             file_extension = match.group(1)
         else:
             file_extension = os.path.splitext(urlparse(url).path)[1]
```

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/generic.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/generic.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/hls.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,19 +134,20 @@
                         codecs=playlist.stream_info.codecs,
                         resolution=res,
                         url=playlist.absolute_uri,
                     )
                 )
 
             for media in self.document.media:
-                index += 1
-                arr.append(
-                    dict(
-                        index=index,
-                        type="media",
-                        manifest=media.uri,
-                        language=media.language,
-                        url=media.absolute_uri,
+                if media.uri:
+                    index += 1
+                    arr.append(
+                        dict(
+                            index=index,
+                            type="media",
+                            manifest=media.uri,
+                            language=media.language,
+                            url=media.absolute_uri,
+                        )
                     )
-                )
 
         return arr
```

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vast.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vast.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/vmap.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/vmap.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/handlers/xml.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/list.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/dash.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/hls.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/profile_generator/profile_generator.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/profile_generator/profile_generator.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/curl.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/curl.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/exporter.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/exporter.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/markdown.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/markdown.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/postman.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/postman.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/session_items.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_items.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/session_recorder.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/recorder/text.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/recorder/text.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/search.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/source_type.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/source_type.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/helpers/times.py` & `bpkio_python_sdk-1.3.0/bpkio_api/helpers/times.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/mappings.py` & `bpkio_python_sdk-1.3.0/bpkio_api/mappings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/models/Services.py` & `bpkio_python_sdk-1.3.0/bpkio_api/models/Services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/models/Slots.py` & `bpkio_python_sdk-1.3.0/bpkio_api/models/Slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/models/Sources.py` & `bpkio_python_sdk-1.3.0/bpkio_api/models/Sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/models/__init__.py` & `bpkio_python_sdk-1.3.0/bpkio_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/models/common.py` & `bpkio_python_sdk-1.3.0/bpkio_api/models/common.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/models/model_graph.py` & `bpkio_python_sdk-1.3.0/bpkio_api/models/model_graph.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/bpkio_api/response_handler.py` & `bpkio_python_sdk-1.3.0/bpkio_api/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.2.0/pyproject.toml` & `bpkio_python_sdk-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-python-sdk"
-version = "1.2.0"
+version = "1.3.0"
 description = "An (opinionated) Python SDK for the broadpeak.io REST APIs"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bpkio_python_sdk-1.2.0/PKG-INFO` & `bpkio_python_sdk-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-python-sdk
-Version: 1.2.0
+Version: 1.3.0
 Summary: An (opinionated) Python SDK for the broadpeak.io REST APIs
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

