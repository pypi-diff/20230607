# Comparing `tmp/findu-0.0.17.tar.gz` & `tmp/findu-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.17.tar", max compression
+gzip compressed data, was "findu-0.0.18.tar", max compression
```

## Comparing `findu-0.0.17.tar` & `findu-0.0.18.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      551 2023-06-07 05:04:50.571497 findu-0.0.17/findu/__init__.py
--rw-r--r--   0        0        0      624 2023-06-07 05:05:57.934455 findu-0.0.17/findu/__main__.py
--rw-r--r--   0        0        0    32739 2023-06-07 04:55:06.206294 findu-0.0.17/findu/findu.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.17/findu/findu2.py
--rw-r--r--   0        0        0     8895 2023-06-07 04:54:06.964355 findu-0.0.17/findu/notify.py
--rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.17/findu/resources/data.json
--rw-r--r--   0        0        0     3203 2023-06-07 04:54:23.272209 findu-0.0.17/findu/result.py
--rw-r--r--   0        0        0     9244 2023-06-07 04:54:40.419398 findu-0.0.17/findu/sites.py
--rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.17/findu/tests/__init__.py
--rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.17/findu/tests/all.py
--rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.17/findu/tests/base.py
--rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.17/findu/tests/test_multiple_usernames.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.17/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.17/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.17/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.17/LICENSE
--rw-r--r--   0        0        0     1594 2023-06-07 05:05:24.200619 findu-0.0.17/pyproject.toml
--rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.17/README.md
--rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      485 2023-06-07 05:08:25.109166 findu-0.0.18/findu/__init__.py
+-rw-r--r--   0        0        0      624 2023-06-07 05:05:57.934455 findu-0.0.18/findu/__main__.py
+-rw-r--r--   0        0        0    32739 2023-06-07 04:55:06.206294 findu-0.0.18/findu/findu.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.18/findu/findu2.py
+-rw-r--r--   0        0        0     8895 2023-06-07 04:54:06.964355 findu-0.0.18/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.18/findu/resources/data.json
+-rw-r--r--   0        0        0     3203 2023-06-07 04:54:23.272209 findu-0.0.18/findu/result.py
+-rw-r--r--   0        0        0     9244 2023-06-07 04:54:40.419398 findu-0.0.18/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.18/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.18/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.18/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.18/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.18/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.18/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.18/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.18/LICENSE
+-rw-r--r--   0        0        0     1594 2023-06-07 05:08:43.125243 findu-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.18/README.md
+-rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.18/PKG-INFO
```

### Comparing `findu-0.0.17/findu/__main__.py` & `findu-0.0.18/findu/__main__.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/findu.py` & `findu-0.0.18/findu/findu.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/findu2.py` & `findu-0.0.18/findu/findu2.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/notify.py` & `findu-0.0.18/findu/notify.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/resources/data.json` & `findu-0.0.18/findu/resources/data.json`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/result.py` & `findu-0.0.18/findu/result.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/sites.py` & `findu-0.0.18/findu/sites.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/tests/all.py` & `findu-0.0.18/findu/tests/all.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/tests/base.py` & `findu-0.0.18/findu/tests/base.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/findu/tests/test_multiple_usernames.py` & `findu-0.0.18/findu/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/LICENSE` & `findu-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/pyproject.toml` & `findu-0.0.18/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.17"
+version = "0.0.18"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
```

### Comparing `findu-0.0.17/README.md` & `findu-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.17/PKG-INFO` & `findu-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.17
+Version: 0.0.18
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

