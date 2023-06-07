# Comparing `tmp/smartapp_sdk-0.6.0.tar.gz` & `tmp/smartapp_sdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartapp_sdk-0.6.0.tar", max compression
+gzip compressed data, was "smartapp_sdk-0.6.1.tar", max compression
```

## Comparing `smartapp_sdk-0.6.0.tar` & `smartapp_sdk-0.6.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1747 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/Changelog
--rw-r--r--   0        0        0    11324 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/LICENSE
--rw-r--r--   0        0        0      761 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/NOTICE
--rw-r--r--   0        0        0     2167 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/PyPI.md
--rw-r--r--   0        0        0     2366 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/README.md
--rw-r--r--   0        0        0       22 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/Makefile
--rw-r--r--   0        0        0      120 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/README.md
--rw-r--r--   0        0        0      130 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13018 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     9479 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/index.rst
--rw-r--r--   0        0        0     6709 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/make.bat
--rw-r--r--   0        0        0     2783 2023-04-09 19:23:11.772697 smartapp_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/__init__.py
--rw-r--r--   0        0        0     6888 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/converter.py
--rw-r--r--   0        0        0     7781 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/dispatcher.py
--rw-r--r--   0        0        0    35006 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/interface.py
--rw-r--r--   0        0        0       60 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/py.typed
--rw-r--r--   0        0        0     9893 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/signature.py
--rw-r--r--   0        0        0       29 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      213 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/live/README.md
--rw-r--r--   0        0        0     2885 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/live/request/INSTALL.1.json
--rw-r--r--   0        0        0     1011 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/README.md
--rw-r--r--   0        0        0      813 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json
--rw-r--r--   0        0        0      457 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIGURATION-PAGE.json
--rw-r--r--   0        0        0      381 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIRMATION.json
--rw-r--r--   0        0        0     1793 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-DEVICE.json
--rw-r--r--   0        0        0     1567 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-TIMER.json
--rw-r--r--   0        0        0     1327 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/INSTALL.json
--rw-r--r--   0        0        0      218 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/OAUTH_CALLBACK.json
--rw-r--r--   0        0        0     1255 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/UNINSTALL.json
--rw-r--r--   0        0        0     2152 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/UPDATE.json
--rw-r--r--   0        0        0      249 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-INITIALIZE.json
--rw-r--r--   0        0        0      742 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json
--rw-r--r--   0        0        0     1251 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json
--rw-r--r--   0        0        0       33 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIRMATION.json
--rw-r--r--   0        0        0       21 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/EVENT.json
--rw-r--r--   0        0        0       23 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/INSTALL.json
--rw-r--r--   0        0        0       29 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/OAUTH_CALLBACK.json
--rw-r--r--   0        0        0       25 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/UNINSTALL.json
--rw-r--r--   0        0        0       22 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/UPDATE.json
--rw-r--r--   0        0        0      156 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/BOOLEAN.json
--rw-r--r--   0        0        0      117 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/DECIMAL.json
--rw-r--r--   0        0        0      231 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/DEVICE.json
--rw-r--r--   0        0        0      114 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/EMAIL.json
--rw-r--r--   0        0        0      700 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ENUM-GROUP.json
--rw-r--r--   0        0        0      292 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ENUM.json
--rw-r--r--   0        0        0      152 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ICON.json
--rw-r--r--   0        0        0      146 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/IMAGE.json
--rw-r--r--   0        0        0      187 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/LINK.json
--rw-r--r--   0        0        0      108 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/NUMBER.json
--rw-r--r--   0        0        0      291 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/OAUTH.json
--rw-r--r--   0        0        0      167 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/PAGE.json
--rw-r--r--   0        0        0      185 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/PARAGRAPH.json
--rw-r--r--   0        0        0      112 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/PHONE.json
--rw-r--r--   0        0        0      165 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/TEXT.json
--rw-r--r--   0        0        0      101 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/TIME.json
--rw-r--r--   0        0        0    38670 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_converter.py
--rw-r--r--   0        0        0    14130 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_dispatcher.py
--rw-r--r--   0        0        0     7893 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_interface.py
--rw-r--r--   0        0        0    25529 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_signature.py
--rw-r--r--   0        0        0      549 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/testutil.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.0/setup.py
--rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1877 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/Changelog
+-rw-r--r--   0        0        0    11324 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/LICENSE
+-rw-r--r--   0        0        0      761 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/NOTICE
+-rw-r--r--   0        0        0     2167 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/PyPI.md
+-rw-r--r--   0        0        0     2366 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13018 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/conf.py
+-rw-r--r--   0        0        0     9479 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/index.rst
+-rw-r--r--   0        0        0     6709 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/make.bat
+-rw-r--r--   0        0        0     2781 2023-06-07 01:05:08.287151 smartapp_sdk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/__init__.py
+-rw-r--r--   0        0        0     6872 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/converter.py
+-rw-r--r--   0        0        0     7781 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/dispatcher.py
+-rw-r--r--   0        0        0    35006 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/interface.py
+-rw-r--r--   0        0        0       60 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/py.typed
+-rw-r--r--   0        0        0     9939 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/src/smartapp/signature.py
+-rw-r--r--   0        0        0       29 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/live/README.md
+-rw-r--r--   0        0        0     2885 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/live/request/INSTALL.1.json
+-rw-r--r--   0        0        0     1011 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/README.md
+-rw-r--r--   0        0        0      813 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json
+-rw-r--r--   0        0        0      457 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIGURATION-PAGE.json
+-rw-r--r--   0        0        0      381 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIRMATION.json
+-rw-r--r--   0        0        0     1793 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-DEVICE.json
+-rw-r--r--   0        0        0     1567 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-TIMER.json
+-rw-r--r--   0        0        0     1327 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/INSTALL.json
+-rw-r--r--   0        0        0      218 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/OAUTH_CALLBACK.json
+-rw-r--r--   0        0        0     1255 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/UNINSTALL.json
+-rw-r--r--   0        0        0     2152 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/UPDATE.json
+-rw-r--r--   0        0        0      249 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-INITIALIZE.json
+-rw-r--r--   0        0        0      742 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json
+-rw-r--r--   0        0        0     1251 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json
+-rw-r--r--   0        0        0       33 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIRMATION.json
+-rw-r--r--   0        0        0       21 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/EVENT.json
+-rw-r--r--   0        0        0       23 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/INSTALL.json
+-rw-r--r--   0        0        0       29 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/OAUTH_CALLBACK.json
+-rw-r--r--   0        0        0       25 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/UNINSTALL.json
+-rw-r--r--   0        0        0       22 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/UPDATE.json
+-rw-r--r--   0        0        0      156 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/BOOLEAN.json
+-rw-r--r--   0        0        0      117 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/DECIMAL.json
+-rw-r--r--   0        0        0      231 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/DEVICE.json
+-rw-r--r--   0        0        0      114 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/EMAIL.json
+-rw-r--r--   0        0        0      700 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ENUM-GROUP.json
+-rw-r--r--   0        0        0      292 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ENUM.json
+-rw-r--r--   0        0        0      152 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ICON.json
+-rw-r--r--   0        0        0      146 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/IMAGE.json
+-rw-r--r--   0        0        0      187 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/LINK.json
+-rw-r--r--   0        0        0      108 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/NUMBER.json
+-rw-r--r--   0        0        0      291 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/OAUTH.json
+-rw-r--r--   0        0        0      167 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/PAGE.json
+-rw-r--r--   0        0        0      185 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/PARAGRAPH.json
+-rw-r--r--   0        0        0      112 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/PHONE.json
+-rw-r--r--   0        0        0      165 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/TEXT.json
+-rw-r--r--   0        0        0      101 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/TIME.json
+-rw-r--r--   0        0        0    38670 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_converter.py
+-rw-r--r--   0        0        0    14130 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_dispatcher.py
+-rw-r--r--   0        0        0     7893 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_interface.py
+-rw-r--r--   0        0        0    25529 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_signature.py
+-rw-r--r--   0        0        0      549 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/testutil.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.1/setup.py
+-rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.1/PKG-INFO
```

### Comparing `smartapp_sdk-0.6.0/Changelog` & `smartapp_sdk-0.6.1/Changelog`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 0.6.1     06 Jun 2023
+
+	* Fix checktabs to be safe for file named '-'.
+	* Update requests dependency for CVE-2023-32681.
+
 Version 0.6.0     09 Apr 2023
 
 	* Add new SubscriptionType enumeration.
 	* Rewrite request-related tests to use the responses framework.
 
 Version 0.5.4     26 Feb 2023
```

