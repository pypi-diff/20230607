# Comparing `tmp/inhandtest-0.0.52.tar.gz` & `tmp/inhandtest-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.52.tar", last modified: Tue Jun  6 05:27:38 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.53.tar", last modified: Wed Jun  7 05:18:23 2023, max compression
```

## Comparing `inhandtest-0.0.52.tar` & `inhandtest-0.0.53.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.52/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-06 05:27:38.000000 inhandtest-0.0.52/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.52/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.52/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.52/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.52/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.52/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    40079 2023-06-06 03:00:03.000000 inhandtest-0.0.52/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.52/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.52/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    58788 2023-06-06 05:15:22.000000 inhandtest-0.0.52/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23364 2023-06-05 10:27:40.000000 inhandtest-0.0.52/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.52/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.52/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.52/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.52/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.52/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    51904 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7588 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.52/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11625 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.52/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     2393 2023-06-06 05:25:15.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     8317 2023-06-06 01:49:59.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67781 2023-06-02 09:30:51.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86145 2023-06-02 02:13:33.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0     9556 2023-06-06 05:26:06.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0     9456 2023-06-06 05:25:15.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.52/inhandtest/pages/locale.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.52/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    33681 2023-06-06 05:26:30.000000 inhandtest-0.0.52/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    27448 2023-06-02 06:02:42.000000 inhandtest-0.0.52/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.52/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 05:27:38.000000 inhandtest-0.0.52/setup.cfg
--rw-rw-rw-   0        0        0     1626 2023-06-06 05:27:26.000000 inhandtest-0.0.52/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.53/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-07 05:18:23.000000 inhandtest-0.0.53/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.53/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.53/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.53/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.53/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.53/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    40079 2023-06-06 03:00:03.000000 inhandtest-0.0.53/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.53/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.53/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    58788 2023-06-06 05:15:22.000000 inhandtest-0.0.53/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23364 2023-06-05 10:27:40.000000 inhandtest-0.0.53/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.53/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.53/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.53/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.53/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.53/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    52197 2023-06-07 03:52:54.000000 inhandtest-0.0.53/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7588 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.53/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11625 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.53/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     2393 2023-06-06 05:25:15.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     8317 2023-06-06 01:49:59.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67781 2023-06-02 09:30:51.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86145 2023-06-02 02:13:33.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0     9556 2023-06-06 05:26:06.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    11230 2023-06-07 02:28:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.53/inhandtest/pages/locale.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.53/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    33681 2023-06-06 05:26:30.000000 inhandtest-0.0.53/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    27509 2023-06-07 03:54:00.000000 inhandtest-0.0.53/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.53/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 05:18:23.000000 inhandtest-0.0.53/setup.cfg
+-rw-rw-rw-   0        0        0     1626 2023-06-07 05:16:53.000000 inhandtest-0.0.53/setup.py
```

### Comparing `inhandtest-0.0.52/PKG-INFO` & `inhandtest-0.0.53/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.52
+Version: 0.0.53
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.52/README.md` & `inhandtest-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/dm/mqtt.py` & `inhandtest-0.0.53/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/dm/register_v1.py` & `inhandtest-0.0.53/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.53/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.53/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.53/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/base_page/base_page.py` & `inhandtest-0.0.53/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.53/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/exception.py` & `inhandtest-0.0.53/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/file.py` & `inhandtest-0.0.53/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/inmodbus.py` & `inhandtest-0.0.53/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/inmongodb.py` & `inhandtest-0.0.53/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/inmqtt.py` & `inhandtest-0.0.53/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/inrequest.py` & `inhandtest-0.0.53/inhandtest/inrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,14 +646,19 @@
         sn = [sn] if isinstance(sn, str) else sn
         device = list(filter(lambda x: x.get('id'), self.device_state(sn)))
         if device:
             for device_ in device:
                 self.api.send_request(f'api/invpn/router/{device_.get("id")}', 'delete', {'oid': self.oid})
                 logging.info(f'the {device_.get("sn")} delete success')
 
