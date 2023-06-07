# Comparing `tmp/bdfrx-1.0.7.tar.gz` & `tmp/bdfrx-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdfrx-1.0.7.tar", last modified: Fri May 26 00:41:05 2023, max compression
+gzip compressed data, was "bdfrx-1.0.8.tar", last modified: Wed Jun  7 00:23:08 2023, max compression
```

## Comparing `bdfrx-1.0.7.tar` & `bdfrx-1.0.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.432501 bdfrx-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-05-26 00:40:49.000000 bdfrx-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-26 00:41:05.432501 bdfrx-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-26 00:40:49.000000 bdfrx-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.420501 bdfrx-1.0.7/bdfrx/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/bdfrx.db
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/default_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_authenticator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.428501 bdfrx-1.0.7/bdfrx/site_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/catbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/delay_for_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/download_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/erome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.428501 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/gfycat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/imgchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/imgur.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/pornhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/redgifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/self_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/vidble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/vreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.424501 bdfrx-1.0.7/bdfrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-26 00:40:49.000000 bdfrx-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:41:05.432501 bdfrx-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.428501 bdfrx-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-06-07 00:22:55.000000 bdfrx-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-06-07 00:23:08.599015 bdfrx-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-06-07 00:22:55.000000 bdfrx-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.595015 bdfrx-1.0.8/bdfrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/bdfrx.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/default_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_authenticator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/bdfrx/site_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/catbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/delay_for_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/download_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/erome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/gfycat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/imgchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/imgur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/pornhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/redgifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/self_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/vidble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/vreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.595015 bdfrx-1.0.8/bdfrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-07 00:22:55.000000 bdfrx-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:23:08.599015 bdfrx-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_resource.py
```

### Comparing `bdfrx-1.0.7/LICENSE` & `bdfrx-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/PKG-INFO` & `bdfrx-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.7
+Version: 1.0.8
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bdfrx-1.0.7/README.md` & `bdfrx-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/__main__.py` & `bdfrx-1.0.8/bdfrx/__main__.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/bdfrx.db` & `bdfrx-1.0.8/bdfrx/bdfrx.db`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/completion.py` & `bdfrx-1.0.8/bdfrx/completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/configuration.py` & `bdfrx-1.0.8/bdfrx/configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/connector.py` & `bdfrx-1.0.8/bdfrx/connector.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/download_filter.py` & `bdfrx-1.0.8/bdfrx/download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/downloader.py` & `bdfrx-1.0.8/bdfrx/downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/file_name_formatter.py` & `bdfrx-1.0.8/bdfrx/file_name_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             out = Path(root, filename + ending)
 
         return out
 
     @staticmethod
     def find_max_path_length() -> int:
         try:
-            return int(subprocess.check_output(["/usr/bin/getconf", "PATH_MAX", "/"]))  # noqa: S603
+            return int(subprocess.check_output(["getconf", "PATH_MAX", "/"]))  # noqa: S603, S607
         except (ValueError, subprocess.CalledProcessError, OSError):
             if platform.system() == "Windows":
                 return FileNameFormatter.WINDOWS_MAX_PATH_LENGTH
             return FileNameFormatter.LINUX_MAX_PATH_LENGTH
 
     def format_resource_paths(
         self,
```

