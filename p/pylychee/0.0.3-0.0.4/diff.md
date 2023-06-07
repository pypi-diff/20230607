# Comparing `tmp/pylychee-0.0.3.tar.gz` & `tmp/pylychee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylychee-0.0.3.tar", last modified: Mon Jun  5 05:46:23 2023, max compression
+gzip compressed data, was "pylychee-0.0.4.tar", last modified: Wed Jun  7 03:19:01 2023, max compression
```

## Comparing `pylychee-0.0.3.tar` & `pylychee-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.801484 pylychee-0.0.3/
--rw-r--r--   0 chenhaiou   (501) staff       (20)     1062 2023-06-05 02:15:54.000000 pylychee-0.0.3/LICENSE
--rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 05:46:23.800882 pylychee-0.0.3/PKG-INFO
--rw-r--r--   0 chenhaiou   (501) staff       (20)      140 2023-06-05 02:15:54.000000 pylychee-0.0.3/README.md
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.796206 pylychee-0.0.3/pylychee/
--rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.3/pylychee/__init__.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.798106 pylychee-0.0.3/pylychee/apps/
--rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.3/pylychee/apps/__init__.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.799421 pylychee-0.0.3/pylychee/apps/feishu/
--rw-r--r--   0 chenhaiou   (501) staff       (20)     1013 2023-06-05 04:31:42.000000 pylychee-0.0.3/pylychee/apps/feishu/__init__.py
--rw-r--r--   0 chenhaiou   (501) staff       (20)     1070 2023-06-05 03:34:28.000000 pylychee-0.0.3/pylychee/apps/feishu/messages.py
-drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-05 05:46:23.797703 pylychee-0.0.3/pylychee.egg-info/
--rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/PKG-INFO
--rw-r--r--   0 chenhaiou   (501) staff       (20)      273 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/SOURCES.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)        1 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/dependency_links.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)        9 2023-06-05 05:46:23.000000 pylychee-0.0.3/pylychee.egg-info/top_level.txt
--rw-r--r--   0 chenhaiou   (501) staff       (20)      572 2023-06-05 05:46:12.000000 pylychee-0.0.3/pyproject.toml
--rw-r--r--   0 chenhaiou   (501) staff       (20)       38 2023-06-05 05:46:23.801607 pylychee-0.0.3/setup.cfg
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-07 03:19:01.752126 pylychee-0.0.4/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1062 2023-06-05 02:15:54.000000 pylychee-0.0.4/LICENSE
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-07 03:19:01.751759 pylychee-0.0.4/PKG-INFO
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      140 2023-06-05 02:15:54.000000 pylychee-0.0.4/README.md
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-07 03:19:01.748086 pylychee-0.0.4/pylychee/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        0 2023-06-05 02:15:54.000000 pylychee-0.0.4/pylychee/__init__.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-07 03:19:01.749397 pylychee-0.0.4/pylychee/apps/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)       50 2023-06-07 03:10:45.000000 pylychee-0.0.4/pylychee/apps/__init__.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-07 03:19:01.750904 pylychee-0.0.4/pylychee/apps/feishu/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1013 2023-06-05 04:31:42.000000 pylychee-0.0.4/pylychee/apps/feishu/__init__.py
+-rw-r--r--   0 chenhaiou   (501) staff       (20)     1033 2023-06-07 03:08:15.000000 pylychee-0.0.4/pylychee/apps/feishu/messages.py
+drwxr-xr-x   0 chenhaiou   (501) staff       (20)        0 2023-06-07 03:19:01.749162 pylychee-0.0.4/pylychee.egg-info/
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      618 2023-06-07 03:19:01.000000 pylychee-0.0.4/pylychee.egg-info/PKG-INFO
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      273 2023-06-07 03:19:01.000000 pylychee-0.0.4/pylychee.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        1 2023-06-07 03:19:01.000000 pylychee-0.0.4/pylychee.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)        9 2023-06-07 03:19:01.000000 pylychee-0.0.4/pylychee.egg-info/top_level.txt
+-rw-r--r--   0 chenhaiou   (501) staff       (20)      572 2023-06-07 03:10:45.000000 pylychee-0.0.4/pyproject.toml
+-rw-r--r--   0 chenhaiou   (501) staff       (20)       38 2023-06-07 03:19:01.752235 pylychee-0.0.4/setup.cfg
```

### Comparing `pylychee-0.0.3/LICENSE` & `pylychee-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylychee-0.0.3/PKG-INFO` & `pylychee-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylychee
-Version: 0.0.3
+Version: 0.0.4
 Summary: SDK合集
 Author-email: chenhaiou <haiou_chen@sina.cn>
 Project-URL: Homepage, https://github.com/MrLawes/pylychee
 Project-URL: Bug Tracker, https://github.com/MrLawes/lychee/pylychee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylychee-0.0.3/pylychee/apps/feishu/__init__.py` & `pylychee-0.0.4/pylychee/apps/feishu/__init__.py`

 * *Files identical despite different names*

### Comparing `pylychee-0.0.3/pylychee/apps/feishu/messages.py` & `pylychee-0.0.4/pylychee/apps/feishu/messages.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import uuid
 
 import requests
 
 from pylychee.apps.feishu import AccessToken
 
-# todo testcases
-# todo 帮助文档
 
 class Messages:
     """ 消息管理 """
 
     def send(self, text, receive_ids=[], ):
         """ 发送消息。文档地址:https://open.feishu.cn/document/uAjLw4CM/ukTMukTMukTM/reference/im-v1/message/create
             @参数:receive_id:            消息接收者的ID
```

### Comparing `pylychee-0.0.3/pylychee.egg-info/PKG-INFO` & `pylychee-0.0.4/pylychee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylychee
-Version: 0.0.3
+Version: 0.0.4
 Summary: SDK合集
 Author-email: chenhaiou <haiou_chen@sina.cn>
 Project-URL: Homepage, https://github.com/MrLawes/pylychee
 Project-URL: Bug Tracker, https://github.com/MrLawes/lychee/pylychee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylychee-0.0.3/pyproject.toml` & `pylychee-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "pylychee"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="chenhaiou", email="haiou_chen@sina.cn" },
 ]
 description = "SDK合集"
 readme = "README.md"
 requires-python = ">=3.8.9"
 classifiers = [
```

