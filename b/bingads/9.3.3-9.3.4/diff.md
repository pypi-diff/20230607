# Comparing `tmp/bingads-9.3.3.zip` & `tmp/bingads-9.3.4.zip`

## zipinfo {}

```diff
@@ -1,82 +1,83 @@
-Zip file size: 134871 bytes, number of entries: 80
--rw-rw-rw-  2.0 fat      324 b- defN 15-Jul-31 11:20 bingads-9.3.3/HISTORY.rst
--rw-rw-rw-  2.0 fat     1129 b- defN 15-May-08 14:35 bingads-9.3.3/LICENSE
--rw-rw-rw-  2.0 fat     5778 b- defN 15-May-08 14:35 bingads-9.3.3/make.py
--rw-rw-rw-  2.0 fat       76 b- defN 15-May-08 14:35 bingads-9.3.3/MANIFEST.in
--rw-rw-rw-  2.0 fat     3742 b- defN 15-Jul-31 11:22 bingads-9.3.3/PKG-INFO
--rw-rw-rw-  2.0 fat     1957 b- defN 15-May-08 14:35 bingads-9.3.3/README.rst
--rw-rw-rw-  2.0 fat      134 b- defN 15-May-11 11:14 bingads-9.3.3/requirements.txt
--rw-rw-rw-  2.0 fat       64 b- defN 15-Jul-31 11:22 bingads-9.3.3/setup.cfg
--rw-rw-rw-  2.0 fat     1702 b- defN 15-Jul-31 10:57 bingads-9.3.3/setup.py
--rw-rw-rw-  2.0 fat    23578 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/authorization.py
--rw-rw-rw-  2.0 fat     1642 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/exceptions.py
--rw-rw-rw-  2.0 fat      137 b- defN 15-Apr-21 12:49 bingads-9.3.3/bingads/manifest.py
--rw-rw-rw-  2.0 fat    10521 b- defN 15-Jul-29 16:15 bingads-9.3.3/bingads/service_client.py
--rw-rw-rw-  2.0 fat     3159 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/service_info.py
--rw-rw-rw-  2.0 fat      245 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/__init__.py
--rw-rw-rw-  2.0 fat    13457 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/bulk_operation.py
--rw-rw-rw-  2.0 fat      640 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/bulk_operation_progress_info.py
--rw-rw-rw-  2.0 fat     2183 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/bulk_operation_status.py
--rw-rw-rw-  2.0 fat    15202 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/bulk_service_manager.py
--rw-rw-rw-  2.0 fat    16697 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/download_parameters.py
--rw-rw-rw-  2.0 fat      803 b- defN 15-Jun-01 10:53 bingads-9.3.3/bingads/bulk/enums.py
--rw-rw-rw-  2.0 fat     2639 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/exceptions.py
--rw-rw-rw-  2.0 fat     5400 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/file_reader.py
--rw-rw-rw-  2.0 fat     2299 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/file_writer.py
--rw-rw-rw-  2.0 fat    10515 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/upload_parameters.py
--rw-rw-rw-  2.0 fat      351 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/__init__.py
--rw-rw-rw-  2.0 fat     6007 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bid_suggestion_data.py
--rw-rw-rw-  2.0 fat     3140 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_account.py
--rw-rw-rw-  2.0 fat    13285 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_ads.py
--rw-rw-rw-  2.0 fat     8327 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/bulk/entities/bulk_ad_group.py
--rw-rw-rw-  2.0 fat     9247 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/bulk/entities/bulk_ad_group_product_partition.py
--rw-rw-rw-  2.0 fat     7850 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_ad_group_product_target.py
--rw-rw-rw-  2.0 fat     9922 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/bulk/entities/bulk_campaign.py
--rw-rw-rw-  2.0 fat     4355 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/bulk/entities/bulk_campaign_product_scope.py
--rw-rw-rw-  2.0 fat     1581 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_entity.py
--rw-rw-rw-  2.0 fat     6000 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_error.py
--rw-rw-rw-  2.0 fat     9224 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_keyword.py
--rw-rw-rw-  2.0 fat    17542 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/bulk_negative_keywords.py
--rw-rw-rw-  2.0 fat    26350 b- defN 15-Apr-21 12:49 bingads-9.3.3/bingads/bulk/entities/bulk_negative_sites.py
--rw-rw-rw-  2.0 fat    12177 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/common.py
--rw-rw-rw-  2.0 fat      911 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/unknown_bulk_entity.py
--rw-rw-rw-  2.0 fat      563 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/bulk/entities/__init__.py
--rw-rw-rw-  2.0 fat     4856 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_app_ad_extensions.py
--rw-rw-rw-  2.0 fat     4587 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_call_ad_extensions.py
--rw-rw-rw-  2.0 fat     4484 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_image_ad_extensions.py
--rw-rw-rw-  2.0 fat     9662 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_location_ad_extensions.py
--rw-rw-rw-  2.0 fat    17722 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_product_ad_extensions.py
--rw-rw-rw-  2.0 fat    15601 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_site_links_ad_extensions.py
--rw-rw-rw-  2.0 fat    12898 b- defN 15-Apr-23 17:40 bingads-9.3.3/bingads/bulk/entities/ad_extensions/common.py
--rw-rw-rw-  2.0 fat      278 b- defN 15-Apr-14 11:06 bingads-9.3.3/bingads/bulk/entities/ad_extensions/__init__.py
--rw-rw-rw-  2.0 fat   124889 b- defN 15-Apr-21 12:49 bingads-9.3.3/bingads/bulk/entities/targets/bulk_targets.py
--rw-rw-rw-  2.0 fat      105 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/bulk/entities/targets/__init__.py
--rw-rw-rw-  2.0 fat      789 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/error_messages.py
--rw-rw-rw-  2.0 fat     6004 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/extensions.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/__init__.py
--rw-rw-rw-  2.0 fat     3909 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/bulk_object.py
--rw-rw-rw-  2.0 fat     9982 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/internal/bulk/bulk_object_factory.py
--rw-rw-rw-  2.0 fat     5149 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/internal/bulk/csv_headers.py
--rw-rw-rw-  2.0 fat     1984 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/csv_reader.py
--rw-rw-rw-  2.0 fat     1610 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/csv_writer.py
--rw-rw-rw-  2.0 fat      280 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/entity_info.py
--rw-rw-rw-  2.0 fat     1207 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/format_version.py
--rw-rw-rw-  2.0 fat     3115 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/internal/bulk/mappings.py
--rw-rw-rw-  2.0 fat     2420 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/object_reader.py
--rw-rw-rw-  2.0 fat     2073 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/object_writer.py
--rw-rw-rw-  2.0 fat     2384 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/internal/bulk/row_values.py
--rw-rw-rw-  2.0 fat     3334 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/stream_reader.py
--rw-rw-rw-  2.0 fat     7219 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/internal/bulk/string_table.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/__init__.py
--rw-rw-rw-  2.0 fat     1098 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/entities/bulk_entity_identifier.py
--rw-rw-rw-  2.0 fat     2423 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/entities/multi_record_bulk_entity.py
--rw-rw-rw-  2.0 fat     4373 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/entities/single_record_bulk_entity.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Apr-09 09:40 bingads-9.3.3/bingads/internal/bulk/entities/__init__.py
--rw-rw-rw-  2.0 fat   679105 b- defN 15-Jul-31 08:55 bingads-9.3.3/bingads/proxies/campaign_management_service.xml
--rw-rw-rw-  2.0 fat        1 b- defN 15-Jul-31 11:22 bingads-9.3.3/bingads.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 15-Jul-31 11:18 bingads-9.3.3/bingads.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat     3742 b- defN 15-Jul-31 11:22 bingads-9.3.3/bingads.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       52 b- defN 15-Jul-31 11:22 bingads-9.3.3/bingads.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     2884 b- defN 15-Jul-31 11:22 bingads-9.3.3/bingads.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        8 b- defN 15-Jul-31 11:22 bingads-9.3.3/bingads.egg-info/top_level.txt
-80 files, 1201084 bytes uncompressed, 120881 bytes compressed:  89.9%
+Zip file size: 135215 bytes, number of entries: 81
+-rw-rw-rw-  2.0 fat      413 b- defN 15-Aug-20 11:48 bingads-9.3.4/HISTORY.rst
+-rw-rw-rw-  2.0 fat     1117 b- defN 15-Aug-21 16:31 bingads-9.3.4/LICENSE
+-rw-rw-rw-  2.0 fat     5573 b- defN 15-Aug-21 16:31 bingads-9.3.4/make.py
+-rw-rw-rw-  2.0 fat       72 b- defN 15-Aug-21 16:31 bingads-9.3.4/MANIFEST.in
+-rw-rw-rw-  2.0 fat     3865 b- defN 15-Aug-25 10:33 bingads-9.3.4/PKG-INFO
+-rw-rw-rw-  2.0 fat     1938 b- defN 15-Aug-10 13:26 bingads-9.3.4/README.rst
+-rw-rw-rw-  2.0 fat      121 b- defN 15-Aug-21 16:31 bingads-9.3.4/requirements.txt
+-rw-rw-rw-  2.0 fat       64 b- defN 15-Aug-25 10:33 bingads-9.3.4/setup.cfg
+-rw-rw-rw-  2.0 fat     1774 b- defN 15-Aug-20 11:33 bingads-9.3.4/setup.py
+-rw-rw-rw-  2.0 fat    23578 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/authorization.py
+-rw-rw-rw-  2.0 fat     1642 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/exceptions.py
+-rw-rw-rw-  2.0 fat      137 b- defN 15-Aug-20 11:46 bingads-9.3.4/bingads/manifest.py
+-rw-rw-rw-  2.0 fat    10521 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/service_client.py
+-rw-rw-rw-  2.0 fat     3159 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/service_info.py
+-rw-rw-rw-  2.0 fat      245 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/__init__.py
+-rw-rw-rw-  2.0 fat    13477 b- defN 15-Aug-20 11:41 bingads-9.3.4/bingads/bulk/bulk_operation.py
+-rw-rw-rw-  2.0 fat      640 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/bulk_operation_progress_info.py
+-rw-rw-rw-  2.0 fat     2183 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/bulk_operation_status.py
+-rw-rw-rw-  2.0 fat    15203 b- defN 15-Aug-20 11:41 bingads-9.3.4/bingads/bulk/bulk_service_manager.py
+-rw-rw-rw-  2.0 fat    16697 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/download_parameters.py
+-rw-rw-rw-  2.0 fat      803 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/enums.py
+-rw-rw-rw-  2.0 fat     2639 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/exceptions.py
+-rw-rw-rw-  2.0 fat     5400 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/file_reader.py
+-rw-rw-rw-  2.0 fat     2299 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/file_writer.py
+-rw-rw-rw-  2.0 fat    10515 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/upload_parameters.py
+-rw-rw-rw-  2.0 fat      351 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/__init__.py
+-rw-rw-rw-  2.0 fat     6007 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bid_suggestion_data.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_account.py
+-rw-rw-rw-  2.0 fat    13285 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_ads.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_ad_group.py
+-rw-rw-rw-  2.0 fat     9247 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_ad_group_product_partition.py
+-rw-rw-rw-  2.0 fat     7850 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_ad_group_product_target.py
+-rw-rw-rw-  2.0 fat     9922 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_campaign.py
+-rw-rw-rw-  2.0 fat     4355 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_campaign_product_scope.py
+-rw-rw-rw-  2.0 fat     1581 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_entity.py
+-rw-rw-rw-  2.0 fat     6000 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_error.py
+-rw-rw-rw-  2.0 fat     9224 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_keyword.py
+-rw-rw-rw-  2.0 fat    17542 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_negative_keywords.py
+-rw-rw-rw-  2.0 fat    26350 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/bulk_negative_sites.py
+-rw-rw-rw-  2.0 fat    12177 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/common.py
+-rw-rw-rw-  2.0 fat      911 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/unknown_bulk_entity.py
+-rw-rw-rw-  2.0 fat      563 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/__init__.py
+-rw-rw-rw-  2.0 fat     4856 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_app_ad_extensions.py
+-rw-rw-rw-  2.0 fat     4587 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_call_ad_extensions.py
+-rw-rw-rw-  2.0 fat     4484 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_image_ad_extensions.py
+-rw-rw-rw-  2.0 fat     9662 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_location_ad_extensions.py
+-rw-rw-rw-  2.0 fat    17722 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_product_ad_extensions.py
+-rw-rw-rw-  2.0 fat    15601 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_site_links_ad_extensions.py
+-rw-rw-rw-  2.0 fat    12898 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/common.py
+-rw-rw-rw-  2.0 fat      278 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/ad_extensions/__init__.py
+-rw-rw-rw-  2.0 fat   124889 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/targets/bulk_targets.py
+-rw-rw-rw-  2.0 fat      105 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/bulk/entities/targets/__init__.py
+-rw-rw-rw-  2.0 fat      789 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/error_messages.py
+-rw-rw-rw-  2.0 fat     6004 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/extensions.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/__init__.py
+-rw-rw-rw-  2.0 fat     3909 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/bulk_object.py
+-rw-rw-rw-  2.0 fat     9982 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/bulk_object_factory.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/csv_headers.py
+-rw-rw-rw-  2.0 fat     1984 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/csv_reader.py
+-rw-rw-rw-  2.0 fat     1610 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/csv_writer.py
+-rw-rw-rw-  2.0 fat      280 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/entity_info.py
+-rw-rw-rw-  2.0 fat     1207 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/format_version.py
+-rw-rw-rw-  2.0 fat     3115 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/mappings.py
+-rw-rw-rw-  2.0 fat     2420 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/object_reader.py
+-rw-rw-rw-  2.0 fat     2073 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/object_writer.py
+-rw-rw-rw-  2.0 fat     2384 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/row_values.py
+-rw-rw-rw-  2.0 fat     3334 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/stream_reader.py
+-rw-rw-rw-  2.0 fat     7219 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/string_table.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/__init__.py
+-rw-rw-rw-  2.0 fat     1098 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/entities/bulk_entity_identifier.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/entities/multi_record_bulk_entity.py
+-rw-rw-rw-  2.0 fat     4373 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/entities/single_record_bulk_entity.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/internal/bulk/entities/__init__.py
+-rw-rw-rw-  2.0 fat   679105 b- defN 15-Aug-10 13:26 bingads-9.3.4/bingads/proxies/campaign_management_service.xml
+-rw-rw-rw-  2.0 fat        1 b- defN 15-Aug-25 10:33 bingads-9.3.4/bingads.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 15-Aug-25 09:45 bingads-9.3.4/bingads.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat       47 b- defN 15-Aug-25 10:33 bingads-9.3.4/bingads.egg-info/pbr.json
+-rw-rw-rw-  2.0 fat     3865 b- defN 15-Aug-25 10:33 bingads-9.3.4/bingads.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat       52 b- defN 15-Aug-25 10:33 bingads-9.3.4/bingads.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat     2910 b- defN 15-Aug-25 10:33 bingads-9.3.4/bingads.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 15-Aug-25 10:33 bingads-9.3.4/bingads.egg-info/top_level.txt
+81 files, 1201332 bytes uncompressed, 121071 bytes compressed:  89.9%
```