+    @loop_inspector('ics user connect openvpn')
+    def assert_user_openvpn_connect(self, email, timeout=60, interval=5):
+        response = self.api.send_request('/api/invpn/users', 'get', param={'verbose': 100, 'email': email}).json()
+        return response['result'][0]['connected']
+
 
 class StarInterface:
 
     def __init__(self, username, password, host='star.inhandcloud.cn'):
         """ 须确保用户关闭了多因素认证
 
         :param username  平台用户名
```

### Comparing `inhandtest-0.0.52/inhandtest/inserial.py` & `inhandtest-0.0.53/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/insocket.py` & `inhandtest-0.0.53/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/inssh.py` & `inhandtest-0.0.53/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/ip.py` & `inhandtest-0.0.53/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/mail.py` & `inhandtest-0.0.53/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.53/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.53/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,15 +108,16 @@
                                 'param': {'manual_refresh': self.locale.manual_refresh, 'sec': self.locale.sec,
                                           'min': self.locale.min}}),
             ('refresh', {'locator': self.page.locator('.ant-btn.ant-btn-sm'), 'type': 'button'}),
             (
                 'clear_history_log',
                 {'locator': self.page.locator('//button[@class="ant-btn"]').nth(0), 'type': 'button'}),
             ('clear_log', {'locator': self.page.locator('//button[@class="ant-btn"]').nth(1), 'type': 'button'}),
-            ('download_log', {'locator': self.page.locator('//button[@class="ant-btn"]').nth(2), 'type': 'download_file'}),
+            ('download_log',
+             {'locator': self.page.locator('//button[@class="ant-btn"]').nth(2), 'type': 'download_file'}),
             ('download_history_log',
              {'locator': self.page.locator('//button[@class="ant-btn"]').nth(3), 'type': 'download_file'}),
             ('download_diagnostic_data',
              {'locator': self.page.locator('//button[@class="ant-btn"]').nth(4), 'type': 'download_file'}),
             ('confirm',
              {'locator': self.page.locator('.ant-popover-content').locator('.ant-btn.ant-btn-primary.ant-btn-sm'),
               'type': 'button'}),
@@ -144,14 +145,45 @@
              {'locator': self.page.locator('.ant-select.ant-select-enabled'), 'type': 'select',
               'param': {'emergency': self.locale.emergency, 'alarm': self.locale.alarm,
                         'serious': self.locale.serious, 'error': self.locale.error, 'warning': self.locale.warning,
                         'notice': self.locale.notice, 'information': self.locale.information,
                         'debug': self.locale.debug}}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
+                                           has_text=self.locale.submit), 'type': 'button'}),
+            ('errors_text', {'type': 'text_messages'}),
+            ('success_tip', {'type': 'tip_messages'}),
+        ]
+
+
+class ConfigLocators:
+    def __init__(self, page: Page, locale: dict):
+        self.page = page
+        self.locale = locale
+        self.pop_up = self.page.locator('.ant-modal-content')
+
+    @property
+    def config_locators(self) -> list:
+        return [
+            ('auto_save', {'locator': self.page.locator('//button[@role="switch"]').nth(0), 'type': 'switch_button'}),
+            ('encrypted', {'locator': self.page.locator('//button[@role="switch"]').nth(1), 'type': 'switch_button'}),
+            ('import_startup_config', {'locator': self.page.locator('//button[@class="ant-btn"]'), 'type': 'upload_file'}),
+            ('import_config',
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]').nth(0), 'type': 'button'}),
+            ('reboot',
+             {'locator': self.page.locator('.ant-modal-content').locator('.ant-btn.ant-btn-primary'), 'type': 'button'}),
+
+            ('export_startup_config',
+             {'locator': self.page.locator('.ant-select.ant-select-enabled'), 'type': 'select',
+              'param': {'emergency': self.locale.emergency, 'alarm': self.locale.alarm,
+                        'serious': self.locale.serious, 'error': self.locale.error, 'warning': self.locale.warning,
+                        'notice': self.locale.notice, 'information': self.locale.information,
+                        'debug': self.locale.debug}}),
+            ('submit',
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit), 'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
         ]
 
 
 class SystemLocators(SystemTimeLocators, LogLocators):
```

### Comparing `inhandtest-0.0.52/inhandtest/pytest_email.html` & `inhandtest-0.0.53/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/telnet.py` & `inhandtest-0.0.53/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/inhandtest/tools.py` & `inhandtest-0.0.53/inhandtest/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,17 +238,19 @@
                     logging.info(f"kill process {proc.pid} success")
 
     def port_is_close(one_port: int):  # 杀死后要一直等到进程完全退出才能继续执行，否则会报错
         for i in range(0, 15):
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 try:
                     s.bind((ip_, one_port))
+                    s.close()
                     time.sleep(1)
-                except socket.error:
                     break
+                except socket.error:
+                    continue
         else:
             raise Exception(f"kill process {one_port} failed")
 
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
     [port_is_close(port_) for port_ in port] if isinstance(port, list) else port_is_close(port)
```

### Comparing `inhandtest-0.0.52/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.53/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.52
+Version: 0.0.53
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.52/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.53/inhandtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.52/setup.py` & `inhandtest-0.0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.52',
+    version='0.0.53',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