### Comparing `smartapp_sdk-0.6.0/LICENSE` & `smartapp_sdk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/NOTICE` & `smartapp_sdk-0.6.1/NOTICE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/PyPI.md` & `smartapp_sdk-0.6.1/PyPI.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/README.md` & `smartapp_sdk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/docs/Makefile` & `smartapp_sdk-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/docs/_themes/LICENSE` & `smartapp_sdk-0.6.1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/docs/_themes/flask_theme_support.py` & `smartapp_sdk-0.6.1/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/docs/conf.py` & `smartapp_sdk-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/docs/index.rst` & `smartapp_sdk-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/docs/make.bat` & `smartapp_sdk-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/pyproject.toml` & `smartapp_sdk-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartapp-sdk"
-version = "0.6.0" # published version is managed using Git tags (see below)
+version = "0.6.1" # published version is managed using Git tags (see below)
 description = "Framework to build a webhook-based SmartThings SmartApp"
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/smartapp-sdk/"
 repository = "https://github.com/pronovic/smartapp-sdk"
 include = [
@@ -41,15 +41,15 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 pendulum = "^2.1.2"
 attrs = "^22.2.0"
 cattrs = "^22.2.0"
 PyYAML = "^6.0"
 pycryptodomex = "^3.17"
-requests = "^2.28.2"
+requests = "^2.31.0"
 tenacity = "^8.2.1"
 importlib-metadata = { version="^6.0.0", optional=true }
 sphinx = { version="^6.1.3", optional=true }
 sphinx-autoapi = { version="^2.0.1", optional=true }
 
 [tool.poetry.extras]
 docs = [ "importlib-metadata", "sphinx", "sphinx-autoapi" ]
@@ -61,15 +61,15 @@
 pylint = "^2.16.2"
 pre-commit = "^3.1.0"
 black = "^23.1.0"
 mypy = "^1.0.1"
 isort = "^5.12.0"
 coveralls = "^3.3.1"
 types-PyYAML = "^6.0.12.8"
-types-requests = "^2.28.11.15"
+types-requests = "^2.31.0.1"
 colorama = "~0, >=0.4.6"
 responses = "~0, >=0.22.0"
 
 [tool.black]
 line-length = 132
 target-version = ['py39', 'py310', 'py311' ]
 include = '(src\/scripts\/.*$|\.pyi?$)'
```

### Comparing `smartapp_sdk-0.6.0/src/smartapp/converter.py` & `smartapp_sdk-0.6.1/src/smartapp/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def from_json(self, data: str, cls: Type[T]) -> T:
         """Deserialize an object from JSON."""
         return self.structure(json.loads(data), cls)
 
     def to_yaml(self, obj: Any) -> str:
         """Serialize an object to YAML."""
-        return yaml.safe_dump(self.unstructure(obj), sort_keys=False)  # type: ignore
+        return yaml.safe_dump(self.unstructure(obj), sort_keys=False)
 
     def from_yaml(self, data: str, cls: Type[T]) -> T:
         """Deserialize an object from YAML."""
         return self.structure(yaml.safe_load(data), cls)
 
     def _to_camel_case(self, name: str) -> str:
         """Convert a snake_case attribute name to camelCase instead."""
```

### Comparing `smartapp_sdk-0.6.0/src/smartapp/dispatcher.py` & `smartapp_sdk-0.6.1/src/smartapp/dispatcher.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/src/smartapp/interface.py` & `smartapp_sdk-0.6.1/src/smartapp/interface.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/src/smartapp/signature.py` & `smartapp_sdk-0.6.1/src/smartapp/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 # vim: set ft=python ts=4 sw=4 expandtab:
+# pylint: disable=too-many-instance-attributes:
 
 """
 Verify HTTP signatures on SmartApp lifecycle event requests.
 """
 
 # This implements HTTP signature verification for the SmartApp lifecycle events.
 # See: https://developer-preview.smartthings.com/docs/connected-services/hosting/webhook-smartapp/
 #
-# SmartThings uses Joyent's HTTP signature scheme to signal all lifecycle events.
+# SmartThings uses Joyent's HTTP signature scheme to sign all lifecycle events.
 # See: https://github.com/TritonDataCenter/node-http-signature/blob/master/http_signing.md
 #
 # Note that only the rsa-sha256 algorithm is supported in this code.  As far as I can
 # tell, this is the only one SmartThings uses.  Limiting to the single algorithm greatly
 # simplifies the implementation, plus we can use the test cases that Joylent includes in
 # their specification document in our own unit tests.
 #
```

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/live/request/INSTALL.1.json` & `smartapp_sdk-0.6.1/tests/fixtures/live/request/INSTALL.1.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/README.md` & `smartapp_sdk-0.6.1/tests/fixtures/samples/README.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-DEVICE.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-DEVICE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-TIMER.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-TIMER.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/request/INSTALL.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/request/INSTALL.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/request/UNINSTALL.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/request/UNINSTALL.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/request/UPDATE.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/request/UPDATE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ENUM-GROUP.json` & `smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ENUM-GROUP.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/test_converter.py` & `smartapp_sdk-0.6.1/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/test_dispatcher.py` & `smartapp_sdk-0.6.1/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/test_interface.py` & `smartapp_sdk-0.6.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/test_signature.py` & `smartapp_sdk-0.6.1/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/tests/testutil.py` & `smartapp_sdk-0.6.1/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.0/setup.py` & `smartapp_sdk-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'attrs>=22.2.0,<23.0.0',
  'cattrs>=22.2.0,<23.0.0',
  'pendulum>=2.1.2,<3.0.0',
  'pycryptodomex>=3.17,<4.0',
- 'requests>=2.28.2,<3.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'tenacity>=8.2.1,<9.0.0']
 
 extras_require = \
 {'docs': ['importlib-metadata>=6.0.0,<7.0.0',
           'sphinx>=6.1.3,<7.0.0',
           'sphinx-autoapi>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'smartapp-sdk',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Framework to build a webhook-based SmartThings SmartApp',
     'long_description': "# SmartApp SDK\n\n[![pypi](https://img.shields.io/pypi/v/smartapp-sdk.svg)](https://pypi.org/project/smartapp-sdk/)\n[![license](https://img.shields.io/pypi/l/smartapp-sdk.svg)](https://github.com/pronovic/smartapp-sdk/blob/master/LICENSE)\n[![wheel](https://img.shields.io/pypi/wheel/smartapp-sdk.svg)](https://pypi.org/project/smartapp-sdk/)\n[![python](https://img.shields.io/pypi/pyversions/smartapp-sdk.svg)](https://pypi.org/project/smartapp-sdk/)\n[![Test Suite](https://github.com/pronovic/smartapp-sdk/workflows/Test%20Suite/badge.svg)](https://github.com/pronovic/smartapp-sdk/actions?query=workflow%3A%22Test+Suite%22)\n[![docs](https://readthedocs.org/projects/smartapp-sdk/badge/?version=stable&style=flat)](https://smartapp-sdk.readthedocs.io/en/stable/)\n[![coverage](https://coveralls.io/repos/github/pronovic/smartapp-sdk/badge.svg?branch=master)](https://coveralls.io/github/pronovic/smartapp-sdk?branch=master)\n\nsmartapp-sdk is a Python library to build a [webhook-based SmartApp](https://developer-preview.smartthings.com/docs/connected-services/smartapp-basics/) for the [SmartThings platform](https://www.smartthings.com/).\n\nThe SDK is intended to be easy to use no matter how you choose to structure your code, whether that's a traditional Python webapp (such as FastAPI on Uvicorn) or a serverless application (such as AWS Lambda).\n\nThe SDK handles all the mechanics of the [webhook lifecycle interface](https://developer-preview.smartthings.com/docs/connected-services/lifecycles/) on your behalf.  You just implement a single endpoint to accept the SmartApp webhook requests, and a single callback class where you define specialized behavior for the webhook events.  A clean [attrs](https://www.attrs.org/en/stable/) object interface is exposed for use by your callback.\n\nSDK documentation is found at [smartapp-sdk.readthedocs.io](https://smartapp-sdk.readthedocs.io/en/stable/).  Look there for installation instructions, the class model documentation, and example code. The [smartapp-sensortrack](https://github.com/pronovic/smartapp-sensortrack) repo on GitHub is also a good example of how to use this SDK to build a traditional Python webapp.\n",
     'author': 'Kenneth J. Pronovici',
     'author_email': 'pronovic@ieee.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/smartapp-sdk/',
```

### Comparing `smartapp_sdk-0.6.0/PKG-INFO` & `smartapp_sdk-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartapp-sdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Framework to build a webhook-based SmartThings SmartApp
 Home-page: https://pypi.org/project/smartapp-sdk/
 License: Apache-2.0
 Author: Kenneth J. Pronovici
 Author-email: pronovic@ieee.org
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Provides-Extra: docs
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0) ; extra == "docs"
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pycryptodomex (>=3.17,<4.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: sphinx-autoapi (>=2.0.1,<3.0.0) ; extra == "docs"
 Requires-Dist: tenacity (>=8.2.1,<9.0.0)
 Project-URL: Repository, https://github.com/pronovic/smartapp-sdk
 Description-Content-Type: text/markdown
 
 # SmartApp SDK
```

