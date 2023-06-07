# Comparing `tmp/im_swagger_spy-0.3.5.tar.gz` & `tmp/im_swagger_spy-0.3.7.tar.gz`

## Comparing `im_swagger_spy-0.3.5.tar` & `im_swagger_spy-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/conftest.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/pytest.ini
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/requirements.txt
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/basic/example.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/pytest_example/conftest.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/pytest_example/pytest.ini
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/pytest_example/tests/test_request.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/__init__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/__main__.py
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/base.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/file_spy.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/http_spy.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/plugin.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/syncdb.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/template.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/.gitignore
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/README.md
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/conftest.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/pytest.ini
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/setup.cfg
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/example/basic/example.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/example/pytest_example/conftest.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/example/pytest_example/pytest.ini
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/example/pytest_example/tests/test_request.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/__init__.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/__main__.py
+-rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/base.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/file_spy.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/http_spy.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/plugin.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/syncdb.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/template.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/im_swagger_spy/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/README.md
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.7/PKG-INFO
```

### Comparing `im_swagger_spy-0.3.5/conftest.py` & `im_swagger_spy-0.3.7/conftest.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/setup.py` & `im_swagger_spy-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/.github/workflows/python-publish.yml` & `im_swagger_spy-0.3.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/example/basic/example.py` & `im_swagger_spy-0.3.7/example/basic/example.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/im_swagger_spy/base.py` & `im_swagger_spy-0.3.7/im_swagger_spy/base.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/im_swagger_spy/file_spy.py` & `im_swagger_spy-0.3.7/im_swagger_spy/file_spy.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/im_swagger_spy/http_spy.py` & `im_swagger_spy-0.3.7/im_swagger_spy/http_spy.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/im_swagger_spy/plugin.py` & `im_swagger_spy-0.3.7/im_swagger_spy/plugin.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/im_swagger_spy/syncdb.py` & `im_swagger_spy-0.3.7/im_swagger_spy/syncdb.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/im_swagger_spy/template.html` & `im_swagger_spy-0.3.7/im_swagger_spy/template.html`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/README.md` & `im_swagger_spy-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.5/pyproject.toml` & `im_swagger_spy-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 Homepage = "https://github.com/dasshit/im-swagger-spy"
 Tracker = "https://github.com/dasshit/im-swagger-spy/issues"
 Source = "https://github.com/dasshit/im-swagger-spy"
 
 [project.scripts]
 im_swagger_spy = "im_swagger_spy.__main__:cli"
 
+[project.entry-points.pytest11]
+im_swagger_spy = "im_swagger_spy.plugin"
+
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
 
 [tool.hatch.version]
 path = "im_swagger_spy/__init__.py"
```

### Comparing `im_swagger_spy-0.3.5/PKG-INFO` & `im_swagger_spy-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-swagger-spy
-Version: 0.3.5
+Version: 0.3.7
 Summary: im-swagger-spy: pytest plugin for matching methods in swagger with those used in tests
 Project-URL: Homepage, https://github.com/dasshit/im-swagger-spy
 Project-URL: Tracker, https://github.com/dasshit/im-swagger-spy/issues
 Project-URL: Source, https://github.com/dasshit/im-swagger-spy
 Author-email: Korobov Valerii <v.korobov@corp.mail.ru>
 Keywords: plugin,pytest,pytest plugin,requests,swagger
 Classifier: Development Status :: 5 - Production/Stable
```

