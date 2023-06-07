# Comparing `tmp/findu-0.0.15.tar.gz` & `tmp/findu-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.15.tar", max compression
+gzip compressed data, was "findu-0.0.16.tar", max compression
```

## Comparing `findu-0.0.15.tar` & `findu-0.0.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      523 2023-06-07 04:57:10.546541 findu-0.0.15/findu/__init__.py
--rw-r--r--   0        0        0      596 2023-06-07 04:38:01.851778 findu-0.0.15/findu/__main__.py
--rw-r--r--   0        0        0    32739 2023-06-07 04:55:06.206294 findu-0.0.15/findu/findu.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.15/findu/findu2.py
--rw-r--r--   0        0        0     8895 2023-06-07 04:54:06.964355 findu-0.0.15/findu/notify.py
--rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.15/findu/resources/data.json
--rw-r--r--   0        0        0     3203 2023-06-07 04:54:23.272209 findu-0.0.15/findu/result.py
--rw-r--r--   0        0        0     9244 2023-06-07 04:54:40.419398 findu-0.0.15/findu/sites.py
--rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.15/findu/tests/__init__.py
--rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.15/findu/tests/all.py
--rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.15/findu/tests/base.py
--rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.15/findu/tests/test_multiple_usernames.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.15/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.15/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.15/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.15/LICENSE
--rw-r--r--   0        0        0     1594 2023-06-07 04:57:52.634048 findu-0.0.15/pyproject.toml
--rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.15/README.md
--rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0      523 2023-06-07 04:57:10.546541 findu-0.0.16/findu/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-07 04:38:01.851778 findu-0.0.16/findu/__main__.py
+-rw-r--r--   0        0        0    32739 2023-06-07 04:55:06.206294 findu-0.0.16/findu/findu.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.16/findu/findu2.py
+-rw-r--r--   0        0        0     8895 2023-06-07 04:54:06.964355 findu-0.0.16/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.16/findu/resources/data.json
+-rw-r--r--   0        0        0     3203 2023-06-07 04:54:23.272209 findu-0.0.16/findu/result.py
+-rw-r--r--   0        0        0     9244 2023-06-07 04:54:40.419398 findu-0.0.16/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.16/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.16/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.16/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.16/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.16/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.16/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.16/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.16/LICENSE
+-rw-r--r--   0        0        0     1593 2023-06-07 04:59:43.715899 findu-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.16/README.md
+-rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.16/PKG-INFO
```

### Comparing `findu-0.0.15/findu/__init__.py` & `findu-0.0.16/findu/__init__.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/__main__.py` & `findu-0.0.16/findu/__main__.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/findu.py` & `findu-0.0.16/findu/findu.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/findu2.py` & `findu-0.0.16/findu/findu2.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/notify.py` & `findu-0.0.16/findu/notify.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/resources/data.json` & `findu-0.0.16/findu/resources/data.json`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/result.py` & `findu-0.0.16/findu/result.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/sites.py` & `findu-0.0.16/findu/sites.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/tests/all.py` & `findu-0.0.16/findu/tests/all.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/tests/base.py` & `findu-0.0.16/findu/tests/base.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/findu/tests/test_multiple_usernames.py` & `findu-0.0.16/findu/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/LICENSE` & `findu-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/pyproject.toml` & `findu-0.0.16/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.15"
+version = "0.0.16"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
@@ -43,12 +43,12 @@
 stem = "^1.8.0"
 torrequest = "^0.1.0"
 pandas = "^2.0.0"
 openpyxl = "^3.0.10"
 exrex = "^0.11.0"
 
 [tool.poetry.scripts]
-findu = "findu:findu"
+findu = "findu:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findu-0.0.15/README.md` & `findu-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.15/PKG-INFO` & `findu-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.15
+Version: 0.0.16
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

