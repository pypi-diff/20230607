# Comparing `tmp/eyes_soatra-0.0.27.tar.gz` & `tmp/eyes_soatra-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.27.tar", last modified: Thu Jun  1 07:22:20 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.28.tar", last modified: Wed Jun  7 04:41:05 2023, max compression
```

## Comparing `eyes_soatra-0.0.27.tar` & `eyes_soatra-0.0.28.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.180416 eyes_soatra-0.0.27/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.27/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 07:22:20.180276 eyes_soatra-0.0.27/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.27/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.174610 eyes_soatra-0.0.27/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.27/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.175650 eyes_soatra-0.0.27/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.27/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.175783 eyes_soatra-0.0.27/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.176265 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.176761 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.177116 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.27/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.177323 eyes_soatra-0.0.27/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.27/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.27/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.177533 eyes_soatra-0.0.27/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.27/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.27/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      747 2023-05-29 02:30:09.000000 eyes_soatra-0.0.27/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.27/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.178939 eyes_soatra-0.0.27/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    20214 2023-06-01 04:21:42.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.179559 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)     1221 2023-05-27 07:50:00.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)    13936 2023-06-01 07:21:31.000000 eyes_soatra-0.0.27/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.175270 eyes_soatra-0.0.27/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       48 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-01 07:22:20.000000 eyes_soatra-0.0.27/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-01 07:22:20.180459 eyes_soatra-0.0.27/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1147 2023-06-01 07:22:07.000000 eyes_soatra-0.0.27/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-01 07:22:20.180061 eyes_soatra-0.0.27/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.27/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.27/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      277 2023-06-01 06:45:42.000000 eyes_soatra-0.0.27/test/test2.py
--rw-r--r--   0 soatra     (501) staff       (20)      236 2023-05-30 04:50:51.000000 eyes_soatra-0.0.27/test/test3.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.932612 eyes_soatra-0.0.28/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.28/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-07 04:41:05.932464 eyes_soatra-0.0.28/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.28/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.922459 eyes_soatra-0.0.28/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.28/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.923729 eyes_soatra-0.0.28/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.28/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.923986 eyes_soatra-0.0.28/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.924729 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.925779 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.926491 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.28/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.926878 eyes_soatra-0.0.28/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.28/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.28/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.927206 eyes_soatra-0.0.28/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.28/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.28/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.28/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.28/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.930104 eyes_soatra-0.0.28/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-07 04:28:32.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.931004 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2538 2023-06-02 06:33:58.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)    14065 2023-06-07 04:33:46.000000 eyes_soatra-0.0.28/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.923162 eyes_soatra-0.0.28/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       34 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-06-07 04:41:05.000000 eyes_soatra-0.0.28/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-06-07 04:41:05.932660 eyes_soatra-0.0.28/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-06-02 04:58:12.000000 eyes_soatra-0.0.28/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-06-07 04:41:05.932122 eyes_soatra-0.0.28/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.28/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.28/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      241 2023-06-07 04:03:02.000000 eyes_soatra-0.0.28/test/test2.py
+-rw-r--r--   0 soatra     (501) staff       (20)      210 2023-06-07 04:38:58.000000 eyes_soatra-0.0.28/test/test3.py
```

### Comparing `eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.28/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.28/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.28/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/eyes_soatra/constant/vars.py` & `eyes_soatra-0.0.28/eyes_soatra/constant/vars.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 from lxml import etree as __etree
 
+main_tags = (
+    'title',
+    'h1',
+    'h2'
+)
+
 header_xpaths = [
     '//title',
     '//h1',
     '//h2',
     '//h3',
     '//h4',
     '//h5',
@@ -69,8 +75,13 @@
     '/',
     '.'
 )
 
 tag_stop = (
     '[',
     ')'
+)
+
+protocols = (
+    'http://',
+    'https://',
 )
```

### Comparing `eyes_soatra-0.0.27/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.28/eyes_soatra/funcs/time_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from eyes_soatra.constant.depends.app_date.end import depends as __depends_end
 from eyes_soatra.constant.depends.app_date.formats.period import formats as __formats_period
 from eyes_soatra.constant.depends.app_date.formats.start import formats as __formats_start
 from eyes_soatra.constant.depends.app_date.formats.end import formats as __formats_end
 from eyes_soatra.constant.user.user_agents import User_Agents as __User_Agents
 from eyes_soatra.funcs.utils.list import find as __find
 from eyes_soatra.funcs.utils.list import map_list as __map_list
-from eyes_soatra.funcs.utils.list import filter_list as __filter
 from eyes_soatra.funcs.utils.string import strip_space as __strip_space
 from eyes_soatra.funcs.utils.string import symbol as __symbol_all
 from eyes_soatra.funcs.utils.string import xpath_tag as __xpath_tag
 from eyes_soatra.constant.libs.requests import requests as __requests
 from eyes_soatra.constant.vars import header_xpaths as __header_xpath
 from eyes_soatra.constant.vars import description_xpath as __description_xpath
 from eyes_soatra.constant.vars import full_stops as __full_stops