### Comparing `bdfrx-1.0.7/bdfrx/oauth2.py` & `bdfrx-1.0.8/bdfrx/oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/resource.py` & `bdfrx-1.0.8/bdfrx/resource.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/base_downloader.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/catbox.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/catbox.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/delay_for_reddit.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/delay_for_reddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/direct.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/direct.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/download_factory.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/download_factory.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/erome.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/erome.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/gallery.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/gallery.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/gfycat.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/gfycat.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/imgchest.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/imgchest.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/imgur.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/imgur.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/pornhub.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/pornhub.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/redgifs.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/redgifs.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/self_post.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/self_post.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/vidble.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/vidble.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/vreddit.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/vreddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx/site_downloaders/youtube.py` & `bdfrx-1.0.8/bdfrx/site_downloaders/youtube.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/bdfrx.egg-info/PKG-INFO` & `bdfrx-1.0.8/bdfrx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.7
+Version: 1.0.8
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bdfrx-1.0.7/bdfrx.egg-info/SOURCES.txt` & `bdfrx-1.0.8/bdfrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/pyproject.toml` & `bdfrx-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/tests/test_completion.py` & `bdfrx-1.0.8/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/tests/test_configuration.py` & `bdfrx-1.0.8/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/tests/test_connector.py` & `bdfrx-1.0.8/tests/test_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,24 +37,24 @@
 
 
 def assert_all_results_are_submissions(result_limit: int, results: list[Iterator]) -> list:
     results = [sub for res in results for sub in res]
     assert all(isinstance(res, praw.models.Submission) for res in results)
     assert not any(isinstance(m, MagicMock) for m in results)
     if result_limit is not None:
-        assert len(results) == result_limit
+        assert len(results) <= result_limit
     return results
 
 
 def assert_all_results_are_submissions_or_comments(result_limit: int, results: list[Iterator]) -> list:
     results = [sub for res in results for sub in res]
     assert all(isinstance(res, (praw.models.Submission, praw.models.Comment)) for res in results)
     assert not any(isinstance(m, MagicMock) for m in results)
     if result_limit is not None:
-        assert len(results) == result_limit
+        assert len(results) <= result_limit
     return results
 
 
 def test_determine_directories(tmp_path: Path, downloader_mock: MagicMock):
     downloader_mock.args.directory = tmp_path / "test"
     downloader_mock.config_directories.user_config_dir = tmp_path
     RedditConnector.determine_directories(downloader_mock)
```

### Comparing `bdfrx-1.0.7/tests/test_download_filter.py` & `bdfrx-1.0.8/tests/test_download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/tests/test_downloader.py` & `bdfrx-1.0.8/tests/test_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import re
-import sys
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 import praw.models
 import pytest
 
 from bdfrx.__main__ import make_console_logging_handler
@@ -153,15 +152,14 @@
     output = capsys.readouterr()
     assert not folder_contents
     assert re.search(r"Resource hash .*? downloaded elsewhere", output.out)
 
 
 @pytest.mark.online
 @pytest.mark.reddit
-@pytest.mark.skipif(sys.platform == "win32", reason="Hangs on Github Windows.")
 def test_download_submission_file_exists(
     downloader_mock: MagicMock,
     reddit_instance: praw.Reddit,
     tmp_path: Path,
     capsys: pytest.CaptureFixture,
 ):
     add_console_handler()
```

### Comparing `bdfrx-1.0.7/tests/test_file_name_formatter.py` & `bdfrx-1.0.8/tests/test_file_name_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,14 @@
     test_comment = reddit_instance.comment(id=test_comment_id)
     test_formatter = FileNameFormatter(test_file_scheme, test_folder_scheme, "ISO")
     test_entry = Resource(test_comment, "", lambda: None, ".json")
     result = test_formatter.format_path(test_entry, tmp_path)
     assert do_test_string_equality(result, expected_name)
 
 
-@pytest.mark.skipif(sys.platform == "win32", reason="Hangs on Github Windows.")
 @pytest.mark.parametrize(
     ("test_folder_scheme", "expected"),
     (
         ("{REDDITOR}/{SUBREDDIT}", "person/randomreddit"),
         ("{POSTID}/{SUBREDDIT}/{REDDITOR}", "12345/randomreddit/person"),
     ),
 )
```

### Comparing `bdfrx-1.0.7/tests/test_oauth2.py` & `bdfrx-1.0.8/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.7/tests/test_resource.py` & `bdfrx-1.0.8/tests/test_resource.py`

 * *Files identical despite different names*

