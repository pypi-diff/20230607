# Comparing `tmp/amazon_ad_sdk-0.2.5.tar.gz` & `tmp/amazon_ad_sdk-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_ad_sdk-0.2.5.tar", last modified: Thu Mar 30 12:07:30 2023, max compression
+gzip compressed data, was "dist/amazon_ad_sdk-0.2.6.tar", last modified: Wed Jun  7 06:50:16 2023, max compression
```

## Comparing `amazon_ad_sdk-0.2.5.tar` & `amazon_ad_sdk-0.2.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/
--rw-r--r--   0 linrenwei   (501) staff       (20)     1068 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/LICENSE
--rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/PKG-INFO
--rw-r--r--   0 linrenwei   (501) staff       (20)     1733 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/README.md
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/__init__.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/__init__.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/amazon_attribution/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-24 08:21:26.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/amazon_attribution/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      338 2022-08-24 08:56:49.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/amazon_attribution/advertisers.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      334 2022-08-24 08:57:59.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/amazon_attribution/publishers.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1963 2022-08-24 08:53:29.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/amazon_attribution/reports.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      761 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/auth.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     2638 2023-03-30 12:04:03.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/base.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/dsp/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/dsp/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    29048 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/dsp/report.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1323 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/profiles.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1052 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sb/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sb/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      503 2022-02-23 08:45:10.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sb/campaigns.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    57122 2022-10-19 05:58:06.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sb/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sd/
--rw-r--r--   0 linrenwei   (501) staff       (20)       46 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sd/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    40139 2022-10-13 12:52:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sd/report.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    26080 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sd/scripts.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sp/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sp/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    27147 2022-03-21 12:32:00.000000 amazon_ad_sdk-0.2.5/amazon_ad/api/sp/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-17 09:27:17.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    25191 2023-01-29 02:36:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/adapters.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      742 2022-08-17 09:31:44.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/base.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      850 2022-08-18 06:39:58.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sb/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-23 05:40:22.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sb/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      846 2022-08-23 08:33:25.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sb/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sp/
--rw-r--r--   0 linrenwei   (501) staff       (20)       24 2022-08-17 11:44:06.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sp/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     5308 2022-08-24 11:51:06.000000 amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sp/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/client/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/client/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1319 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/client/auth.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     8080 2022-08-24 08:18:35.000000 amazon_ad_sdk-0.2.5/amazon_ad/client/base.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     4861 2022-09-19 06:11:33.000000 amazon_ad_sdk-0.2.5/amazon_ad/client/service.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1437 2023-03-30 12:06:22.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/consts.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     2091 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/exceptions.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/utils/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/utils/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      893 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/utils/amazon.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      534 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/utils/serialize.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1141 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.5/amazon_ad/core/utils/text.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/
--rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/PKG-INFO
--rw-r--r--   0 linrenwei   (501) staff       (20)     1369 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)        1 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)      158 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/requires.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)       10 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/top_level.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)       38 2023-03-30 12:07:30.000000 amazon_ad_sdk-0.2.5/setup.cfg
--rw-r--r--   0 linrenwei   (501) staff       (20)     1067 2023-03-30 12:06:45.000000 amazon_ad_sdk-0.2.5/setup.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1068 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/LICENSE
+-rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/PKG-INFO
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1733 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/README.md
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/__init__.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/__init__.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/amazon_attribution/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-24 08:21:26.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/amazon_attribution/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      338 2022-08-24 08:56:49.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/amazon_attribution/advertisers.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      334 2022-08-24 08:57:59.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/amazon_attribution/publishers.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1963 2022-08-24 08:53:29.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/amazon_attribution/reports.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      761 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/auth.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     2638 2023-03-30 12:04:03.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/base.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/dsp/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/dsp/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    29048 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/dsp/report.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1323 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/profiles.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1052 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sb/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2023-06-07 06:33:01.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sb/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      503 2022-02-23 08:45:10.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sb/campaigns.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    58155 2023-06-07 06:47:49.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sb/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sd/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       46 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sd/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    40139 2022-10-13 12:52:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sd/report.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    26080 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sd/scripts.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sp/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sp/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    27147 2022-03-21 12:32:00.000000 amazon_ad_sdk-0.2.6/amazon_ad/api/sp/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-17 09:27:17.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    25502 2023-06-07 03:33:10.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/adapters.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      742 2022-08-17 09:31:44.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/base.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      850 2022-08-18 06:39:58.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sb/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-23 05:40:22.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sb/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      846 2022-08-23 08:33:25.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sb/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sp/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       24 2022-08-17 11:44:06.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sp/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     5308 2022-08-24 11:51:06.000000 amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sp/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/client/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/client/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1319 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/client/auth.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     8080 2022-08-24 08:18:35.000000 amazon_ad_sdk-0.2.6/amazon_ad/client/base.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     4861 2022-09-19 06:11:33.000000 amazon_ad_sdk-0.2.6/amazon_ad/client/service.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1437 2023-03-30 12:06:22.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/consts.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     2091 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/exceptions.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/utils/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/utils/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      893 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/utils/amazon.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      534 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/utils/serialize.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1141 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.6/amazon_ad/core/utils/text.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/
+-rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1369 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)        1 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)      158 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/requires.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)       10 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/top_level.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)       38 2023-06-07 06:50:16.000000 amazon_ad_sdk-0.2.6/setup.cfg
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1067 2023-06-07 06:48:53.000000 amazon_ad_sdk-0.2.6/setup.py
```

### Comparing `amazon_ad_sdk-0.2.5/LICENSE` & `amazon_ad_sdk-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/README.md` & `amazon_ad_sdk-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/amazon_attribution/reports.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/amazon_attribution/reports.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/auth.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/auth.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/base.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/base.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/dsp/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/dsp/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/profiles.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/profiles.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/sb/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/sb/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,14 +561,18 @@
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
                 'vtr',
