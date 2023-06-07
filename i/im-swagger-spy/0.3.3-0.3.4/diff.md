# Comparing `tmp/im_swagger_spy-0.3.3.tar.gz` & `tmp/im_swagger_spy-0.3.4.tar.gz`

## Comparing `im_swagger_spy-0.3.3.tar` & `im_swagger_spy-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/conftest.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/pytest.ini
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/requirements.txt
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/example/basic/example.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/example/pytest_example/conftest.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/example/pytest_example/pytest.ini
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/example/pytest_example/tests/test_request.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/__init__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/__main__.py
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/base.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/file_spy.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/http_spy.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/plugin.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/syncdb.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/template.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/im_swagger_spy/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/.gitignore
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/README.md
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/conftest.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/pytest.ini
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/requirements.txt
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/basic/example.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/pytest_example/conftest.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/pytest_example/pytest.ini
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/pytest_example/tests/test_request.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/__init__.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/__main__.py
+-rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/base.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/file_spy.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/http_spy.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/plugin.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/syncdb.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/template.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/README.md
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/PKG-INFO
```

### Comparing `im_swagger_spy-0.3.3/conftest.py` & `im_swagger_spy-0.3.4/conftest.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/setup.py` & `im_swagger_spy-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/.github/workflows/python-publish.yml` & `im_swagger_spy-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/example/basic/example.py` & `im_swagger_spy-0.3.4/example/basic/example.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/im_swagger_spy/base.py` & `im_swagger_spy-0.3.4/im_swagger_spy/base.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/im_swagger_spy/file_spy.py` & `im_swagger_spy-0.3.4/im_swagger_spy/file_spy.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/im_swagger_spy/http_spy.py` & `im_swagger_spy-0.3.4/im_swagger_spy/http_spy.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/im_swagger_spy/plugin.py` & `im_swagger_spy-0.3.4/im_swagger_spy/plugin.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/im_swagger_spy/syncdb.py` & `im_swagger_spy-0.3.4/im_swagger_spy/syncdb.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/im_swagger_spy/template.html` & `im_swagger_spy-0.3.4/im_swagger_spy/template.html`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/README.md` & `im_swagger_spy-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.3/pyproject.toml` & `im_swagger_spy-0.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -36,18 +36,17 @@
     "PyYAML>=6.0",
     "requests>=2.26.0"
 ]
 
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://lancetnik.github.io/Propan/"
-Documentation = "https://lancetnik.github.io/Propan/"
-Tracker = "https://github.com/Lancetnik/Propan/issues"
-Source = "https://github.com/Lancetnik/Propan"
+Homepage = "https://github.com/dasshit/im-swagger-spy"
+Tracker = "https://github.com/dasshit/im-swagger-spy/issues"
+Source = "https://github.com/dasshit/im-swagger-spy"
 
 [project.scripts]
 im_swagger_spy = "im_swagger_spy.__main__:cli"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
```

### Comparing `im_swagger_spy-0.3.3/PKG-INFO` & `im_swagger_spy-0.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: im-swagger-spy
-Version: 0.3.3
+Version: 0.3.4
 Summary: im-swagger-spy: pytest plugin for matching methods in swagger with those used in tests
-Project-URL: Homepage, https://lancetnik.github.io/Propan/
-Project-URL: Documentation, https://lancetnik.github.io/Propan/
-Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
-Project-URL: Source, https://github.com/Lancetnik/Propan
+Project-URL: Homepage, https://github.com/dasshit/im-swagger-spy
+Project-URL: Tracker, https://github.com/dasshit/im-swagger-spy/issues
+Project-URL: Source, https://github.com/dasshit/im-swagger-spy
 Author-email: Korobov Valerii <v.korobov@corp.mail.ru>
 Keywords: plugin,pytest,pytest plugin,requests,swagger
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