```

### Comparing `eyes_soatra-0.0.27/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.28/eyes_soatra/funcs/utils/string.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from eyes_soatra.constant.vars import xpath_prefix as __xpath_prefix
 from eyes_soatra.constant.vars import tag_stop as __tag_stop
+from eyes_soatra.constant.vars import protocols as __protocols
 import re as __re
 
 def strip_space(text):
     return __re.sub(r'\s+', ' ', text).strip()
 
 def symbol(string):
     temp_symbol = True
@@ -45,7 +46,70 @@
     for char in string:
         if char in __tag_stop:
             break
         
         tag += char
     
     return tag
+
+def protocol(url):
+    for each in __protocols:
+        if url.startswith(each):
+            return each
+        
+    return None
+
+def get_domain(url):
+    url = remove_protocol(url)
+    url = url.split('/')[0]
+
+    return url
+
+def join_path(*args):
+    result = ''
+    
+    for each in args:
+        if result == '':
+            result += each
+        
+        else:
+            if result.endswith('/'):
+                if each.startswith('/'):
+                    result += each.removeprefix('/')
+
+                else:
+                    result += each
+
+            else:
+                if each.startswith('/'):
+                    result += each
+
+                else:
+                    result += '/' + each
+
+    return result
+
+def raw_url(url):
+    return remove_slash(remove_protocol(url))
+
+def remove_protocol(url):
+    return url.removeprefix('http://').removeprefix('https://')
+
+def remove_slash(url):
+    while url.endswith('/'):
+        url = url.removesuffix('/')
+    
+    return url
+
+def back_home(url, response):
+    if remove_slash(url) == remove_slash(response.url):
+        return False
+    
+    path = remove_protocol(response.url)
+    path = remove_slash(path)
+    
+    if not '/' in path:
+        return True
+
+    return False
+
+
```

### Comparing `eyes_soatra-0.0.27/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.28/eyes_soatra/funcs/view_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from eyes_soatra.constant.depends.view.no_data import depends as __depends_no_data
 from eyes_soatra.constant.depends.view.not_found import depends as __depends_404
 from eyes_soatra.constant.user.user_agents import User_Agents as __User_Agents
 from eyes_soatra.constant.libs.requests import requests as __requests
 from eyes_soatra.constant.vars import header_xpaths as __header_xpaths_all
 from eyes_soatra.constant.vars import remove_tags as __remove_tags
 from eyes_soatra.funcs.utils.string import strip_space as __strip_space
+from eyes_soatra.funcs.utils.string import back_home as __back_home
+from eyes_soatra.funcs.utils.string import protocol as __protocol
+from eyes_soatra.funcs.utils.string import join_path as __join_path
+from eyes_soatra.funcs.utils.string import get_domain as __get_domain
+from eyes_soatra.funcs.utils.string import raw_url as __raw_url
 
 from translate import Translator as __Translator
 from lxml import html as __html
 from lxml import etree as __etree
 
 import jellyfish as __jellyfish
 import random as __random
@@ -61,47 +66,47 @@
     separator = __separator + (separator if separator else '')
     
     for xpath in (__header_xpaths_all if allow_all_tags else __header_xpaths) + (header_xpath if type(header_xpath) == list else []):
         element_list = html.xpath(xpath)
         
         for element in element_list:
             header_list = element.xpath('.//text()')
-            
-            for header in header_list:
-                for token in __re.split(separator, header):
+            header = ' '.join(header_list)
+
+            for token in __re.split(separator, header):
                     token = __strip_space(token)
-                    
+
                     if len(token) >= __header_min_length:
                         header_texts.append(token)
-    
+
     for xpath in __paragraph_xpaths + (paragraph_xpath if type(paragraph_xpath) == list else []):
         element_list = html.xpath(xpath)
         
         for element in element_list:
             paragraph_list = element.xpath('.//text()')
-            
-            for paragraph in paragraph_list:
-                for token in __re.split(separator, paragraph):
-                    token = __strip_space(token)
+            paragraph = ' '.join(paragraph_list)
 
-                    if len(token) >= __paragraph_min_length:
-                        paragraph_texts.append(token)
+            for token in __re.split(separator, paragraph):
+                token = __strip_space(token)
+
+                if len(token) >= __paragraph_min_length:
+                    paragraph_texts.append(token)
     
     for xpath in __content_xpaths + (content_xpath if type(content_xpath) == list else []):
         element_list = html.xpath(xpath)
-        
+
         for element in element_list:
             content_list = element.xpath('.//text()')