+
+                'attributedBrandedSearches14d',
+                'currency',
+                'topOfSearchImpressionShare',
             ]
 
         return self.request('campaigns', report_date, metrics, creative_type=creative_type)
 
     def placements(self, report_date, metrics=None):
         """
         placements = set(json.loads(client.sb_report.placements(report_date=report_date)['kwargs']['data'].decode('utf-8'))['metrics'].split(','))
@@ -728,15 +732,22 @@
                 'video5SecondViews',
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
-                'vtr'
+                'vtr',
+
+                'applicableBudgetRuleId',
+                'applicableBudgetRuleName',
+                'attributedBrandedSearches14d',
+                'campaignRuleBasedBudget',
+                'currency',
+                'topOfSearchImpressionShare',
             ]
         return self.request('campaigns', report_date, metrics, segment=segment, creative_type=creative_type)
 
     def ad_groups(self, report_date, metrics=None):
         """
         ad_groups = set(json.loads(client.sb_report.ad_groups(report_date=report_date)['kwargs']['data'].decode('utf-8'))['metrics'].split(','))
 
@@ -901,15 +912,18 @@
                 'video5SecondViews',
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
-                'vtr'
+                'vtr',
+
+                'attributedBrandedSearches14d',
+                'currency',
             ]
         return self.request('adGroups', report_date, metrics, creative_type=creative_type)
 
     def keywords(self, report_date, metrics=None):
         """
         keywords = set(json.loads(client.sb_report.keywords(report_date=report_date)['kwargs']['data'].decode('utf-8'))['metrics'].split(','))
 
@@ -1102,14 +1116,22 @@
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
                 'vtr',
+
+                'applicableBudgetRuleId',
+                'applicableBudgetRuleName',
+                'attributedBrandedSearches14d',
+                'campaignRuleBasedBudget',
+                'currency',
+                'keywordId',
+                'topOfSearchImpressionShare',
             ]
         return self.request('keywords', report_date, metrics, creative_type=creative_type)
 
     def keywords_query(self, report_date, metrics=None):
         """
         keywords_query = set(json.loads(client.sb_report.keywords_query(report_date=report_date)['kwargs']['data'].decode('utf-8'))['metrics'].split(','))
 
@@ -1245,15 +1267,20 @@
                 'video5SecondViews',
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
-                'vtr'
+                'vtr',
+
+                'keywordId',
+                'query',
+                'searchTermImpressionRank',
+                'searchTermImpressionShare',
             ]
         return self.request('keywords', report_date, metrics, segment=segment, creative_type=creative_type)
 
     def keywords_placement(self, report_date, metrics=None):
         """
         keywords_placement = set(json.loads(client.sb_report.keywords_placement(report_date=report_date)['kwargs']['data'].decode('utf-8'))['metrics'].split(','))
 
@@ -1630,15 +1657,19 @@
                 'video5SecondViews',
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
-                'vtr'
+                'vtr',
+
+                'attributedBrandedSearches14d',
+                'currency',
+                'topOfSearchImpressionShare',
             ]
         return self.request('targets', report_date, metrics, creative_type=creative_type)
 
     def ads_all(self, report_date, metrics=None):
         """
         ads_all = set(json.loads(client.sb_report.ads_all(report_date=report_date)['kwargs']['data'].decode('utf-8'))['metrics'].split(','))
 
