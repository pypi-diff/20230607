# Comparing `tmp/im_swagger_spy-0.3.4.tar.gz` & `tmp/im_swagger_spy-0.3.5.tar.gz`

## Comparing `im_swagger_spy-0.3.4.tar` & `im_swagger_spy-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/conftest.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/pytest.ini
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/requirements.txt
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/basic/example.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/pytest_example/conftest.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/pytest_example/pytest.ini
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/example/pytest_example/tests/test_request.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/__init__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/__main__.py
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/base.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/file_spy.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/http_spy.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/plugin.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/syncdb.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/template.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/im_swagger_spy/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/.gitignore
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/README.md
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/conftest.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/pytest.ini
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/requirements.txt
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/basic/example.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/pytest_example/conftest.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/pytest_example/pytest.ini
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/example/pytest_example/tests/test_request.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/__init__.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/__main__.py
+-rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/base.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/file_spy.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/http_spy.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/plugin.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/syncdb.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/template.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/im_swagger_spy/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/README.md
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 im_swagger_spy-0.3.5/PKG-INFO
```

### Comparing `im_swagger_spy-0.3.4/conftest.py` & `im_swagger_spy-0.3.5/conftest.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/setup.py` & `im_swagger_spy-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/.github/workflows/python-publish.yml` & `im_swagger_spy-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/example/basic/example.py` & `im_swagger_spy-0.3.5/example/basic/example.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/im_swagger_spy/base.py` & `im_swagger_spy-0.3.5/im_swagger_spy/base.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/im_swagger_spy/file_spy.py` & `im_swagger_spy-0.3.5/im_swagger_spy/file_spy.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/im_swagger_spy/http_spy.py` & `im_swagger_spy-0.3.5/im_swagger_spy/http_spy.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/im_swagger_spy/plugin.py` & `im_swagger_spy-0.3.5/im_swagger_spy/plugin.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/im_swagger_spy/syncdb.py` & `im_swagger_spy-0.3.5/im_swagger_spy/syncdb.py`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/im_swagger_spy/template.html` & `im_swagger_spy-0.3.5/im_swagger_spy/template.html`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/README.md` & `im_swagger_spy-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `im_swagger_spy-0.3.4/pyproject.toml` & `im_swagger_spy-0.3.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 ]
 
 keywords = ["swagger", "pytest", "pytest plugin", "plugin", "requests"]
 
 requires-python = ">=3.8"
 
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    'Development Status :: 5 - Production/Stable',
+    'Framework :: Pytest',
+    'Intended Audience :: Developers',
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Operating System :: OS Independent"
+    'Topic :: Software Development :: Quality Assurance',
+    'Topic :: Software Development :: Testing',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 
 dependencies = [
     "Jinja2>=3.0.0",
     "peewee>=3.0.0",
     "pytest>=7.0.0",
     "PyYAML>=6.0",
```

### Comparing `im_swagger_spy-0.3.4/PKG-INFO` & `im_swagger_spy-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: im-swagger-spy
-Version: 0.3.4
+Version: 0.3.5
 Summary: im-swagger-spy: pytest plugin for matching methods in swagger with those used in tests
 Project-URL: Homepage, https://github.com/dasshit/im-swagger-spy
 Project-URL: Tracker, https://github.com/dasshit/im-swagger-spy/issues
 Project-URL: Source, https://github.com/dasshit/im-swagger-spy
 Author-email: Korobov Valerii <v.korobov@corp.mail.ru>
 Keywords: plugin,pytest,pytest plugin,requests,swagger
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: peewee>=3.0.0
 Requires-Dist: pytest>=7.0.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.26.0
 Description-Content-Type: text/markdown
```

