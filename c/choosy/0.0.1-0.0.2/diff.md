# Comparing `tmp/choosy-0.0.1.tar.gz` & `tmp/choosy-0.0.2.tar.gz`

## Comparing `choosy-0.0.1.tar` & `choosy-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 choosy-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 choosy-0.0.1/src/choosy/__about__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 choosy-0.0.1/src/choosy/__init__.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 choosy-0.0.1/src/choosy/base.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 choosy-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 choosy-0.0.1/tests/test_base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 choosy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 choosy-0.0.1/LICENSE
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 choosy-0.0.1/README.md
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 choosy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 choosy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 choosy-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 choosy-0.0.2/src/choosy/__about__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 choosy-0.0.2/src/choosy/__init__.py
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 choosy-0.0.2/src/choosy/base.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 choosy-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 choosy-0.0.2/tests/test_base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 choosy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 choosy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 choosy-0.0.2/README.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 choosy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 choosy-0.0.2/PKG-INFO
```

### Comparing `choosy-0.0.1/.github/workflows/python-package.yml` & `choosy-0.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `choosy-0.0.1/src/choosy/base.py` & `choosy-0.0.2/src/choosy/base.py`

 * *Files identical despite different names*

### Comparing `choosy-0.0.1/tests/test_base.py` & `choosy-0.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `choosy-0.0.1/.gitignore` & `choosy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `choosy-0.0.1/LICENSE` & `choosy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `choosy-0.0.1/README.md` & `choosy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `choosy-0.0.1/pyproject.toml` & `choosy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,31 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+  "pandas",
+  "numpy",
+]
 
 [project.urls]
 Documentation = "https://github.com/ceesem/choosy#readme"
 Issues = "https://github.com/ceesem/choosy/issues"
 Source = "https://github.com/ceesem/choosy"
 
 [tool.hatch.version]
 path = "src/choosy/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
-  "pandas",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `choosy-0.0.1/PKG-INFO` & `choosy-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: choosy
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/ceesem/choosy#readme
 Project-URL: Issues, https://github.com/ceesem/choosy/issues
 Project-URL: Source, https://github.com/ceesem/choosy
 Author-email: Casey Schneider-Mizell <caseysm@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: numpy
+Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 # choosy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/choosy.svg)](https://pypi.org/project/choosy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/choosy.svg)](https://pypi.org/project/choosy)
```