@@ -1683,14 +1714,16 @@
                 'videoCompleteViews',
                 'videoFirstQuartileViews',
                 'videoMidpointViews',
                 'videoThirdQuartileViews',
                 'videoUnmutes',
                 'viewableImpressions',
                 'vtr',
+
+                'currency',
             ]
         return self.request('ads', report_date, metrics, creative_type=creative_type)
 
     def local_test(self, **kwargs):
         """
         测试用的接口
         """
```

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/sd/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/sd/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/sd/scripts.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/sd/scripts.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api/sp/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api/sp/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api_v3/adapters.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api_v3/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
             "campaignStatus",
             "campaignBudgetAmount",
             "campaignBudgetType",
             "campaignRuleBasedBudgetAmount",
             "campaignApplicableBudgetRuleId",
             "campaignApplicableBudgetRuleName",
             "campaignBudgetCurrencyCode",
+            # "topOfSearchImpressionShare",  # 特殊处理下；仅单独 groupBy campaign 时才会有这个字段
         ]
 
         adGroup = [
             "adGroupName",
             "adGroupId",
             "adStatus",
         ]
@@ -179,22 +180,26 @@
         ]
 
         def __init__(self, columns):
             """Easy dot access like: GroupBy.campaign.columns"""
             self.columns = columns
 
     def get_data_raw(self):
+        columns = self.get_columns()
+        if len(self.group_by) == 1 and self.group_by[0] == "campaign":
+            columns.append("topOfSearchImpressionShare")
+
         data = {
             "name": self.name,
             "startDate": self.start_date,
             "endDate": self.end_date,
             "configuration": {
                 "adProduct": "SPONSORED_PRODUCTS",
                 "groupBy": self.group_by,
-                "columns": self.get_columns(),
+                "columns": columns,
                 "reportTypeId": self._report_type_id,
                 "timeUnit": self.time_unit,
                 "format": self._format
             }
         }
         return data
 
@@ -267,14 +272,16 @@
         'campaignStatus',
         'keywordBid',
         'adGroupName',
         'adGroupId',
         'keywordType',
         'matchType',
         'targeting',
+
+        "topOfSearchImpressionShare",
     ]
 
     class GroupBy(Enum):
 
         targeting = [
             "adKeywordStatus",
         ]
```

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api_v3/base.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api_v3/base.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api_v3/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api_v3/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sb/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sb/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/api_v3/sp/report.py` & `amazon_ad_sdk-0.2.6/amazon_ad/api_v3/sp/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/client/auth.py` & `amazon_ad_sdk-0.2.6/amazon_ad/client/auth.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/client/base.py` & `amazon_ad_sdk-0.2.6/amazon_ad/client/base.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/client/service.py` & `amazon_ad_sdk-0.2.6/amazon_ad/client/service.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/core/consts.py` & `amazon_ad_sdk-0.2.6/amazon_ad/core/consts.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/core/exceptions.py` & `amazon_ad_sdk-0.2.6/amazon_ad/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/core/utils/amazon.py` & `amazon_ad_sdk-0.2.6/amazon_ad/core/utils/amazon.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/core/utils/serialize.py` & `amazon_ad_sdk-0.2.6/amazon_ad/core/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad/core/utils/text.py` & `amazon_ad_sdk-0.2.6/amazon_ad/core/utils/text.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/amazon_ad_sdk.egg-info/SOURCES.txt` & `amazon_ad_sdk-0.2.6/amazon_ad_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.5/setup.py` & `amazon_ad_sdk-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='amazon_ad_sdk',
-    version='0.2.5',
+    version='0.2.6',
     packages=['amazon_ad',
               'amazon_ad.api',
               'amazon_ad.api.sb',
               'amazon_ad.api.sp',
               'amazon_ad.api.sd',
               'amazon_ad.api.dsp',
               'amazon_ad.api.amazon_attribution',
```

