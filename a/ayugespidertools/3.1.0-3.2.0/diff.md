# Comparing `tmp/ayugespidertools-3.1.0.tar.gz` & `tmp/ayugespidertools-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.1.0.tar", max compression
+gzip compressed data, was "ayugespidertools-3.2.0.tar", max compression
```

## Comparing `ayugespidertools-3.1.0.tar` & `ayugespidertools-3.2.0.tar`

### file list

```diff
@@ -1,88 +1,84 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/LICENSE
--rw-r--r--   0        0        0    14107 2023-05-29 07:10:35.000000 ayugespidertools-3.1.0/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-3.1.0/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.1.0/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.1.0/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.1.0/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.1.0/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-3.1.0/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6618 2023-05-26 02:04:03.000000 ayugespidertools-3.1.0/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     6622 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    16599 2023-05-29 02:04:03.000000 ayugespidertools-3.1.0/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13558 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-3.1.0/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4240 2023-05-26 02:05:31.000000 ayugespidertools-3.1.0/ayugespidertools/common/spiderdbconf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-3.1.0/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     2838 2023-05-29 03:26:37.000000 ayugespidertools-3.1.0/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11321 2023-05-26 02:04:35.000000 ayugespidertools-3.1.0/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-3.1.0/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-3.1.0/ayugespidertools/config.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-3.1.0/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-3.1.0/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     5065 2023-05-25 07:32:25.000000 ayugespidertools-3.1.0/ayugespidertools/items.py
--rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-3.1.0/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-3.1.0/ayugespidertools/oss.py
--rw-r--r--   0        0        0      904 2023-05-29 03:26:43.000000 ayugespidertools-3.1.0/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/processmanager.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.1.0/ayugespidertools/request.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/rpa.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/runjs.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10515 2023-05-26 02:02:45.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0     1042 2023-05-26 07:14:18.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     2115 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2898 2023-05-26 06:58:42.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1361 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     2673 2023-05-29 05:56:21.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0    12465 2023-05-26 02:04:46.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     4371 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3956 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     7167 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.1.0/ayugespidertools/spiders.py
--rw-r--r--   0        0        0     2065 2023-05-18 08:39:18.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      729 2023-05-29 07:36:32.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6327 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1829 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.1.0/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.1.0/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3091 2023-05-29 07:19:55.000000 ayugespidertools-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    15882 1970-01-01 00:00:00.000000 ayugespidertools-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/LICENSE
+-rw-r--r--   0        0        0    14157 2023-06-07 06:26:34.000000 ayugespidertools-3.2.0/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-3.2.0/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.2.0/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.2.0/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.2.0/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.2.0/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3696 2023-06-07 02:13:50.000000 ayugespidertools-3.2.0/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6610 2023-06-07 02:13:56.000000 ayugespidertools-3.2.0/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     5269 2023-06-06 08:28:35.000000 ayugespidertools-3.2.0/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    16994 2023-06-07 07:22:39.000000 ayugespidertools-3.2.0/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13306 2023-06-07 01:56:44.000000 ayugespidertools-3.2.0/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-06-07 06:20:10.000000 ayugespidertools-3.2.0/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     6000 2023-06-06 07:14:58.000000 ayugespidertools-3.2.0/ayugespidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3718 2023-06-07 02:14:02.000000 ayugespidertools-3.2.0/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     3158 2023-06-07 07:53:47.000000 ayugespidertools-3.2.0/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11402 2023-06-07 02:14:12.000000 ayugespidertools-3.2.0/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3685 2023-06-07 02:14:19.000000 ayugespidertools-3.2.0/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      388 2023-06-07 02:14:26.000000 ayugespidertools-3.2.0/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9982 2023-06-07 02:14:34.000000 ayugespidertools-3.2.0/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7673 2023-06-07 02:14:39.000000 ayugespidertools-3.2.0/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     5065 2023-05-25 07:32:25.000000 ayugespidertools-3.2.0/ayugespidertools/items.py
+-rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.2.0/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8542 2023-06-07 02:14:45.000000 ayugespidertools-3.2.0/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.2.0/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5423 2023-06-07 02:14:57.000000 ayugespidertools-3.2.0/ayugespidertools/oss.py
+-rw-r--r--   0        0        0     1015 2023-06-06 07:39:29.000000 ayugespidertools-3.2.0/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.2.0/ayugespidertools/request.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1049 2023-06-07 06:21:05.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-07 02:13:19.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10500 2023-06-07 06:02:16.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3779 2023-06-07 02:15:17.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2429 2023-06-07 02:15:24.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0     1042 2023-05-26 07:14:18.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1569 2023-06-07 02:15:30.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2161 2023-06-06 09:22:26.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1302 2023-06-06 08:33:11.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3132 2023-06-06 08:44:33.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     1726 2023-06-07 07:28:59.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0    11521 2023-06-06 08:20:22.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     4109 2023-06-06 08:42:02.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2734 2023-06-06 08:35:52.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3854 2023-06-06 08:41:13.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7938 2023-06-06 07:14:49.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.2.0/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     5992 2023-06-07 07:57:01.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1685 2023-06-06 08:24:33.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.2.0/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.2.0/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3073 2023-06-07 01:35:09.000000 ayugespidertools-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15887 1970-01-01 00:00:00.000000 ayugespidertools-3.2.0/PKG-INFO
```

### Comparing `ayugespidertools-3.1.0/LICENSE` & `ayugespidertools-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/README.md` & `ayugespidertools-3.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,15 @@
 # 采集数据存入 `MongoDB` 的场景：
 + 2).demo_two: 采集数据存入 `MongoDB` 的场景（配置根据本地 `settings` 的 `LOCAL_MONGODB_CONFIG` 中取值）
 + 4).demo_four: 采集数据存入 `MongoDB` 的场景（配置根据 `consul` 的应用管理中心中取值）
 + 6).demo_six: 异步存入 `MongoDB` 的场景
 
 # 将 `Scrapy` 的 `Request`，`FormRequest` 替换为其它工具实现的场景
 - 以上为使用 scrapy Request 的场景
-+ 7).demo_seven: scrapy Request 替换为 requests 请求的场景(一般情况下不推荐使用，同步库
-+ 会拖慢 scrapy 速度，可用于测试场景)
+- 7).demo_seven: scrapy Request 替换为 requests 请求的场景(已删除此功能，更推荐使用 aiohttp 方式)
 
 + 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
 
 + 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
 + 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
 
 + 11).demo_proxy_one: 快代理动态隧道代理示例
@@ -105,15 +104,16 @@
 +14).demo_crawl: 支持 scrapy CrawlSpider 的示例
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
 +15).demo_item_loader: 本库中使用 Item Loaders 的示例
 -16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目前已经可以很方便的使用 Item Loaders 功能了
 
 +17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
-+18).demo_mq: 数据存入 rabbitmq 的模板示例，通过 pika 库实现
++18).demo_mq: 数据存入 rabbitmq 的模板示例
++19).demo_kafka: 数据存入 rabbitmq 的模板示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
@@ -168,23 +168,23 @@
 - [x] `scrapy` 的扩展功能场景
   - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
   - [x] 自定义模板，在 `ayugespidertools startproject <projname>` 和 `ayugespidertools genspider <spidername>` 时生成适合本库的模板文件
   - [x] ~~增加根据 `nacos` 来获取配置的功能~~ -> 改为增加根据 `consul` 来获取配置的功能
   - [x] 代理中间件（独享代理、动态隧道代理）
   - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
   - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-    - [x] `requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率
+    - [x] ~~`requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率~~（已移除此功能，更推荐 `aiohttp` 的方式）
     - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
   - [x] `Mysql` 存储的场景下适配
     - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
   - [x] `MongoDB` 存储的场景下适配，编写风格与 `Mysql` 存储等场景下一致
   - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
     - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
     - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
-  - [ ] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
+  - [x] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
 - [x] 常用开发场景
   - [x] `sql` 语句拼接，只是简单场景，后续优化。已给出优化方向，参考库等信息。
   - [x] `mongoDB` 语句拼接
   - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
   - [x] 字体反爬还原方法
     - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
       - [x] 可以直接在字体文件 `xml` 中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.2.0/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/commands/version.py` & `ayugespidertools-3.2.0/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/encryption.py` & `ayugespidertools-3.2.0/ayugespidertools/common/encryption.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from Crypto.PublicKey import RSA
 
 __all__ = [
     "EncryptOperation",
 ]
 
 
