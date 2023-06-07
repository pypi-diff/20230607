# Comparing `tmp/BasicLibrary.PY-0.5.1.tar.gz` & `tmp/BasicLibrary.PY-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BasicLibrary.PY-0.5.1.tar", last modified: Tue Jun  6 10:10:25 2023, max compression
+gzip compressed data, was "BasicLibrary.PY-0.5.2.tar", last modified: Wed Jun  7 07:56:47 2023, max compression
```

## Comparing `BasicLibrary.PY-0.5.1.tar` & `BasicLibrary.PY-0.5.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.830735 BasicLibrary.PY-0.5.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:24.937441 BasicLibrary.PY-0.5.1/BasicLibrary/
--rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/__init__.py
--rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.1/BasicLibrary/__projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.009437 BasicLibrary.PY-0.5.1/BasicLibrary/biz/
--rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.1/BasicLibrary/biz/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/biz/stockHelper.py
--rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.1/BasicLibrary/biz/tencentHelper.py
--rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/configHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.243019 BasicLibrary.PY-0.5.1/BasicLibrary/data/
--rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/__init__.py
--rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/collectionHelper.py
--rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/dateTimeHelper.py
--rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/dictHelper.py
--rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/htmlHelper.py
--rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/listHelper.py
--rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/numberHelper.py
--rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/objectHelper.py
--rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/pandasHelper.py
--rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/randomHelper.py
--rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/reflectHelper.py
--rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/regexHelper.py
--rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/setHelper.py
--rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/stringHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.338546 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.398497 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/ddl.py
--rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/helper.py
--rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/mate.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.455553 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/ddl.py
--rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/mate.py
--rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/pool.py
--rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/__init__.py
--rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseClient.py
--rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseDDL.py
--rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseEnum.py
--rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseHelper.py
--rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseMate.py
--rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseUnitTest.py
--rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.1/BasicLibrary/enums.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.488736 BasicLibrary.PY-0.5.1/BasicLibrary/environment/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.1/BasicLibrary/environment/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/environment/consoleHelper.py
--rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/environment/envHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.566734 BasicLibrary.PY-0.5.1/BasicLibrary/io/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/dirHelper.py
--rw-rw-rw-   0        0        0     5194 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/fileHelper.py
--rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/ioHelper.py
--rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/pathHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.655736 BasicLibrary.PY-0.5.1/BasicLibrary/model/
--rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/__init__.py
--rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/container.py
--rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/dataCompare.py
--rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/kvPair.py
--rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/stopWatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.750734 BasicLibrary.PY-0.5.1/BasicLibrary/office/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelBookMate.py
--rw-rw-rw-   0        0        0     2418 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelHelper.py
--rw-rw-rw-   0        0        0     3047 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelMisc.py
--rw-rw-rw-   0        0        0    10519 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelSheetMate.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.774737 BasicLibrary.PY-0.5.1/BasicLibrary/pattern/
--rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.1/BasicLibrary/pattern/__init__.py
--rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.1/BasicLibrary/pattern/singleton.py
--rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.1/BasicLibrary/projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.785744 BasicLibrary.PY-0.5.1/BasicLibrary/syntax/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.1/BasicLibrary/syntax/__init__.py
--rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.1/BasicLibrary/syntax/switch.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.818741 BasicLibrary.PY-0.5.1/BasicLibrary/web/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.1/BasicLibrary/web/__init__.py
--rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/web/beautifulSoupHelper.py
--rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.1/BasicLibrary/web/requestHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:10:24.960435 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/
--rw-rw-rw-   0        0        0     2896 2023-06-06 10:10:23.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-06-06 10:10:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:10:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 10:10:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2896 2023-06-06 10:10:25.827737 BasicLibrary.PY-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 10:10:25.831739 BasicLibrary.PY-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     4281 2023-06-06 10:10:09.000000 BasicLibrary.PY-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.328417 BasicLibrary.PY-0.5.2/
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:45.800300 BasicLibrary.PY-0.5.2/BasicLibrary/
+-rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/__init__.py
+-rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.2/BasicLibrary/__projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:45.921295 BasicLibrary.PY-0.5.2/BasicLibrary/biz/
+-rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.2/BasicLibrary/biz/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/biz/stockHelper.py
+-rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.2/BasicLibrary/biz/tencentHelper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/configHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.246298 BasicLibrary.PY-0.5.2/BasicLibrary/data/
+-rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/__init__.py
+-rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/collectionHelper.py
+-rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/dateTimeHelper.py
+-rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/dictHelper.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/htmlHelper.py
+-rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/listHelper.py
+-rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/numberHelper.py
+-rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/objectHelper.py
+-rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/pandasHelper.py
+-rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/randomHelper.py
+-rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/reflectHelper.py
+-rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/regexHelper.py
+-rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/setHelper.py
+-rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/data/stringHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.474293 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.571296 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/ddl.py
+-rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/helper.py
+-rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/mate.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.661293 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/ddl.py
+-rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/mate.py
+-rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/pool.py
+-rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/__init__.py
+-rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseClient.py
+-rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseDDL.py
+-rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseEnum.py
+-rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseHelper.py
+-rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseMate.py
+-rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseUnitTest.py
+-rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.2/BasicLibrary/enums.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.725291 BasicLibrary.PY-0.5.2/BasicLibrary/environment/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.2/BasicLibrary/environment/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/environment/consoleHelper.py
+-rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/environment/envHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:46.854291 BasicLibrary.PY-0.5.2/BasicLibrary/io/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/dirHelper.py
+-rw-rw-rw-   0        0        0     5979 2023-06-07 07:54:07.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/fileHelper.py
+-rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/ioHelper.py
+-rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/io/pathHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.121424 BasicLibrary.PY-0.5.2/BasicLibrary/model/
+-rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/__init__.py
+-rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/container.py
+-rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/dataCompare.py
+-rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/kvPair.py
+-rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.2/BasicLibrary/model/stopWatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.217422 BasicLibrary.PY-0.5.2/BasicLibrary/office/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelBookMate.py
+-rw-rw-rw-   0        0        0     2418 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelHelper.py
+-rw-rw-rw-   0        0        0     3047 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelMisc.py
+-rw-rw-rw-   0        0        0    10519 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.2/BasicLibrary/office/excelSheetMate.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.243420 BasicLibrary.PY-0.5.2/BasicLibrary/pattern/
+-rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.2/BasicLibrary/pattern/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.2/BasicLibrary/pattern/singleton.py
+-rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.2/BasicLibrary/projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.274423 BasicLibrary.PY-0.5.2/BasicLibrary/syntax/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.2/BasicLibrary/syntax/__init__.py
+-rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.2/BasicLibrary/syntax/switch.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:47.317416 BasicLibrary.PY-0.5.2/BasicLibrary/web/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.2/BasicLibrary/web/__init__.py
+-rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.2/BasicLibrary/web/beautifulSoupHelper.py
+-rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.2/BasicLibrary/web/requestHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:56:45.874293 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:56:44.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-06-07 07:56:45.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:56:45.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 07:56:45.000000 BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:56:47.326420 BasicLibrary.PY-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 07:56:47.331440 BasicLibrary.PY-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     4281 2023-06-06 12:49:38.000000 BasicLibrary.PY-0.5.2/setup.py
```

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/__init__.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/__projectHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/__projectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/biz/stockHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/biz/stockHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/configHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/configHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/collectionHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/collectionHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/dateTimeHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/dateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/dictHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/dictHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/listHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/listHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/numberHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/numberHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/objectHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/objectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/pandasHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/pandasHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/randomHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/randomHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/reflectHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/reflectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/regexHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/regexHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/data/stringHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/data/stringHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/ddl.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/helper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/helper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/mate.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MongoDB/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/ddl.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/mate.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/pool.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/MySql/pool.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseClient.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseClient.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseDDL.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseDDL.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseMate.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseUnitTest.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/dataBase/databaseUnitTest.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/environment/consoleHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/environment/consoleHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/environment/envHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/environment/envHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/io/dirHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/io/dirHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/io/fileHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/io/fileHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,20 @@
         :param file_name:
         :return:
         """
         filepath, filename = os.path.split(file_name)
         return filepath
 
     @staticmethod
-    def load(file_full_name):
+    def load(file_full_name: str) -> object:
+        """
+
+        :param file_full_name:
+        :return:
+        """
         with open(file_full_name, "r", encoding='utf-8') as file_pointer:
             data = file_pointer.read()
         return data
 
     @staticmethod
     def load_with_lines(file_full_name):
         """
@@ -157,7 +162,29 @@
         :param source_file_full_name:
         :param target_dir_full_name:
         :param target_file_base_name:
         :return:
         """
         cls.copy(source_file_full_name, target_dir_full_name, target_file_base_name)
         cls.remove(source_file_full_name)
+
+    @classmethod
+    def is_exist(cls, file_full_name):
+        """
+        判断为文件是否存在
+        :param file_full_name: 带全路径的文件名称
+        :return:
+        """
+        return os.path.isfile(file_full_name)
+
+    @classmethod
+    def rename(cls, old_file_full_name, new_file_name):
+        """
+
+        :param old_file_full_name: 旧有的带路径的文件全名称
+        :param new_file_name: 要改名的新的名称（不带文件路径）
+        :return:
+        """
+        file_path = cls.get_path_name(old_file_full_name)
+        new_file_full_name = PathHelper.combine(file_path, new_file_name)
+        os.rename(old_file_full_name, new_file_full_name)
+
```

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/io/ioHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/io/ioHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/io/pathHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/io/pathHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/model/container.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/model/container.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/model/dataCompare.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/model/dataCompare.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/model/kvPair.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/model/kvPair.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelBookMate.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelBookMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelMisc.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelMisc.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelSheetMate.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/office/excelSheetMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/syntax/switch.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/syntax/switch.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/web/beautifulSoupHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/web/beautifulSoupHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary/web/requestHelper.py` & `BasicLibrary.PY-0.5.2/BasicLibrary/web/requestHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/PKG-INFO` & `BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.1
+Version: 0.5.2
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/SOURCES.txt` & `BasicLibrary.PY-0.5.2/BasicLibrary.PY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/PKG-INFO` & `BasicLibrary.PY-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.1
+Version: 0.5.2
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.1/README.md` & `BasicLibrary.PY-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.1/setup.py` & `BasicLibrary.PY-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 NAME = 'BasicLibrary.PY'
 DESCRIPTION = '企业级的 PYTHON 库'
 URL = 'https://github.com/notinmood/BasicLibrary.PY'
 EMAIL = '9727005@qq.com'
 AUTHOR = 'xiedali'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.01'
+VERSION = '0.5.02'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