## zipnote {}

```diff
@@ -1,241 +1,244 @@
-Filename: bingads-9.3.3/HISTORY.rst
+Filename: bingads-9.3.4/HISTORY.rst
 Comment: 
 
-Filename: bingads-9.3.3/LICENSE
+Filename: bingads-9.3.4/LICENSE
 Comment: 
 
-Filename: bingads-9.3.3/make.py
+Filename: bingads-9.3.4/make.py
 Comment: 
 
-Filename: bingads-9.3.3/MANIFEST.in
+Filename: bingads-9.3.4/MANIFEST.in
 Comment: 
 
-Filename: bingads-9.3.3/PKG-INFO
+Filename: bingads-9.3.4/PKG-INFO
 Comment: 
 
-Filename: bingads-9.3.3/README.rst
+Filename: bingads-9.3.4/README.rst
 Comment: 
 
-Filename: bingads-9.3.3/requirements.txt
+Filename: bingads-9.3.4/requirements.txt
 Comment: 
 
-Filename: bingads-9.3.3/setup.cfg
+Filename: bingads-9.3.4/setup.cfg
 Comment: 
 
-Filename: bingads-9.3.3/setup.py
+Filename: bingads-9.3.4/setup.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/authorization.py
+Filename: bingads-9.3.4/bingads/authorization.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/exceptions.py
+Filename: bingads-9.3.4/bingads/exceptions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/manifest.py
+Filename: bingads-9.3.4/bingads/manifest.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/service_client.py
+Filename: bingads-9.3.4/bingads/service_client.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/service_info.py
+Filename: bingads-9.3.4/bingads/service_info.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/__init__.py
+Filename: bingads-9.3.4/bingads/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/bulk_operation.py
+Filename: bingads-9.3.4/bingads/bulk/bulk_operation.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/bulk_operation_progress_info.py
+Filename: bingads-9.3.4/bingads/bulk/bulk_operation_progress_info.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/bulk_operation_status.py
+Filename: bingads-9.3.4/bingads/bulk/bulk_operation_status.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/bulk_service_manager.py
+Filename: bingads-9.3.4/bingads/bulk/bulk_service_manager.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/download_parameters.py
+Filename: bingads-9.3.4/bingads/bulk/download_parameters.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/enums.py
+Filename: bingads-9.3.4/bingads/bulk/enums.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/exceptions.py
+Filename: bingads-9.3.4/bingads/bulk/exceptions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/file_reader.py
+Filename: bingads-9.3.4/bingads/bulk/file_reader.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/file_writer.py
+Filename: bingads-9.3.4/bingads/bulk/file_writer.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/upload_parameters.py
+Filename: bingads-9.3.4/bingads/bulk/upload_parameters.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/__init__.py
+Filename: bingads-9.3.4/bingads/bulk/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bid_suggestion_data.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bid_suggestion_data.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_account.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_account.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_ads.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_ads.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_ad_group.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_ad_group.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_ad_group_product_partition.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_ad_group_product_partition.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_ad_group_product_target.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_ad_group_product_target.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_campaign.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_campaign.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_campaign_product_scope.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_campaign_product_scope.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_entity.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_entity.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_error.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_error.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_keyword.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_keyword.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_negative_keywords.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_negative_keywords.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/bulk_negative_sites.py
+Filename: bingads-9.3.4/bingads/bulk/entities/bulk_negative_sites.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/common.py
+Filename: bingads-9.3.4/bingads/bulk/entities/common.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/unknown_bulk_entity.py
+Filename: bingads-9.3.4/bingads/bulk/entities/unknown_bulk_entity.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/__init__.py
+Filename: bingads-9.3.4/bingads/bulk/entities/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_app_ad_extensions.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_app_ad_extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_call_ad_extensions.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_call_ad_extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_image_ad_extensions.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_image_ad_extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_location_ad_extensions.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_location_ad_extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_product_ad_extensions.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_product_ad_extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_site_links_ad_extensions.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_site_links_ad_extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/common.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/common.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/ad_extensions/__init__.py
+Filename: bingads-9.3.4/bingads/bulk/entities/ad_extensions/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/targets/bulk_targets.py
+Filename: bingads-9.3.4/bingads/bulk/entities/targets/bulk_targets.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/bulk/entities/targets/__init__.py
+Filename: bingads-9.3.4/bingads/bulk/entities/targets/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/error_messages.py
+Filename: bingads-9.3.4/bingads/internal/error_messages.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/extensions.py
+Filename: bingads-9.3.4/bingads/internal/extensions.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/__init__.py
+Filename: bingads-9.3.4/bingads/internal/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/bulk_object.py
+Filename: bingads-9.3.4/bingads/internal/bulk/bulk_object.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/bulk_object_factory.py
+Filename: bingads-9.3.4/bingads/internal/bulk/bulk_object_factory.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/csv_headers.py
+Filename: bingads-9.3.4/bingads/internal/bulk/csv_headers.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/csv_reader.py
+Filename: bingads-9.3.4/bingads/internal/bulk/csv_reader.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/csv_writer.py
+Filename: bingads-9.3.4/bingads/internal/bulk/csv_writer.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/entity_info.py
+Filename: bingads-9.3.4/bingads/internal/bulk/entity_info.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/format_version.py
+Filename: bingads-9.3.4/bingads/internal/bulk/format_version.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/mappings.py
+Filename: bingads-9.3.4/bingads/internal/bulk/mappings.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/object_reader.py
+Filename: bingads-9.3.4/bingads/internal/bulk/object_reader.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/object_writer.py
+Filename: bingads-9.3.4/bingads/internal/bulk/object_writer.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/row_values.py
+Filename: bingads-9.3.4/bingads/internal/bulk/row_values.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/stream_reader.py
+Filename: bingads-9.3.4/bingads/internal/bulk/stream_reader.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/string_table.py
+Filename: bingads-9.3.4/bingads/internal/bulk/string_table.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/__init__.py
+Filename: bingads-9.3.4/bingads/internal/bulk/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/entities/bulk_entity_identifier.py
+Filename: bingads-9.3.4/bingads/internal/bulk/entities/bulk_entity_identifier.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/entities/multi_record_bulk_entity.py
+Filename: bingads-9.3.4/bingads/internal/bulk/entities/multi_record_bulk_entity.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/entities/single_record_bulk_entity.py
+Filename: bingads-9.3.4/bingads/internal/bulk/entities/single_record_bulk_entity.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/internal/bulk/entities/__init__.py
+Filename: bingads-9.3.4/bingads/internal/bulk/entities/__init__.py
 Comment: 
 
-Filename: bingads-9.3.3/bingads/proxies/campaign_management_service.xml
+Filename: bingads-9.3.4/bingads/proxies/campaign_management_service.xml
 Comment: 
 
-Filename: bingads-9.3.3/bingads.egg-info/dependency_links.txt
+Filename: bingads-9.3.4/bingads.egg-info/dependency_links.txt
 Comment: 
 
-Filename: bingads-9.3.3/bingads.egg-info/not-zip-safe
+Filename: bingads-9.3.4/bingads.egg-info/not-zip-safe
 Comment: 
 
-Filename: bingads-9.3.3/bingads.egg-info/PKG-INFO
+Filename: bingads-9.3.4/bingads.egg-info/pbr.json
 Comment: 
 
-Filename: bingads-9.3.3/bingads.egg-info/requires.txt
+Filename: bingads-9.3.4/bingads.egg-info/PKG-INFO
 Comment: 
 
-Filename: bingads-9.3.3/bingads.egg-info/SOURCES.txt
+Filename: bingads-9.3.4/bingads.egg-info/requires.txt
 Comment: 
 
-Filename: bingads-9.3.3/bingads.egg-info/top_level.txt
+Filename: bingads-9.3.4/bingads.egg-info/SOURCES.txt
+Comment: 
+
+Filename: bingads-9.3.4/bingads.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `bingads-9.3.3/LICENSE` & `bingads-9.3.4/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Bing Ads Python SDK
-
-Copyright (c) Microsoft Corporation
-
-All rights reserved.
-
-MIT License
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ""Software""), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Bing Ads Python SDK
+
+Copyright (c) Microsoft Corporation
+
+All rights reserved.
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ""Software""), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED *AS IS*, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `bingads-9.3.3/make.py` & `bingads-9.3.4/make.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-import os
-from subprocess import call
-
-dependent_graph = {}
-tasks = {}
-
-
-def dependent_on(*dependent_funcs):
-    """ Describe the dependencies of a specific functions.
-
-    :param dependent_funcs: dependent functions
-    :return: decorated function
-    """
-
-    def dependencies_wrapper(func):
-        dependent_graph[func.__name__] = [dependent_func.__name__ for dependent_func in dependent_funcs]
-        return func
-
-    return dependencies_wrapper
-
-
-def task(description=None):
-    """ Describe the function be decorated by this task function.
-
-    :param description: the description of decorated function
-    :return: decorated function
-    """
-
-    if description is None:
-        description = ''
-
-    def task_wrapper(func):
-        tasks[func.__name__] = description
-        return func
-
-    return task_wrapper
-
-
-def delete_file(file_path):
-    """ Delete file specified by path.
-
-    :param file_path: the file path
-    :type file_path: str
-    :return: None
-    """
-
-    try:
-        os.remove(file_path)
-    except OSError:
-        pass
-
-
-def delete_folder(folder_path):
-    """ Delete folder specified by path and all the files under it recursively.
-
-    :param folder_path: the folder path
-    :type folder_path: the folder path
-    :return: None
-    """
-
-    import shutil
-
-    shutil.rmtree(folder_path, ignore_errors=True)
-
-
-def run_cmd(command):
-    """ Run os command.
-
-    :param command: the concrete content of command
-    :type command: str
-    :return: None
-    """
-
-    print(command)
-    call(command, shell=True)
-
-
-def make_execution_plan(func_name):
-    """ Make the execution plan for a specific function, consider the dependencies.
-
-    After analyze the dependency graph, use topological sort to give a proper execution order
-
-    :param func_name: the function name to be executed
-    :type func_name: str
-    :return: the iterable function names, by execution order
-    :rtype: iter(str)
-    """
-
-    in_degree = {}
-    next_tasks = {}
-
-    remaining = [func_name]
-    while len(remaining) != 0:
-        current = remaining.pop()
-        if current not in dependent_graph:
-            if current not in in_degree:
-                in_degree[current] = 0
-            if current not in next_tasks:
-                next_tasks[current] = []
-            continue
-        if current not in in_degree:
-            in_degree[current] = 0
-        in_degree[current] += len(dependent_graph[current])
-        if current not in next_tasks:
-            next_tasks[current] = []
-        for dependent_func in dependent_graph[current]:
-            if dependent_func not in in_degree:
-                in_degree[dependent_func] = 0
-            if dependent_func not in next_tasks:
-                next_tasks[dependent_func] = []
-            next_tasks[dependent_func].append(current)
-    while len(in_degree) != 0:
-        for t in in_degree.keys():
-            # can be optimized here, use linear search for easy to implemented and no performance concern currently
-            if in_degree[t] == 0:
-                t_selected = t
-                break
-        for t_next in next_tasks[t_selected]:
-            in_degree[t_next] -= 1
-        in_degree.pop(t_selected)
-        next_tasks.pop(t_selected)
-        yield t_selected
-
-
-##########################
-# Define Tasks From Here #
-##########################
-
-
-@task('clean the temporary output file')
-def clean():
-    delete_folder('.tox')
-    delete_folder('bingads.egg-info')
-    delete_folder('docs/_build')
-    delete_folder('dist')
-    delete_file('.coverage')
-
-
-@task('code style check by flake8')
-def lint():
-    run_cmd('flake8 bingads tests')
-
-
-@task('run all tests under current interpreter, and print coverage report')
-def test():
-    run_cmd('coverage run --source bingads -m py.test -v --strict')
-    run_cmd('coverage report')
-
-
-@task('run all unit tests under current interpreter, and print coverage report')
-def ut():
-    run_cmd('coverage run --source bingads -m py.test -k "not functional" -v --strict')
-    run_cmd('coverage report')
-
-
-@task('run all functional tests under current interpreter.')
-def ft():
-    run_cmd('py.test -k "functional" -v --strict')
-
-
-@task('run tests on all supported interpreters (check tox.ini)')
-@dependent_on(clean)
-def test_all():
-    run_cmd('tox')
-
-
-@task('generate static html documents, by sphinx, under docs/_build/html')
-@dependent_on(clean)
-def docs():
-    run_cmd('sphinx-apidoc -F -o docs bingads')  # generate API rst file, may need to check-in
-    run_cmd('sphinx-build -b html docs docs/_build/html')  # generate html file
-
-
-@task('make compressed installation package')
-@dependent_on(clean)
-def dist():
-    run_cmd('python setup.py sdist --formats=gztar,zip')
-
-
-if __name__ == '__main__':
-    from sys import argv, exit, modules
-
-    if len(argv) == 1:
-        if len(tasks) == 0:
-            print('No task defined yet.')
-            exit(0)
-        max_length = 0
-        for key in tasks.keys():
-            if len(key) > max_length:
-                max_length = len(key)
-        format_str = '{0:<' + str(max_length) + '}  --  {1}'
-        for key in tasks.keys():
-            print(format_str.format(key, tasks[key]))
-    elif len(argv) > 2:
-        print('Only support one task at a time')
-        exit(-1)
-    else:
-        task_name = argv[1]
-        if task_name not in tasks:
-            print(str.format("Task: '{0}' not defined", task_name))
-            exit(-1)
-        task_names = make_execution_plan(task_name)
-        for task_name in task_names:
-            task = getattr(modules[__name__], task_name)
-            task()
+import os
+from subprocess import call
+
+dependent_graph = {}
+tasks = {}
+
+
+def dependent_on(*dependent_funcs):
+    """ Describe the dependencies of a specific functions.
+
+    :param dependent_funcs: dependent functions
+    :return: decorated function
+    """
+
+    def dependencies_wrapper(func):
+        dependent_graph[func.__name__] = [dependent_func.__name__ for dependent_func in dependent_funcs]
+        return func
+
+    return dependencies_wrapper
+
+
+def task(description=None):
+    """ Describe the function be decorated by this task function.
+
+    :param description: the description of decorated function
+    :return: decorated function
+    """
+
+    if description is None:
+        description = ''
+
+    def task_wrapper(func):
+        tasks[func.__name__] = description
+        return func
+
+    return task_wrapper
+
+
+def delete_file(file_path):
+    """ Delete file specified by path.
+
+    :param file_path: the file path
+    :type file_path: str
+    :return: None
+    """
+
+    try:
+        os.remove(file_path)
+    except OSError:
+        pass
+
+
+def delete_folder(folder_path):
+    """ Delete folder specified by path and all the files under it recursively.
+
+    :param folder_path: the folder path
+    :type folder_path: the folder path
+    :return: None
+    """
+
+    import shutil
+
+    shutil.rmtree(folder_path, ignore_errors=True)
+
+
+def run_cmd(command):
+    """ Run os command.
+
+    :param command: the concrete content of command
+    :type command: str
+    :return: None
+    """
+
+    print(command)
+    call(command, shell=True)
+
+
+def make_execution_plan(func_name):
+    """ Make the execution plan for a specific function, consider the dependencies.
+
+    After analyze the dependency graph, use topological sort to give a proper execution order
+
+    :param func_name: the function name to be executed
+    :type func_name: str
+    :return: the iterable function names, by execution order
+    :rtype: iter(str)
+    """
+
+    in_degree = {}
+    next_tasks = {}
+
+    remaining = [func_name]
+    while len(remaining) != 0:
+        current = remaining.pop()
+        if current not in dependent_graph:
+            if current not in in_degree:
+                in_degree[current] = 0
+            if current not in next_tasks:
+                next_tasks[current] = []
+            continue
+        if current not in in_degree:
+            in_degree[current] = 0
+        in_degree[current] += len(dependent_graph[current])
+        if current not in next_tasks:
+            next_tasks[current] = []
+        for dependent_func in dependent_graph[current]:
+            if dependent_func not in in_degree:
+                in_degree[dependent_func] = 0
+            if dependent_func not in next_tasks:
+                next_tasks[dependent_func] = []
+            next_tasks[dependent_func].append(current)
+    while len(in_degree) != 0:
+        for t in in_degree.keys():
+            # can be optimized here, use linear search for easy to implemented and no performance concern currently
+            if in_degree[t] == 0:
+                t_selected = t
+                break
+        for t_next in next_tasks[t_selected]:
+            in_degree[t_next] -= 1
+        in_degree.pop(t_selected)
+        next_tasks.pop(t_selected)
+        yield t_selected
+
+
+##########################
+# Define Tasks From Here #
+##########################
+
+
+@task('clean the temporary output file')
+def clean():
+    delete_folder('.tox')
+    delete_folder('bingads.egg-info')
+    delete_folder('docs/_build')
+    delete_folder('dist')
+    delete_file('.coverage')
+
+
+@task('code style check by flake8')
+def lint():
+    run_cmd('flake8 bingads tests')
+
+
+@task('run all tests under current interpreter, and print coverage report')
+def test():
+    run_cmd('coverage run --source bingads -m py.test -v --strict')
+    run_cmd('coverage report')
+
+
+@task('run all unit tests under current interpreter, and print coverage report')
+def ut():
+    run_cmd('coverage run --source bingads -m py.test -k "not functional" -v --strict')
+    run_cmd('coverage report')
+
+
+@task('run all functional tests under current interpreter.')
+def ft():
+    run_cmd('py.test -k "functional" -v --strict')
+
+
+@task('run tests on all supported interpreters (check tox.ini)')
+@dependent_on(clean)
+def test_all():
+    run_cmd('tox')
+
+
+@task('generate static html documents, by sphinx, under docs/_build/html')
+@dependent_on(clean)
+def docs():
+    run_cmd('sphinx-apidoc -F -o docs bingads')  # generate API rst file, may need to check-in
+    run_cmd('sphinx-build -b html docs docs/_build/html')  # generate html file
+
+
+@task('make compressed installation package')
+@dependent_on(clean)
+def dist():
+    run_cmd('python setup.py sdist --formats=gztar,zip')
+
+
+if __name__ == '__main__':
+    from sys import argv, exit, modules
+
+    if len(argv) == 1:
+        if len(tasks) == 0:
+            print('No task defined yet.')
+            exit(0)
+        max_length = 0
+        for key in tasks.keys():
+            if len(key) > max_length:
+                max_length = len(key)
+        format_str = '{0:<' + str(max_length) + '}  --  {1}'
+        for key in tasks.keys():
+            print(format_str.format(key, tasks[key]))
+    elif len(argv) > 2:
+        print('Only support one task at a time')
+        exit(-1)
+    else:
+        task_name = argv[1]
+        if task_name not in tasks:
+            print(str.format("Task: '{0}' not defined", task_name))
+            exit(-1)
+        task_names = make_execution_plan(task_name)
+        for task_name in task_names:
+            task = getattr(modules[__name__], task_name)
+            task()
```