-class EncryptOperation(object):
+class EncryptOperation:
     """
     普通加密方法
     """
 
     @classmethod
     def md5(cls, encrypt_data: str) -> str:
         """
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/expend.py` & `ayugespidertools-3.2.0/ayugespidertools/common/expend.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ayugespidertools.config import logger
 
 __all__ = [
     "MysqlPipeEnhanceMixin",
 ]
 
 
-class MysqlPipeEnhanceMixin(object):
+class MysqlPipeEnhanceMixin:
     """
     用于扩展 pipelines 中的功能，作为 Mixin 使用，不要对其实例化和单独使用等
     """
 
     @retry(
         stop_max_attempt_number=Param.retry_num,
         wait_random_min=Param.retry_time_min,
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.2.0/ayugespidertools/common/mongodbpipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,32 +15,14 @@
 
 
 class AbstractClass(ABC):
     """
     用于处理 mongodb pipeline 存储的模板方法类
     """
 
-    def _get_collection_name(self, table: str, collection_prefix: str = "") -> str:
-        """
-        获取集合名称
-        Args:
-            table: item 中的 table 字段
-            collection_prefix: 集合前缀
-
-        Returns:
-            full_collection_name: 完整的集合名称
-        """
-        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
-        full_collection_name = f"""{collection_prefix}{table}"""
-
-        assert (
-            " " not in full_collection_name
-        ), "集合名不能含空格，请检查 MONGODB_COLLECTION_PREFIX 参数和 item 中的 table 参数"
-        return full_collection_name
-
     def _get_insert_data(
         self,
         item_dict: Union[ItemAdapter, dict],
     ) -> dict:
         """
         获取要插入的数据，将 item 中的存储数据提取出来
         Args:
@@ -60,36 +42,29 @@
         # 是普通的 dict 格式，则直接为 insert_data
         return insert_data
 
     def process_item_template(
         self,
         item_dict: Union[ItemAdapter, dict],
         db: Param.PymongoDataBase,
-        collection_prefix: str = "",
     ) -> None:
         """
         模板方法，用于处理 mongodb pipeline 存储的模板方法类
         Args:
             item_dict: item ItemAdapter 或 dict 格式数据
             db: mongodb 数据库连接
-            collection_prefix: 集合前缀
 
         Returns:
             None
         """
         insert_data = self._get_insert_data(item_dict)
-        # 真实的集合名称为：集合前缀名 + 集合名称
-        collection_name = self._get_collection_name(
-            table=item_dict["_table"],
-            collection_prefix=collection_prefix,
-        )
         self._data_storage_logic(
             db=db,
             item_dict=item_dict,
-            collection_name=collection_name,
+            collection_name=item_dict["_table"],
             insert_data=insert_data,
         )
 
     @abstractmethod
     def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
@@ -181,35 +156,26 @@
                 item_dict["_mongo_update_rule"], {"$set": insert_data}, True
             )
 
     async def process_item_template(
         self,
         item_dict: Union[ItemAdapter, dict],
         db: Param.PymongoDataBase,
-        collection_prefix: str = "",
     ) -> None:
         insert_data = self._get_insert_data(item_dict)
-        # 真实的集合名称为：集合前缀名 + 集合名称
-        collection_name = self._get_collection_name(
-            table=item_dict["_table"],
-            collection_prefix=collection_prefix,
-        )
         await self._data_storage_logic(
             db=db,
             item_dict=item_dict,
-            collection_name=collection_name,
+            collection_name=item_dict["_table"],
             insert_data=insert_data,
         )
 
 
 def mongodb_pipe(
     abstract_class: AbstractClass,
     item_dict: Union[ItemAdapter, dict],
     db: Param.PymongoDataBase,
-    collection_prefix: str = "",
 ) -> None:
     """
     mongodb pipeline 存储的通用调用方法
     """
-    abstract_class.process_item_template(
-        item_dict=item_dict, db=db, collection_prefix=collection_prefix
-    )
+    abstract_class.process_item_template(item_dict=item_dict, db=db)
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.2.0/ayugespidertools/common/multiplexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ayugespidertools.items import MongoDataItem, MysqlDataItem, ScrapyItem
 
 __all__ = [
     "ReuseOperation",
 ]
 
 
-class ReuseOperation(object):
+class ReuseOperation:
     """
     用于存放经常复用的一些操作
     """
 
     @staticmethod
     def as_deferred(f):
         """
@@ -48,26 +48,24 @@
         Returns:
             inner_settings: 本库所需的配置
         """
         # 加载秘钥等配置信息
         config_parser = configparser.ConfigParser()
         config_parser.read(f"{vit_dir}/.conf", encoding="utf-8")
         # Mysql 数据库配置
-        inner_settings["LOCAL_MYSQL_CONFIG"] = {
+        inner_settings["MYSQL_CONFIG"] = {
             "host": config_parser.get("mysql", "host", fallback=None),
             "port": config_parser.getint("mysql", "port", fallback=3306),
             "user": config_parser.get("mysql", "user", fallback="root"),
             "password": config_parser.get("mysql", "password", fallback=None),
             "charset": config_parser.get("mysql", "charset", fallback="utf8mb4"),
             "database": config_parser.get("mysql", "database", fallback=None),
-            # 数据库 engin 采用的驱动，可不填此参数
-            "driver": "mysqlconnector",
         }
         # MongoDB 数据库配置
-        inner_settings["LOCAL_MONGODB_CONFIG"] = {
+        inner_settings["MONGODB_CONFIG"] = {
             "host": config_parser.get("mongodb", "host", fallback=None),
             "port": config_parser.getint("mongodb", "port", fallback=27017),
             "authsource": config_parser.get("mongodb", "authsource", fallback="admin"),
             "user": config_parser.get("mongodb", "user", fallback="admin"),
             "password": config_parser.get("mongodb", "password", fallback=None),
             "database": config_parser.get("mongodb", "database", fallback=None),
         }
@@ -111,28 +109,38 @@
         # mq 配置
         inner_settings["MQ_CONFIG"] = {
             "host": config_parser.get("mq", "host", fallback=None),
             "port": config_parser.getint("mq", "port", fallback=5672),
             "username": config_parser.get("mq", "username", fallback="guest"),
             "password": config_parser.get("mq", "password", fallback="guest"),
             "virtualhost": config_parser.get("mq", "virtualhost", fallback="/"),
+            "heartbeat": config_parser.getint("mq", "heartbeat", fallback=0),
+            "socket_timeout": config_parser.getint("mq", "socket_timeout", fallback=1),
             "queue": config_parser.get("mq", "queue", fallback=None),
             "durable": config_parser.getboolean("mq", "durable", fallback=True),
             "exclusive": config_parser.getboolean("mq", "exclusive", fallback=False),
             "auto_delete": config_parser.getboolean(
                 "mq", "auto_delete", fallback=False
             ),
             "exchange": config_parser.get("mq", "exchange", fallback=None),
             "routing_key": config_parser.get("mq", "routing_key", fallback=None),
             "content_type": config_parser.getint(
                 "mq", "content_type", fallback="text/plain"
             ),
             "delivery_mode": config_parser.getint("mq", "delivery_mode", fallback=1),
             "mandatory": config_parser.getboolean("mq", "mandatory", fallback=True),
         }
+        # kafka 配置
+        inner_settings["KAFKA_CONFIG"] = {
+            "bootstrap_servers": config_parser.get(
+                "kafka", "bootstrap_servers", fallback="127.0.0.1:9092"
+            ),
+            "topic": config_parser.get("kafka", "topic", fallback=None),
+            "key": config_parser.get("kafka", "key", fallback=None),
+        }
         return inner_settings
 
     @staticmethod
     def item_to_dict(
         item: Union[MysqlDataItem, MongoDataItem, ScrapyItem, dict]
     ) -> dict:
         """
@@ -213,15 +221,14 @@
 
         if isinstance(tp, bytes):
             tp_buf = np.frombuffer(tp, np.uint8)
             tp_cv = cv2.imdecode(tp_buf, cv2.IMREAD_ANYCOLOR)
         else:
             # 0 表示采用黑白的方式读取图片
             tp_cv = cv2.imread(tp, 0)
-
         return bg_cv, tp_cv
 
     @staticmethod
     def random_weight(weight_data: list):
         """
         带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
         Args:
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.2.0/ayugespidertools/common/mysqlerrhandle.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,29 +107,27 @@
         err_msg: str,
         conn: Param.PymysqlConnect,
         cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
         charset: str,
         collate: str,
         database: str,
         table: str,
-        table_prefix: str,
         table_enum: Type[TableEnumTypeVar],
         note_dic: dict,
     ) -> None:
         """
         模板方法，用于处理 mysql 存储场景的异常
         Args:
             err_msg: pipeline 存储时报错内容
             conn: mysql conn
             cursor: mysql connect cursor
             charset: mysql table charset
             collate: mysql table collate
             database: 数据库
             table: 数据表
-            table_prefix: 数据表前缀
             table_enum: 数据表枚举类
             note_dic: 当前表字段注释
 
         Returns:
             None
         """
         if "1054" in err_msg:
@@ -137,15 +135,14 @@
                 err_msg=err_msg, table=table, note_dic=note_dic
             )
             self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
 
         elif "1146" in err_msg:
             table_name, table_notes, demand_code = self.deal_1146_error(
                 err_msg=err_msg,
-                table_prefix=table_prefix,
                 table_enum=table_enum,
             )
             self._create_table(
                 cursor=cursor,
                 table_name=table_name,
                 charset=charset,
                 collate=collate,
@@ -201,37 +198,35 @@
         else:
             sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(190) NULL DEFAULT '' COMMENT '{notes}';"
         return sql, f"1054: 添加字段 {colum} 已存在"
 
     def deal_1146_error(
         self,
         err_msg: str,
-        table_prefix: str,
         table_enum: Type[TableEnumTypeVar],
     ) -> (str, str, str):
         """
         解决 1146, u"Table '(.*?)' doesn't exist"
         Args:
             err_msg: 报错内容
-            table_prefix: 数据表前缀
             table_enum: 数据表的枚举信息
 
         Returns:
             1). table_name: 数据表名
             2). table_notes: 数据表注释
             3). demand_code: 数据表对应的需求 code
         """
         table_pattern = re.compile(r"Table '(.*?)' doesn't exist")
         text = re.findall(table_pattern, err_msg)
         table = text[0].split(".")[1]
 
         # 写入表枚举
         if table_enum:
             for _, member in table_enum.__members__.items():
-                table_name = f'{table_prefix}{member.value.get("value", "")}'
+                table_name = member.value.get("value", "")
                 table_notes = member.value.get("notes", "")
                 demand_code = member.value.get("demand_code", "")
                 if table_name == table:
                     return table_name, table_notes, demand_code
         else:
             # 未定义 Tabel_Enum 则建表
             logger.info("未定义数据库表枚举 Tabel_Enum 参数，进行创表操作")
@@ -374,24 +369,22 @@
     abstract_class: AbstractClass,
     err_msg: str,
     cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
     charset: str,
     collate: str,
     database: str,
     table: str,
-    table_prefix: str,
     table_enum: Type[TableEnumTypeVar],
     note_dic: dict,
     conn: Optional[Param.PymysqlConnect] = None,
 ) -> None:
     abstract_class.template_method(
         err_msg,
         conn,
         cursor,
         charset,
         collate,
         database,
         table,
-        table_prefix,
         table_enum,
         note_dic,
     )
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/params.py` & `ayugespidertools-3.2.0/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.2.0/ayugespidertools/common/sqlformat.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __all__ = [
     "AboutSql",
 ]
 
 SqlModeStr = Literal["and", "or"]
 
 
