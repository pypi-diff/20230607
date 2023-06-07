# Comparing `tmp/BasicLibrary.PY-0.5.2.tar.gz` & `tmp/BasicLibrary.PY-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BasicLibrary.PY-0.5.2.tar", last modified: Wed Jun  7 07:56:47 2023, max compression
+gzip compressed data, was "BasicLibrary.PY-0.5.4.tar", last modified: Wed Jun  7 14:06:45 2023, max compression
```

## Comparing `BasicLibrary.PY-0.5.2.tar` & `BasicLibrary.PY-0.5.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.328417 BasicLibrary.PY-0.5.2/
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:45.800300 BasicLibrary.PY-0.5.2/BasicLibrary/
--rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/__init__.py
--rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.2/BasicLibrary/__projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:45.921295 BasicLibrary.PY-0.5.2/BasicLibrary/biz/
--rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.2/BasicLibrary/biz/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/biz/stockHelper.py
--rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.2/BasicLibrary/biz/tencentHelper.py
--rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/configHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.246298 BasicLibrary.PY-0.5.2/BasicLibrary/data/
--rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/__init__.py
--rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/collectionHelper.py
--rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/dateTimeHelper.py
--rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/dictHelper.py
--rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/htmlHelper.py
--rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/listHelper.py
--rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/numberHelper.py
--rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/objectHelper.py
--rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/pandasHelper.py
--rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/randomHelper.py
--rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/reflectHelper.py
--rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/regexHelper.py
--rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/setHelper.py
--rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/stringHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.474293 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.571296 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/ddl.py
--rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/helper.py
--rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/mate.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.661293 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/ddl.py
--rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/mate.py
--rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/pool.py
--rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/__init__.py
--rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseClient.py
--rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseDDL.py
--rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseEnum.py
--rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseHelper.py
--rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseMate.py
--rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseUnitTest.py
--rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.2/BasicLibrary/enums.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.725291 BasicLibrary.PY-0.5.2/BasicLibrary/environment/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.2/BasicLibrary/environment/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/environment/consoleHelper.py
--rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/environment/envHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.854291 BasicLibrary.PY-0.5.2/BasicLibrary/io/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/dirHelper.py
--rw-rw-rw-   0        0        0     5979 2023-06-07 07:54:07.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/fileHelper.py
--rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/ioHelper.py
--rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/pathHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.121424 BasicLibrary.PY-0.5.2/BasicLibrary/model/
--rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/__init__.py
--rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/container.py
--rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/dataCompare.py
--rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/kvPair.py
--rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/stopWatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.217422 BasicLibrary.PY-0.5.2/BasicLibrary/office/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelBookMate.py
--rw-rw-rw-   0        0        0     2418 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelHelper.py
--rw-rw-rw-   0        0        0     3047 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelMisc.py
--rw-rw-rw-   0        0        0    10519 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelSheetMate.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.243420 BasicLibrary.PY-0.5.2/BasicLibrary/pattern/
--rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.2/BasicLibrary/pattern/__init__.py
--rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.2/BasicLibrary/pattern/singleton.py
--rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.2/BasicLibrary/projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.274423 BasicLibrary.PY-0.5.2/BasicLibrary/syntax/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.2/BasicLibrary/syntax/__init__.py
--rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.2/BasicLibrary/syntax/switch.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.317416 BasicLibrary.PY-0.5.2/BasicLibrary/web/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.2/BasicLibrary/web/__init__.py
--rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/web/beautifulSoupHelper.py
--rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.2/BasicLibrary/web/requestHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:56:45.874293 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:56:44.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-06-07 07:56:45.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:56:45.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-07 07:56:45.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:56:47.326420 BasicLibrary.PY-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 07:56:47.331440 BasicLibrary.PY-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     4281 2023-06-06 12:49:38.000000 BasicLibrary.PY-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.256817 BasicLibrary.PY-0.5.4/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.196821 BasicLibrary.PY-0.5.4/BasicLibrary/
+-rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/__init__.py
+-rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.4/BasicLibrary/__projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.339817 BasicLibrary.PY-0.5.4/BasicLibrary/biz/
+-rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.4/BasicLibrary/biz/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/biz/stockHelper.py
+-rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.4/BasicLibrary/biz/tencentHelper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/configHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.628822 BasicLibrary.PY-0.5.4/BasicLibrary/data/
+-rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/__init__.py
+-rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/collectionHelper.py
+-rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/dateTimeHelper.py
+-rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/dictHelper.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/htmlHelper.py
+-rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/listHelper.py
+-rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/numberHelper.py
+-rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/objectHelper.py
+-rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/pandasHelper.py
+-rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/randomHelper.py
+-rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/reflectHelper.py
+-rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/regexHelper.py
+-rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/setHelper.py
+-rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/stringHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.745815 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.822815 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/ddl.py
+-rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/helper.py
+-rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/mate.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.881820 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/ddl.py
+-rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/mate.py
+-rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/pool.py
+-rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/__init__.py
+-rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseClient.py
+-rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseDDL.py
+-rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseEnum.py
+-rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseHelper.py
+-rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseMate.py
+-rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseUnitTest.py
+-rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.4/BasicLibrary/enums.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.937821 BasicLibrary.PY-0.5.4/BasicLibrary/environment/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.4/BasicLibrary/environment/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/environment/consoleHelper.py
+-rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/environment/envHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.039818 BasicLibrary.PY-0.5.4/BasicLibrary/io/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/dirHelper.py
+-rw-rw-rw-   0        0        0     5979 2023-06-07 07:54:07.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/fileHelper.py
+-rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/ioHelper.py
+-rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/pathHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.125815 BasicLibrary.PY-0.5.4/BasicLibrary/model/
+-rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/__init__.py
+-rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/container.py
+-rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/dataCompare.py
+-rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/kvPair.py
+-rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/stopWatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.174818 BasicLibrary.PY-0.5.4/BasicLibrary/office/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelBookMate.py
+-rw-rw-rw-   0        0        0     2458 2023-06-07 11:39:53.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelHelper.py
+-rw-rw-rw-   0        0        0     3375 2023-06-07 11:44:09.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelMisc.py
+-rw-rw-rw-   0        0        0    11164 2023-06-07 14:03:03.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelSheetMate.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.187821 BasicLibrary.PY-0.5.4/BasicLibrary/pattern/
+-rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.4/BasicLibrary/pattern/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.4/BasicLibrary/pattern/singleton.py
+-rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.4/BasicLibrary/projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.201821 BasicLibrary.PY-0.5.4/BasicLibrary/syntax/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.4/BasicLibrary/syntax/__init__.py
+-rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.4/BasicLibrary/syntax/switch.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.242815 BasicLibrary.PY-0.5.4/BasicLibrary/web/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.4/BasicLibrary/web/__init__.py
+-rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/web/beautifulSoupHelper.py
+-rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.4/BasicLibrary/web/requestHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.253819 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/
+-rw-rw-rw-   0        0        0     2896 2023-06-07 14:06:42.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-06-07 14:06:43.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:06:43.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 14:06:43.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2896 2023-06-07 14:06:45.253816 BasicLibrary.PY-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:06:45.256817 BasicLibrary.PY-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     4280 2023-06-07 14:06:11.000000 BasicLibrary.PY-0.5.4/setup.py
```

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/__init__.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/__projectHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/__projectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/biz/stockHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/biz/stockHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/configHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/configHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/collectionHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/collectionHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/dateTimeHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/dateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/dictHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/dictHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/listHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/listHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/numberHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/numberHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/objectHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/objectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/pandasHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/pandasHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/randomHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/randomHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/reflectHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/reflectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/regexHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/regexHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/data/stringHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/data/stringHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/ddl.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/helper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/helper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/mate.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/ddl.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/mate.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/pool.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/pool.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseClient.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseClient.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseDDL.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseDDL.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseMate.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseUnitTest.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseUnitTest.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/environment/consoleHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/environment/consoleHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/environment/envHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/environment/envHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/io/dirHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/io/dirHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/io/fileHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/io/fileHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/io/ioHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/io/ioHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/io/pathHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/io/pathHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/model/container.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/model/container.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/model/dataCompare.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/model/dataCompare.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/model/kvPair.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/model/kvPair.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelBookMate.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelBookMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,46 +11,46 @@
 
 class ExcelHelper:
     """
 
     """
 
     @classmethod
-    def operate(cls, file_full_name, callback_in__book):
+    def operate(cls, file_full_name, callback_in_book_mate):
         """
         对 Excel 文件的 book 进行地快捷操作（operate_book 方法的别名）
         :param file_full_name: Excel 文件带路径的全名称
-        :param callback_in__book: 对 Excel 文件进行操作的回调方法。此方法要求一个类型为 ExcelBookMate 的输入参数。
+        :param callback_in_book_mate: 对 Excel 文件进行操作的回调方法。此方法要求一个类型为 ExcelBookMate 的输入参数。
         :return:
         """
-        cls.operate_book(file_full_name, callback_in__book)
+        cls.operate_book(file_full_name, callback_in_book_mate)
 
     @staticmethod
-    def operate_book(file_full_name, callback_in__book):
+    def operate_book(file_full_name, callback_in_book_mate):
         """
         对 Excel 文件的 book 进行地快捷操作
         :param file_full_name: Excel 文件带路径的全名称
-        :param callback_in__book: 对 Excel 文件进行操作的回调方法。此方法要求一个类型为 ExcelBookMate 的输入参数。
+        :param callback_in_book_mate: 对 Excel 文件进行操作的回调方法。此方法要求一个类型为 ExcelBookMate 的输入参数。
         :return:
         """
         with ExcelBookMate(file_full_name) as excel:
-            callback_in__book(excel)
+            callback_in_book_mate(excel)
 
     @staticmethod
-    def operate_sheet(file_full_name, callback_in_sheet, sheet_marker=0):
+    def operate_sheet(file_full_name, callback_in_sheet_mate, sheet_marker=0):
         """
         对 Excel 文件的 sheet 进行地快捷操作
         :param sheet_marker: sheet 的标识（sheet 索引号index 或者 sheet 的名称）
         :param file_full_name: Excel 文件带路径的全名称
-        :param callback_in_sheet: 对 Excel 文件的 sheet 进行操作的回调方法。此方法要求一个类型为 ExcelBookMate 的输入参数。
+        :param callback_in_sheet_mate: 对 Excel 文件的 sheet 进行操作的回调方法。此方法要求一个类型为 ExcelSheetMate 的输入参数。
         :return:
         """
         with ExcelBookMate(file_full_name) as excel:
             sheet = excel.get_sheet(sheet_marker)
-            callback_in_sheet(sheet)
+            callback_in_sheet_mate(sheet)
 
     @staticmethod
     def calc_column_name(start_column_name, delta):
         return _calc_column_name(start_column_name, delta)
 
     @staticmethod
     def calc_cell_marker(original_cell_marker, row_delta, column_delta):
```

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelMisc.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelMisc.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 
         return f"{new_marker_begin}:{new_marker_end}"
     else:
         return _calc_cell_marker(original_range_marker, row_delta, column_delta)
 
 
 def _calc_cell_marker(original_cell_marker, row_delta, column_delta=0):