## Comparing `bingads-9.3.3/PKG-INFO` & `bingads-9.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bingads
-Version: 9.3.3
+Version: 9.3.4
 Summary: A library to make working with the Bing Ads APIs and bulk services easy
 Home-page: https://github.com/bing-ads-sdk/BingAds-Python-SDK
 Author: Bing Ads SDK Team
 Author-email: bing_ads_sdk@microsoft.com
 License: MIT
 Description: ===================
         Bing Ads Python SDK
@@ -15,15 +15,15 @@
         
         .. image:: https://img.shields.io/pypi/dm/bingads.svg
                 :target: https://pypi.python.org/pypi/bingads
         
         
         The Bing Ads Python Software Development Kit (SDK) Version 9.3 enhances the experience of developing Bing Ads applications
         with the Python programming language.
-        The SDK uses the `suds-jurko`_ library as a proxy for all Bing Ads API web services and abstracts the low level details of authentication with OAuth.
+        The SDK includes proxy classes for all Bing Ads API web services and abstracts the low level details of authentication with OAuth.
         You can also read and write bulk files with the SDK BulkFileReader and BulkFileWriter,
         and use the high level BulkServiceManager interface to abstract and execute operations in the low level Bulk API.
         For more information, see `Bing Ads Python SDK`_ on MSDN.
         
         Getting Started
         ---------------
         