-class AboutSql(object):
+class AboutSql:
     """
     sql 相关处理: sql 语句的管理方法，
     这里的 sql 拼接只能做到最简单的逻辑，如果需要灵活或稍复杂的情况，请参考 directsql, python-sql, pypika
     或 pymilk 等第三方类似功能库的实现方法，以后会再优化此场景
     """
 
     @staticmethod
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/typevars.py` & `ayugespidertools-3.2.0/ayugespidertools/common/typevars.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     "TableEnumTypeVar",
     "AlterItem",
     "MysqlConf",
     "MongoDBConf",
     "AiohttpConf",
     "AiohttpRequestArgs",
     "MQConf",
+    "KafkaConf",
+    "DynamicProxyConf",
+    "ExclusiveProxyConf",
 ]
 
 AiohttpRequestMethodStr = Literal["GET", "POST"]
 TableEnumTypeVar = TypeVar("TableEnumTypeVar", bound="TableEnum")
 
 sentinel: Any = object()
 
@@ -47,15 +50,15 @@
 
 class MysqlConf(NamedTuple):
     host: str
     port: int
     user: str
     password: str
     database: Optional[str] = None
-    charset: Optional[str] = "utf8mb4"
+    charset: str = "utf8mb4"
 
 
 class MongoDBConf(NamedTuple):
     host: str
     port: int
     user: str
     password: str
@@ -95,17 +98,38 @@
 
 
 class MQConf(NamedTuple):
     host: str
     port: int
     username: str
     password: str
-    virtualhost: Optional[str] = "/"
+    virtualhost: str = "/"
+    heartbeat: int = 0
+    socket_timeout: int = 1
     queue: Optional[str] = None
-    durable: Optional[bool] = True
-    exclusive: Optional[bool] = False
-    auto_delete: Optional[bool] = False
+    durable: bool = True
+    exclusive: bool = False
+    auto_delete: bool = False
     exchange: Optional[str] = None
     routing_key: Optional[str] = None
-    content_type: Optional[str] = "text/plain"
-    delivery_mode: Optional[int] = 1
-    mandatory: Optional[bool] = True
+    content_type: str = "text/plain"
+    delivery_mode: int = 1
+    mandatory: bool = True
+
+
+class DynamicProxyConf(NamedTuple):
+    proxy: str
+    username: str
+    password: str
+
+
+class ExclusiveProxyConf(NamedTuple):
+    proxy: str
+    username: str
+    password: str
+    index: int
+
+
+class KafkaConf(NamedTuple):
+    bootstrap_servers: list
+    topic: str
+    key: str
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/utils.py` & `ayugespidertools-3.2.0/ayugespidertools/common/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,25 @@
 from ayugespidertools.formatdata import DataHandle
 
 __all__ = [
     "ToolsForAyu",
 ]
 
 ConsulFormatStr = Literal["json", "hcl", "yaml", "xml"]