+    """
+    通過單元格的標識值和偏移量，計算新單元格的標識值
+    :param original_cell_marker:
+    :param row_delta:
+    :param column_delta:
+    :return:
+    """
     # 先从类似 "A2" 里面分离出 字母和数字
     column_pattern = r"[a-zA-Z]+"
     column_matched = RegexHelper.get_matched_items(original_cell_marker, column_pattern)
 
     row_pattern = r"\d+"
     row_matched = RegexHelper.get_matched_items(original_cell_marker, row_pattern)
 
@@ -50,14 +57,20 @@
 
         return f"{new_column_name}{new_row_name}"
     else:
         return None
 
 
 def _calc_column_name(start_column_name, delta):
+    """
+    通過當前列的名稱和偏移量，計算新列的名稱
+    :param start_column_name:
+    :param delta:
+    :return:
+    """
     _len = ObjectHelper.get_length(start_column_name)
 
     """
     列名称的最大长度为2，超过2不接受，直接返回 false
     """
     if _len > 2:
         return False
```

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelSheetMate.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelSheetMate.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
  * @file   : hilandSheet.py
  * @time   : 20:45
  * @date   : 2021/11/9
  * @mail   : 9727005@qq.com
  * @creator: ShanDong Xiedali
  * @company: HiLand & RainyTop
 """
+import string
+
+from BasicLibrary.data.stringHelper import StringHelper
+from BasicLibrary.office.excelMisc import _calc_range_marker, _calc_cell_marker
 
 
 class ExcelSheetMate:
     """
     Excel 工作表
     !!!特别注意，单列数据的写入用二维数组，但单列数据的读出为一维数组。
     """
@@ -36,34 +40,47 @@
         """
         获取列数
         :return:
         """
         row_value = self.original_sheet.used_range.last_cell.row
         return row_value
 
-    def read(self, range_marker):
+    def read(self, range_marker=None):
         """
         获取指定区块内的数值(get方法的别名)
         :param range_marker:区块的标志信息，可以取值如下几种之一：
             1. "A1"  # 返回单个单元格内的值信息 '姓名'
             2. "A1:A2" # 一维数组 ['姓名', '张三']
             3. "A1:B2" # 二维数组 [['姓名', '年龄'], ['张三', 20.0]]
         :return:
         """
         return self.get(range_marker)
 
-    def get(self, range_marker):
+    def get(self, range_marker=None):
         """
         获取指定区块内的数值
         :param range_marker:区块的标志信息，可以取值如下几种之一：
             1. "A1"  # 返回单个单元格内的值信息 '姓名'
             2. "A1:A2" # 一维数组 ['姓名', '张三']
             3. "A1:B2" # 二维数组 [['姓名', '年龄'], ['张三', 20.0]]
+            4. None # 通過二維數組的方式返回全部數據
         :return:
         """
+        if range_marker is None:
+            row_count = self.get_row_count()
+            column_count = self.get_column_count()
+            if row_count > 0:
+                row_count = row_count - 1
+
+            if column_count > 0:
+                column_count = column_count - 1
+
+            last_cell_marker = _calc_cell_marker("A1", row_count, column_count)
+            range_marker = f"A1:{last_cell_marker}"
+
         value = self.original_sheet.range(range_marker).value
         return value
 
     def write(self, range_marker, range_data):
         """
         写入数据(set方法的别名)
         1. 严格模式：请必须匹配 range_marker 和 range_data 的格式相同，数据量相同。
@@ -125,15 +142,14 @@
         """
         if not range_data:
             range_data = self.range_selected
 
         self.original_sheet.range(range_marker).value = range_data
         return
 
-
     # # # 复制
     # def copy(self, sheet_name, range_col_row):
     #     self.my_range = self.original_sheet.range(sheet_name, range_col_row).value
     #     return self.my_range
     #
     # # 粘贴
     # def paste(self, sheet_name, range_col_row):
```

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/syntax/switch.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/syntax/switch.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/web/beautifulSoupHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/web/beautifulSoupHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary/web/requestHelper.py` & `BasicLibrary.PY-0.5.4/BasicLibrary/web/requestHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/PKG-INFO` & `BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.2
+Version: 0.5.4
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/SOURCES.txt` & `BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/PKG-INFO` & `BasicLibrary.PY-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.2
+Version: 0.5.4
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.2/README.md` & `BasicLibrary.PY-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.2/setup.py` & `BasicLibrary.PY-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 NAME = 'BasicLibrary.PY'
 DESCRIPTION = '企业级的 PYTHON 库'
 URL = 'https://github.com/notinmood/BasicLibrary.PY'
 EMAIL = '9727005@qq.com'
 AUTHOR = 'xiedali'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.02'
+VERSION = '0.5.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