@@ -54,36 +54,41 @@
         
         
         
         
         Release History
         ---------------
         
+        9.3.4 (2015-08-20)
+        ++++++++++++++++++
+        
+        * Replace SSLv3 with SSLv23 for TLS support
+        
+        
         9.3.3 (2015-07-31)
         ++++++++++++++++++
         
         * Add Bing Shopping Campaign Support
         * Add Native Ads Support
         
         
         9.3.2 (2015-04-24)
         ++++++++++++++++++
         
         * Add App AdExtension support.
         * Bug Fixes.
         
-        
         9.3.1 (2015-03-31)
         ++++++++++++++++++
         
         * First release on PyPI.
         
 Keywords: bingads
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
```

## Comparing `bingads-9.3.3/README.rst` & `bingads-9.3.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 .. image:: https://img.shields.io/pypi/dm/bingads.svg
         :target: https://pypi.python.org/pypi/bingads
 
 
 The Bing Ads Python Software Development Kit (SDK) Version 9.3 enhances the experience of developing Bing Ads applications
 with the Python programming language.
-The SDK uses the `suds-jurko`_ library as a proxy for all Bing Ads API web services and abstracts the low level details of authentication with OAuth.
+The SDK includes proxy classes for all Bing Ads API web services and abstracts the low level details of authentication with OAuth.
 You can also read and write bulk files with the SDK BulkFileReader and BulkFileWriter,
 and use the high level BulkServiceManager interface to abstract and execute operations in the low level Bulk API.
 For more information, see `Bing Ads Python SDK`_ on MSDN.
 
 Getting Started
 ---------------