-            
-            for content in content_list:
-                for token in __re.split(separator, content):
-                    token = __strip_space(token)
-                    
-                    if len(token) >= __content_min_length:
-                        content_texts.append(token)
+            content = ' '.join(content_list)
+
+            for token in __re.split(separator, content):
+                token = __strip_space(token)
+                
+                if len(token) >= __content_min_length:
+                    content_texts.append(token)
             
     return {
         'headers': header_texts,
         'paragraphs': paragraph_texts,
         'contents': content_texts,
     }
 
@@ -131,15 +136,15 @@
     }
 
     if len(headers):
         header_similar = ''
         header_keyword = ''
         
         for depend in __depends_404 + (depends if type(depends) == list else []):
-            for token in headers:                
+            for token in headers:
                 point = __jellyfish.jaro_similarity(depend, token)
                 
                 if point > header_high_point:
                     header_high_point = point
                     header_similar = depend
                     header_keyword = token
                     
@@ -194,35 +199,14 @@
         result = {
             **result,
             'blank': True,
         }
         
     return result
 
-def __remove_protocol(url):
-    return url.removeprefix('http://').removeprefix('https://')
-
-def __remove_slash(url):
-    while url.endswith('/'):
-        url = url.removesuffix('/')
-    
-    return url
-
-def __back_home(url, response: __requests.models.Response):
-    if __remove_slash(url) == __remove_slash(response.url):
-        return False
-    
-    path = __remove_protocol(response.url)
-    path = __remove_slash(path)
-    
-    if not '/' in path:
-        return True
-
-    return False
-
 # ------------------------ public function
 def view_page(
     url,
     lang='ja',
     timeout=15,
     verify=False,
     headers=None,
@@ -244,23 +228,24 @@
     show_header=False,
     show_paragraph=False,
     show_content=False,
     
     **requests_options
 ):
     url = __re.sub(r'\s', '', url)
+    start_url = url
     tried = 0
     agents = []
     redirected_forward = False
     
     while True:
         try:
             tried += 1
             user_agent = __random.choice(__User_Agents)
-            
+
             while user_agent in agents:
                 user_agent = __random.choice(__User_Agents)
                 
             agents.append(user_agent)
             response = __requests.get(
                 **requests_options,
                 url=url,
@@ -273,28 +258,31 @@
                     'ACCEPT' : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
                     'ACCEPT-ENCODING' : 'gzip, deflate, br',
                     'ACCEPT-LANGUAGE' : 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,km-KH;q=0.6,km;q=0.5,ja-JP;q=0.4,ja;q=0.3',
                     'REFERER' : 'https://www.google.com/'
                 },
             )
             status_code = response.status_code
-            redirected = redirected_forward if redirected_forward else response.is_redirect
+            redirected = redirected_forward if redirected_forward else __raw_url(start_url) != __raw_url(response.url)
             expired = response.headers.get('Expires')
             expired = expired if expired else (response.headers.get('expires') or False)
             expired_obj = {'expired': expired} if expired else {}
             current_url = response.url
 
-            back_home = __back_home(url, response)
+            back_home = __back_home(
+                url,
+                response
+            )
 
             if back_home:
                 return {
-                    'active': False,
+                    'active': None,
                     'checked': False,
                     **expired_obj,
-                    'error': f'Redirected to Home Page',
+                    'error': f'Back to Home Page',
                     'redirected': True,
                     'url': current_url,
                     'status': status_code,
                     'tried': tried,
                 }
             
             if status_code >= 400 and status_code <= 499:
@@ -335,15 +323,23 @@
                         if len(content_slices) > 1:
                             url_refresh = __strip_space(content_slices[1])
                             
                             if url_refresh.lower().startswith('url='):
                                 url_refresh = url_refresh[4:]
                                 
                             redirected_forward = True
-                            url = url_refresh
+                            
+                            if __protocol(url_refresh):
+                                url = url_refresh
+
+                            else:
+                                protocol = __protocol(url)
+                                domain = __get_domain(url)
+                                url = __join_path(protocol, domain, url_refresh)
+
                             continue
 
                     else:
                         return {
                             'active': None,
                             'checked': False,
                             'error': f'Out of forwarding tries.',
```

### Comparing `eyes_soatra-0.0.27/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.28/eyes_soatra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/setup.py` & `eyes_soatra-0.0.28/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.27'
+VERSION = '0.0.28'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
@@ -21,15 +21,14 @@
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'requests',
-        'requests_html',
         'lxml',
         'jellyfish',
         'translate',
     ],
     keywords=[
         'python',
         'crawler',
```

### Comparing `eyes_soatra-0.0.27/test/test.py` & `eyes_soatra-0.0.28/test/test.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.27/test/test1.py` & `eyes_soatra-0.0.28/test/test1.py`

 * *Files identical despite different names*