-ConsulConfNameStr = Literal["mongodb", "mysql"]
+ConsulConfNameStr = Literal[
+    "mongodb",
+    "mysql",
+    "rabbitmq",
+    "kafka",
+    "dynamicproxy",
+    "exclusiveproxy",
+]
 
 
-class ToolsForAyu(object):
+class ToolsForAyu:
     """
     这里用于存放框架所依赖的方法
     """
 
     @classmethod
     def get_kvs_detail_by_consul(
         cls,
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.2.0/ayugespidertools/common/yidungap.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ayugespidertools.common.multiplexing import ReuseOperation
 
 __all__ = [
     "YiDunGetGap",
 ]
 
 
-class YiDunGetGap(object):
+class YiDunGetGap:
     """
     易盾获取滑块缺口距离的相关方法，也可能适配于其它平台
     """
 
     @classmethod
     def clear_white(cls, img):
         """
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/formatdata.py` & `ayugespidertools-3.2.0/ayugespidertools/formatdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from w3lib.html import remove_tags, replace_entities
 
 __all__ = [
     "DataHandle",
 ]
 
 
-class DataHandle(object):
+class DataHandle:
     """数据处理相关方法"""
 
     @staticmethod
     def get_full_url(domain_name: str, deal_url: str) -> str:
         """
         根据域名 domain_name 拼接 deal_url 来获得完整链接
         Args:
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/imgoperation.py` & `ayugespidertools-3.2.0/ayugespidertools/imgoperation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ayugespidertools.common.multiplexing import ReuseOperation
 
 __all__ = [
     "Picture",
 ]
 
 
-class Picture(object):
+class Picture:
     """
     对验证码图片的一些操作
     """
 
     @classmethod
     def convert_index_to_offset(cls, index):
         """
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/items.py` & `ayugespidertools-3.2.0/ayugespidertools/items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/middlewares.py` & `ayugespidertools-3.2.0/ayugespidertools/middlewares.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from ayugespidertools.scraper.middlewares.headers.ua import RandomRequestUaMiddleware
 from ayugespidertools.scraper.middlewares.netlib.aiohttplib import (
     AiohttpAsyncDownloaderMiddleware,
     AiohttpDownloaderMiddleware,
 )
-from ayugespidertools.scraper.middlewares.netlib.requestslib import (
-    RequestsDownloaderMiddleware,
-)
 from ayugespidertools.scraper.middlewares.proxy.dynamic import (
     AbuDynamicProxyDownloaderMiddleware,
     DynamicProxyDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.exclusive import (
     ExclusiveProxyDownloaderMiddleware,
 )
 
 __all__ = [
     "RandomRequestUaMiddleware",
     "AiohttpAsyncDownloaderMiddleware",
     "AiohttpDownloaderMiddleware",
-    "RequestsDownloaderMiddleware",
     "AbuDynamicProxyDownloaderMiddleware",
     "DynamicProxyDownloaderMiddleware",
     "ExclusiveProxyDownloaderMiddleware",
 ]
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/mongoclient.py` & `ayugespidertools-3.2.0/ayugespidertools/mongoclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pymongo import MongoClient
 
 __all__ = [
     "MongoDbBase",
 ]
 
 
-class MongoDbBase(object):
+class MongoDbBase:
     """
     mongodb 数据库的相关操作（此功能暂时为残废状态，请参考 pymilk 库中的实现）
     """
 
     def __init__(
         self,
         user: str,
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.2.0/ayugespidertools/mysqlclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __all__ = [
     "MysqlOrm",
 ]
 
 SearchTypeStr = Literal["all", "one"]
 
 
-class MysqlOrm(object):
+class MysqlOrm:
     """数据库的简单使用，结合 SqlFormat 方法使用（临时使用）"""
 
     def __init__(self, pymsql_connect_conf: dict):
         self.conn = pymysql.connect(**pymsql_connect_conf)
         self.cursor = self.conn.cursor()
 
     def insert_data(self, sql_pre: str, sql_after: tuple):
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/oss.py` & `ayugespidertools-3.2.0/ayugespidertools/oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warnings.filterwarnings("ignore")
 
 __all__ = [
     "AliOssBase",
 ]
 
 
-class AliOssBase(object):
+class AliOssBase:
     """
     阿里云 Oss 对象存储 python sdk 示例
     其 GitHub 官方文档地址：
         https://github.com/aliyun/aliyun-oss-python-sdk?spm=5176.8465980.tools.dpython-github.572b1450ON6Z9R
     阿里云官方 oss sdk 文档地址：
         https://www.alibabacloud.com/help/zh/object-storage-service/latest/python-quick-start
     """
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/pipelines.py` & `ayugespidertools-3.2.0/ayugespidertools/pipelines.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ayugespidertools.scraper.pipelines.mongo.asynced import AsyncMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.twisted import AyuTwistedMongoPipeline
+from ayugespidertools.scraper.pipelines.msgproducer.kafkapub import AyuKafkaPipeline
 from ayugespidertools.scraper.pipelines.msgproducer.mqpub import AyuMQPipeline
 from ayugespidertools.scraper.pipelines.mysql.asynced import AsyncMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.fantasy import AyuFtyMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.turbo import AyuTurboMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.twisted import AyuTwistedMysqlPipeline
 
 __all__ = [
@@ -12,8 +13,9 @@
     "AyuTurboMysqlPipeline",
     "AyuTwistedMysqlPipeline",
     "AsyncMongoPipeline",
     "AsyncMysqlPipeline",
     "AyuFtyMongoPipeline",
     "AyuTwistedMongoPipeline",
     "AyuMQPipeline",
+    "AyuKafkaPipeline",
 ]
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,31 +3,27 @@
 # See documentation in:
 # https://docs.scrapy.org/en/latest/topics/spider-middleware.html
 from ayugespidertools.scraper.middlewares.headers.ua import RandomRequestUaMiddleware
 from ayugespidertools.scraper.middlewares.netlib.aiohttplib import (
     AiohttpAsyncDownloaderMiddleware,
     AiohttpDownloaderMiddleware,
 )
-from ayugespidertools.scraper.middlewares.netlib.requestslib import (
-    RequestsDownloaderMiddleware,
-)
 from ayugespidertools.scraper.middlewares.proxy.dynamic import (
     AbuDynamicProxyDownloaderMiddleware,
     DynamicProxyDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.exclusive import (
     ExclusiveProxyDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.private import (
     PrivateProxyDownloaderMiddleware,
 )
 
 __all__ = [
     "RandomRequestUaMiddleware",
-    "RequestsDownloaderMiddleware",
     "AiohttpAsyncDownloaderMiddleware",
     "AiohttpDownloaderMiddleware",
     "DynamicProxyDownloaderMiddleware",
     "AbuDynamicProxyDownloaderMiddleware",
     "ExclusiveProxyDownloaderMiddleware",
     "PrivateProxyDownloaderMiddleware",
 ]
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ayugespidertools.common.params import Param
 
 __all__ = [
     "RandomRequestUaMiddleware",
 ]
 
 
-class RandomRequestUaMiddleware(object):
+class RandomRequestUaMiddleware:
     """
     随机请求头中间件
     """
 
     def __init__(self):
         self.explorer_types = None
         self.explorer_weights = None
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 __all__ = [
     "AiohttpDownloaderMiddleware",
     "AiohttpAsyncDownloaderMiddleware",
 ]
 
 
-class AiohttpDownloaderMiddleware(object):
+class AiohttpDownloaderMiddleware:
     """
     Downloader middleware handling the requests with aiohttp
     """
 
     def __init__(self):
         self.aiohttp_args = None
 
@@ -78,15 +78,15 @@
     @classmethod
     def from_crawler(cls, crawler):
         """
         初始化 middleware
         """
         settings = crawler.settings
         # 自定义 aiohttp 全局配置信息，优先级小于 aiohttp_meta 中的配置
-        if local_aiohttp_conf := settings.get("LOCAL_AIOHTTP_CONFIG", {}):
+        if local_aiohttp_conf := settings.get("AIOHTTP_CONFIG", {}):
             # 这里的配置信息如果在 aiohttp_meta 中重复设置，则会更新当前请求的参数
             _aiohttp_conf = AiohttpConf(
                 timeout=local_aiohttp_conf.get("timeout"),
                 sleep=local_aiohttp_conf.get("sleep"),
                 proxy=local_aiohttp_conf.get("proxy"),
                 proxy_auth=local_aiohttp_conf.get("proxy_auth"),
                 proxy_headers=local_aiohttp_conf.get("proxy_headers"),
@@ -109,15 +109,14 @@
             cls.sleep = _aiohttp_conf.sleep
             cls.retry_times = _aiohttp_conf.retry_times
             cls.limit = _aiohttp_conf.limit
             cls.ssl = _aiohttp_conf.ssl
             cls.verify_ssl = _aiohttp_conf.verify_ssl
             cls.limit_per_host = _aiohttp_conf.limit_per_host
             cls.priority_adjust = settings.getint("RETRY_PRIORITY_ADJUST")
-
         return cls()
 
     async def _request_by_aiohttp(
         self,
         aio_request_args: Param.ItemAdapterType,
         timeout: Optional[aiohttp.ClientTimeout] = None,
         connector: Optional[BaseConnector] = None,
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,38 +2,27 @@
 
 from scrapy import signals
 
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
 
 
-class DynamicProxyDownloaderMiddleware(object):
+class DynamicProxyDownloaderMiddleware:
     """
     动态隧道代理中间件
     """
 
-    def __init__(self, settings):
-        """
-        从 scrapy 配置中取出动态隧道代理的信息
-        """
-        dynamic_proxy_conf = settings.get("DYNAMIC_PROXY_CONFIG", None)
-        # 查看动态隧道代理配置是否符合要求
-        is_match = ReuseOperation.is_dict_meet_min_limit(
-            dict_conf=dynamic_proxy_conf,
-            key_list=["proxy", "username", "password"],
-        )
-        assert is_match, f"没有配置动态隧道代理，配置示例为：{Param.dynamic_proxy_conf_example}"
-
-        self.proxy_url = dynamic_proxy_conf["proxy"]
-        self.username = dynamic_proxy_conf["username"]
-        self.password = dynamic_proxy_conf["password"]
+    def __init__(self):
+        self.proxy_url = None
+        self.username = None
+        self.password = None
 
     @classmethod
     def from_crawler(cls, crawler):
-        s = cls(crawler.settings)
+        s = cls()
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
     def process_request(self, request, spider):
         # TODO: 根据权重来随机获取一个账号 DYNAMIC_PROXY_CONFIG
         # account = ReuseOperation.random_weight(self.account_arr)
         if request.url.startswith("https://"):
@@ -55,16 +44,20 @@
         request.headers["Accept-Encoding"] = "gzip"
 
     def spider_opened(self, spider):
         spider.slog.info(
             f"动态隧道代理中间件: DynamicProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
         )
 
+        self.proxy_url = spider.dynamicproxy_conf.proxy
+        self.username = spider.dynamicproxy_conf.username
+        self.password = spider.dynamicproxy_conf.password
+
 
-class AbuDynamicProxyDownloaderMiddleware(object):
+class AbuDynamicProxyDownloaderMiddleware:
     """
     阿布云动态代理 - 隧道验证方式（其实和快代理的写法一致）
     """
 
     def __init__(self, settings):
         """
         从 scrapy 配置中取出动态隧道代理的信息
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 import base64
 
 import requests
 from scrapy import signals
 
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.params import Param
+__all__ = [
+    "ExclusiveProxyDownloaderMiddleware",
+]
 
 
-class ExclusiveProxyDownloaderMiddleware(object):
+class ExclusiveProxyDownloaderMiddleware:
     """
     独享代理中间件
     """
 
-    def __init__(self, exclusive_proxy_conf):
-        """
-        初始化独享代理设置
-        Args:
-            exclusive_proxy_conf: 使用的独享代理的配置信息
-        """
+    def __init__(self):
+        self.proxy_url = None
+        self.username = None
+        self.password = None
+        self.proxy_index = None
+        # 从 proxy_list 中取出索引为 proxy_index 的值
         self.proxy = None
-        # 查看独享代理配置是否符合要求
-        is_match = ReuseOperation.is_dict_meet_min_limit(
-            dict_conf=exclusive_proxy_conf,
-            key_list=["proxy", "username", "password", "index"],
-        )
-        assert is_match, f"没有配置独享代理，配置示例为：{Param.exclusive_proxy_conf_example}"
-
-        self.proxy_url = exclusive_proxy_conf["proxy"]
-        self.username = exclusive_proxy_conf["username"]
-        self.password = exclusive_proxy_conf["password"]
-        self.proxy_index = exclusive_proxy_conf["index"]
 
     @classmethod
     def from_crawler(cls, crawler):
-        s = cls(
-            exclusive_proxy_conf=crawler.settings.get("EXCLUSIVE_PROXY_CONFIG", None)
-        )
+        s = cls()
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
-    def get_proxy_ip(self):
+    def get_proxy_ip(self, proxy_url: str, index: int) -> str:
         """获取独享代理接口的索引为 proxy_index 的代理信息"""
         try:
-            r = requests.get(self.proxy_url)
+            r = requests.get(proxy_url)
             proxy_list = r.json().get("data").get("proxy_list")
             proxy_list.sort()
-            if self.proxy_index < len(proxy_list):
-                self.proxy = proxy_list[self.proxy_index]
+            if index < len(proxy_list):
+                return proxy_list[index]
             else:
-                raise Exception("独享代理索引超出范围，请确认独享代理服务情况。")
+                raise IndexError("独享代理取值索引超出范围，请确认独享代理服务情况。")
 
         except Exception:
             raise Exception("获取独享代理时失败，请查看独享配置及网络是否正常。")
 
     def process_request(self, request, spider):
         if request.url.startswith("https://"):
             request.meta["proxy"] = f"https://{self.proxy}"
@@ -64,11 +52,16 @@
         proxy_user_pass = f"{self.username}:{self.password}"
         encoded_user_pass = "Basic " + base64.urlsafe_b64encode(
             bytes(proxy_user_pass, "ascii")
         ).decode("utf8")
         request.headers["Proxy-Authorization"] = encoded_user_pass
 
     def spider_opened(self, spider):
-        self.get_proxy_ip()
         spider.slog.info(
-            f"独享代理中间件: ExclusiveProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}，当前独享代理为: {self.proxy}"
+            f"独享代理中间件: ExclusiveProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
         )
+
+        self.proxy_url = spider.exclusiveproxy_conf.proxy
+        self.username = spider.exclusiveproxy_conf.username
+        self.password = spider.exclusiveproxy_conf.password
+        self.proxy_index = spider.exclusiveproxy_conf.index
+        self.proxy = self.get_proxy_ip(proxy_url=self.proxy_url, index=self.proxy_index)
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,19 @@
 
 import motor.motor_asyncio
 
 from ayugespidertools.common.mongodbpipe import AsyncioAsynchronous
 from ayugespidertools.common.multiplexing import ReuseOperation
 
 
-class AsyncMongoPipeline(object):
+class AsyncMongoPipeline:
     """
     通过 motor 实现异步写入 MongoDB 的存储管道
     """
 
-    def __init__(
-        self,
-        collection_prefix: str = "",
-    ) -> None:
-        assert isinstance(collection_prefix, str), "mongoDB 所要存储的集合前缀名称需要是 str 格式！"
-
-        self.collection_prefix = collection_prefix or ""
-        self.mongo_uri = None
-
-    @classmethod
-    def from_crawler(cls, crawler):
-        return cls(
-            collection_prefix=crawler.settings.get("MONGODB_COLLECTION_PREFIX", ""),
-        )
-
     def open_spider(self, spider):
         assert hasattr(
             spider, "mongodb_conf"
         ), "未配置 MongoDB 连接信息，请查看 .conf 或 consul 上对应配置信息！"
 
         _encoded_pwd = urllib.parse.quote_plus(spider.mongodb_conf.password)
         self.mongo_uri = (
@@ -50,11 +35,10 @@
     async def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
         if item_dict["_item_mode"] == "MongoDB":
             await asyncio.shield(
                 AsyncioAsynchronous().process_item_template(
                     item_dict=item_dict,
                     db=self.db,
-                    collection_prefix=self.collection_prefix,
                 )
             )
         return item
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,37 +8,18 @@
 
 
 class AyuFtyMongoPipeline(MongoDbBase):
     """
     MongoDB 存储场景的 scrapy pipeline 扩展
     """
 
-    def __init__(
-        self,
-        collection_prefix: str = "",
-    ) -> None:
-        """
-        初始化
-        Args:
-            mongodb_conf: mongDB 的连接配置
-            collection_prefix: mongDB 存储集合的前缀，默认为空字符
-        """
-        assert isinstance(collection_prefix, str), "mongoDB 所要存储的集合前缀名称需要是 str 格式！"
-
-        self.collection_prefix = collection_prefix or ""
-        # conn 和 db 为父类的属性，用于存储连接信息
+    def __init__(self):
         self.conn = None
         self.db = None
 
-    @classmethod
-    def from_crawler(cls, crawler):
-        return cls(
-            collection_prefix=crawler.settings.get("MONGODB_COLLECTION_PREFIX", ""),
-        )
-
     def open_spider(self, spider):
         assert hasattr(
             spider, "mongodb_conf"
         ), "未配置 MongoDB 连接信息，请查看 .conf 或 consul 上对应配置信息！"
         super(AyuFtyMongoPipeline, self).__init__(
             user=spider.mongodb_conf.user,
             password=spider.mongodb_conf.password,
@@ -74,10 +55,9 @@
         item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
         if item_dict["_item_mode"] == "MongoDB":
             mongodb_pipe(
                 Synchronize(),
                 item_dict=item_dict,
                 db=self.db,
-                collection_prefix=self.collection_prefix,
             )
         return item
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,9 @@
         item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
         if item_dict["_item_mode"] == "MongoDB":
             mongodb_pipe(
                 TwistedAsynchronous(),
                 item_dict=item_dict,
                 db=self.db,
-                collection_prefix=self.collection_prefix,
             )
             reactor.callFromThread(out.callback, item_dict)
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,44 +25,39 @@
 class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
     """
     Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例
     """
 
     def __init__(
         self,
-        table_prefix: str,
         table_enum: Type[TableEnumTypeVar],
         env: str,
         record_log_to_mysql: Optional[bool] = False,
     ) -> None:
         """
         初始化 Mysql 链接所需要的信息
         Args:
-            table_prefix: 数据库表前缀
             table_enum: 数据表的枚举信息
             env: 当前程序部署环境名
             record_log_to_mysql: 是否需要记录程序采集的基本信息到 Mysql 中
         """
-        self.table_prefix = table_prefix
         self.table_enum = table_enum
         self.env = env
         self.record_log_to_mysql = record_log_to_mysql
         # 排序规则，用于创建数据库时使用
         self.collate = None
         self.mysql_conf: Optional[MysqlConf] = None
         self.conn = None
         self.slog = None
         self.cursor = None
         self.crawl_time = datetime.date.today()
 
     @classmethod
     def from_crawler(cls, crawler):
         return cls(
-            # 数据库表前缀
-            table_prefix=crawler.settings.get("MYSQL_TABLE_PREFIX", ""),
             # 数据库表枚举是否开启
             table_enum=crawler.settings.get("DATA_ENUM"),
             # 获取部署的环境
             env=crawler.settings.get("ENV"),
             # 当 record_log_to_mysql 为 True 时，会记录运行情况
             record_log_to_mysql=crawler.settings.get("RECORD_LOG_TO_MYSQL", False),
         )
@@ -72,32 +67,14 @@
 
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
         self.conn = self._connect(self.mysql_conf)
         self.cursor = self.conn.cursor()
 
-    def get_table_name(self, table: str) -> str:
-        """
-        组合完整的数据库表
-        Args:
-            table: 数据表的后缀
-
-        Returns:
-            1). 拼接成完整的数据表的值
-        """
-        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
-        full_table_name = f"{self.table_prefix}{table}"
-
-        # 最终的数据表名不能含有空格
-        assert (
-            " " not in full_table_name
-        ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
-        return full_table_name
-
     def get_new_item(self, item_dict: Dict[str, Any]) -> AlterItem:
         """
         重新整合 item
         Args:
             item_dict: dict 类型的 item
 
         Returns:
@@ -125,15 +102,15 @@
 
     def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
         if item_dict["_item_mode"] == "Mysql":
             self.insert_item(
                 alter_item=self.get_new_item(item_dict),
-                table=self.get_table_name(item_dict["_table"]),
+                table=item_dict["_table"],
             )
         return item
 
     def insert_item(self, alter_item: AlterItem, table: str):
         """
         通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
         Args:
@@ -162,15 +139,14 @@
                 err_msg=str(e),
                 conn=self.conn,
                 cursor=self.cursor,
                 charset=self.mysql_conf.charset,
                 collate=self.collate,
                 database=self.mysql_conf.database,
                 table=table,
-                table_prefix=self.table_prefix,
                 table_enum=self.table_enum,
                 note_dic=note_dic,
             )
             return self.insert_item(alter_item, table)
 
     def close_spider(self, spider):
         # 是否记录程序采集的基本信息到 Mysql 中，只有打开 record_log_to_mysql 配置才会收集和存储相关的统计信息
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,101 @@
-import asyncio
-
-import aiomysql
+from pymysql import cursors
+from twisted.enterprise import adbapi
 
 from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.mysqlerrhandle import TwistedAsynchronous, deal_mysql_err
 from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 
 __all__ = [
-    "AsyncMysqlPipeline",
-    "AsyncNormalMysqlPipeline",
+    "AyuTwistedMysqlPipeline",
 ]
 
 
-class AsyncNormalMysqlPipeline(AyuMysqlPipeline):
+class AyuTwistedMysqlPipeline(AyuMysqlPipeline):
     """
-    通过 aiomysql 实现异步写入 Mysql 数据库的普通版本
+    使用 twisted 的 adbapi 实现 Mysql 存储场景下的异步操作
+    注意：
+        1. 推荐先用 AyuFtyMysqlPipeline 使用稳定后，再迁移至此管道
     """
 
-    def open_spider(self, spider):
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
+    def __init__(self, *args, **kwargs):
+        super(AyuTwistedMysqlPipeline, self).__init__(*args, **kwargs)
+        self.dbpool = None
 
+    def open_spider(self, spider):
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
-        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=spider.mysql_conf)
-        return ReuseOperation.as_deferred(self._open_spider(spider))
+        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
 
-    async def _open_spider(self, spider):
-        self.loop = asyncio.get_event_loop()
-        self.lock = asyncio.Lock()
-        self.db = await aiomysql.connect(
-            loop=self.loop,
-            host=self.mysql_conf.host,
-            port=self.mysql_conf.port,
-            user=self.mysql_conf.user,
-            password=self.mysql_conf.password,
-            db=self.mysql_conf.database,
-            charset=self.mysql_conf.charset,
-            cursorclass=aiomysql.DictCursor,
-        )
+        # 判断目标数据库是否连接正常。若连接目标数据库错误时，创建缺失的目标数据库。
+        # 记录日志时需要此连接对象，否则直接关闭
+        if self.record_log_to_mysql:
+            self.conn = self._connect(self.mysql_conf)
+            self.cursor = self.conn.cursor()
+        else:
+            self._connect(self.mysql_conf).close()
+
+        _mysql_conf = {
+            "user": spider.mysql_conf.user,
+            "password": spider.mysql_conf.password,
+            "host": spider.mysql_conf.host,
+            "port": spider.mysql_conf.port,
+            "db": spider.mysql_conf.database,
+            "charset": spider.mysql_conf.charset,
+            "cursorclass": cursors.DictCursor,
+        }
+        self.dbpool = adbapi.ConnectionPool("pymysql", cp_reconnect=True, **_mysql_conf)
+        query = self.dbpool.runInteraction(self.db_create)
+        query.addErrback(self.db_create_err)
 
-    async def process_item(self, item, spider):
-        item_dict = ReuseOperation.item_to_dict(item)
-        if item_dict["_item_mode"] == "Mysql":
-            async with self.db.cursor() as cursor:
-                async with self.lock:
-                    alter_item = super(AsyncNormalMysqlPipeline, self).get_new_item(
-                        item_dict
-                    )
-                    table = super(AsyncNormalMysqlPipeline, self).get_table_name(
-                        item_dict["_table"]
-                    )
-                    new_item = alter_item.new_item
-                    sql = self._get_sql_by_item(table=table, item=new_item)
-                    await cursor.execute(sql, tuple(new_item.values()) * 2)
-                    await self.db.commit()
-        return item
-
-    async def _close_spider(self):
+    def db_create(self, cursor):
         pass
 
-    def close_spider(self, spider):
-        self.db.close()
-        return ReuseOperation.as_deferred(self._close_spider())
-
+    def db_create_err(self, failure):
+        self.slog.error(f"创建数据表失败: {failure}")
 
-class AsyncMysqlPipeline(AyuMysqlPipeline):
-    """
-    通过 aiomysql 实现异步写入 Mysql 数据库的连接池版本
-    """
-
-    def open_spider(self, spider):
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
-
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=spider.mysql_conf)
-        return ReuseOperation.as_deferred(self._open_spider(spider))
-
-    async def _open_spider(self, spider):
-        self.pool = await aiomysql.create_pool(
-            host=self.mysql_conf.host,
-            port=self.mysql_conf.port,
-            user=self.mysql_conf.user,
-            password=self.mysql_conf.password,
-            db=self.mysql_conf.database,
-            charset=self.mysql_conf.charset,
-            cursorclass=aiomysql.DictCursor,
-            autocommit=True,
-            # 连接池最大连接数
-            maxsize=10,
-            # 连接池最小连接数
-            minsize=1,
-        )
-
-    async def process_item(self, item, spider):
+    def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
+        # 先查看存储场景是否匹配
         if item_dict["_item_mode"] == "Mysql":
-            async with self.pool.acquire() as conn:
-                async with conn.cursor() as cursor:
-                    alter_item = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
-                    table = super(AsyncMysqlPipeline, self).get_table_name(
-                        item_dict["_table"]
-                    )
-                    new_item = alter_item.new_item
-                    sql = self._get_sql_by_item(table=table, item=new_item)
-                    await asyncio.shield(
-                        cursor.execute(sql, tuple(new_item.values()) * 2)
-                    )
+            query = self.dbpool.runInteraction(self.db_insert, item_dict)
+            query.addErrback(self.handle_error, item)
+        return item
+
+    def db_insert(self, cursor, item):
+        alter_item = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
+        table = item["_table"]
+
+        if not (new_item := alter_item.new_item):
+            return
+
+        note_dic = alter_item.notes_dic
+        sql = self._get_sql_by_item(table=table, item=new_item)
+
+        try:
+            cursor.execute(sql, tuple(new_item.values()) * 2)
+
+        except Exception as e:
+            self.slog.warning(f":{e}")
+            self.slog.warning(f"Item:{new_item}  Table: {table}")
+            deal_mysql_err(
+                TwistedAsynchronous(),
+                err_msg=str(e),
+                cursor=cursor,
+                charset=self.mysql_conf.charset,
+                collate=self.collate,
+                database=self.mysql_conf.database,
+                table=table,
+                table_enum=self.table_enum,
+                note_dic=note_dic,
+            )
+            return self.db_insert(cursor, item)
+
         return item
 
-    async def _close_spider(self):
-        self.pool.close()
-        await self.pool.wait_closed()
+    def handle_error(self, failure, item):
+        self.slog.error(f"插入数据失败:{failure}, item: {item}")
 
     def close_spider(self, spider):
-        return ReuseOperation.as_deferred(self._close_spider())
+        # 这里新建数据库链接，是为了正常继承父类的脚本运行统计的方法（需要 self 的 mysql 连接对象存在）
+        super(AyuTwistedMysqlPipeline, self).close_spider(spider)
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,14 @@
         super(AyuTurboMysqlPipeline, self).__init__(*args, **kwargs)
         self.pool_db_conf = pool_db_conf
 
     @classmethod
     def from_crawler(cls, crawler):
         pool_db_conf = crawler.settings.get("POOL_DB_CONFIG", None)
         return cls(
-            # 数据库表前缀
-            table_prefix=crawler.settings.get("MYSQL_TABLE_PREFIX", ""),
             # 数据库表枚举是否开启
             table_enum=crawler.settings.get("DATA_ENUM"),
             # 获取部署的环境
             env=crawler.settings.get("ENV"),
             # 当 record_log_to_mysql 为 True 时，会记录运行情况
             record_log_to_mysql=crawler.settings.get("RECORD_LOG_TO_MYSQL", False),
             # 数据库连接池配置
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files 8% similar despite different names*

```diff
@@ -12,35 +12,41 @@
 000000b0: 5b6d 715d 0d0a 686f 7374 3d2a 2a2a 0d0a  [mq]..host=***..
 000000c0: 706f 7274 3d35 3637 320d 0a75 7365 726e  port=5672..usern
 000000d0: 616d 653d 2a2a 2a0d 0a70 6173 7377 6f72  ame=***..passwor
 000000e0: 643d 2a2a 2a0d 0a76 6972 7475 616c 686f  d=***..virtualho
 000000f0: 7374 3d2a 2a2a 0d0a 7175 6575 653d 2a2a  st=***..queue=**
 00000100: 2a0d 0a65 7863 6861 6e67 653d 2a2a 2a0d  *..exchange=***.
 00000110: 0a72 6f75 7469 6e67 5f6b 6579 3d2a 2a2a  .routing_key=***
-00000120: 0d0a 0d0a 5b63 6f6e 7375 6c5d 0d0a 746f  ....[consul]..to
-00000130: 6b65 6e3d 0d0a 7572 6c3d 6874 7470 3a2f  ken=..url=http:/
-00000140: 2f68 6f73 743a 706f 7274 2f76 312f 6b76  /host:port/v1/kv
-00000150: 2f2e 2e2e 3f64 633d 6463 310d 0a66 6f72  /...?dc=dc1..for
-00000160: 6d61 743d 6a73 6f6e 0d0a 0d0a 5b77 7862  mat=json....[wxb
-00000170: 6f74 5d0d 0a6b 6579 3d2a 2a2a 0d0a 0d0a  ot]..key=***....
-00000180: 5b6b 646c 5f64 796e 616d 6963 5f70 726f  [kdl_dynamic_pro
-00000190: 7879 5d0d 0a70 726f 7879 3d6f 3636 382e  xy]..proxy=o668.
-000001a0: 6b64 6c74 7073 2e63 6f6d 3a31 3538 3138  kdltps.com:15818
-000001b0: 0d0a 7573 6572 6e61 6d65 3d2a 2a2a 0d0a  ..username=***..
-000001c0: 7061 7373 776f 7264 3d2a 2a2a 0d0a 0d0a  password=***....
-000001d0: 5b6b 646c 5f65 7863 6c75 7369 7665 5f70  [kdl_exclusive_p
-000001e0: 726f 7879 5d0d 0a70 726f 7879 3d68 7474  roxy]..proxy=htt
-000001f0: 703a 2f2f 6b70 732e 6b64 6c61 7069 2e63  p://kps.kdlapi.c
-00000200: 6f6d 2f61 7069 2f67 6574 6b70 733f 6f72  om/api/getkps?or
-00000210: 6465 7269 643d 2a2a 2a26 6e75 6d3d 3130  derid=***&num=10
-00000220: 3026 666f 726d 6174 3d6a 736f 6e0d 0a75  0&format=json..u
-00000230: 7365 726e 616d 653d 2a2a 2a0d 0a70 6173  sername=***..pas
-00000240: 7377 6f72 643d 2a2a 2a0d 0a69 6e64 6578  sword=***..index
-00000250: 3d31 0d0a 0d0a 5b61 6c69 5f6f 7373 5d0d  =1....[ali_oss].
-00000260: 0a61 6363 6573 736b 6579 6964 3d4c 5441  .accesskeyid=LTA
-00000270: 2a2a 2a2a 2a2a 0d0a 6163 6365 7373 6b65  ******..accesske
-00000280: 7973 6563 7265 743d 2a2a 2a2a 2a2a 0d0a  ysecret=******..
-00000290: 656e 6470 6f69 6e74 3d68 7474 7073 3a2f  endpoint=https:/
-000002a0: 2f6f 7373 2d63 6e2d 2a2a 2a2a 2a2a 2e61  /oss-cn-******.a
-000002b0: 6c69 7975 6e63 732e 636f 6d0d 0a62 7563  liyuncs.com..buc
-000002c0: 6b65 743d 2a2a 2a2a 2a2a 0d0a 646f 633d  ket=******..doc=
-000002d0: 2a2a 2a2a 2a2a 2a0d 0a                   *******..
+00000120: 0d0a 0d0a 5b6b 6166 6b61 5d0d 0a62 6f6f  ....[kafka]..boo
+00000130: 7473 7472 6170 5f73 6572 7665 7273 3d31  tstrap_servers=1
+00000140: 3237 2e30 2e30 2e31 3a39 3039 3220 23e8  27.0.0.1:9092 #.
+00000150: 8ba5 e5a4 9ae4 b8aa e794 a8e9 8097 e58f  ................
+00000160: b7e5 8886 e99a 940d 0a74 6f70 6963 3d2a  .........topic=*
+00000170: 2a2a 0d0a 6b65 793d 2a2a 2a0d 0a0d 0a5b  **..key=***....[
+00000180: 636f 6e73 756c 5d0d 0a74 6f6b 656e 3d0d  consul]..token=.
+00000190: 0a75 726c 3d68 7474 703a 2f2f 686f 7374  .url=http://host
+000001a0: 3a70 6f72 742f 7631 2f6b 762f 2e2e 2e3f  :port/v1/kv/...?
+000001b0: 6463 3d64 6331 0d0a 666f 726d 6174 3d6a  dc=dc1..format=j
+000001c0: 736f 6e0d 0a0d 0a5b 7778 626f 745d 0d0a  son....[wxbot]..
+000001d0: 6b65 793d 2a2a 2a0d 0a0d 0a5b 6b64 6c5f  key=***....[kdl_
+000001e0: 6479 6e61 6d69 635f 7072 6f78 795d 0d0a  dynamic_proxy]..
+000001f0: 7072 6f78 793d 6f36 3638 2e6b 646c 7470  proxy=o668.kdltp
+00000200: 732e 636f 6d3a 3135 3831 380d 0a75 7365  s.com:15818..use
+00000210: 726e 616d 653d 2a2a 2a0d 0a70 6173 7377  rname=***..passw
+00000220: 6f72 643d 2a2a 2a0d 0a0d 0a5b 6b64 6c5f  ord=***....[kdl_
+00000230: 6578 636c 7573 6976 655f 7072 6f78 795d  exclusive_proxy]
+00000240: 0d0a 7072 6f78 793d 6874 7470 3a2f 2f6b  ..proxy=http://k
+00000250: 7073 2e6b 646c 6170 692e 636f 6d2f 6170  ps.kdlapi.com/ap
+00000260: 692f 6765 746b 7073 3f6f 7264 6572 6964  i/getkps?orderid
+00000270: 3d2a 2a2a 266e 756d 3d31 3030 2666 6f72  =***&num=100&for
+00000280: 6d61 743d 6a73 6f6e 0d0a 7573 6572 6e61  mat=json..userna
+00000290: 6d65 3d2a 2a2a 0d0a 7061 7373 776f 7264  me=***..password
+000002a0: 3d2a 2a2a 0d0a 696e 6465 783d 310d 0a0d  =***..index=1...
+000002b0: 0a5b 616c 695f 6f73 735d 0d0a 6163 6365  .[ali_oss]..acce
+000002c0: 7373 6b65 7969 643d 4c54 412a 2a2a 2a2a  sskeyid=LTA*****
+000002d0: 2a0d 0a61 6363 6573 736b 6579 7365 6372  *..accesskeysecr
+000002e0: 6574 3d2a 2a2a 2a2a 2a0d 0a65 6e64 706f  et=******..endpo
+000002f0: 696e 743d 6874 7470 733a 2f2f 6f73 732d  int=https://oss-
+00000300: 636e 2d2a 2a2a 2a2a 2a2e 616c 6979 756e  cn-******.aliyun
+00000310: 6373 2e63 6f6d 0d0a 6275 636b 6574 3d2a  cs.com..bucket=*
+00000320: 2a2a 2a2a 2a0d 0a64 6f63 3d2a 2a2a 2a2a  *****..doc=*****
+00000330: 2a2a 0d0a                                **..
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files 6% similar despite different names*

```diff
@@ -30,18 +30,14 @@
     custom_settings = {
         # scrapy 日志等级配置
         "LOG_LEVEL": "DEBUG",
         # 是否开启记录项目相关运行统计信息。不配置默认为 False
         "RECORD_LOG_TO_MYSQL": False,
         # 以 loguru 来管理日志，本库会在 settings 中生成规则示例，可自行修改。也可不配置
         "LOGURU_CONFIG": logger,
-        # Mysql 数据表的前缀名称，用于标记属于哪个项目，可不配置
-        "MYSQL_TABLE_PREFIX": "demo_basic_",
-        # MongoDB 集合的前缀名称，用于标记属于哪个项目，可不配置
-        "MONGODB_COLLECTION_PREFIX": "demo_basic_",
         "ITEM_PIPELINES": {
             # 激活此项则数据会存储至 Mysql
             "ayugespidertools.pipelines.AyuFtyMysqlPipeline": 300,
             # 激活此项则数据会存储至 MongoDB
             "ayugespidertools.pipelines.AyuFtyMongoPipeline": 301,
         },
         "DOWNLOADER_MIDDLEWARES": {
@@ -104,15 +100,15 @@
                 nick_name=DataItem(nick_name, "文章作者昵称"),
                 _table=TableEnum.article_list_table.value["value"],
             )
             self.slog.info(f"ArticleInfoMysqlItem: {ArticleInfoMysqlItem}")
 
             # 数据入库逻辑，你可以使用 mysql_engine 来去重或自定义规则
             try:
-                save_table = f'{self.custom_settings.get("MYSQL_TABLE_PREFIX", "")}{TableEnum.article_list_table.value["value"]}'
+                save_table = TableEnum.article_list_table.value["value"]
                 sql = f'''select `id` from `{save_table}` where `article_detail_url` = "{article_detail_url}" limit 1'''
                 df = pandas.read_sql(sql, self.mysql_engine)
 
                 # 如果为空，说明此数据不存在于数据库，则新增
                 if df.empty:
                     yield ArticleInfoMysqlItem
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     # 数据库表的枚举信息
     custom_table_enum = TableEnum
     # 初始化配置的类型
     settings_type = "debug"
     custom_settings = {
         # scrapy 日志等级配置
         "LOG_LEVEL": "DEBUG",
-        # Mysql数据表的前缀名称，用于标记属于哪个项目，也可以不用配置
-        "MYSQL_TABLE_PREFIX": "demo_crawl_",
         "ITEM_PIPELINES": {
             # 激活此项则数据会存储至 Mysql
             "ayugespidertools.pipelines.AyuFtyMysqlPipeline": 300,
         },
         "DOWNLOADER_MIDDLEWARES": {
             # 随机请求头
             "ayugespidertools.middlewares.RandomRequestUaMiddleware": 400,
```

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.2.0/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/ayugespidertools/verificationcode.py` & `ayugespidertools-3.2.0/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.1.0/pyproject.toml` & `ayugespidertools-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "3.1.0"
+version = "3.2.0"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -12,18 +12,16 @@
 homepage = "https://www.ayuge.top/mkdocs-material/"
 include = ["pyproject.toml"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 opencv-python = "^4.6.0.66"
 PyMySQL = "^1.0.2"
-environs = "^9.5.0"
 loguru = "^0.6.0"
 numpy = "1.24.2"
-PyExecJS = "^1.5.1"
 requests = "^2.28.1"
 Pillow = "^9.2.0"
 Scrapy = "2.9.0"
 pandas = "^1.5.0"
 WorkWeixinRobot = "^1.0.1"
 retrying = "^1.3.3"
 SQLAlchemy = "^1.4.41"
@@ -38,14 +36,15 @@
 aiomysql = "^0.1.1"
 attrs = "^22.2.0"
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
 motor = "2.5.1"
 urllib3 = "~1.26.15"
 pika = "~1.3.2"
+kafka-python = "2.0.2"
 
 [tool.poetry.scripts]
 ayuge = "ayugespidertools.utils.cmdline:execute"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^23.1.0"
```

### Comparing `ayugespidertools-3.1.0/PKG-INFO` & `ayugespidertools-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 3.1.0
+Version: 3.2.0
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: DBUtils (>=3.0.2,<4.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: PyExecJS (>=1.5.1,<2.0.0)
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: Scrapy (==2.9.0)
 Requires-Dist: WorkWeixinRobot (>=1.0.1,<2.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
-Requires-Dist: environs (>=9.5.0,<10.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: itemadapter (>=0.7.0,<0.8.0)
+Requires-Dist: kafka-python (==2.0.2)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: motor (==2.5.1)
 Requires-Dist: numpy (==1.24.2)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: oss2 (>=2.16.0,<3.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
@@ -133,16 +132,15 @@
 # 采集数据存入 `MongoDB` 的场景：
 + 2).demo_two: 采集数据存入 `MongoDB` 的场景（配置根据本地 `settings` 的 `LOCAL_MONGODB_CONFIG` 中取值）
 + 4).demo_four: 采集数据存入 `MongoDB` 的场景（配置根据 `consul` 的应用管理中心中取值）
 + 6).demo_six: 异步存入 `MongoDB` 的场景
 
 # 将 `Scrapy` 的 `Request`，`FormRequest` 替换为其它工具实现的场景
 - 以上为使用 scrapy Request 的场景
-+ 7).demo_seven: scrapy Request 替换为 requests 请求的场景(一般情况下不推荐使用，同步库
-+ 会拖慢 scrapy 速度，可用于测试场景)
+- 7).demo_seven: scrapy Request 替换为 requests 请求的场景(已删除此功能，更推荐使用 aiohttp 方式)
 
 + 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
 
 + 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
 + 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
 
 + 11).demo_proxy_one: 快代理动态隧道代理示例
@@ -152,15 +150,16 @@
 +14).demo_crawl: 支持 scrapy CrawlSpider 的示例
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
 +15).demo_item_loader: 本库中使用 Item Loaders 的示例
 -16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目前已经可以很方便的使用 Item Loaders 功能了
 
 +17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
-+18).demo_mq: 数据存入 rabbitmq 的模板示例，通过 pika 库实现
++18).demo_mq: 数据存入 rabbitmq 的模板示例
++19).demo_kafka: 数据存入 rabbitmq 的模板示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
@@ -215,23 +214,23 @@
 - [x] `scrapy` 的扩展功能场景
   - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
   - [x] 自定义模板，在 `ayugespidertools startproject <projname>` 和 `ayugespidertools genspider <spidername>` 时生成适合本库的模板文件
   - [x] ~~增加根据 `nacos` 来获取配置的功能~~ -> 改为增加根据 `consul` 来获取配置的功能
   - [x] 代理中间件（独享代理、动态隧道代理）
   - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
   - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-    - [x] `requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率
+    - [x] ~~`requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率~~（已移除此功能，更推荐 `aiohttp` 的方式）
     - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
   - [x] `Mysql` 存储的场景下适配
     - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
   - [x] `MongoDB` 存储的场景下适配，编写风格与 `Mysql` 存储等场景下一致
   - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
     - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
     - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
-  - [ ] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
+  - [x] 集成 `Kafka`，`RabbitMQ` 等数据推送功能
 - [x] 常用开发场景
   - [x] `sql` 语句拼接，只是简单场景，后续优化。已给出优化方向，参考库等信息。
   - [x] `mongoDB` 语句拼接
   - [x] 数据格式化处理，比如：去除网页标签，去除无效空格等
   - [x] 字体反爬还原方法
     - [x] 基于 `ttf`，`woff` 之类的字体文件映射，或结合 `css` 等实现
       - [x] 可以直接在字体文件 `xml` 中找到映射关系的：使用 [fontforge](https://github.com/fontforge/fontforge/releases) 工具导出映射即可。
```