```

## Comparing `bingads-9.3.3/setup.py` & `bingads-9.3.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-VERSION = '9.3.3'
-
-with open('README.rst', 'r') as f:
-    readme = f.read()
-with open('HISTORY.rst', 'r') as f:
-    history = f.read().replace('.. :changelog:', '')
-
-requirements = [
-    'suds-jurko==0.6.0',
-    'future',
-    'six',
-    'requests',
-    'enum34',
-    'chardet',
-]
-
-setup(
-    name='bingads',
-    version=VERSION,
-    description='A library to make working with the Bing Ads APIs and bulk services easy',
-    long_description=readme + '\n\n' + history,
-    author='Bing Ads SDK Team',
-    author_email='bing_ads_sdk@microsoft.com',
-    url='https://github.com/bing-ads-sdk/BingAds-Python-SDK',
-    packages=[
-        'bingads',
-        'bingads.bulk',
-        'bingads.bulk.entities',
-        'bingads.bulk.entities.ad_extensions',
-        'bingads.bulk.entities.targets',
-        'bingads.internal',
-        'bingads.internal.bulk',
-        'bingads.internal.bulk.entities',
-    ],
-    include_package_data=True,
-    install_requires=requirements,
-    license='MIT',
-    zip_safe=False,
-    keywords='bingads',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-    ],
-)
+try:
+    from setuptools import setup
+except ImportError:
+    from distutils.core import setup
+
+VERSION = '9.3.4'
+
+with open('README.rst', 'r') as f:
+    readme = f.read()
+with open('HISTORY.rst', 'r') as f:
+    history = f.read().replace('.. :changelog:', '')
+
+requirements = [
+    'suds-jurko==0.6.0',
+    'future',
+    'six',
+    'requests',
+    'enum34',
+    'chardet',
+]
+
+setup(
+    name='bingads',
+    version=VERSION,
+    description='A library to make working with the Bing Ads APIs and bulk services easy',
+    long_description=readme + '\n\n' + history,
+    author='Bing Ads SDK Team',
+    author_email='bing_ads_sdk@microsoft.com',
+    url='https://github.com/bing-ads-sdk/BingAds-Python-SDK',
+    packages=[
+        'bingads',
+        'bingads.bulk',
+        'bingads.bulk.entities',
+        'bingads.bulk.entities.ad_extensions',
+        'bingads.bulk.entities.targets',
+        'bingads.internal',
+        'bingads.internal.bulk',
+        'bingads.internal.bulk.entities',
+    ],
+    include_package_data=True,
+    install_requires=requirements,
+    license='MIT',
+    zip_safe=False,
+    keywords='bingads',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 2.6',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.4',
+    ],
+)
```

## Comparing `bingads-9.3.3/bingads/authorization.py` & `bingads-9.3.4/bingads/authorization.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/exceptions.py` & `bingads-9.3.4/bingads/exceptions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/service_client.py` & `bingads-9.3.4/bingads/service_client.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/service_info.py` & `bingads-9.3.4/bingads/service_info.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/bulk_operation.py` & `bingads-9.3.4/bingads/bulk/bulk_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from ..service_client import ServiceClient
 from ..manifest import *
 
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.poolmanager import PoolManager
 
 
-class Ssl3HttpAdapter(HTTPAdapter):
-    """" Transport adapter" that allows us to use SSLv3. """
+class Ssl23HttpAdapter(HTTPAdapter):
+    """" Transport adapter" that allows us to use SSLv3 and TLS protocols """
 
     def init_poolmanager(self, connections, maxsize, block=False):
         self.poolmanager = PoolManager(
             num_pools=connections,
             maxsize=maxsize,
             block=block,
-            ssl_version=ssl.PROTOCOL_SSLv3,
+            ssl_version=ssl.PROTOCOL_SSLv23,
         )
 
 
 class BulkOperation(object):
     """ The base class that can be derived to represent a bulk operation requested by a user.
 
     You can use either the :class:`.BulkDownloadOperation` or :class:`.BulkUploadOperation`
@@ -87,15 +87,15 @@
                 raise FileExistsError('Result file: {0} exists'.format(result_file_path))
             else:
                 raise OSError('Result file: {0} exists'.format(result_file_path))
         headers = {
             'User-Agent': USER_AGENT,
         }
         s = requests.Session()
-        s.mount('https://', Ssl3HttpAdapter())
+        s.mount('https://', Ssl23HttpAdapter())
         r = s.get(url, headers=headers, stream=True, verify=True)
         r.raise_for_status()
         try:
             with open(zip_file_path, 'wb') as f:
                 for chunk in r.iter_content(chunk_size=4096):
                     if chunk:
                         f.write(chunk)
```

## Comparing `bingads-9.3.3/bingads/bulk/bulk_operation_progress_info.py` & `bingads-9.3.4/bingads/bulk/bulk_operation_progress_info.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/bulk_operation_status.py` & `bingads-9.3.4/bingads/bulk/bulk_operation_status.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/bulk_service_manager.py` & `bingads-9.3.4/bingads/bulk/bulk_service_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
             self._authorization_data.authentication.enrich_headers(headers)
 
             with open(upload_file_path, 'rb') as f:
                 name, ext = path.splitext(upload_file_path)
 
                 filename = '{0}{1}'.format(uuid.uuid1(), ext)
                 s = requests.Session()
-                s.mount('https://', Ssl3HttpAdapter())
+                s.mount('https://', Ssl23HttpAdapter())
                 r = s.post(url, files={'file': (filename, f)}, verify=True, headers=headers)
                 r.raise_for_status()
         except Exception as ex:
             raise ex
         finally:
             if should_compress:
                 name, ext = path.splitext(upload_file_path)
```

## Comparing `bingads-9.3.3/bingads/bulk/download_parameters.py` & `bingads-9.3.4/bingads/bulk/download_parameters.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/enums.py` & `bingads-9.3.4/bingads/bulk/enums.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/exceptions.py` & `bingads-9.3.4/bingads/bulk/exceptions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/file_reader.py` & `bingads-9.3.4/bingads/bulk/file_reader.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/file_writer.py` & `bingads-9.3.4/bingads/bulk/file_writer.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/upload_parameters.py` & `bingads-9.3.4/bingads/bulk/upload_parameters.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bid_suggestion_data.py` & `bingads-9.3.4/bingads/bulk/entities/bid_suggestion_data.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_account.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_account.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_ads.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_ads.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_ad_group.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_ad_group.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_ad_group_product_partition.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_ad_group_product_partition.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_ad_group_product_target.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_ad_group_product_target.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_campaign.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_campaign.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_campaign_product_scope.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_campaign_product_scope.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_entity.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_entity.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_error.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_error.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_keyword.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_keyword.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_negative_keywords.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_negative_keywords.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/bulk_negative_sites.py` & `bingads-9.3.4/bingads/bulk/entities/bulk_negative_sites.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/common.py` & `bingads-9.3.4/bingads/bulk/entities/common.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/unknown_bulk_entity.py` & `bingads-9.3.4/bingads/bulk/entities/unknown_bulk_entity.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/__init__.py` & `bingads-9.3.4/bingads/bulk/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_app_ad_extensions.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_app_ad_extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_call_ad_extensions.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_call_ad_extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_image_ad_extensions.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_image_ad_extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_location_ad_extensions.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_location_ad_extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_product_ad_extensions.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_product_ad_extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/bulk_site_links_ad_extensions.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/bulk_site_links_ad_extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/ad_extensions/common.py` & `bingads-9.3.4/bingads/bulk/entities/ad_extensions/common.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/bulk/entities/targets/bulk_targets.py` & `bingads-9.3.4/bingads/bulk/entities/targets/bulk_targets.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/error_messages.py` & `bingads-9.3.4/bingads/internal/error_messages.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/extensions.py` & `bingads-9.3.4/bingads/internal/extensions.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/bulk_object.py` & `bingads-9.3.4/bingads/internal/bulk/bulk_object.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/bulk_object_factory.py` & `bingads-9.3.4/bingads/internal/bulk/bulk_object_factory.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/csv_headers.py` & `bingads-9.3.4/bingads/internal/bulk/csv_headers.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/csv_reader.py` & `bingads-9.3.4/bingads/internal/bulk/csv_reader.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/csv_writer.py` & `bingads-9.3.4/bingads/internal/bulk/csv_writer.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/format_version.py` & `bingads-9.3.4/bingads/internal/bulk/format_version.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/mappings.py` & `bingads-9.3.4/bingads/internal/bulk/mappings.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/object_reader.py` & `bingads-9.3.4/bingads/internal/bulk/object_reader.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/object_writer.py` & `bingads-9.3.4/bingads/internal/bulk/object_writer.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/row_values.py` & `bingads-9.3.4/bingads/internal/bulk/row_values.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/stream_reader.py` & `bingads-9.3.4/bingads/internal/bulk/stream_reader.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/string_table.py` & `bingads-9.3.4/bingads/internal/bulk/string_table.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/entities/bulk_entity_identifier.py` & `bingads-9.3.4/bingads/internal/bulk/entities/bulk_entity_identifier.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/entities/multi_record_bulk_entity.py` & `bingads-9.3.4/bingads/internal/bulk/entities/multi_record_bulk_entity.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/internal/bulk/entities/single_record_bulk_entity.py` & `bingads-9.3.4/bingads/internal/bulk/entities/single_record_bulk_entity.py`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads/proxies/campaign_management_service.xml` & `bingads-9.3.4/bingads/proxies/campaign_management_service.xml`

 * *Files identical despite different names*

## Comparing `bingads-9.3.3/bingads.egg-info/PKG-INFO` & `bingads-9.3.4/bingads.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bingads
-Version: 9.3.3
+Version: 9.3.4
 Summary: A library to make working with the Bing Ads APIs and bulk services easy
 Home-page: https://github.com/bing-ads-sdk/BingAds-Python-SDK
 Author: Bing Ads SDK Team
 Author-email: bing_ads_sdk@microsoft.com
 License: MIT
 Description: ===================
         Bing Ads Python SDK
@@ -15,15 +15,15 @@
         
         .. image:: https://img.shields.io/pypi/dm/bingads.svg
                 :target: https://pypi.python.org/pypi/bingads
         
         
         The Bing Ads Python Software Development Kit (SDK) Version 9.3 enhances the experience of developing Bing Ads applications
         with the Python programming language.
-        The SDK uses the `suds-jurko`_ library as a proxy for all Bing Ads API web services and abstracts the low level details of authentication with OAuth.
+        The SDK includes proxy classes for all Bing Ads API web services and abstracts the low level details of authentication with OAuth.
         You can also read and write bulk files with the SDK BulkFileReader and BulkFileWriter,
         and use the high level BulkServiceManager interface to abstract and execute operations in the low level Bulk API.
         For more information, see `Bing Ads Python SDK`_ on MSDN.
         
         Getting Started
         ---------------
         
@@ -54,36 +54,41 @@
         
         
         
         
         Release History
         ---------------
         
+        9.3.4 (2015-08-20)
+        ++++++++++++++++++
+        
+        * Replace SSLv3 with SSLv23 for TLS support
+        
+        
         9.3.3 (2015-07-31)
         ++++++++++++++++++
         
         * Add Bing Shopping Campaign Support
         * Add Native Ads Support
         
         
         9.3.2 (2015-04-24)
         ++++++++++++++++++
         
         * Add App AdExtension support.
         * Bug Fixes.
         
-        
         9.3.1 (2015-03-31)
         ++++++++++++++++++
         
         * First release on PyPI.
         
 Keywords: bingads
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
```

## Comparing `bingads-9.3.3/bingads.egg-info/SOURCES.txt` & `bingads-9.3.4/bingads.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 bingads/manifest.py
 bingads/service_client.py
 bingads/service_info.py
 bingads.egg-info/PKG-INFO
 bingads.egg-info/SOURCES.txt
 bingads.egg-info/dependency_links.txt
 bingads.egg-info/not-zip-safe
+bingads.egg-info/pbr.json
 bingads.egg-info/requires.txt
 bingads.egg-info/top_level.txt
 bingads/bulk/__init__.py
 bingads/bulk/bulk_operation.py
 bingads/bulk/bulk_operation_progress_info.py
 bingads/bulk/bulk_operation_status.py
 bingads/bulk/bulk_service_manager.py
```

