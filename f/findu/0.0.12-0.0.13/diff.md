# Comparing `tmp/findu-0.0.12.tar.gz` & `tmp/findu-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.12.tar", max compression
+gzip compressed data, was "findu-0.0.13.tar", max compression
```

## Comparing `findu-0.0.12.tar` & `findu-0.0.13.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      112 2023-04-16 06:26:44.829145 findu-0.0.12/findu/__init__.py
--rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.12/findu/__main__.py
--rw-r--r--   0        0        0    32712 2023-06-07 04:19:34.717509 findu-0.0.12/findu/findu.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.12/findu/findu2.py
--rw-r--r--   0        0        0     7211 2023-06-04 14:22:33.985163 findu-0.0.12/findu/jack.txt
--rw-r--r--   0        0        0     1363 2023-06-04 14:06:36.562095 findu-0.0.12/findu/markhoo.txt
--rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.12/findu/notify.py
--rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.12/findu/resources/data.json
--rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.12/findu/result.py
--rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.12/findu/sites.py
--rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.12/findu/tests/__init__.py
--rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.12/findu/tests/all.py
--rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.12/findu/tests/base.py
--rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.12/findu/tests/test_multiple_usernames.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.12/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.12/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.12/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.12/LICENSE
--rw-r--r--   0        0        0     1594 2023-06-07 04:26:11.217366 findu-0.0.12/pyproject.toml
--rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.12/README.md
--rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-06-07 04:32:01.441958 findu-0.0.13/findu/__init__.py
+-rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.13/findu/__main__.py
+-rw-r--r--   0        0        0    32712 2023-06-07 04:19:34.717509 findu-0.0.13/findu/findu.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.13/findu/findu2.py
+-rw-r--r--   0        0        0     7211 2023-06-04 14:22:33.985163 findu-0.0.13/findu/jack.txt
+-rw-r--r--   0        0        0     1363 2023-06-04 14:06:36.562095 findu-0.0.13/findu/markhoo.txt
+-rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.13/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.13/findu/resources/data.json
+-rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.13/findu/result.py
+-rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.13/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.13/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.13/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.13/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.13/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.13/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.13/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.13/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.13/LICENSE
+-rw-r--r--   0        0        0     1594 2023-06-07 04:33:28.965360 findu-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0    10885 2023-06-04 14:32:59.022396 findu-0.0.13/README.md
+-rw-r--r--   0        0        0    12314 1970-01-01 00:00:00.000000 findu-0.0.13/PKG-INFO
```

### Comparing `findu-0.0.12/findu/__main__.py` & `findu-0.0.13/findu/__main__.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/findu.py` & `findu-0.0.13/findu/findu.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/findu2.py` & `findu-0.0.13/findu/findu2.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/jack.txt` & `findu-0.0.13/findu/jack.txt`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/markhoo.txt` & `findu-0.0.13/findu/markhoo.txt`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/notify.py` & `findu-0.0.13/findu/notify.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/resources/data.json` & `findu-0.0.13/findu/resources/data.json`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/result.py` & `findu-0.0.13/findu/result.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/sites.py` & `findu-0.0.13/findu/sites.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/tests/all.py` & `findu-0.0.13/findu/tests/all.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/tests/base.py` & `findu-0.0.13/findu/tests/base.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/findu/tests/test_multiple_usernames.py` & `findu-0.0.13/findu/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/LICENSE` & `findu-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/pyproject.toml` & `findu-0.0.13/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.12"
+version = "0.0.13"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
```

### Comparing `findu-0.0.12/README.md` & `findu-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.12/PKG-INFO` & `findu-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.12
+Version: 0.0.13
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

