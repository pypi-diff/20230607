# Comparing `tmp/findu-0.0.10.tar.gz` & `tmp/findu-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.10.tar", max compression
+gzip compressed data, was "findu-0.0.11.tar", max compression
```

## Comparing `findu-0.0.10.tar` & `findu-0.0.11.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      112 2023-04-16 06:26:44.829145 findu-0.0.10/findu/__init__.py
--rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.10/findu/__main__.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.10/findu/findu.py
--rw-r--r--   0        0        0     7211 2023-06-04 14:22:33.985163 findu-0.0.10/findu/jack.txt
--rw-r--r--   0        0        0     1363 2023-06-04 14:06:36.562095 findu-0.0.10/findu/markhoo.txt
--rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.10/findu/notify.py
--rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.10/findu/resources/data.json
--rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.10/findu/result.py
--rw-r--r--   0        0        0    32714 2023-04-16 06:26:44.833138 findu-0.0.10/findu/sherlock.py
--rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.10/findu/sites.py
--rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.10/findu/tests/__init__.py
--rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.10/findu/tests/all.py
--rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.10/findu/tests/base.py
--rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.10/findu/tests/test_multiple_usernames.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.10/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.10/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.10/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.10/LICENSE
--rw-r--r--   0        0        0     1546 2023-06-04 15:05:05.846709 findu-0.0.10/pyproject.toml
--rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.10/README.md
--rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-04-16 06:26:44.829145 findu-0.0.11/findu/__init__.py
+-rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.11/findu/__main__.py
+-rw-r--r--   0        0        0    32712 2023-06-07 04:19:34.717509 findu-0.0.11/findu/findu.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.11/findu/findu2.py
+-rw-r--r--   0        0        0     7211 2023-06-04 14:22:33.985163 findu-0.0.11/findu/jack.txt
+-rw-r--r--   0        0        0     1363 2023-06-04 14:06:36.562095 findu-0.0.11/findu/markhoo.txt
+-rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.11/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.11/findu/resources/data.json
+-rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.11/findu/result.py
+-rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.11/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.11/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.11/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.11/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.11/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.11/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.11/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.11/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.11/LICENSE
+-rw-r--r--   0        0        0     1593 2023-06-07 04:18:31.202887 findu-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.11/README.md
+-rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.11/PKG-INFO
```

### Comparing `findu-0.0.10/findu/__main__.py` & `findu-0.0.11/findu/__main__.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/findu.py` & `findu-0.0.11/findu/findu2.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/jack.txt` & `findu-0.0.11/findu/jack.txt`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/markhoo.txt` & `findu-0.0.11/findu/markhoo.txt`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/notify.py` & `findu-0.0.11/findu/notify.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/resources/data.json` & `findu-0.0.11/findu/resources/data.json`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/result.py` & `findu-0.0.11/findu/result.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/sherlock.py` & `findu-0.0.11/findu/findu.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from torrequest import TorRequest
 from result import QueryStatus
 from result import QueryResult
 from notify import QueryNotifyPrint
 from sites import SitesInformation
 from colorama import init
 
-module_name = "Sherlock: Find Usernames Across Social Networks"
-__version__ = "0.14.3"
+module_name = "Find U: Find Usernames Across Social Networks"
+__version__ = "0.0.11"
 
 
 class SherlockFuturesSession(FuturesSession):
     def request(self, method, url, hooks=None, *args, **kwargs):
         """Request URL.
 
         This extends the FuturesSession request method to calculate a response
```

### Comparing `findu-0.0.10/findu/sites.py` & `findu-0.0.11/findu/sites.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/tests/all.py` & `findu-0.0.11/findu/tests/all.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/tests/base.py` & `findu-0.0.11/findu/tests/base.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/findu/tests/test_multiple_usernames.py` & `findu-0.0.11/findu/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/LICENSE` & `findu-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/pyproject.toml` & `findu-0.0.11/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.10"
+version = "0.0.11"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
@@ -42,10 +42,13 @@
 requests-futures = "^1.0.0"
 stem = "^1.8.0"
 torrequest = "^0.1.0"
 pandas = "^2.0.0"
 openpyxl = "^3.0.10"
 exrex = "^0.11.0"
 
+[tool.poetry.scripts]
+findu = "findu:main"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findu-0.0.10/README.md` & `findu-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.10/PKG-INFO` & `findu-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.10
+Version: 0.0.11
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

